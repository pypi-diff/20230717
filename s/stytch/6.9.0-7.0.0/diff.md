# Comparing `tmp/stytch-6.9.0.tar.gz` & `tmp/stytch-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stytch-6.9.0.tar", last modified: Wed May 31 19:24:08 2023, max compression
+gzip compressed data, was "stytch-7.0.0.tar", last modified: Mon Jul 17 17:51:51 2023, max compression
```

## Comparing `stytch-6.9.0.tar` & `stytch-7.0.0.tar`

### file list

```diff
@@ -1,98 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:24:08.179835 stytch-6.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-31 19:23:52.000000 stytch-6.9.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-05-31 19:24:08.179835 stytch-6.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-05-31 19:23:52.000000 stytch-6.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-31 19:24:08.179835 stytch-6.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-31 19:23:52.000000 stytch-6.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:24:08.171835 stytch-6.9.0/stytch/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:24:08.175835 stytch-6.9.0/stytch/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/crypto_wallets.py
--rw-r--r--   0 runner    (1001) docker     (123)    12541 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    28137 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/otp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/otp_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/otp_whatsapp.py
--rw-r--r--   0 runner    (1001) docker     (123)    17096 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    13713 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/totps.py
--rw-r--r--   0 runner    (1001) docker     (123)    24338 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/users.py
--rw-r--r--   0 runner    (1001) docker     (123)    12985 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/webauthn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:24:08.175835 stytch-6.9.0/stytch/b2b/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:24:08.175835 stytch-6.9.0/stytch/b2b/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/api/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/api/discovery_intermediate_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17277 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/api/discovery_organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/api/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/api/magic_links_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    16357 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/api/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/api/magic_links_email_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    49021 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/api/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)    17130 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/api/passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/api/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/api/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/api/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/api/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:24:08.175835 stytch-6.9.0/stytch/b2b/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/core/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:24:08.175835 stytch-6.9.0/stytch/b2b/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/models/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/models/discovery_intermediate_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/models/discovery_organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/models/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/models/magic_links_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/models/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/models/magic_links_email_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/models/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/models/passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/models/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/models/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/models/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/models/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:24:08.179835 stytch-6.9.0/stytch/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/core/api_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:24:08.179835 stytch-6.9.0/stytch/core/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/core/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/core/http/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/core/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:24:08.179835 stytch-6.9.0/stytch/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/crypto_wallets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/otp.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/otp_email.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/otp_whatsapp.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/totps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/users.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/webauthn.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:24:08.171835 stytch-6.9.0/stytch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-05-31 19:24:08.000000 stytch-6.9.0/stytch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-31 19:24:08.000000 stytch-6.9.0/stytch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 19:24:08.000000 stytch-6.9.0/stytch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-31 19:24:08.000000 stytch-6.9.0/stytch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 19:24:08.000000 stytch-6.9.0/stytch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:24:08.179835 stytch-6.9.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-05-31 19:23:52.000000 stytch-6.9.0/test/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    12774 2023-05-31 19:23:52.000000 stytch-6.9.0/test/test_integration_async.py
+drwxr-xr-x   0 gorel      (501) staff       (20)        0 2023-07-17 17:51:51.610122 stytch-7.0.0/
+-rw-r--r--   0 gorel      (501) staff       (20)     1059 2022-12-06 17:10:39.000000 stytch-7.0.0/LICENSE.txt
+-rw-r--r--   0 gorel      (501) staff       (20)     5142 2023-07-17 17:51:51.610184 stytch-7.0.0/PKG-INFO
+-rw-r--r--   0 gorel      (501) staff       (20)     4367 2023-04-20 19:06:08.000000 stytch-7.0.0/README.md
+-rw-r--r--   0 gorel      (501) staff       (20)      110 2023-07-17 17:51:51.610404 stytch-7.0.0/setup.cfg
+-rw-r--r--   0 gorel      (501) staff       (20)     1739 2022-12-16 21:16:07.000000 stytch-7.0.0/setup.py
+drwxr-xr-x   0 gorel      (501) staff       (20)        0 2023-07-17 17:51:51.601994 stytch-7.0.0/stytch/
+-rw-r--r--   0 gorel      (501) staff       (20)      181 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/__init__.py
+drwxr-xr-x   0 gorel      (501) staff       (20)        0 2023-07-17 17:51:51.602757 stytch-7.0.0/stytch/b2b/
+-rw-r--r--   0 gorel      (501) staff       (20)        0 2023-02-22 04:57:31.000000 stytch-7.0.0/stytch/b2b/__init__.py
+drwxr-xr-x   0 gorel      (501) staff       (20)        0 2023-07-17 17:51:51.605898 stytch-7.0.0/stytch/b2b/api/
+-rw-r--r--   0 gorel      (501) staff       (20)        0 2023-02-22 04:57:31.000000 stytch-7.0.0/stytch/b2b/api/__init__.py
+-rw-r--r--   0 gorel      (501) staff       (20)      892 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/discovery.py
+-rw-r--r--   0 gorel      (501) staff       (20)     7036 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/discovery_intermediate_sessions.py
+-rw-r--r--   0 gorel      (501) staff       (20)    21373 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/discovery_organizations.py
+-rw-r--r--   0 gorel      (501) staff       (20)     8980 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/magic_links.py
+-rw-r--r--   0 gorel      (501) staff       (20)     2833 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/magic_links_discovery.py
+-rw-r--r--   0 gorel      (501) staff       (20)    16783 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/magic_links_email.py
+-rw-r--r--   0 gorel      (501) staff       (20)     5807 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/magic_links_email_discovery.py
+-rw-r--r--   0 gorel      (501) staff       (20)    31415 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/organizations.py
+-rw-r--r--   0 gorel      (501) staff       (20)    22509 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/organizations_members.py
+-rw-r--r--   0 gorel      (501) staff       (20)    22270 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/passwords.py
+-rw-r--r--   0 gorel      (501) staff       (20)    18614 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/passwords_email.py
+-rw-r--r--   0 gorel      (501) staff       (20)     8525 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/passwords_existing_password.py
+-rw-r--r--   0 gorel      (501) staff       (20)     3439 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/passwords_session.py
+-rw-r--r--   0 gorel      (501) staff       (20)    19582 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/sessions.py
+-rw-r--r--   0 gorel      (501) staff       (20)    11114 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/sso.py
+-rw-r--r--   0 gorel      (501) staff       (20)    10786 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/sso_oidc.py
+-rw-r--r--   0 gorel      (501) staff       (20)    10369 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/sso_saml.py
+-rw-r--r--   0 gorel      (501) staff       (20)     1423 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/client.py
+drwxr-xr-x   0 gorel      (501) staff       (20)        0 2023-07-17 17:51:51.608427 stytch-7.0.0/stytch/b2b/models/
+-rw-r--r--   0 gorel      (501) staff       (20)        0 2023-02-22 04:57:31.000000 stytch-7.0.0/stytch/b2b/models/__init__.py
+-rw-r--r--   0 gorel      (501) staff       (20)     1452 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/discovery.py
+-rw-r--r--   0 gorel      (501) staff       (20)     1159 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/discovery_intermediate_sessions.py
+-rw-r--r--   0 gorel      (501) staff       (20)     2325 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/discovery_organizations.py
+-rw-r--r--   0 gorel      (501) staff       (20)     1712 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/magic_links.py
+-rw-r--r--   0 gorel      (501) staff       (20)     1674 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/magic_links_discovery.py
+-rw-r--r--   0 gorel      (501) staff       (20)     1536 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/magic_links_email.py
+-rw-r--r--   0 gorel      (501) staff       (20)      431 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/magic_links_email_discovery.py
+-rw-r--r--   0 gorel      (501) staff       (20)    11086 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/organizations.py
+-rw-r--r--   0 gorel      (501) staff       (20)     2938 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/organizations_members.py
+-rw-r--r--   0 gorel      (501) staff       (20)     5719 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/passwords.py
+-rw-r--r--   0 gorel      (501) staff       (20)     1883 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/passwords_email.py
+-rw-r--r--   0 gorel      (501) staff       (20)     1149 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/passwords_existing_password.py
+-rw-r--r--   0 gorel      (501) staff       (20)      957 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/passwords_session.py
+-rw-r--r--   0 gorel      (501) staff       (20)     3802 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/sessions.py
+-rw-r--r--   0 gorel      (501) staff       (20)     3314 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/sso.py
+-rw-r--r--   0 gorel      (501) staff       (20)     1400 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/sso_oidc.py
+-rw-r--r--   0 gorel      (501) staff       (20)     1307 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/sso_saml.py
+drwxr-xr-x   0 gorel      (501) staff       (20)        0 2023-07-17 17:51:51.609203 stytch-7.0.0/stytch/core/
+-rw-r--r--   0 gorel      (501) staff       (20)        0 2022-12-16 21:16:07.000000 stytch-7.0.0/stytch/core/__init__.py
+-rw-r--r--   0 gorel      (501) staff       (20)      586 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/core/api_base.py
+-rw-r--r--   0 gorel      (501) staff       (20)     1210 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/core/client_base.py
+drwxr-xr-x   0 gorel      (501) staff       (20)        0 2023-07-17 17:51:51.609454 stytch-7.0.0/stytch/core/http/
+-rw-r--r--   0 gorel      (501) staff       (20)        0 2022-12-20 16:48:17.000000 stytch-7.0.0/stytch/core/http/__init__.py
+-rw-r--r--   0 gorel      (501) staff       (20)     3605 2023-06-05 21:01:43.000000 stytch-7.0.0/stytch/core/http/client.py
+-rw-r--r--   0 gorel      (501) staff       (20)     2106 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/core/response_base.py
+-rw-r--r--   0 gorel      (501) staff       (20)       22 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/version.py
+drwxr-xr-x   0 gorel      (501) staff       (20)        0 2023-07-17 17:51:51.602556 stytch-7.0.0/stytch.egg-info/
+-rw-r--r--   0 gorel      (501) staff       (20)     5142 2023-07-17 17:51:51.000000 stytch-7.0.0/stytch.egg-info/PKG-INFO
+-rw-r--r--   0 gorel      (501) staff       (20)     1776 2023-07-17 17:51:51.000000 stytch-7.0.0/stytch.egg-info/SOURCES.txt
+-rw-r--r--   0 gorel      (501) staff       (20)        1 2023-07-17 17:51:51.000000 stytch-7.0.0/stytch.egg-info/dependency_links.txt
+-rw-r--r--   0 gorel      (501) staff       (20)       69 2023-07-17 17:51:51.000000 stytch-7.0.0/stytch.egg-info/requires.txt
+-rw-r--r--   0 gorel      (501) staff       (20)        7 2023-07-17 17:51:51.000000 stytch-7.0.0/stytch.egg-info/top_level.txt
+drwxr-xr-x   0 gorel      (501) staff       (20)        0 2023-07-17 17:51:51.609961 stytch-7.0.0/test/
+-rw-r--r--   0 gorel      (501) staff       (20)     9527 2023-07-17 16:16:44.000000 stytch-7.0.0/test/test_integration.py
+-rw-r--r--   0 gorel      (501) staff       (20)    12747 2023-07-17 16:16:44.000000 stytch-7.0.0/test/test_integration_async.py
```

### Comparing `stytch-6.9.0/LICENSE.txt` & `stytch-7.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stytch-6.9.0/PKG-INFO` & `stytch-7.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stytch
-Version: 6.9.0
+Version: 7.0.0
 Summary: Stytch python client
 Download-URL: https://github.com/stytchauth/stytch-python
 Author: Stytch
 Author-email: hello@stytch.com
 License: MIT
 Keywords: stytch,user,authentication
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stytch-6.9.0/README.md` & `stytch-7.0.0/README.md`

 * *Files identical despite different names*

### Comparing `stytch-6.9.0/setup.py` & `stytch-7.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `stytch-6.9.0/stytch/api/magic_links.py` & `stytch-7.0.0/stytch/b2b/api/sso.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,227 +1,217 @@
 # !!!
 # WARNING: This file is autogenerated
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
+from __future__ import annotations
+
 from typing import Any, Dict, Optional
 
-from stytch.api.magic_links_email import Email
+from stytch.b2b.api.sso_oidc import OIDC
+from stytch.b2b.api.sso_saml import SAML
+from stytch.b2b.models.sso import (
+    AuthenticateResponse,
+    DeleteConnectionResponse,
+    GetConnectionsResponse,
+)
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
-from stytch.models.magic_links import AuthenticateResponse, CreateResponse
 
 
-class MagicLinks:
+class SSO:
     def __init__(
         self,
         api_base: ApiBase,
         sync_client: SyncClient,
         async_client: AsyncClient,
     ) -> None:
         self.api_base = api_base
         self.sync_client = sync_client
         self.async_client = async_client
-        self.email = Email(api_base, sync_client, async_client)
-
-    @property
-    def sub_url(self) -> str:
-        return "magic_links"
+        self.oidc = OIDC(api_base, sync_client, async_client)
+        self.saml = SAML(api_base, sync_client, async_client)
 
-    def create(
+    def get_connections(
         self,
-        user_id: str,
-        expiration_minutes: Optional[int] = None,
-        attributes: Optional[Dict[str, str]] = None,
-    ) -> CreateResponse:
-        """[Stytch docs](https://stytch.com/docs/api/create-magic-link)
-
-        Create a magic link token for a user. Access to this endpoint is restricted, to be enabled for it, please send us a note at support@stytch.com.
-
-        Parameters:
-
-        - `user_id`: The user ID for the magic link token.
-
-        - `expiration_minutes`: Set the expiration for the magic token, in minutes. By default, it expires in 1 hour. The minimum expiration is 5 minutes and the maximum is 7 days (10080 mins).
+        organization_id: str,
+    ) -> GetConnectionsResponse:
+        """Get all SSO Connections owned by the organization.
 
-        - `attributes`: Provided attributes help with fraud detection. When authenticating a user's magic link token, you can require the IP address and/or the user agent to match that user's attributes when they originated the initial authentication request. To enable this functionality, you can use the options parameter in [AuthenticateMagic](https://stytch.com/docs/api/authenticate-magic-link).
+        Fields:
+          - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
         """  # noqa
-
-        payload: Dict[str, Any] = {
-            "user_id": user_id,
+        data: Dict[str, Any] = {
+            "organization_id": organization_id,
         }
 
-        if expiration_minutes is not None:
-            payload["expiration_minutes"] = expiration_minutes
-        if attributes is not None:
-            payload["attributes"] = attributes
-
-        url = self.api_base.route_with_sub_url(self.sub_url, None)
-
-        res = self.sync_client.post(url, json=payload)
-        return CreateResponse.from_json(res.response.status_code, res.json)
+        url = self.api_base.url_for("/v1/b2b/sso/{organization_id}", data)
+        res = self.sync_client.get(url, data)
+        return GetConnectionsResponse.from_json(res.response.status_code, res.json)
 
-    async def create_async(
+    async def get_connections_async(
         self,
-        user_id: str,
-        expiration_minutes: Optional[int] = None,
-        attributes: Optional[Dict[str, str]] = None,
-    ) -> CreateResponse:
-        """[Stytch docs](https://stytch.com/docs/api/create-magic-link)
+        organization_id: str,
+    ) -> GetConnectionsResponse:
+        """Get all SSO Connections owned by the organization.
 
-        Create a magic link token for a user. Access to this endpoint is restricted, to be enabled for it, please send us a note at support@stytch.com.
-
-        Parameters:
-
-        - `user_id`: The user ID for the magic link token.
+        Fields:
+          - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
+        """  # noqa
+        data: Dict[str, Any] = {
+            "organization_id": organization_id,
+        }
 
-        - `expiration_minutes`: Set the expiration for the magic token, in minutes. By default, it expires in 1 hour. The minimum expiration is 5 minutes and the maximum is 7 days (10080 mins).
+        url = self.api_base.url_for("/v1/b2b/sso/{organization_id}", data)
+        res = await self.async_client.get(url, data)
+        return GetConnectionsResponse.from_json(res.response.status, res.json)
 
-        - `attributes`: Provided attributes help with fraud detection. When authenticating a user's magic link token, you can require the IP address and/or the user agent to match that user's attributes when they originated the initial authentication request. To enable this functionality, you can use the options parameter in [AuthenticateMagic](https://stytch.com/docs/api/authenticate-magic-link).
+    def delete_connection(
+        self,
+        organization_id: str,
+        connection_id: str,
+    ) -> DeleteConnectionResponse:
+        """Delete an existing SSO connection.
+
+        Fields:
+          - organization_id: The organization ID that the SSO connection belongs to.
+          - connection_id: The ID of the SSO connection. Both SAML and OIDC connection IDs can be provided.
         """  # noqa
-
-        payload: Dict[str, Any] = {
-            "user_id": user_id,
+        data: Dict[str, Any] = {
+            "organization_id": organization_id,
+            "connection_id": connection_id,
         }
 
-        if expiration_minutes is not None:
-            payload["expiration_minutes"] = expiration_minutes
-        if attributes is not None:
-            payload["attributes"] = attributes
+        url = self.api_base.url_for(
+            "/v1/b2b/sso/{organization_id}/connections/{connection_id}", data
+        )
+        res = self.sync_client.delete(url)
+        return DeleteConnectionResponse.from_json(res.response.status_code, res.json)
 
-        url = self.api_base.route_with_sub_url(self.sub_url, None)
+    async def delete_connection_async(
+        self,
+        organization_id: str,
+        connection_id: str,
+    ) -> DeleteConnectionResponse:
+        """Delete an existing SSO connection.
+
+        Fields:
+          - organization_id: The organization ID that the SSO connection belongs to.
+          - connection_id: The ID of the SSO connection. Both SAML and OIDC connection IDs can be provided.
+        """  # noqa
+        data: Dict[str, Any] = {
+            "organization_id": organization_id,
+            "connection_id": connection_id,
+        }
 
-        res = await self.async_client.post(url, json=payload)
-        return CreateResponse.from_json(res.response.status, res.json)
+        url = self.api_base.url_for(
+            "/v1/b2b/sso/{organization_id}/connections/{connection_id}", data
+        )
+        res = await self.async_client.delete(url)
+        return DeleteConnectionResponse.from_json(res.response.status, res.json)
 
     def authenticate(
         self,
-        token: str,
-        attributes: Optional[Dict[str, str]] = None,
-        options: Optional[Dict[str, str]] = None,
+        sso_token: str,
+        pkce_code_verifier: Optional[str] = None,
         session_token: Optional[str] = None,
         session_jwt: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
-        code_verifier: Optional[str] = None,
     ) -> AuthenticateResponse:
-        """[Stytch docs](https://stytch.com/docs/api/authenticate-magic-link)
-
-        Authenticate a user given a magic link. This endpoint verifies that the magic link `token` is valid, hasn't expired or been previously used, and any optional security settings such as IP match or user agent match are satisfied.
-
-        Parameters:
-
-        - `token`: The token to authenticate.
-
-        - `options`: Specify optional security settings
-
-        - `attributes`: Provided attributes help with fraud detection. You can require the IP address and/or the user agent to match the request used to send the magic link using the options parameter.
+        """Authenticate a user given a token.
+        This endpoint verifies that the user completed the SSO Authentication flow by verifying that the token is valid and hasn't expired.
+        Provide the `session_duration_minutes` parameter to set the lifetime of the session.
+        If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration.
+        To link this authentication event to an existing Stytch session, include either the `session_token` or `session_jwt` param.
+
+        Fields:
+          - sso_token: The token to authenticate.
+          - pkce_code_verifier: A base64url encoded one time secret used to validate that the request starts and ends on the same device.
+          - session_token: The `session_token` belonging to the member that you wish to associate the email with.
+          - session_jwt: The `session_jwt` belonging to the member that you wish to associate the email with.
+          - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
+          returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
+          five minutes regardless of the underlying session duration, and will need to be refreshed over time.
 
-        - `session_duration_minutes`: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist, returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of five minutes regardless of the underlying session duration, and will need to be refreshed over time.
-
-          This value must be a minimum of 5 and a maximum of 129600 minutes (90 days).
+          This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
 
           If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
 
-          If the `session_duration_minutes` parameter is not specified, a Stytch session will not be created.
-
-        - `session_custom_claims`: Add a custom claims map to the session being authenticated. Claims are only created if a session is initialized by providing a value in `session_duration_minutes`. Claims will be included on the session object and in the JWT. To update a key in an existing session, supply a new value. To delete a key, supply a null value
-
-          Custom claims made with reserved claims ("iss", "sub", "aud", "exp", "nbf", "iat", "jti") will be ignored. Total custom claims size cannot exceed four kilobytes
-
-        - `session_jwt`: Reuse an existing session instead of creating a new one. If you provide us with a `session_jwt`, then we'll update the session represented by this JWT with this magic link factor. If this `session_jwt` belongs to a different user than the magic token, the `session_jwt` will be ignored. This endpoint will error if both `session_token` and `session_jwt` are provided.
-
-        - `session_token`: Reuse an existing session instead of creating a new one. If you provide us with a `session_token`, then we'll update the session represented by this session token with this magic link factor. If this `session_token` belongs to a different user than the magic token, the `session_token` will be ignored. This endpoint will error if both `session_token` and `session_jwt` are provided.
-
-        - `code_verifier`: A base64url encoded one time secret used to validate that the request starts and ends on the same device.
+          If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
+          to use the Stytch session product, you can ignore the session fields in the response.
+          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
+          `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
+          delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
+          Total custom claims size cannot exceed four kilobytes.
         """  # noqa
-
-        payload: Dict[str, Any] = {
-            "token": token,
+        data: Dict[str, Any] = {
+            "sso_token": sso_token,
         }
-
-        if attributes is not None:
-            payload["attributes"] = attributes
-        if options is not None:
-            payload["options"] = options
+        if pkce_code_verifier is not None:
+            data["pkce_code_verifier"] = pkce_code_verifier
         if session_token is not None:
-            payload["session_token"] = session_token
+            data["session_token"] = session_token
         if session_jwt is not None:
-            payload["session_jwt"] = session_jwt
+            data["session_jwt"] = session_jwt
         if session_duration_minutes is not None:
-            payload["session_duration_minutes"] = session_duration_minutes
+            data["session_duration_minutes"] = session_duration_minutes
         if session_custom_claims is not None:
-            payload["session_custom_claims"] = session_custom_claims
-        if code_verifier is not None:
-            payload["code_verifier"] = code_verifier
-
-        url = self.api_base.route_with_sub_url(self.sub_url, "authenticate")
+            data["session_custom_claims"] = session_custom_claims
 
-        res = self.sync_client.post(url, json=payload)
+        url = self.api_base.url_for("/v1/b2b/sso/authenticate", data)
+        res = self.sync_client.post(url, data)
         return AuthenticateResponse.from_json(res.response.status_code, res.json)
 
     async def authenticate_async(
         self,
-        token: str,
-        attributes: Optional[Dict[str, str]] = None,
-        options: Optional[Dict[str, str]] = None,
+        sso_token: str,
+        pkce_code_verifier: Optional[str] = None,
         session_token: Optional[str] = None,
         session_jwt: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
-        code_verifier: Optional[str] = None,
     ) -> AuthenticateResponse:
-        """[Stytch docs](https://stytch.com/docs/api/authenticate-magic-link)
-
-        Authenticate a user given a magic link. This endpoint verifies that the magic link `token` is valid, hasn't expired or been previously used, and any optional security settings such as IP match or user agent match are satisfied.
-
-        Parameters:
-
-        - `token`: The token to authenticate.
+        """Authenticate a user given a token.
+        This endpoint verifies that the user completed the SSO Authentication flow by verifying that the token is valid and hasn't expired.
+        Provide the `session_duration_minutes` parameter to set the lifetime of the session.
+        If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration.
+        To link this authentication event to an existing Stytch session, include either the `session_token` or `session_jwt` param.
+
+        Fields:
+          - sso_token: The token to authenticate.
+          - pkce_code_verifier: A base64url encoded one time secret used to validate that the request starts and ends on the same device.
+          - session_token: The `session_token` belonging to the member that you wish to associate the email with.
+          - session_jwt: The `session_jwt` belonging to the member that you wish to associate the email with.
+          - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
+          returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
+          five minutes regardless of the underlying session duration, and will need to be refreshed over time.
 
-        - `options`: Specify optional security settings
-
-        - `attributes`: Provided attributes help with fraud detection. You can require the IP address and/or the user agent to match the request used to send the magic link using the options parameter.
-
-        - `session_duration_minutes`: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist, returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of five minutes regardless of the underlying session duration, and will need to be refreshed over time.
-
-          This value must be a minimum of 5 and a maximum of 129600 minutes (90 days).
+          This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
 
           If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
 
-          If the `session_duration_minutes` parameter is not specified, a Stytch session will not be created.
-
-        - `session_custom_claims`: Add a custom claims map to the session being authenticated. Claims are only created if a session is initialized by providing a value in `session_duration_minutes`. Claims will be included on the session object and in the JWT. To update a key in an existing session, supply a new value. To delete a key, supply a null value
-
-          Custom claims made with reserved claims ("iss", "sub", "aud", "exp", "nbf", "iat", "jti") will be ignored. Total custom claims size cannot exceed four kilobytes
-
-        - `session_jwt`: Reuse an existing session instead of creating a new one. If you provide us with a `session_jwt`, then we'll update the session represented by this JWT with this magic link factor. If this `session_jwt` belongs to a different user than the magic token, the `session_jwt` will be ignored. This endpoint will error if both `session_token` and `session_jwt` are provided.
-
-        - `session_token`: Reuse an existing session instead of creating a new one. If you provide us with a `session_token`, then we'll update the session represented by this session token with this magic link factor. If this `session_token` belongs to a different user than the magic token, the `session_token` will be ignored. This endpoint will error if both `session_token` and `session_jwt` are provided.
-
-        - `code_verifier`: A base64url encoded one time secret used to validate that the request starts and ends on the same device.
+          If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
+          to use the Stytch session product, you can ignore the session fields in the response.
+          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
+          `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
+          delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
+          Total custom claims size cannot exceed four kilobytes.
         """  # noqa
-
-        payload: Dict[str, Any] = {
-            "token": token,
+        data: Dict[str, Any] = {
+            "sso_token": sso_token,
         }
-
-        if attributes is not None:
-            payload["attributes"] = attributes
-        if options is not None:
-            payload["options"] = options
+        if pkce_code_verifier is not None:
+            data["pkce_code_verifier"] = pkce_code_verifier
         if session_token is not None:
-            payload["session_token"] = session_token
+            data["session_token"] = session_token
         if session_jwt is not None:
-            payload["session_jwt"] = session_jwt
+            data["session_jwt"] = session_jwt
         if session_duration_minutes is not None:
-            payload["session_duration_minutes"] = session_duration_minutes
+            data["session_duration_minutes"] = session_duration_minutes
         if session_custom_claims is not None:
-            payload["session_custom_claims"] = session_custom_claims
-        if code_verifier is not None:
-            payload["code_verifier"] = code_verifier
-
-        url = self.api_base.route_with_sub_url(self.sub_url, "authenticate")
+            data["session_custom_claims"] = session_custom_claims
 
-        res = await self.async_client.post(url, json=payload)
+        url = self.api_base.url_for("/v1/b2b/sso/authenticate", data)
+        res = await self.async_client.post(url, data)
         return AuthenticateResponse.from_json(res.response.status, res.json)
```

### Comparing `stytch-6.9.0/stytch/api/oauth.py` & `stytch-7.0.0/stytch/b2b/api/passwords_existing_password.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,189 +1,145 @@
 # !!!
 # WARNING: This file is autogenerated
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
+from __future__ import annotations
+
 from typing import Any, Dict, Optional
 
+from stytch.b2b.models.passwords_existing_password import ResetResponse
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
-from stytch.models.oauth import AttachResponse, AuthenticateResponse
 
 
-class OAuth:
+class ExistingPassword:
     def __init__(
         self,
         api_base: ApiBase,
         sync_client: SyncClient,
         async_client: AsyncClient,
     ) -> None:
         self.api_base = api_base
         self.sync_client = sync_client
         self.async_client = async_client
 
-    @property
-    def sub_url(self) -> str:
-        return "oauth"
-
-    def authenticate(
+    def reset(
         self,
-        token: str,
+        email_address: str,
+        existing_password: str,
+        new_password: str,
+        organization_id: str,
         session_token: Optional[str] = None,
-        session_jwt: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
+        session_jwt: Optional[str] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
-        code_verifier: Optional[str] = None,
-    ) -> AuthenticateResponse:
-        """[Stytch docs](https://stytch.com/docs/api/oauth-authenticate)
-
-        Authenticate a user given a token. This endpoint verifies that the user completed the OAuth flow by verifying that the token is valid and hasn't expired. To initiate a Stytch session for the user while authenticating their OAuth token, include `session_duration_minutes`; a session with the identity provider, e.g. Google or Facebook, will always be initiated upon successful authentication.
-
-        Parameters:
-
-        - `token`: The token to authenticate.
-
-        - `session_custom_claims`: Add a custom claims map to the session being authenticated. Claims are only created if a session is initialized by providing a value in `session duration minutes`. Claims will be included on the session object and in the JWT. To update a key in an existing session, supply a new value. To delete a key, supply a null value
-
-          Custom claims made with reserved claims ("iss", "sub", "aud", "exp", "nbf", "iat", "jti") will be ignored. Total custom claims size cannot exceed four kilobytes
-
-        - `session_duration_minutes`: (Stytch sessions only) Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist, returning both an opaque `session_token` and `session_jwt` for this session. Remember that `session_jwt` will have a fixed lifetime of five minutes regardless of the underlying session duration, and will need to be refreshed over time.
-
-          This argument only sets the lifetime for Stytch sessions, not for IdP sessions. This value must be a minimum of 5 and a maximum of 129600 minutes (90 days).
-
-          If a session_token or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
-
-          If the `session_duration_minutes` parameter is not specified, a Stytch session will not be created.
-
-        - `session_jwt`: (Stytch sessions only) Reuse an existing session instead of creating a new one. If you provide us with a `session_jwt`, then we'll update the session represented by this JWT with this OAuth factor. If this `session_jwt` belongs to a different user than the OAuth token, the `session_jwt` will be ignored. This endpoint will error if both session_token and `session_jwt` are provided.
-
-        - `session_token`: (Stytch sessions only) Reuse an existing session instead of creating a new one. If you provide us with a `session_token`, then we'll update the session represented by this session token with this OAuth factor. If this `session_token` belongs to a different user than the OAuth token, the `session_token` will be ignored. This endpoint will error if both `session_token` and `session_jwt` are provided.
+    ) -> ResetResponse:
+        """Reset the member’s password using their existing password.
 
-        - `code_verifier`: A base64url encoded one time secret used to validate that the request starts and ends on the same device. See the [PKCE OAuth guide](https://stytch.com/docs/oauth#guides_pkce) for usage instructions.
+        This endpoint adapts to your Project's password strength configuration.
+        If you're using [zxcvbn](https://stytch.com/docs/passwords#strength-requirements), the default, your passwords are considered valid
+        if the strength score is >= 3. If you're using [LUDS](https://stytch.com/docs/passwords#strength-requirements), your passwords are
+        considered valid if they meet the requirements that you've set with Stytch.
+        You may update your password strength configuration in the [stytch dashboard](https://stytch.com/dashboard/password-strength-config).
+
+        Fields:
+          - email_address: The email address of the Member.
+          - existing_password: The member's current password that they supplied.
+          - new_password: The member's elected new password.
+          - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
+          - session_token: A secret token for a given Stytch Session.
+          - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
+          returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
+          five minutes regardless of the underlying session duration, and will need to be refreshed over time.
+
+          This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
+
+          If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
+
+          If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
+          to use the Stytch session product, you can ignore the session fields in the response.
+          - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
+          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
+          `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
+          delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
+          Total custom claims size cannot exceed four kilobytes.
         """  # noqa
-
-        payload: Dict[str, Any] = {
-            "token": token,
+        data: Dict[str, Any] = {
+            "email_address": email_address,
+            "existing_password": existing_password,
+            "new_password": new_password,
+            "organization_id": organization_id,
         }
-
         if session_token is not None:
-            payload["session_token"] = session_token
-        if session_jwt is not None:
-            payload["session_jwt"] = session_jwt
+            data["session_token"] = session_token
         if session_duration_minutes is not None:
-            payload["session_duration_minutes"] = session_duration_minutes
+            data["session_duration_minutes"] = session_duration_minutes
+        if session_jwt is not None:
+            data["session_jwt"] = session_jwt
         if session_custom_claims is not None:
-            payload["session_custom_claims"] = session_custom_claims
-        if code_verifier is not None:
-            payload["code_verifier"] = code_verifier
+            data["session_custom_claims"] = session_custom_claims
 
-        url = self.api_base.route_with_sub_url(self.sub_url, "authenticate")
+        url = self.api_base.url_for("/v1/b2b/passwords/existing_password/reset", data)
+        res = self.sync_client.post(url, data)
+        return ResetResponse.from_json(res.response.status_code, res.json)
 
-        res = self.sync_client.post(url, json=payload)
-        return AuthenticateResponse.from_json(res.response.status_code, res.json)
-
-    async def authenticate_async(
+    async def reset_async(
         self,
-        token: str,
+        email_address: str,
+        existing_password: str,
+        new_password: str,
+        organization_id: str,
         session_token: Optional[str] = None,
-        session_jwt: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
+        session_jwt: Optional[str] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
-        code_verifier: Optional[str] = None,
-    ) -> AuthenticateResponse:
-        """[Stytch docs](https://stytch.com/docs/api/oauth-authenticate)
-
-        Authenticate a user given a token. This endpoint verifies that the user completed the OAuth flow by verifying that the token is valid and hasn't expired. To initiate a Stytch session for the user while authenticating their OAuth token, include `session_duration_minutes`; a session with the identity provider, e.g. Google or Facebook, will always be initiated upon successful authentication.
-
-        Parameters:
-
-        - `token`: The token to authenticate.
-
-        - `session_custom_claims`: Add a custom claims map to the session being authenticated. Claims are only created if a session is initialized by providing a value in `session duration minutes`. Claims will be included on the session object and in the JWT. To update a key in an existing session, supply a new value. To delete a key, supply a null value
-
-          Custom claims made with reserved claims ("iss", "sub", "aud", "exp", "nbf", "iat", "jti") will be ignored. Total custom claims size cannot exceed four kilobytes
-
-        - `session_duration_minutes`: (Stytch sessions only) Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist, returning both an opaque `session_token` and `session_jwt` for this session. Remember that `session_jwt` will have a fixed lifetime of five minutes regardless of the underlying session duration, and will need to be refreshed over time.
-
-          This argument only sets the lifetime for Stytch sessions, not for IdP sessions. This value must be a minimum of 5 and a maximum of 129600 minutes (90 days).
-
-          If a session_token or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
+    ) -> ResetResponse:
+        """Reset the member’s password using their existing password.
 
-          If the `session_duration_minutes` parameter is not specified, a Stytch session will not be created.
-
-        - `session_jwt`: (Stytch sessions only) Reuse an existing session instead of creating a new one. If you provide us with a `session_jwt`, then we'll update the session represented by this JWT with this OAuth factor. If this `session_jwt` belongs to a different user than the OAuth token, the `session_jwt` will be ignored. This endpoint will error if both session_token and `session_jwt` are provided.
-
-        - `session_token`: (Stytch sessions only) Reuse an existing session instead of creating a new one. If you provide us with a `session_token`, then we'll update the session represented by this session token with this OAuth factor. If this `session_token` belongs to a different user than the OAuth token, the `session_token` will be ignored. This endpoint will error if both `session_token` and `session_jwt` are provided.
-
-        - `code_verifier`: A base64url encoded one time secret used to validate that the request starts and ends on the same device. See the [PKCE OAuth guide](https://stytch.com/docs/oauth#guides_pkce) for usage instructions.
+        This endpoint adapts to your Project's password strength configuration.
+        If you're using [zxcvbn](https://stytch.com/docs/passwords#strength-requirements), the default, your passwords are considered valid
+        if the strength score is >= 3. If you're using [LUDS](https://stytch.com/docs/passwords#strength-requirements), your passwords are
+        considered valid if they meet the requirements that you've set with Stytch.
+        You may update your password strength configuration in the [stytch dashboard](https://stytch.com/dashboard/password-strength-config).
+
+        Fields:
+          - email_address: The email address of the Member.
+          - existing_password: The member's current password that they supplied.
+          - new_password: The member's elected new password.
+          - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
+          - session_token: A secret token for a given Stytch Session.
+          - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
+          returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
+          five minutes regardless of the underlying session duration, and will need to be refreshed over time.
+
+          This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
+
+          If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
+
+          If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
+          to use the Stytch session product, you can ignore the session fields in the response.
+          - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
+          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
+          `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
+          delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
+          Total custom claims size cannot exceed four kilobytes.
         """  # noqa
-
-        payload: Dict[str, Any] = {
-            "token": token,
+        data: Dict[str, Any] = {
+            "email_address": email_address,
+            "existing_password": existing_password,
+            "new_password": new_password,
+            "organization_id": organization_id,
         }
-
         if session_token is not None:
-            payload["session_token"] = session_token
-        if session_jwt is not None:
-            payload["session_jwt"] = session_jwt
+            data["session_token"] = session_token
         if session_duration_minutes is not None:
-            payload["session_duration_minutes"] = session_duration_minutes
-        if session_custom_claims is not None:
-            payload["session_custom_claims"] = session_custom_claims
-        if code_verifier is not None:
-            payload["code_verifier"] = code_verifier
-
-        url = self.api_base.route_with_sub_url(self.sub_url, "authenticate")
-
-        res = await self.async_client.post(url, json=payload)
-        return AuthenticateResponse.from_json(res.response.status, res.json)
-
-    def attach(
-        self,
-        provider: str,
-        user_id: Optional[str] = None,
-        session_token: Optional[str] = None,
-        session_jwt: Optional[str] = None,
-    ) -> AttachResponse:
-        """[Stytch docs](https://stytch.com/docs/api/oauth-overview)"""  # noqa
-
-        payload: Dict[str, Any] = {
-            "provider": provider,
-        }
-
-        if user_id is not None:
-            payload["user_id"] = user_id
-        if session_token is not None:
-            payload["session_token"] = session_token
+            data["session_duration_minutes"] = session_duration_minutes
         if session_jwt is not None:
-            payload["session_jwt"] = session_jwt
-
-        url = self.api_base.route_with_sub_url(self.sub_url, "attach")
-
-        res = self.sync_client.post(url, json=payload)
-        return AttachResponse.from_json(res.response.status_code, res.json)
-
-    async def attach_async(
-        self,
-        provider: str,
-        user_id: Optional[str] = None,
-        session_token: Optional[str] = None,
-        session_jwt: Optional[str] = None,
-    ) -> AttachResponse:
-        """[Stytch docs](https://stytch.com/docs/api/oauth-overview)"""  # noqa
-
-        payload: Dict[str, Any] = {
-            "provider": provider,
-        }
-
-        if user_id is not None:
-            payload["user_id"] = user_id
-        if session_token is not None:
-            payload["session_token"] = session_token
-        if session_jwt is not None:
-            payload["session_jwt"] = session_jwt
-
-        url = self.api_base.route_with_sub_url(self.sub_url, "attach")
+            data["session_jwt"] = session_jwt
+        if session_custom_claims is not None:
+            data["session_custom_claims"] = session_custom_claims
 
-        res = await self.async_client.post(url, json=payload)
-        return AttachResponse.from_json(res.response.status, res.json)
+        url = self.api_base.url_for("/v1/b2b/passwords/existing_password/reset", data)
+        res = await self.async_client.post(url, data)
+        return ResetResponse.from_json(res.response.status, res.json)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `stytch-6.9.0/stytch/api/passwords_existing_password.py` & `stytch-7.0.0/stytch/b2b/api/passwords_session.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,97 +1,81 @@
 # !!!
 # WARNING: This file is autogenerated
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
+from __future__ import annotations
+
 from typing import Any, Dict, Optional
 
+from stytch.b2b.models.passwords_session import ResetResponse
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
-from stytch.models.passwords_existing_password import ResetResponse
 
 
-class ExistingPassword:
+class Sessions:
     def __init__(
         self,
         api_base: ApiBase,
         sync_client: SyncClient,
         async_client: AsyncClient,
     ) -> None:
         self.api_base = api_base
         self.sync_client = sync_client
         self.async_client = async_client
 
-    @property
-    def sub_url(self) -> str:
-        return "passwords/existing_password"
-
     def reset(
         self,
-        email: str,
-        existing_password: str,
-        new_password: str,
+        organization_id: str,
+        password: str,
         session_token: Optional[str] = None,
         session_jwt: Optional[str] = None,
-        session_duration_minutes: Optional[int] = None,
-        session_custom_claims: Optional[Dict[str, Any]] = None,
     ) -> ResetResponse:
-        """[Stytch docs](https://stytch.com/docs/api/password-existing-password-reset)
+        """Reset the Member's password using their existing session. The endpoint will error if the session does not contain an authentication factor that has been issued within the last 5 minutes. Either `session_token` or `session_jwt` should be provided.
 
-        Reset the user’s password using their existing password.
+        Fields:
+          - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
+          - password: The password to authenticate.
+          - session_token: A secret token for a given Stytch Session.
+          - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
         """  # noqa
-
-        payload: Dict[str, Any] = {
-            "email": email,
-            "existing_password": existing_password,
-            "new_password": new_password,
+        data: Dict[str, Any] = {
+            "organization_id": organization_id,
+            "password": password,
         }
-
         if session_token is not None:
-            payload["session_token"] = session_token
+            data["session_token"] = session_token
         if session_jwt is not None:
-            payload["session_jwt"] = session_jwt
-        if session_duration_minutes is not None:
-            payload["session_duration_minutes"] = session_duration_minutes
-        if session_custom_claims is not None:
-            payload["session_custom_claims"] = session_custom_claims
+            data["session_jwt"] = session_jwt
 
-        url = self.api_base.route_with_sub_url(self.sub_url, "reset")
-
-        res = self.sync_client.post(url, json=payload)
+        url = self.api_base.url_for("/v1/b2b/passwords/session/reset", data)
+        res = self.sync_client.post(url, data)
         return ResetResponse.from_json(res.response.status_code, res.json)
 
     async def reset_async(
         self,
-        email: str,
-        existing_password: str,
-        new_password: str,
+        organization_id: str,
+        password: str,
         session_token: Optional[str] = None,
         session_jwt: Optional[str] = None,
-        session_duration_minutes: Optional[int] = None,
-        session_custom_claims: Optional[Dict[str, Any]] = None,
     ) -> ResetResponse:
-        """[Stytch docs](https://stytch.com/docs/api/password-existing-password-reset)
+        """Reset the Member's password using their existing session. The endpoint will error if the session does not contain an authentication factor that has been issued within the last 5 minutes. Either `session_token` or `session_jwt` should be provided.
 
-        Reset the user’s password using their existing password.
+        Fields:
+          - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
+          - password: The password to authenticate.
+          - session_token: A secret token for a given Stytch Session.
+          - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
         """  # noqa
-
-        payload: Dict[str, Any] = {
-            "email": email,
-            "existing_password": existing_password,
-            "new_password": new_password,
+        data: Dict[str, Any] = {
+            "organization_id": organization_id,
+            "password": password,
         }
-
         if session_token is not None:
-            payload["session_token"] = session_token
+            data["session_token"] = session_token
         if session_jwt is not None:
-            payload["session_jwt"] = session_jwt
-        if session_duration_minutes is not None:
-            payload["session_duration_minutes"] = session_duration_minutes
-        if session_custom_claims is not None:
-            payload["session_custom_claims"] = session_custom_claims
-
-        url = self.api_base.route_with_sub_url(self.sub_url, "reset")
+            data["session_jwt"] = session_jwt
 
-        res = await self.async_client.post(url, json=payload)
+        url = self.api_base.url_for("/v1/b2b/passwords/session/reset", data)
+        res = await self.async_client.post(url, data)
         return ResetResponse.from_json(res.response.status, res.json)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `stytch-6.9.0/stytch/b2b/api/discovery.py` & `stytch-7.0.0/stytch/b2b/api/discovery.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # !!!
 # WARNING: This file is autogenerated
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
+from __future__ import annotations
 
 from stytch.b2b.api.discovery_intermediate_sessions import IntermediateSessions
 from stytch.b2b.api.discovery_organizations import Organizations
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
 
 
@@ -17,15 +18,11 @@
         api_base: ApiBase,
         sync_client: SyncClient,
         async_client: AsyncClient,
     ) -> None:
         self.api_base = api_base
         self.sync_client = sync_client
         self.async_client = async_client
-        self.organizations = Organizations(api_base, sync_client, async_client)
         self.intermediate_sessions = IntermediateSessions(
             api_base, sync_client, async_client
         )
-
-    @property
-    def sub_url(self) -> str:
-        return "discovery"
+        self.organizations = Organizations(api_base, sync_client, async_client)
```

### Comparing `stytch-6.9.0/stytch/b2b/api/discovery_intermediate_sessions.py` & `stytch-7.0.0/stytch/b2b/api/discovery_intermediate_sessions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # !!!
 # WARNING: This file is autogenerated
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
+from __future__ import annotations
+
 from typing import Any, Dict, Optional
 
 from stytch.b2b.models.discovery_intermediate_sessions import ExchangeResponse
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
 
 
@@ -18,90 +20,96 @@
         sync_client: SyncClient,
         async_client: AsyncClient,
     ) -> None:
         self.api_base = api_base
         self.sync_client = sync_client
         self.async_client = async_client
 
-    @property
-    def sub_url(self) -> str:
-        return "discovery/intermediate_sessions"
-
     def exchange(
         self,
         intermediate_session_token: str,
         organization_id: str,
         session_duration_minutes: Optional[int] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
     ) -> ExchangeResponse:
-        """Exchange an Intermediate Session for a fully realized Member Session in a desired Organization. This operation consumes the Intermediate Session.
+        """Exchange an Intermediate Session for a fully realized [Member Session](https://stytch.com/docs/b2b/api/session-object) in a desired [Organization](https://stytch.com/docs/b2b/api/organization-object).
+        This operation consumes the Intermediate Session.
 
         This endpoint can be used to accept invites and create new members via domain matching.
 
-        Parameters:
-
-        - `intermediate_session_token`: The Intermediate Session Token to consume to create the new Member.
-
-        - `organization_id`: The UUID of the Organization to create the new Member and Member Session in.
-
-        - `session_duration_minutes`: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist, returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of five minutes regardless of the underlying session duration, and will need to be refreshed over time.
-            - This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
-            - If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
-            - If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want to use the Stytch session product, you can ignore the session fields in the response.
-
-        - `session_custom_claims`: Add a custom claims map to the session being authenticated. Claims will be included on the session object and in the JWT. To update a key in an existing session, supply a new value. To delete a key, supply a null value.
+        Fields:
+          - intermediate_session_token: The Intermediate Session Token. This token does not belong to a specific instance of a member, but may be exchanged for an existing Member Session or used to create a new organization.
+          - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
+          - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
+          returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
+          five minutes regardless of the underlying session duration, and will need to be refreshed over time.
+
+          This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
+
+          If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
+
+          If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
+          to use the Stytch session product, you can ignore the session fields in the response.
+          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
+          `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
+          delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
+          Total custom claims size cannot exceed four kilobytes.
         """  # noqa
-
-        payload: Dict[str, Any] = {
+        data: Dict[str, Any] = {
             "intermediate_session_token": intermediate_session_token,
             "organization_id": organization_id,
         }
-
         if session_duration_minutes is not None:
-            payload["session_duration_minutes"] = session_duration_minutes
+            data["session_duration_minutes"] = session_duration_minutes
         if session_custom_claims is not None:
-            payload["session_custom_claims"] = session_custom_claims
+            data["session_custom_claims"] = session_custom_claims
 
-        url = self.api_base.route_with_sub_url(self.sub_url, "exchange")
-
-        res = self.sync_client.post(url, json=payload)
+        url = self.api_base.url_for(
+            "/v1/b2b/discovery/intermediate_sessions/exchange", data
+        )
+        res = self.sync_client.post(url, data)
         return ExchangeResponse.from_json(res.response.status_code, res.json)
 
     async def exchange_async(
         self,
         intermediate_session_token: str,
         organization_id: str,
         session_duration_minutes: Optional[int] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
     ) -> ExchangeResponse:
-        """Exchange an Intermediate Session for a fully realized Member Session in a desired Organization. This operation consumes the Intermediate Session.
+        """Exchange an Intermediate Session for a fully realized [Member Session](https://stytch.com/docs/b2b/api/session-object) in a desired [Organization](https://stytch.com/docs/b2b/api/organization-object).
+        This operation consumes the Intermediate Session.
 
         This endpoint can be used to accept invites and create new members via domain matching.
 
-        Parameters:
-
-        - `intermediate_session_token`: The Intermediate Session Token to consume to create the new Member.
-
-        - `organization_id`: The UUID of the Organization to create the new Member and Member Session in.
-
-        - `session_duration_minutes`: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist, returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of five minutes regardless of the underlying session duration, and will need to be refreshed over time.
-            - This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
-            - If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
-            - If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want to use the Stytch session product, you can ignore the session fields in the response.
-
-        - `session_custom_claims`: Add a custom claims map to the session being authenticated. Claims will be included on the session object and in the JWT. To update a key in an existing session, supply a new value. To delete a key, supply a null value.
+        Fields:
+          - intermediate_session_token: The Intermediate Session Token. This token does not belong to a specific instance of a member, but may be exchanged for an existing Member Session or used to create a new organization.
+          - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
+          - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
+          returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
+          five minutes regardless of the underlying session duration, and will need to be refreshed over time.
+
+          This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
+
+          If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
+
+          If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
+          to use the Stytch session product, you can ignore the session fields in the response.
+          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
+          `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
+          delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
+          Total custom claims size cannot exceed four kilobytes.
         """  # noqa
-
-        payload: Dict[str, Any] = {
+        data: Dict[str, Any] = {
             "intermediate_session_token": intermediate_session_token,
             "organization_id": organization_id,
         }
-
         if session_duration_minutes is not None:
-            payload["session_duration_minutes"] = session_duration_minutes
+            data["session_duration_minutes"] = session_duration_minutes
         if session_custom_claims is not None:
-            payload["session_custom_claims"] = session_custom_claims
-
-        url = self.api_base.route_with_sub_url(self.sub_url, "exchange")
+            data["session_custom_claims"] = session_custom_claims
 
-        res = await self.async_client.post(url, json=payload)
+        url = self.api_base.url_for(
+            "/v1/b2b/discovery/intermediate_sessions/exchange", data
+        )
+        res = await self.async_client.post(url, data)
         return ExchangeResponse.from_json(res.response.status, res.json)
```

### Comparing `stytch-6.9.0/stytch/b2b/api/discovery_organizations.py` & `stytch-7.0.0/stytch/b2b/api/discovery_organizations.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # !!!
 # WARNING: This file is autogenerated
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
+from __future__ import annotations
+
 from typing import Any, Dict, List, Optional
 
 from stytch.b2b.models.discovery_organizations import CreateResponse, ListResponse
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
 
 
@@ -18,284 +20,300 @@
         sync_client: SyncClient,
         async_client: AsyncClient,
     ) -> None:
         self.api_base = api_base
         self.sync_client = sync_client
         self.async_client = async_client
 
-    @property
-    def sub_url(self) -> str:
-        return "discovery/organizations"
-
-    def list(
-        self,
-        intermediate_session_token: Optional[str] = None,
-        session_token: Optional[str] = None,
-        session_jwt: Optional[str] = None,
-    ) -> ListResponse:
-        """List all possible organization relationships connected to a Member Session or Intermediate Session.
-
-        When a Member Session is passed in, relationships with a type of `active_member`, `pending_member`, or `invited_member` will be returned, and any membership can be assumed by calling the [Exchange Session](https://stytch.com/docs/b2b/api/exchange-session) endpoint.
-
-        When an Intermediate Session is passed in, all relationship types - `active_member`, `pending_member`, `invited_member`, and `eligible_to_join_by_email_domain` - will be returned, and any membership can be assumed by calling the [Exchange Intermediate Session](https://stytch.com/docs/b2b/api/exchange-intermediate-session) endpoint.
-
-        This endpoint requires either an `intermediate_session_token`, `session_jwt` or `session_token` be included in the request. It will return an error if multiple are present.
-
-        This operation does not consume the Intermediate Session or Session Token passed in.
-
-        Parameters:
-
-        - `intermediate_session_token`: The intermediate session token.
-
-        - `session_token`: A secret token for a given Stytch Session.
-
-        - `session_jwt`: The JSON Web Token (JWT) for a given Stytch Session.
-        """  # noqa
-
-        payload: Dict[str, Any] = {}
-
-        if intermediate_session_token is not None:
-            payload["intermediate_session_token"] = intermediate_session_token
-        if session_token is not None:
-            payload["session_token"] = session_token
-        if session_jwt is not None:
-            payload["session_jwt"] = session_jwt
-
-        url = self.api_base.route_with_sub_url(self.sub_url, None)
-
-        res = self.sync_client.post(url, json=payload)
-        return ListResponse.from_json(res.response.status_code, res.json)
-
-    async def list_async(
-        self,
-        intermediate_session_token: Optional[str] = None,
-        session_token: Optional[str] = None,
-        session_jwt: Optional[str] = None,
-    ) -> ListResponse:
-        """List all possible organization relationships connected to a Member Session or Intermediate Session.
-
-        When a Member Session is passed in, relationships with a type of `active_member`, `pending_member`, or `invited_member` will be returned, and any membership can be assumed by calling the [Exchange Session](https://stytch.com/docs/b2b/api/exchange-session) endpoint.
-
-        When an Intermediate Session is passed in, all relationship types - `active_member`, `pending_member`, `invited_member`, and `eligible_to_join_by_email_domain` - will be returned, and any membership can be assumed by calling the [Exchange Intermediate Session](https://stytch.com/docs/b2b/api/exchange-intermediate-session) endpoint.
-
-        This endpoint requires either an `intermediate_session_token`, `session_jwt` or `session_token` be included in the request. It will return an error if multiple are present.
-
-        This operation does not consume the Intermediate Session or Session Token passed in.
-
-        Parameters:
-
-        - `intermediate_session_token`: The intermediate session token.
-
-        - `session_token`: A secret token for a given Stytch Session.
-
-        - `session_jwt`: The JSON Web Token (JWT) for a given Stytch Session.
-        """  # noqa
-
-        payload: Dict[str, Any] = {}
-
-        if intermediate_session_token is not None:
-            payload["intermediate_session_token"] = intermediate_session_token
-        if session_token is not None:
-            payload["session_token"] = session_token
-        if session_jwt is not None:
-            payload["session_jwt"] = session_jwt
-
-        url = self.api_base.route_with_sub_url(self.sub_url, None)
-
-        res = await self.async_client.post(url, json=payload)
-        return ListResponse.from_json(res.response.status, res.json)
-
     def create(
         self,
         intermediate_session_token: str,
         organization_name: str,
         organization_slug: str,
         session_duration_minutes: Optional[int] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
         organization_logo_url: Optional[str] = None,
         trusted_metadata: Optional[Dict[str, Any]] = None,
+        sso_jit_provisioning: Optional[str] = None,
+        email_allowed_domains: Optional[List[str]] = None,
         email_jit_provisioning: Optional[str] = None,
         email_invites: Optional[str] = None,
-        email_allowed_domains: Optional[List[str]] = None,
-        sso_jit_provisioning: Optional[str] = None,
         auth_methods: Optional[str] = None,
         allowed_auth_methods: Optional[List[str]] = None,
     ) -> CreateResponse:
-        """If an end user does not want to join any already-existing organization, or has no possible organizations to join, this endpoint can be used to create a new Organization and Member.
+        """If an end user does not want to join any already-existing organization, or has no possible organizations to join, this endpoint can be used to create a new
+        [Organization](https://stytch.com/docs/b2b/api/organization-object) and [Member](https://stytch.com/docs/b2b/api/member-object).
 
         This operation consumes the Intermediate Session.
 
         This endpoint can also be used to start an initial session for the newly created member and organization.
 
-        Parameters:
+        Fields:
+          - intermediate_session_token: The Intermediate Session Token. This token does not belong to a specific instance of a member, but may be exchanged for an existing Member Session or used to create a new organization.
+          - organization_name: The name of the Organization. If the name is not specified, a default name will be created based on the email used to initiate the discovery flow. If the email domain is a common email provider such as gmail.com, or if the email is a .edu email, the organization name will be generated based on the name portion of the email. Otherwise, the organization name will be generated based on the email domain.
+          - organization_slug: The unique URL slug of the Organization. A minimum of two characters is required. The slug only accepts alphanumeric characters and the following reserved characters: `-` `.` `_` `~`. If the slug is not specified, a default slug will be created based on the email used to initiate the discovery flow. If the email domain is a common email provider such as gmail.com, or if the email is a .edu email, the organization slug will be generated based on the name portion of the email. Otherwise, the organization slug will be generated based on the email domain.
+          - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
+          returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
+          five minutes regardless of the underlying session duration, and will need to be refreshed over time.
 
-        - `intermediate_session_token`: The Intermediate Session Token to consume to create the new Organization and Member.
+          This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
 
-        - `session_duration_minutes`: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist, returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of five minutes regardless of the underlying session duration, and will need to be refreshed over time.
-          - This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
-          - If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
-          - If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want to use the Stytch session product, you can ignore the session fields in the response.
+          If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
 
-        - `session_custom_claims`: Add a custom claims map to the session being authenticated. Claims will be included on the session object and in the JWT. To update a key in an existing session, supply a new value. To delete a key, supply a null value.
+          If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
+          to use the Stytch session product, you can ignore the session fields in the response.
+          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
+          `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
+          delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
+          Total custom claims size cannot exceed four kilobytes.
+          - organization_logo_url: The image URL of the Organization logo.
+          - trusted_metadata: An arbitrary JSON object for storing application-specific data or identity-provider-specific data.
+          - sso_jit_provisioning: The authentication setting that controls the JIT provisioning of Members when authenticating via SSO. The accepted values are:
 
-        - `organization_name`: The name of the Organization.
+          `ALL_ALLOWED` – new Members will be automatically provisioned upon successful authentication via any of the Organization's `sso_active_connections`.
 
-        - `organization_slug`: The unique URL slug of the Organization.
+          `RESTRICTED` – only new Members with SSO logins that comply with `sso_jit_provisioning_allowed_connections` can be provisioned upon authentication.
 
-        - `organization_logo_url`: The image URL of the Organization’s logo.
+          `NOT_ALLOWED` – disable JIT provisioning via SSO.
 
-        - `trusted_metadata`: An arbitrary JSON object for storing application-specific data.
+          - email_allowed_domains: An array of email domains that allow invites or JIT provisioning for new Members. This list is enforced when either `email_invites` or `email_jit_provisioning` is set to `RESTRICTED`.
 
-        - `email_jit_provisioning`: The setting that controls the JIT provisioning of new Members when authenticating via email. The accepted values are:
 
-            - RESTRICTED – only new Members with verified emails that comply with `email_allowed_domains` can be provisioned upon authentication.
-            - NOT_ALLOWED – disable JIT provisioning.
+            Common domains such as `gmail.com` are not allowed. See the [common email domains resource](https://stytch.com/docs/b2b/api/common-email-domains) for the full list.
+          - email_jit_provisioning: The authentication setting that controls how a new Member can be provisioned by authenticating via Email Magic Link. The accepted values are:
 
-        - `email_invites`: The setting that controls how a new Member can be invited to an organization by email. The accepted values are:
+          `RESTRICTED` – only new Members with verified emails that comply with `email_allowed_domains` can be provisioned upon authentication via Email Magic Link.
 
-            - ALL_ALLOWED – any new Member can be invited to join
-            - RESTRICTED – only new Members with verified emails that comply with `email_allowed_domains` can be invited
-            - NOT_ALLOWED – disable invites
+          `NOT_ALLOWED` – disable JIT provisioning via Email Magic Link.
 
-        - `email_allowed_domains`: An array of email domains that allow invitations or JIT provisioning for new Members. This list is enforced when either email_invites or email_jit_provisioning is set to RESTRICTED.
+          - email_invites: The authentication setting that controls how a new Member can be invited to an organization by email. The accepted values are:
 
-        - `sso_jit_provisioning`: The setting that controls the JIT provisioning of Members when authenticating via SSO. The accepted values are:
-            - ALL_ALLOWED – any new Member can be provisioned upon authentication
-            - RESTRICTED – only new Members with SSO logins that comply with `sso_jit_provisioning_allowed_connections` can be provisioned upon authentication
-            - NOT_ALLOWED – disable JIT provisioning
+          `ALL_ALLOWED` – any new Member can be invited to join via email.
 
-        - `auth_methods`: The setting that controls which authentication methods can be used by Members of an Organization. The accepted values are:
-            - ALL_ALLOWED – the default setting which allows all authentication methods to be used.
-            - RESTRICTED - only methods that comply with `allowed_auth_methods` can be used for authentication. This setting does not apply to Members with `is_breakglass` set to `true`.
+          `RESTRICTED` – only new Members with verified emails that comply with `email_allowed_domains` can be invited via email.
 
-        - `allowed_auth_methods`: An array of allowed authentication methods. This list is enforced when auth_methods is set to RESTRICTED. The list's accepted values are: `sso`, `magic_link`, and `password`.
-        """  # noqa
+          `NOT_ALLOWED` – disable email invites.
+
+          - auth_methods: The setting that controls which authentication methods can be used by Members of an Organization. The accepted values are:
+
+          `ALL_ALLOWED` – the default setting which allows all authentication methods to be used.
+
+          `RESTRICTED` – only methods that comply with `allowed_auth_methods` can be used for authentication. This setting does not apply to Members with `is_breakglass` set to `true`.
+
+          - allowed_auth_methods:
+          An array of allowed authentication methods. This list is enforced when `auth_methods` is set to `RESTRICTED`.
+          The list's accepted values are: `sso`, `magic_link`, `password`, `google_oauth`, and `microsoft_oauth`.
 
-        payload: Dict[str, Any] = {
+        """  # noqa
+        data: Dict[str, Any] = {
             "intermediate_session_token": intermediate_session_token,
             "organization_name": organization_name,
             "organization_slug": organization_slug,
         }
-
         if session_duration_minutes is not None:
-            payload["session_duration_minutes"] = session_duration_minutes
+            data["session_duration_minutes"] = session_duration_minutes
         if session_custom_claims is not None:
-            payload["session_custom_claims"] = session_custom_claims
+            data["session_custom_claims"] = session_custom_claims
         if organization_logo_url is not None:
-            payload["organization_logo_url"] = organization_logo_url
+            data["organization_logo_url"] = organization_logo_url
         if trusted_metadata is not None:
-            payload["trusted_metadata"] = trusted_metadata
+            data["trusted_metadata"] = trusted_metadata
+        if sso_jit_provisioning is not None:
+            data["sso_jit_provisioning"] = sso_jit_provisioning
+        if email_allowed_domains is not None:
+            data["email_allowed_domains"] = email_allowed_domains
         if email_jit_provisioning is not None:
-            payload["email_jit_provisioning"] = email_jit_provisioning
+            data["email_jit_provisioning"] = email_jit_provisioning
         if email_invites is not None:
-            payload["email_invites"] = email_invites
-        if email_allowed_domains is not None:
-            payload["email_allowed_domains"] = email_allowed_domains
-        if sso_jit_provisioning is not None:
-            payload["sso_jit_provisioning"] = sso_jit_provisioning
+            data["email_invites"] = email_invites
         if auth_methods is not None:
-            payload["auth_methods"] = auth_methods
+            data["auth_methods"] = auth_methods
         if allowed_auth_methods is not None:
-            payload["allowed_auth_methods"] = allowed_auth_methods
+            data["allowed_auth_methods"] = allowed_auth_methods
 
-        url = self.api_base.route_with_sub_url(self.sub_url, "create")
-
-        res = self.sync_client.post(url, json=payload)
+        url = self.api_base.url_for("/v1/b2b/discovery/organizations/create", data)
+        res = self.sync_client.post(url, data)
         return CreateResponse.from_json(res.response.status_code, res.json)
 
     async def create_async(
         self,
         intermediate_session_token: str,
         organization_name: str,
         organization_slug: str,
         session_duration_minutes: Optional[int] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
         organization_logo_url: Optional[str] = None,
         trusted_metadata: Optional[Dict[str, Any]] = None,
+        sso_jit_provisioning: Optional[str] = None,
+        email_allowed_domains: Optional[List[str]] = None,
         email_jit_provisioning: Optional[str] = None,
         email_invites: Optional[str] = None,
-        email_allowed_domains: Optional[List[str]] = None,
-        sso_jit_provisioning: Optional[str] = None,
         auth_methods: Optional[str] = None,
         allowed_auth_methods: Optional[List[str]] = None,
     ) -> CreateResponse:
-        """If an end user does not want to join any already-existing organization, or has no possible organizations to join, this endpoint can be used to create a new Organization and Member.
+        """If an end user does not want to join any already-existing organization, or has no possible organizations to join, this endpoint can be used to create a new
+        [Organization](https://stytch.com/docs/b2b/api/organization-object) and [Member](https://stytch.com/docs/b2b/api/member-object).
 
         This operation consumes the Intermediate Session.
 
         This endpoint can also be used to start an initial session for the newly created member and organization.
 
-        Parameters:
+        Fields:
+          - intermediate_session_token: The Intermediate Session Token. This token does not belong to a specific instance of a member, but may be exchanged for an existing Member Session or used to create a new organization.
+          - organization_name: The name of the Organization. If the name is not specified, a default name will be created based on the email used to initiate the discovery flow. If the email domain is a common email provider such as gmail.com, or if the email is a .edu email, the organization name will be generated based on the name portion of the email. Otherwise, the organization name will be generated based on the email domain.
+          - organization_slug: The unique URL slug of the Organization. A minimum of two characters is required. The slug only accepts alphanumeric characters and the following reserved characters: `-` `.` `_` `~`. If the slug is not specified, a default slug will be created based on the email used to initiate the discovery flow. If the email domain is a common email provider such as gmail.com, or if the email is a .edu email, the organization slug will be generated based on the name portion of the email. Otherwise, the organization slug will be generated based on the email domain.
+          - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
+          returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
+          five minutes regardless of the underlying session duration, and will need to be refreshed over time.
 
-        - `intermediate_session_token`: The Intermediate Session Token to consume to create the new Organization and Member.
+          This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
 
-        - `session_duration_minutes`: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist, returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of five minutes regardless of the underlying session duration, and will need to be refreshed over time.
-          - This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
-          - If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
-          - If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want to use the Stytch session product, you can ignore the session fields in the response.
+          If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
 
-        - `session_custom_claims`: Add a custom claims map to the session being authenticated. Claims will be included on the session object and in the JWT. To update a key in an existing session, supply a new value. To delete a key, supply a null value.
+          If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
+          to use the Stytch session product, you can ignore the session fields in the response.
+          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
+          `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
+          delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
+          Total custom claims size cannot exceed four kilobytes.
+          - organization_logo_url: The image URL of the Organization logo.
+          - trusted_metadata: An arbitrary JSON object for storing application-specific data or identity-provider-specific data.
+          - sso_jit_provisioning: The authentication setting that controls the JIT provisioning of Members when authenticating via SSO. The accepted values are:
 
-        - `organization_name`: The name of the Organization.
+          `ALL_ALLOWED` – new Members will be automatically provisioned upon successful authentication via any of the Organization's `sso_active_connections`.
 
-        - `organization_slug`: The unique URL slug of the Organization.
+          `RESTRICTED` – only new Members with SSO logins that comply with `sso_jit_provisioning_allowed_connections` can be provisioned upon authentication.
 
-        - `organization_logo_url`: The image URL of the Organization’s logo.
+          `NOT_ALLOWED` – disable JIT provisioning via SSO.
 
-        - `trusted_metadata`: An arbitrary JSON object for storing application-specific data.
+          - email_allowed_domains: An array of email domains that allow invites or JIT provisioning for new Members. This list is enforced when either `email_invites` or `email_jit_provisioning` is set to `RESTRICTED`.
 
-        - `email_jit_provisioning`: The setting that controls the JIT provisioning of new Members when authenticating via email. The accepted values are:
 
-            - RESTRICTED – only new Members with verified emails that comply with `email_allowed_domains` can be provisioned upon authentication.
-            - NOT_ALLOWED – disable JIT provisioning.
+            Common domains such as `gmail.com` are not allowed. See the [common email domains resource](https://stytch.com/docs/b2b/api/common-email-domains) for the full list.
+          - email_jit_provisioning: The authentication setting that controls how a new Member can be provisioned by authenticating via Email Magic Link. The accepted values are:
 
-        - `email_invites`: The setting that controls how a new Member can be invited to an organization by email. The accepted values are:
+          `RESTRICTED` – only new Members with verified emails that comply with `email_allowed_domains` can be provisioned upon authentication via Email Magic Link.
 
-            - ALL_ALLOWED – any new Member can be invited to join
-            - RESTRICTED – only new Members with verified emails that comply with `email_allowed_domains` can be invited
-            - NOT_ALLOWED – disable invites
+          `NOT_ALLOWED` – disable JIT provisioning via Email Magic Link.
 
-        - `email_allowed_domains`: An array of email domains that allow invitations or JIT provisioning for new Members. This list is enforced when either email_invites or email_jit_provisioning is set to RESTRICTED.
+          - email_invites: The authentication setting that controls how a new Member can be invited to an organization by email. The accepted values are:
 
-        - `sso_jit_provisioning`: The setting that controls the JIT provisioning of Members when authenticating via SSO. The accepted values are:
-            - ALL_ALLOWED – any new Member can be provisioned upon authentication
-            - RESTRICTED – only new Members with SSO logins that comply with `sso_jit_provisioning_allowed_connections` can be provisioned upon authentication
-            - NOT_ALLOWED – disable JIT provisioning
+          `ALL_ALLOWED` – any new Member can be invited to join via email.
 
-        - `auth_methods`: The setting that controls which authentication methods can be used by Members of an Organization. The accepted values are:
-            - ALL_ALLOWED – the default setting which allows all authentication methods to be used.
-            - RESTRICTED - only methods that comply with `allowed_auth_methods` can be used for authentication. This setting does not apply to Members with `is_breakglass` set to `true`.
+          `RESTRICTED` – only new Members with verified emails that comply with `email_allowed_domains` can be invited via email.
 
-        - `allowed_auth_methods`: An array of allowed authentication methods. This list is enforced when auth_methods is set to RESTRICTED. The list's accepted values are: `sso`, `magic_link`, and `password`.
-        """  # noqa
+          `NOT_ALLOWED` – disable email invites.
+
+          - auth_methods: The setting that controls which authentication methods can be used by Members of an Organization. The accepted values are:
+
+          `ALL_ALLOWED` – the default setting which allows all authentication methods to be used.
+
+          `RESTRICTED` – only methods that comply with `allowed_auth_methods` can be used for authentication. This setting does not apply to Members with `is_breakglass` set to `true`.
+
+          - allowed_auth_methods:
+          An array of allowed authentication methods. This list is enforced when `auth_methods` is set to `RESTRICTED`.
+          The list's accepted values are: `sso`, `magic_link`, `password`, `google_oauth`, and `microsoft_oauth`.
 
-        payload: Dict[str, Any] = {
+        """  # noqa
+        data: Dict[str, Any] = {
             "intermediate_session_token": intermediate_session_token,
             "organization_name": organization_name,
             "organization_slug": organization_slug,
         }
-
         if session_duration_minutes is not None:
-            payload["session_duration_minutes"] = session_duration_minutes
+            data["session_duration_minutes"] = session_duration_minutes
         if session_custom_claims is not None:
-            payload["session_custom_claims"] = session_custom_claims
+            data["session_custom_claims"] = session_custom_claims
         if organization_logo_url is not None:
-            payload["organization_logo_url"] = organization_logo_url
+            data["organization_logo_url"] = organization_logo_url
         if trusted_metadata is not None:
-            payload["trusted_metadata"] = trusted_metadata
+            data["trusted_metadata"] = trusted_metadata
+        if sso_jit_provisioning is not None:
+            data["sso_jit_provisioning"] = sso_jit_provisioning
+        if email_allowed_domains is not None:
+            data["email_allowed_domains"] = email_allowed_domains
         if email_jit_provisioning is not None:
-            payload["email_jit_provisioning"] = email_jit_provisioning
+            data["email_jit_provisioning"] = email_jit_provisioning
         if email_invites is not None:
-            payload["email_invites"] = email_invites
-        if email_allowed_domains is not None:
-            payload["email_allowed_domains"] = email_allowed_domains
-        if sso_jit_provisioning is not None:
-            payload["sso_jit_provisioning"] = sso_jit_provisioning
+            data["email_invites"] = email_invites
         if auth_methods is not None:
-            payload["auth_methods"] = auth_methods
+            data["auth_methods"] = auth_methods
         if allowed_auth_methods is not None:
-            payload["allowed_auth_methods"] = allowed_auth_methods
+            data["allowed_auth_methods"] = allowed_auth_methods
 
-        url = self.api_base.route_with_sub_url(self.sub_url, "create")
-
-        res = await self.async_client.post(url, json=payload)
+        url = self.api_base.url_for("/v1/b2b/discovery/organizations/create", data)
+        res = await self.async_client.post(url, data)
         return CreateResponse.from_json(res.response.status, res.json)
+
+    def list(
+        self,
+        intermediate_session_token: Optional[str] = None,
+        session_token: Optional[str] = None,
+        session_jwt: Optional[str] = None,
+    ) -> ListResponse:
+        """List all possible organization relationships connected to a [Member Session](https://stytch.com/docs/b2b/api/session-object) or Intermediate Session.
+
+        When a Member Session is passed in, relationships with a type of `active_member`, `pending_member`, or `invited_member`
+        will be returned, and any membership can be assumed by calling the [Exchange Session](https://stytch.com/docs/b2b/api/exchange-session) endpoint.
+
+        When an Intermediate Session is passed in, all relationship types - `active_member`, `pending_member`, `invited_member`,
+        and `eligible_to_join_by_email_domain` - will be returned,
+        and any membership can be assumed by calling the [Exchange Intermediate Session](https://stytch.com/docs/b2b/api/exchange-intermediate-session) endpoint.
+
+        This endpoint requires either an `intermediate_session_token`, `session_jwt` or `session_token` be included in the request.
+        It will return an error if multiple are present.
+
+        This operation does not consume the Intermediate Session or Session Token passed in.
+
+        Fields:
+          - intermediate_session_token: The Intermediate Session Token. This token does not belong to a specific instance of a member, but may be exchanged for an existing Member Session or used to create a new organization.
+          - session_token: A secret token for a given Stytch Session.
+          - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
+        """  # noqa
+        data: Dict[str, Any] = {}
+        if intermediate_session_token is not None:
+            data["intermediate_session_token"] = intermediate_session_token
+        if session_token is not None:
+            data["session_token"] = session_token
+        if session_jwt is not None:
+            data["session_jwt"] = session_jwt
+
+        url = self.api_base.url_for("/v1/b2b/discovery/organizations", data)
+        res = self.sync_client.post(url, data)
+        return ListResponse.from_json(res.response.status_code, res.json)
+
+    async def list_async(
+        self,
+        intermediate_session_token: Optional[str] = None,
+        session_token: Optional[str] = None,
+        session_jwt: Optional[str] = None,
+    ) -> ListResponse:
+        """List all possible organization relationships connected to a [Member Session](https://stytch.com/docs/b2b/api/session-object) or Intermediate Session.
+
+        When a Member Session is passed in, relationships with a type of `active_member`, `pending_member`, or `invited_member`
+        will be returned, and any membership can be assumed by calling the [Exchange Session](https://stytch.com/docs/b2b/api/exchange-session) endpoint.
+
+        When an Intermediate Session is passed in, all relationship types - `active_member`, `pending_member`, `invited_member`,
+        and `eligible_to_join_by_email_domain` - will be returned,
+        and any membership can be assumed by calling the [Exchange Intermediate Session](https://stytch.com/docs/b2b/api/exchange-intermediate-session) endpoint.
+
+        This endpoint requires either an `intermediate_session_token`, `session_jwt` or `session_token` be included in the request.
+        It will return an error if multiple are present.
+
+        This operation does not consume the Intermediate Session or Session Token passed in.
+
+        Fields:
+          - intermediate_session_token: The Intermediate Session Token. This token does not belong to a specific instance of a member, but may be exchanged for an existing Member Session or used to create a new organization.
+          - session_token: A secret token for a given Stytch Session.
+          - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
+        """  # noqa
+        data: Dict[str, Any] = {}
+        if intermediate_session_token is not None:
+            data["intermediate_session_token"] = intermediate_session_token
+        if session_token is not None:
+            data["session_token"] = session_token
+        if session_jwt is not None:
+            data["session_jwt"] = session_jwt
+
+        url = self.api_base.url_for("/v1/b2b/discovery/organizations", data)
+        res = await self.async_client.post(url, data)
+        return ListResponse.from_json(res.response.status, res.json)
```

### Comparing `stytch-6.9.0/stytch/b2b/api/magic_links.py` & `stytch-7.0.0/stytch/b2b/api/magic_links.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # !!!
 # WARNING: This file is autogenerated
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
+from __future__ import annotations
+
 from typing import Any, Dict, Optional
 
 from stytch.b2b.api.magic_links_discovery import Discovery
 from stytch.b2b.api.magic_links_email import Email
 from stytch.b2b.models.magic_links import AuthenticateResponse
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
@@ -22,104 +24,112 @@
     ) -> None:
         self.api_base = api_base
         self.sync_client = sync_client
         self.async_client = async_client
         self.email = Email(api_base, sync_client, async_client)
         self.discovery = Discovery(api_base, sync_client, async_client)
 
-    @property
-    def sub_url(self) -> str:
-        return "magic_links"
-
     def authenticate(
         self,
         magic_links_token: str,
         pkce_code_verifier: Optional[str] = None,
         session_token: Optional[str] = None,
         session_jwt: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
     ) -> AuthenticateResponse:
-        """Authenticate a Member with a magic link. This endpoint requires a magic link token to validate, making sure it's not expired or previously used. If the Member’s status is invited or pending, they will be updated to active.
-
-        Parameters:
-
-        - `magic_links_token`: The token to authenticate.
-
-        - `pkce_code_verifier`: A base64url encoded one-time secret used to validate that the request starts and ends on the same device.
+        """Authenticate a Member with a Magic Link. This endpoint requires a Magic Link token that is not expired or previously used. If the Member’s status is `pending` or `invited`, they will be updated to `active`. Provide the `session_duration_minutes` parameter to set the lifetime of the session. If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration.
 
-        - `session_token`: A secret token for a given Stytch Session. Read more about session_token in our Session management guide.
-
-        - `session_jwt`: The JSON Web Token (JWT) for a given Stytch Session. Read more about session_token in our Session management guide.
-
-        - `session_duration_minutes`: The Session lifetime of this many minutes from now; minimum of 5 and a maximum of 129600 minutes (90 days). Note that a successful authentication will continue to extend the Session this many minutes.
-
-        - `session_custom_claims`: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in Session duration minutes. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To delete a key, supply a null value.
-          Custom claims made with reserved claims ("iss", "sub", "aud", "exp", "nbf", "iat", "jti") will be ignored. Total custom claims size cannot exceed four kilobytes
+        Fields:
+          - magic_links_token: The Email Magic Link token to authenticate.
+          - pkce_code_verifier: A base64url encoded one time secret used to validate that the request starts and ends on the same device.
+          - session_token: Reuse an existing session instead of creating a new one. If you provide a `session_token`, Stytch will update the session.
+              If the `session_token` and `magic_links_token` belong to different Members, the `session_token` will be ignored. This endpoint will error if
+              both `session_token` and `session_jwt` are provided.
+          - session_jwt: Reuse an existing session instead of creating a new one. If you provide a `session_jwt`, Stytch will update the session. If the `session_jwt`
+              and `magic_links_token` belong to different Members, the `session_jwt` will be ignored. This endpoint will error if both `session_token` and `session_jwt`
+              are provided.
+          - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
+          returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
+          five minutes regardless of the underlying session duration, and will need to be refreshed over time.
+
+          This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
+
+          If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
+
+          If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
+          to use the Stytch session product, you can ignore the session fields in the response.
+          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
+          `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
+          delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
+          Total custom claims size cannot exceed four kilobytes.
         """  # noqa
-
-        payload: Dict[str, Any] = {
+        data: Dict[str, Any] = {
             "magic_links_token": magic_links_token,
         }
-
         if pkce_code_verifier is not None:
-            payload["pkce_code_verifier"] = pkce_code_verifier
+            data["pkce_code_verifier"] = pkce_code_verifier
         if session_token is not None:
-            payload["session_token"] = session_token
+            data["session_token"] = session_token
         if session_jwt is not None:
-            payload["session_jwt"] = session_jwt
+            data["session_jwt"] = session_jwt
         if session_duration_minutes is not None:
-            payload["session_duration_minutes"] = session_duration_minutes
+            data["session_duration_minutes"] = session_duration_minutes
         if session_custom_claims is not None:
-            payload["session_custom_claims"] = session_custom_claims
+            data["session_custom_claims"] = session_custom_claims
 
-        url = self.api_base.route_with_sub_url(self.sub_url, "authenticate")
-
-        res = self.sync_client.post(url, json=payload)
+        url = self.api_base.url_for("/v1/b2b/magic_links/authenticate", data)
+        res = self.sync_client.post(url, data)
         return AuthenticateResponse.from_json(res.response.status_code, res.json)
 
     async def authenticate_async(
         self,
         magic_links_token: str,
         pkce_code_verifier: Optional[str] = None,
         session_token: Optional[str] = None,
         session_jwt: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
     ) -> AuthenticateResponse:
-        """Authenticate a Member with a magic link. This endpoint requires a magic link token to validate, making sure it's not expired or previously used. If the Member’s status is invited or pending, they will be updated to active.
-
-        Parameters:
-
-        - `magic_links_token`: The token to authenticate.
-
-        - `pkce_code_verifier`: A base64url encoded one-time secret used to validate that the request starts and ends on the same device.
-
-        - `session_token`: A secret token for a given Stytch Session. Read more about session_token in our Session management guide.
+        """Authenticate a Member with a Magic Link. This endpoint requires a Magic Link token that is not expired or previously used. If the Member’s status is `pending` or `invited`, they will be updated to `active`. Provide the `session_duration_minutes` parameter to set the lifetime of the session. If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration.
 
-        - `session_jwt`: The JSON Web Token (JWT) for a given Stytch Session. Read more about session_token in our Session management guide.
-
-        - `session_duration_minutes`: The Session lifetime of this many minutes from now; minimum of 5 and a maximum of 129600 minutes (90 days). Note that a successful authentication will continue to extend the Session this many minutes.
-
-        - `session_custom_claims`: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in Session duration minutes. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To delete a key, supply a null value.
-          Custom claims made with reserved claims ("iss", "sub", "aud", "exp", "nbf", "iat", "jti") will be ignored. Total custom claims size cannot exceed four kilobytes
+        Fields:
+          - magic_links_token: The Email Magic Link token to authenticate.
+          - pkce_code_verifier: A base64url encoded one time secret used to validate that the request starts and ends on the same device.
+          - session_token: Reuse an existing session instead of creating a new one. If you provide a `session_token`, Stytch will update the session.
+              If the `session_token` and `magic_links_token` belong to different Members, the `session_token` will be ignored. This endpoint will error if
+              both `session_token` and `session_jwt` are provided.
+          - session_jwt: Reuse an existing session instead of creating a new one. If you provide a `session_jwt`, Stytch will update the session. If the `session_jwt`
+              and `magic_links_token` belong to different Members, the `session_jwt` will be ignored. This endpoint will error if both `session_token` and `session_jwt`
+              are provided.
+          - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
+          returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
+          five minutes regardless of the underlying session duration, and will need to be refreshed over time.
+
+          This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
+
+          If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
+
+          If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
+          to use the Stytch session product, you can ignore the session fields in the response.
+          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
+          `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
+          delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
+          Total custom claims size cannot exceed four kilobytes.
         """  # noqa
-
-        payload: Dict[str, Any] = {
+        data: Dict[str, Any] = {
             "magic_links_token": magic_links_token,
         }
-
         if pkce_code_verifier is not None:
-            payload["pkce_code_verifier"] = pkce_code_verifier
+            data["pkce_code_verifier"] = pkce_code_verifier
         if session_token is not None:
-            payload["session_token"] = session_token
+            data["session_token"] = session_token
         if session_jwt is not None:
-            payload["session_jwt"] = session_jwt
+            data["session_jwt"] = session_jwt
         if session_duration_minutes is not None:
-            payload["session_duration_minutes"] = session_duration_minutes
+            data["session_duration_minutes"] = session_duration_minutes
         if session_custom_claims is not None:
-            payload["session_custom_claims"] = session_custom_claims
-
-        url = self.api_base.route_with_sub_url(self.sub_url, "authenticate")
+            data["session_custom_claims"] = session_custom_claims
 
-        res = await self.async_client.post(url, json=payload)
+        url = self.api_base.url_for("/v1/b2b/magic_links/authenticate", data)
+        res = await self.async_client.post(url, data)
         return AuthenticateResponse.from_json(res.response.status, res.json)
```

### Comparing `stytch-6.9.0/stytch/b2b/api/magic_links_discovery.py` & `stytch-7.0.0/stytch/b2b/api/magic_links_discovery.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # !!!
 # WARNING: This file is autogenerated
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
+from __future__ import annotations
+
 from typing import Any, Dict, Optional
 
 from stytch.b2b.models.magic_links_discovery import AuthenticateResponse
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
 
 
@@ -18,62 +20,48 @@
         sync_client: SyncClient,
         async_client: AsyncClient,
     ) -> None:
         self.api_base = api_base
         self.sync_client = sync_client
         self.async_client = async_client
 
-    @property
-    def sub_url(self) -> str:
-        return "magic_links/discovery"
-
     def authenticate(
         self,
         discovery_magic_links_token: str,
         pkce_code_verifier: Optional[str] = None,
     ) -> AuthenticateResponse:
-        """Authenticates the discovery Magic Link token and exchanges it for an Intermediate Session Token. Intermediate Session Tokens can be used for various [Discovery](https://stytch.com/docs/b2b/api/discovery-overview) login flows and are valid for 10 minutes.
-
-        Parameters:
+        """Authenticates the Discovery Magic Link token and exchanges it for an Intermediate Session Token. Intermediate Session Tokens can be used for various Discovery login flows and are valid for 10 minutes.
 
-        - `discovery_magic_links_token`: The Discovery Email Magic Link token to authenticate.
-
-        - `pkce_code_verifier`: A base64url encoded one time secret used to validate that the request starts and ends on the same device.
+        Fields:
+          - discovery_magic_links_token: The Discovery Email Magic Link token to authenticate.
+          - pkce_code_verifier: A base64url encoded one time secret used to validate that the request starts and ends on the same device.
         """  # noqa
-
-        payload: Dict[str, Any] = {
+        data: Dict[str, Any] = {
             "discovery_magic_links_token": discovery_magic_links_token,
         }
-
         if pkce_code_verifier is not None:
-            payload["pkce_code_verifier"] = pkce_code_verifier
+            data["pkce_code_verifier"] = pkce_code_verifier
 
-        url = self.api_base.route_with_sub_url(self.sub_url, "authenticate")
-
-        res = self.sync_client.post(url, json=payload)
+        url = self.api_base.url_for("/v1/b2b/magic_links/discovery/authenticate", data)
+        res = self.sync_client.post(url, data)
         return AuthenticateResponse.from_json(res.response.status_code, res.json)
 
     async def authenticate_async(
         self,
         discovery_magic_links_token: str,
         pkce_code_verifier: Optional[str] = None,
     ) -> AuthenticateResponse:
-        """Authenticates the discovery Magic Link token and exchanges it for an Intermediate Session Token. Intermediate Session Tokens can be used for various [Discovery](https://stytch.com/docs/b2b/api/discovery-overview) login flows and are valid for 10 minutes.
-
-        Parameters:
-
-        - `discovery_magic_links_token`: The Discovery Email Magic Link token to authenticate.
+        """Authenticates the Discovery Magic Link token and exchanges it for an Intermediate Session Token. Intermediate Session Tokens can be used for various Discovery login flows and are valid for 10 minutes.
 
-        - `pkce_code_verifier`: A base64url encoded one time secret used to validate that the request starts and ends on the same device.
+        Fields:
+          - discovery_magic_links_token: The Discovery Email Magic Link token to authenticate.
+          - pkce_code_verifier: A base64url encoded one time secret used to validate that the request starts and ends on the same device.
         """  # noqa
-
-        payload: Dict[str, Any] = {
+        data: Dict[str, Any] = {
             "discovery_magic_links_token": discovery_magic_links_token,
         }
-
         if pkce_code_verifier is not None:
-            payload["pkce_code_verifier"] = pkce_code_verifier
-
-        url = self.api_base.route_with_sub_url(self.sub_url, "authenticate")
+            data["pkce_code_verifier"] = pkce_code_verifier
 
-        res = await self.async_client.post(url, json=payload)
+        url = self.api_base.url_for("/v1/b2b/magic_links/discovery/authenticate", data)
+        res = await self.async_client.post(url, data)
         return AuthenticateResponse.from_json(res.response.status, res.json)
```

### Comparing `stytch-6.9.0/stytch/b2b/api/magic_links_email.py` & `stytch-7.0.0/stytch/b2b/api/magic_links_email.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 # !!!
 # WARNING: This file is autogenerated
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
+from __future__ import annotations
+
 from typing import Any, Dict, Optional
 
 from stytch.b2b.api.magic_links_email_discovery import Discovery
-from stytch.b2b.models.magic_links_email import InviteResponse, LoginOrSignupResponse
+from stytch.b2b.models.magic_links_email import (
+    InviteRequestLocale,
+    InviteResponse,
+    LoginOrSignupRequestLocale,
+    LoginOrSignupResponse,
+)
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
 
 
 class Email:
     def __init__(
         self,
@@ -20,256 +27,232 @@
         async_client: AsyncClient,
     ) -> None:
         self.api_base = api_base
         self.sync_client = sync_client
         self.async_client = async_client
         self.discovery = Discovery(api_base, sync_client, async_client)
 
-    @property
-    def sub_url(self) -> str:
-        return "magic_links/email"
-
     def login_or_signup(
         self,
         organization_id: str,
         email_address: str,
         login_redirect_url: Optional[str] = None,
         signup_redirect_url: Optional[str] = None,
         pkce_code_challenge: Optional[str] = None,
         login_template_id: Optional[str] = None,
         signup_template_id: Optional[str] = None,
-        locale: Optional[str] = None,
+        locale: Optional[LoginOrSignupRequestLocale] = None,
     ) -> LoginOrSignupResponse:
-        """Send either a login or signup magic link to a Member. A new or pending Member will receive a signup Email Magic Link. An active Member will receive a login Email Magic Link.
-
-        Parameters:
-
-        - `organization_id`: Globally unique UUID that identifies a specific Organization. The organization_id is critical to perform operations on an Organization, so be sure to preserve this value.
-
-        - `email_address`: The email of the Member who will receive the Email Magic Link for login or signup.
-
-        - `login_redirect_url`: The URL that Member clicks from the login email magic link. This URL should be an endpoint in the backend server that verifies the request by querying Stytch's authenticate endpoint and finishes the login. If this value is not passed, the default login redirect URL that you set in your Dashboard is used. If you have not set a default login redirect URL, an error is returned.
+        """Send either a login or signup magic link to a Member. A new, pending, or invited Member will receive a signup Email Magic Link. Members will have a `pending` status until they successfully authenticate. An active Member will receive a login Email Magic Link.
 
-        - `signup_redirect_url`: The url the Member clicks from the sign-up email magic link. This URL should be an endpoint in the backend server that verifies the request by querying Stytch's authenticate endpoint and finishes the login. If this value is not passed, the default sign-up redirect URL that you set in your Dashboard is used. If you have not set a default sign-up redirect URL, an error is returned.
+        Fields:
+          - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
+          - email_address: The email address of the Member.
+          - login_redirect_url: The URL that the Member clicks from the login Email Magic Link. This URL should be an endpoint in the backend server that
+          verifies the request by querying Stytch's authenticate endpoint and finishes the login. If this value is not passed, the default login
+          redirect URL that you set in your Dashboard is used. If you have not set a default login redirect URL, an error is returned.
+          - signup_redirect_url: The URL the Member clicks from the signup Email Magic Link. This URL should be an endpoint in the backend server that verifies
+          the request by querying Stytch's authenticate endpoint and finishes the login. If this value is not passed, the default sign-up redirect URL
+          that you set in your Dashboard is used. If you have not set a default sign-up redirect URL, an error is returned.
+          - pkce_code_challenge: A base64url encoded SHA256 hash of a one time secret used to validate that the request starts and ends on the same device.
+          - login_template_id: Use a custom template for login emails. By default, it will use your default email template. The template must be from Stytch's
+        built-in customizations or a custom HTML email for Magic Links - Login.
+          - signup_template_id: Use a custom template for signup emails. By default, it will use your default email template. The template must be from Stytch's
+        built-in customizations or a custom HTML email for Magic Links - Signup.
+          - locale: Used to determine which language to use when sending the user this delivery method. Parameter is a [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"`.
 
-        - `pkce_code_challenge`: A base64url encoded SHA256 hash of a one time secret used to validate that the request starts and ends on the same device. See the PKCE OAuth guide for usage instructions.
+        Currently supported languages are English (`"en"`), Spanish (`"es"`), and Brazilian Portuguese (`"pt-br"`); if no value is provided, the copy defaults to English.
 
-        - `login_template_id`: Use a custom template for login emails. By default, it will use your default email template The template must be a template using our built-in customizations or a custom HTML email for Magic links - Login.
+        Request support for additional languages [here](https://docs.google.com/forms/d/e/1FAIpQLScZSpAu_m2AmLXRT3F3kap-s_mcV6UTBitYn6CdyWP0-o7YjQ/viewform?usp=sf_link")!
 
-        - `signup_template_id`: Use a custom template for sign-up emails. By default, it will use your default email template. The template must be a template using our built-in customizations or a custom HTML email for Magic links - Sign-up.
-
-        - `locale`: Used to determine which language to use when sending the user this delivery method. Parameter is a two character [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"` or `"es"`.
-
-          Currently supported languages are English (en) and Spanish (es); if no value is provided, the copy defaults to English.
-
-          Request more languages for support [here](https://docs.google.com/forms/d/e/1FAIpQLScZSpAu_m2AmLXRT3F3kap-s_mcV6UTBitYn6CdyWP0-o7YjQ/viewform?usp=sf_link)!
         """  # noqa
-
-        payload: Dict[str, Any] = {
+        data: Dict[str, Any] = {
             "organization_id": organization_id,
             "email_address": email_address,
         }
-
         if login_redirect_url is not None:
-            payload["login_redirect_url"] = login_redirect_url
+            data["login_redirect_url"] = login_redirect_url
         if signup_redirect_url is not None:
-            payload["signup_redirect_url"] = signup_redirect_url
+            data["signup_redirect_url"] = signup_redirect_url
         if pkce_code_challenge is not None:
-            payload["pkce_code_challenge"] = pkce_code_challenge
+            data["pkce_code_challenge"] = pkce_code_challenge
         if login_template_id is not None:
-            payload["login_template_id"] = login_template_id
+            data["login_template_id"] = login_template_id
         if signup_template_id is not None:
-            payload["signup_template_id"] = signup_template_id
+            data["signup_template_id"] = signup_template_id
         if locale is not None:
-            payload["locale"] = locale
+            data["locale"] = locale.value
 
-        url = self.api_base.route_with_sub_url(self.sub_url, "login_or_signup")
-
-        res = self.sync_client.post(url, json=payload)
+        url = self.api_base.url_for("/v1/b2b/magic_links/email/login_or_signup", data)
+        res = self.sync_client.post(url, data)
         return LoginOrSignupResponse.from_json(res.response.status_code, res.json)
 
     async def login_or_signup_async(
         self,
         organization_id: str,
         email_address: str,
         login_redirect_url: Optional[str] = None,
         signup_redirect_url: Optional[str] = None,
         pkce_code_challenge: Optional[str] = None,
         login_template_id: Optional[str] = None,
         signup_template_id: Optional[str] = None,
-        locale: Optional[str] = None,
+        locale: Optional[LoginOrSignupRequestLocale] = None,
     ) -> LoginOrSignupResponse:
-        """Send either a login or signup magic link to a Member. A new or pending Member will receive a signup Email Magic Link. An active Member will receive a login Email Magic Link.
-
-        Parameters:
-
-        - `organization_id`: Globally unique UUID that identifies a specific Organization. The organization_id is critical to perform operations on an Organization, so be sure to preserve this value.
-
-        - `email_address`: The email of the Member who will receive the Email Magic Link for login or signup.
-
-        - `login_redirect_url`: The URL that Member clicks from the login email magic link. This URL should be an endpoint in the backend server that verifies the request by querying Stytch's authenticate endpoint and finishes the login. If this value is not passed, the default login redirect URL that you set in your Dashboard is used. If you have not set a default login redirect URL, an error is returned.
-
-        - `signup_redirect_url`: The url the Member clicks from the sign-up email magic link. This URL should be an endpoint in the backend server that verifies the request by querying Stytch's authenticate endpoint and finishes the login. If this value is not passed, the default sign-up redirect URL that you set in your Dashboard is used. If you have not set a default sign-up redirect URL, an error is returned.
+        """Send either a login or signup magic link to a Member. A new, pending, or invited Member will receive a signup Email Magic Link. Members will have a `pending` status until they successfully authenticate. An active Member will receive a login Email Magic Link.
 
-        - `pkce_code_challenge`: A base64url encoded SHA256 hash of a one time secret used to validate that the request starts and ends on the same device. See the PKCE OAuth guide for usage instructions.
+        Fields:
+          - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
+          - email_address: The email address of the Member.
+          - login_redirect_url: The URL that the Member clicks from the login Email Magic Link. This URL should be an endpoint in the backend server that
+          verifies the request by querying Stytch's authenticate endpoint and finishes the login. If this value is not passed, the default login
+          redirect URL that you set in your Dashboard is used. If you have not set a default login redirect URL, an error is returned.
+          - signup_redirect_url: The URL the Member clicks from the signup Email Magic Link. This URL should be an endpoint in the backend server that verifies
+          the request by querying Stytch's authenticate endpoint and finishes the login. If this value is not passed, the default sign-up redirect URL
+          that you set in your Dashboard is used. If you have not set a default sign-up redirect URL, an error is returned.
+          - pkce_code_challenge: A base64url encoded SHA256 hash of a one time secret used to validate that the request starts and ends on the same device.
+          - login_template_id: Use a custom template for login emails. By default, it will use your default email template. The template must be from Stytch's
+        built-in customizations or a custom HTML email for Magic Links - Login.
+          - signup_template_id: Use a custom template for signup emails. By default, it will use your default email template. The template must be from Stytch's
+        built-in customizations or a custom HTML email for Magic Links - Signup.
+          - locale: Used to determine which language to use when sending the user this delivery method. Parameter is a [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"`.
 
-        - `login_template_id`: Use a custom template for login emails. By default, it will use your default email template The template must be a template using our built-in customizations or a custom HTML email for Magic links - Login.
+        Currently supported languages are English (`"en"`), Spanish (`"es"`), and Brazilian Portuguese (`"pt-br"`); if no value is provided, the copy defaults to English.
 
-        - `signup_template_id`: Use a custom template for sign-up emails. By default, it will use your default email template. The template must be a template using our built-in customizations or a custom HTML email for Magic links - Sign-up.
+        Request support for additional languages [here](https://docs.google.com/forms/d/e/1FAIpQLScZSpAu_m2AmLXRT3F3kap-s_mcV6UTBitYn6CdyWP0-o7YjQ/viewform?usp=sf_link")!
 
-        - `locale`: Used to determine which language to use when sending the user this delivery method. Parameter is a two character [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"` or `"es"`.
-
-          Currently supported languages are English (en) and Spanish (es); if no value is provided, the copy defaults to English.
-
-          Request more languages for support [here](https://docs.google.com/forms/d/e/1FAIpQLScZSpAu_m2AmLXRT3F3kap-s_mcV6UTBitYn6CdyWP0-o7YjQ/viewform?usp=sf_link)!
         """  # noqa
-
-        payload: Dict[str, Any] = {
+        data: Dict[str, Any] = {
             "organization_id": organization_id,
             "email_address": email_address,
         }
-
         if login_redirect_url is not None:
-            payload["login_redirect_url"] = login_redirect_url
+            data["login_redirect_url"] = login_redirect_url
         if signup_redirect_url is not None:
-            payload["signup_redirect_url"] = signup_redirect_url
+            data["signup_redirect_url"] = signup_redirect_url
         if pkce_code_challenge is not None:
-            payload["pkce_code_challenge"] = pkce_code_challenge
+            data["pkce_code_challenge"] = pkce_code_challenge
         if login_template_id is not None:
-            payload["login_template_id"] = login_template_id
+            data["login_template_id"] = login_template_id
         if signup_template_id is not None:
-            payload["signup_template_id"] = signup_template_id
+            data["signup_template_id"] = signup_template_id
         if locale is not None:
-            payload["locale"] = locale
-
-        url = self.api_base.route_with_sub_url(self.sub_url, "login_or_signup")
+            data["locale"] = locale.value
 
-        res = await self.async_client.post(url, json=payload)
+        url = self.api_base.url_for("/v1/b2b/magic_links/email/login_or_signup", data)
+        res = await self.async_client.post(url, data)
         return LoginOrSignupResponse.from_json(res.response.status, res.json)
 
     def invite(
         self,
         organization_id: str,
         email_address: str,
         invite_redirect_url: Optional[str] = None,
         invited_by_member_id: Optional[str] = None,
         name: Optional[str] = None,
         trusted_metadata: Optional[Dict[str, Any]] = None,
         untrusted_metadata: Optional[Dict[str, Any]] = None,
         invite_template_id: Optional[str] = None,
-        locale: Optional[str] = None,
+        locale: Optional[InviteRequestLocale] = None,
     ) -> InviteResponse:
-        """Send an invite email to a new Member to join an Organization. The Member will be created with a pending status until they successfully authenticate.
+        """Send an invite email to a new Member to join an Organization. The Member will be created with an `invited` status until they successfully authenticate. Sending invites to `pending` Members will update their status to `invited`. Sending invites to already `active` Members will return an error.
 
-        Parameters:
+        Fields:
+          - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
+          - email_address: The email address of the Member.
+          - invite_redirect_url: The URL that the Member clicks from the invite Email Magic Link. This URL should be an endpoint in the backend server that verifies
+          the request by querying Stytch's authenticate endpoint and finishes the invite flow. If this value is not passed, the default `invite_redirect_url`
+          that you set in your Dashboard is used. If you have not set a default `invite_redirect_url`, an error is returned.
+          - invited_by_member_id: The `member_id` of the Member who sends the invite.
+          - name: The name of the Member.
+          - trusted_metadata: An arbitrary JSON object for storing application-specific data or identity-provider-specific data.
+          - untrusted_metadata: An arbitrary JSON object of application-specific data. These fields can be edited directly by the
+          frontend SDK, and should not be used to store critical information. See the [Metadata resource](https://stytch.com/docs/b2b/api/metadata)
+          for complete field behavior details.
+          - invite_template_id: Use a custom template for invite emails. By default, it will use your default email template. The template must be a template
+          using our built-in customizations or a custom HTML email for Magic Links - Invite.
+          - locale: Used to determine which language to use when sending the user this delivery method. Parameter is a [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"`.
 
-        - `organization_id`: Globally unique UUID that identifies a specific Organization in the Stytch API. The organization_id is critical to perform operations on an Organization so be sure to preserve this value.
+        Currently supported languages are English (`"en"`), Spanish (`"es"`), and Brazilian Portuguese (`"pt-br"`); if no value is provided, the copy defaults to English.
 
-        - `email_address`: The email address of the Member.
+        Request support for additional languages [here](https://docs.google.com/forms/d/e/1FAIpQLScZSpAu_m2AmLXRT3F3kap-s_mcV6UTBitYn6CdyWP0-o7YjQ/viewform?usp=sf_link")!
 
-        - `invite_redirect_url`: The URL that Members click from the login email magic link. This URL should be an endpoint in the backend server that verifies the request by querying Stytch's authenticate endpoint and finishes the login. If this value is not passed, the default login redirect URL that you set in your Dashboard is used. If you have not set a default login redirect URL, an error is returned.
-
-        - `invited_by_member_id`: The member_id of the Member who sent the invite.
-
-        - `name`: The name of the invited Member.
-
-        - `trusted_metadata`: An arbitrary JSON object for storing application-specific or identity-provider-specific data.
-
-        - `untrusted_metadata`: The untrusted_metadata field contains an arbitrary JSON object of application-specific data. Untrusted metadata can be edited by end Members directly via the SDK, and cannot be used to store critical information. See the [Metadata reference](https://stytch.com/docs/b2b/api/metadata) for complete field behavior details.
-
-        - `invite_template_id`: Use a custom template for invite emails. By default, it will use your default email template. The template must be a template using our built-in customizations or a custom HTML email for Magic links - Invite.
-
-        - `locale`: Used to determine which language to use when sending the user this delivery method. Parameter is a two character [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"` or `"es"`.
-
-          Currently supported languages are English (en) and Spanish (es); if no value is provided, the copy defaults to English.
-
-          Request more languages for support [here](https://docs.google.com/forms/d/e/1FAIpQLScZSpAu_m2AmLXRT3F3kap-s_mcV6UTBitYn6CdyWP0-o7YjQ/viewform?usp=sf_link)!
         """  # noqa
-
-        payload: Dict[str, Any] = {
+        data: Dict[str, Any] = {
             "organization_id": organization_id,
             "email_address": email_address,
         }
-
         if invite_redirect_url is not None:
-            payload["invite_redirect_url"] = invite_redirect_url
+            data["invite_redirect_url"] = invite_redirect_url
         if invited_by_member_id is not None:
-            payload["invited_by_member_id"] = invited_by_member_id
+            data["invited_by_member_id"] = invited_by_member_id
         if name is not None:
-            payload["name"] = name
+            data["name"] = name
         if trusted_metadata is not None:
-            payload["trusted_metadata"] = trusted_metadata
+            data["trusted_metadata"] = trusted_metadata
         if untrusted_metadata is not None:
-            payload["untrusted_metadata"] = untrusted_metadata
+            data["untrusted_metadata"] = untrusted_metadata
         if invite_template_id is not None:
-            payload["invite_template_id"] = invite_template_id
+            data["invite_template_id"] = invite_template_id
         if locale is not None:
-            payload["locale"] = locale
-
-        url = self.api_base.route_with_sub_url(self.sub_url, "invite")
+            data["locale"] = locale.value
 
-        res = self.sync_client.post(url, json=payload)
+        url = self.api_base.url_for("/v1/b2b/magic_links/email/invite", data)
+        res = self.sync_client.post(url, data)
         return InviteResponse.from_json(res.response.status_code, res.json)
 
     async def invite_async(
         self,
         organization_id: str,
         email_address: str,
         invite_redirect_url: Optional[str] = None,
         invited_by_member_id: Optional[str] = None,
         name: Optional[str] = None,
         trusted_metadata: Optional[Dict[str, Any]] = None,
         untrusted_metadata: Optional[Dict[str, Any]] = None,
         invite_template_id: Optional[str] = None,
-        locale: Optional[str] = None,
+        locale: Optional[InviteRequestLocale] = None,
     ) -> InviteResponse:
-        """Send an invite email to a new Member to join an Organization. The Member will be created with a pending status until they successfully authenticate.
+        """Send an invite email to a new Member to join an Organization. The Member will be created with an `invited` status until they successfully authenticate. Sending invites to `pending` Members will update their status to `invited`. Sending invites to already `active` Members will return an error.
 
-        Parameters:
+        Fields:
+          - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
+          - email_address: The email address of the Member.
+          - invite_redirect_url: The URL that the Member clicks from the invite Email Magic Link. This URL should be an endpoint in the backend server that verifies
+          the request by querying Stytch's authenticate endpoint and finishes the invite flow. If this value is not passed, the default `invite_redirect_url`
+          that you set in your Dashboard is used. If you have not set a default `invite_redirect_url`, an error is returned.
+          - invited_by_member_id: The `member_id` of the Member who sends the invite.
+          - name: The name of the Member.
+          - trusted_metadata: An arbitrary JSON object for storing application-specific data or identity-provider-specific data.
+          - untrusted_metadata: An arbitrary JSON object of application-specific data. These fields can be edited directly by the
+          frontend SDK, and should not be used to store critical information. See the [Metadata resource](https://stytch.com/docs/b2b/api/metadata)
+          for complete field behavior details.
+          - invite_template_id: Use a custom template for invite emails. By default, it will use your default email template. The template must be a template
+          using our built-in customizations or a custom HTML email for Magic Links - Invite.
+          - locale: Used to determine which language to use when sending the user this delivery method. Parameter is a [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"`.
 
-        - `organization_id`: Globally unique UUID that identifies a specific Organization in the Stytch API. The organization_id is critical to perform operations on an Organization so be sure to preserve this value.
+        Currently supported languages are English (`"en"`), Spanish (`"es"`), and Brazilian Portuguese (`"pt-br"`); if no value is provided, the copy defaults to English.
 
-        - `email_address`: The email address of the Member.
+        Request support for additional languages [here](https://docs.google.com/forms/d/e/1FAIpQLScZSpAu_m2AmLXRT3F3kap-s_mcV6UTBitYn6CdyWP0-o7YjQ/viewform?usp=sf_link")!
 
-        - `invite_redirect_url`: The URL that Members click from the login email magic link. This URL should be an endpoint in the backend server that verifies the request by querying Stytch's authenticate endpoint and finishes the login. If this value is not passed, the default login redirect URL that you set in your Dashboard is used. If you have not set a default login redirect URL, an error is returned.
-
-        - `invited_by_member_id`: The member_id of the Member who sent the invite.
-
-        - `name`: The name of the invited Member.
-
-        - `trusted_metadata`: An arbitrary JSON object for storing application-specific or identity-provider-specific data.
-
-        - `untrusted_metadata`: The untrusted_metadata field contains an arbitrary JSON object of application-specific data. Untrusted metadata can be edited by end Members directly via the SDK, and cannot be used to store critical information. See the [Metadata reference](https://stytch.com/docs/b2b/api/metadata) for complete field behavior details.
-
-        - `invite_template_id`: Use a custom template for invite emails. By default, it will use your default email template. The template must be a template using our built-in customizations or a custom HTML email for Magic links - Invite.
-
-        - `locale`: Used to determine which language to use when sending the user this delivery method. Parameter is a two character [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"` or `"es"`.
-
-          Currently supported languages are English (en) and Spanish (es); if no value is provided, the copy defaults to English.
-
-          Request more languages for support [here](https://docs.google.com/forms/d/e/1FAIpQLScZSpAu_m2AmLXRT3F3kap-s_mcV6UTBitYn6CdyWP0-o7YjQ/viewform?usp=sf_link)!
         """  # noqa
-
-        payload: Dict[str, Any] = {
+        data: Dict[str, Any] = {
             "organization_id": organization_id,
             "email_address": email_address,
         }
-
         if invite_redirect_url is not None:
-            payload["invite_redirect_url"] = invite_redirect_url
+            data["invite_redirect_url"] = invite_redirect_url
         if invited_by_member_id is not None:
-            payload["invited_by_member_id"] = invited_by_member_id
+            data["invited_by_member_id"] = invited_by_member_id
         if name is not None:
-            payload["name"] = name
+            data["name"] = name
         if trusted_metadata is not None:
-            payload["trusted_metadata"] = trusted_metadata
+            data["trusted_metadata"] = trusted_metadata
         if untrusted_metadata is not None:
-            payload["untrusted_metadata"] = untrusted_metadata
+            data["untrusted_metadata"] = untrusted_metadata
         if invite_template_id is not None:
-            payload["invite_template_id"] = invite_template_id
+            data["invite_template_id"] = invite_template_id
         if locale is not None:
-            payload["locale"] = locale
-
-        url = self.api_base.route_with_sub_url(self.sub_url, "invite")
+            data["locale"] = locale.value
 
-        res = await self.async_client.post(url, json=payload)
+        url = self.api_base.url_for("/v1/b2b/magic_links/email/invite", data)
+        res = await self.async_client.post(url, data)
         return InviteResponse.from_json(res.response.status, res.json)
```

### Comparing `stytch-6.9.0/stytch/b2b/api/sessions.py` & `stytch-7.0.0/stytch/b2b/api/sessions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 # !!!
 # WARNING: This file is autogenerated
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
+from __future__ import annotations
+
 from typing import Any, Dict, Optional
 
 from stytch.b2b.models.sessions import (
     AuthenticateResponse,
     ExchangeResponse,
+    GetJWKSResponse,
     GetResponse,
     RevokeResponse,
 )
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
 
 
@@ -23,298 +26,318 @@
         sync_client: SyncClient,
         async_client: AsyncClient,
     ) -> None:
         self.api_base = api_base
         self.sync_client = sync_client
         self.async_client = async_client
 
-    @property
-    def sub_url(self) -> str:
-        return "sessions"
-
     def get(
         self,
         organization_id: str,
         member_id: str,
     ) -> GetResponse:
         """Retrieves all active Sessions for a Member.
 
-        Parameters:
-
-        - `organization_id`: Globally unique UUID that identifies a specific Organization in the Stytch API. The organization_id is critical to perform operations on an Organization, so be sure to preserve this value.
-
-        - `member_id`: Globally unique UUID that identifies a specific Member. The member_id is critical to perform operations on a Member, so be sure to preserve this value.
+        Fields:
+          - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
+          - member_id: Globally unique UUID that identifies a specific Member. The `member_id` is critical to perform operations on a Member, so be sure to preserve this value.
         """  # noqa
-
-        payload: Dict[str, Any] = {
+        data: Dict[str, Any] = {
             "organization_id": organization_id,
             "member_id": member_id,
         }
 
-        url = self.api_base.route_with_sub_url(self.sub_url, None)
-
-        res = self.sync_client.get(url, params=payload)
+        url = self.api_base.url_for("/v1/b2b/sessions", data)
+        res = self.sync_client.get(url, data)
         return GetResponse.from_json(res.response.status_code, res.json)
 
     async def get_async(
         self,
         organization_id: str,
         member_id: str,
     ) -> GetResponse:
         """Retrieves all active Sessions for a Member.
 
-        Parameters:
-
-        - `organization_id`: Globally unique UUID that identifies a specific Organization in the Stytch API. The organization_id is critical to perform operations on an Organization, so be sure to preserve this value.
-
-        - `member_id`: Globally unique UUID that identifies a specific Member. The member_id is critical to perform operations on a Member, so be sure to preserve this value.
+        Fields:
+          - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
+          - member_id: Globally unique UUID that identifies a specific Member. The `member_id` is critical to perform operations on a Member, so be sure to preserve this value.
         """  # noqa
-
-        payload: Dict[str, Any] = {
+        data: Dict[str, Any] = {
             "organization_id": organization_id,
             "member_id": member_id,
         }
 
-        url = self.api_base.route_with_sub_url(self.sub_url, None)
-
-        res = await self.async_client.get(url, params=payload)
+        url = self.api_base.url_for("/v1/b2b/sessions", data)
+        res = await self.async_client.get(url, data)
         return GetResponse.from_json(res.response.status, res.json)
 
     def authenticate(
         self,
         session_token: Optional[str] = None,
-        session_jwt: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
+        session_jwt: Optional[str] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
     ) -> AuthenticateResponse:
-        """Authenticates a Session. You may provide a JWT that needs to be refreshed and is expired according to its exp claim. A new JWT will be returned if both the signature and the underlying Session are still valid.
-
-        This endpoint requires only one of either the `session_jwt` or `session_token` be included in the request. It will return an error if both are present.
-
-        Parameters:
-
-        - `session_token`: A secret token for a given Stytch Session. Read more about session_token in our Session management guide.
+        """Authenticates a Session and updates its lifetime by the specified `session_duration_minutes`. If the `session_duration_minutes` is not specified, a Session will not be extended. This endpoint requires either a `session_jwt` or `session_token` be included in the request. It will return an error if both are present.
 
-        - `session_jwt`: The JSON Web Token (JWT) for a given Stytch Session. Read more about session_token in our Session management guide.
+        You may provide a JWT that needs to be refreshed and is expired according to its `exp` claim. A new JWT will be returned if both the signature and the underlying Session are still valid.
 
-        - `session_duration_minutes`: The Session lifetime of this many minutes from now; minimum of 5 and a maximum of 129600 minutes (90 days). Note that a successful authentication will continue to extend the Session this many minutes.
-
-        - `sessions_custom_claims`: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in session_duration_minutes. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To delete a key, supply a null value. Custom claims made with reserved claims ("iss", "sub", "aud", "exp", "nbf", "iat", "jti") will be ignored. Total custom claims size cannot exceed four kilobytes
+        Fields:
+          - session_token: A secret token for a given Stytch Session.
+          - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
+          returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
+          five minutes regardless of the underlying session duration, and will need to be refreshed over time.
+
+          This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
+
+          If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
+
+          If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
+          to use the Stytch session product, you can ignore the session fields in the response.
+          - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
+          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
+          `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
+          delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
+          Total custom claims size cannot exceed four kilobytes.
         """  # noqa
-
-        payload: Dict[str, Any] = {}
-
+        data: Dict[str, Any] = {}
         if session_token is not None:
-            payload["session_token"] = session_token
-        if session_jwt is not None:
-            payload["session_jwt"] = session_jwt
+            data["session_token"] = session_token
         if session_duration_minutes is not None:
-            payload["session_duration_minutes"] = session_duration_minutes
+            data["session_duration_minutes"] = session_duration_minutes
+        if session_jwt is not None:
+            data["session_jwt"] = session_jwt
         if session_custom_claims is not None:
-            payload["session_custom_claims"] = session_custom_claims
-
-        url = self.api_base.route_with_sub_url(self.sub_url, "authenticate")
+            data["session_custom_claims"] = session_custom_claims
 
-        res = self.sync_client.post(url, json=payload)
+        url = self.api_base.url_for("/v1/b2b/sessions/authenticate", data)
+        res = self.sync_client.post(url, data)
         return AuthenticateResponse.from_json(res.response.status_code, res.json)
 
     async def authenticate_async(
         self,
         session_token: Optional[str] = None,
-        session_jwt: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
+        session_jwt: Optional[str] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
     ) -> AuthenticateResponse:
-        """Authenticates a Session. You may provide a JWT that needs to be refreshed and is expired according to its exp claim. A new JWT will be returned if both the signature and the underlying Session are still valid.
-
-        This endpoint requires only one of either the `session_jwt` or `session_token` be included in the request. It will return an error if both are present.
+        """Authenticates a Session and updates its lifetime by the specified `session_duration_minutes`. If the `session_duration_minutes` is not specified, a Session will not be extended. This endpoint requires either a `session_jwt` or `session_token` be included in the request. It will return an error if both are present.
 
-        Parameters:
+        You may provide a JWT that needs to be refreshed and is expired according to its `exp` claim. A new JWT will be returned if both the signature and the underlying Session are still valid.
 
-        - `session_token`: A secret token for a given Stytch Session. Read more about session_token in our Session management guide.
-
-        - `session_jwt`: The JSON Web Token (JWT) for a given Stytch Session. Read more about session_token in our Session management guide.
-
-        - `session_duration_minutes`: The Session lifetime of this many minutes from now; minimum of 5 and a maximum of 129600 minutes (90 days). Note that a successful authentication will continue to extend the Session this many minutes.
-
-        - `sessions_custom_claims`: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in session_duration_minutes. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To delete a key, supply a null value. Custom claims made with reserved claims ("iss", "sub", "aud", "exp", "nbf", "iat", "jti") will be ignored. Total custom claims size cannot exceed four kilobytes
+        Fields:
+          - session_token: A secret token for a given Stytch Session.
+          - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
+          returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
+          five minutes regardless of the underlying session duration, and will need to be refreshed over time.
+
+          This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
+
+          If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
+
+          If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
+          to use the Stytch session product, you can ignore the session fields in the response.
+          - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
+          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
+          `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
+          delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
+          Total custom claims size cannot exceed four kilobytes.
         """  # noqa
-
-        payload: Dict[str, Any] = {}
-
+        data: Dict[str, Any] = {}
         if session_token is not None:
-            payload["session_token"] = session_token
-        if session_jwt is not None:
-            payload["session_jwt"] = session_jwt
+            data["session_token"] = session_token
         if session_duration_minutes is not None:
-            payload["session_duration_minutes"] = session_duration_minutes
+            data["session_duration_minutes"] = session_duration_minutes
+        if session_jwt is not None:
+            data["session_jwt"] = session_jwt
         if session_custom_claims is not None:
-            payload["session_custom_claims"] = session_custom_claims
+            data["session_custom_claims"] = session_custom_claims
 
-        url = self.api_base.route_with_sub_url(self.sub_url, "authenticate")
-
-        res = await self.async_client.post(url, json=payload)
+        url = self.api_base.url_for("/v1/b2b/sessions/authenticate", data)
+        res = await self.async_client.post(url, data)
         return AuthenticateResponse.from_json(res.response.status, res.json)
 
     def revoke(
         self,
         member_session_id: Optional[str] = None,
         session_token: Optional[str] = None,
         session_jwt: Optional[str] = None,
         member_id: Optional[str] = None,
     ) -> RevokeResponse:
-        """Revoke a Session and immediately invalidate all its tokens. To revoke a specific Session, pass either the `member_session_id`, `session_token`, or `session_jwt`. To revoke all Sessions for a Member, pass the `member_id`. This endpoint requires exactly one body param to be included in the request. It will return an error if multiple are present.
-
-        Parameters:
+        """Revoke a Session and immediately invalidate all its tokens. To revoke a specific Session, pass either the `member_session_id`, `session_token`, or `session_jwt`. To revoke all Sessions for a Member, pass the `member_id`.
 
-        - `member_session_id`: The UUID of the specific Member Session to revoke.
-
-        - `session_token`: The `session_token` of the specific Member Session to revoke.
-
-        - `session_jwt`: The JSON Web Token (JWT) of the specific Member Session to revoke.
-
-        - `member_id`: The UUID of the Member to revoke all sessions for.
+        Fields:
+          - member_session_id: Globally unique UUID that identifies a specific Session in the Stytch API. The `member_session_id` is critical to perform operations on an Session, so be sure to preserve this value.
+          - session_token: A secret token for a given Stytch Session.
+          - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
+          - member_id: Globally unique UUID that identifies a specific Member. The `member_id` is critical to perform operations on a Member, so be sure to preserve this value.
         """  # noqa
-
-        payload: Dict[str, Any] = {}
-
+        data: Dict[str, Any] = {}
         if member_session_id is not None:
-            payload["member_session_id"] = member_session_id
+            data["member_session_id"] = member_session_id
         if session_token is not None:
-            payload["session_token"] = session_token
+            data["session_token"] = session_token
         if session_jwt is not None:
-            payload["session_jwt"] = session_jwt
+            data["session_jwt"] = session_jwt
         if member_id is not None:
-            payload["member_id"] = member_id
-
-        url = self.api_base.route_with_sub_url(self.sub_url, "revoke")
+            data["member_id"] = member_id
 
-        res = self.sync_client.post(url, json=payload)
+        url = self.api_base.url_for("/v1/b2b/sessions/revoke", data)
+        res = self.sync_client.post(url, data)
         return RevokeResponse.from_json(res.response.status_code, res.json)
 
     async def revoke_async(
         self,
         member_session_id: Optional[str] = None,
         session_token: Optional[str] = None,
         session_jwt: Optional[str] = None,
         member_id: Optional[str] = None,
     ) -> RevokeResponse:
-        """Revoke a Session and immediately invalidate all its tokens. To revoke a specific Session, pass either the `member_session_id`, `session_token`, or `session_jwt`. To revoke all Sessions for a Member, pass the `member_id`. This endpoint requires exactly one body param to be included in the request. It will return an error if multiple are present.
-
-        Parameters:
-
-        - `member_session_id`: The UUID of the specific Member Session to revoke.
-
-        - `session_token`: The `session_token` of the specific Member Session to revoke.
+        """Revoke a Session and immediately invalidate all its tokens. To revoke a specific Session, pass either the `member_session_id`, `session_token`, or `session_jwt`. To revoke all Sessions for a Member, pass the `member_id`.
 
-        - `session_jwt`: The JSON Web Token (JWT) of the specific Member Session to revoke.
-
-        - `member_id`: The UUID of the Member to revoke all sessions for.
+        Fields:
+          - member_session_id: Globally unique UUID that identifies a specific Session in the Stytch API. The `member_session_id` is critical to perform operations on an Session, so be sure to preserve this value.
+          - session_token: A secret token for a given Stytch Session.
+          - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
+          - member_id: Globally unique UUID that identifies a specific Member. The `member_id` is critical to perform operations on a Member, so be sure to preserve this value.
         """  # noqa
-
-        payload: Dict[str, Any] = {}
-
+        data: Dict[str, Any] = {}
         if member_session_id is not None:
-            payload["member_session_id"] = member_session_id
+            data["member_session_id"] = member_session_id
         if session_token is not None:
-            payload["session_token"] = session_token
+            data["session_token"] = session_token
         if session_jwt is not None:
-            payload["session_jwt"] = session_jwt
+            data["session_jwt"] = session_jwt
         if member_id is not None:
-            payload["member_id"] = member_id
+            data["member_id"] = member_id
 
-        url = self.api_base.route_with_sub_url(self.sub_url, "revoke")
-
-        res = await self.async_client.post(url, json=payload)
+        url = self.api_base.url_for("/v1/b2b/sessions/revoke", data)
+        res = await self.async_client.post(url, data)
         return RevokeResponse.from_json(res.response.status, res.json)
 
     def exchange(
         self,
         organization_id: str,
         session_token: Optional[str] = None,
         session_jwt: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
     ) -> ExchangeResponse:
         """Use this endpoint to exchange a Member's existing session for another session in a different Organization. This can be used to accept an invite, but not to create a new member via domain matching.
 
         To create a new member via domain matching, use the [Exchange Intermediate Session](https://stytch.com/docs/b2b/api/exchange-intermediate-session) flow instead.
 
-        Parameters:
-
-        - `organization_id`: The UUID of the Organization to create the new session in.
-
-        - `session_token`: The `session_token` belonging to the member that you wish to associate the email with.
-
-        - `session_jwt`: The `session_jwt` belonging to the member that you wish to associate the email with.
-
-        - `session_duration_minutes`: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist, returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of five minutes regardless of the underlying session duration, and will need to be refreshed over time.
-          - This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
-          - If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
-          - If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want to use the Stytch session product, you can ignore the session fields in the response.
-
-        - `session_custom_claims`: Add a custom claims map to the session being authenticated. Claims will be included on the session object and in the JWT. To update a key in an existing session, supply a new value. To delete a key, supply a null value.
+        Fields:
+          - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
+          - session_token: The `session_token` belonging to the member that you wish to associate the email with.
+          - session_jwt: The `session_jwt` belonging to the member that you wish to associate the email with.
+          - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
+          returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
+          five minutes regardless of the underlying session duration, and will need to be refreshed over time.
+
+          This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
+
+          If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
+
+          If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
+          to use the Stytch session product, you can ignore the session fields in the response.
+          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
+          `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
+          delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
+          Total custom claims size cannot exceed four kilobytes.
         """  # noqa
-
-        payload: Dict[str, Any] = {
+        data: Dict[str, Any] = {
             "organization_id": organization_id,
         }
-
         if session_token is not None:
-            payload["session_token"] = session_token
+            data["session_token"] = session_token
         if session_jwt is not None:
-            payload["session_jwt"] = session_jwt
+            data["session_jwt"] = session_jwt
         if session_duration_minutes is not None:
-            payload["session_duration_minutes"] = session_duration_minutes
+            data["session_duration_minutes"] = session_duration_minutes
         if session_custom_claims is not None:
-            payload["session_custom_claims"] = session_custom_claims
-
-        url = self.api_base.route_with_sub_url(self.sub_url, "exchange")
+            data["session_custom_claims"] = session_custom_claims
 
-        res = self.sync_client.post(url, json=payload)
+        url = self.api_base.url_for("/v1/b2b/sessions/exchange", data)
+        res = self.sync_client.post(url, data)
         return ExchangeResponse.from_json(res.response.status_code, res.json)
 
     async def exchange_async(
         self,
         organization_id: str,
         session_token: Optional[str] = None,
         session_jwt: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
     ) -> ExchangeResponse:
         """Use this endpoint to exchange a Member's existing session for another session in a different Organization. This can be used to accept an invite, but not to create a new member via domain matching.
 
         To create a new member via domain matching, use the [Exchange Intermediate Session](https://stytch.com/docs/b2b/api/exchange-intermediate-session) flow instead.
 
-        Parameters:
-
-        - `organization_id`: The UUID of the Organization to create the new session in.
-
-        - `session_token`: The `session_token` belonging to the member that you wish to associate the email with.
-
-        - `session_jwt`: The `session_jwt` belonging to the member that you wish to associate the email with.
-
-        - `session_duration_minutes`: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist, returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of five minutes regardless of the underlying session duration, and will need to be refreshed over time.
-          - This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
-          - If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
-          - If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want to use the Stytch session product, you can ignore the session fields in the response.
-
-        - `session_custom_claims`: Add a custom claims map to the session being authenticated. Claims will be included on the session object and in the JWT. To update a key in an existing session, supply a new value. To delete a key, supply a null value.
+        Fields:
+          - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
+          - session_token: The `session_token` belonging to the member that you wish to associate the email with.
+          - session_jwt: The `session_jwt` belonging to the member that you wish to associate the email with.
+          - session_duration_minutes: Set the session lifetime to be this many minutes from now. This will start a new session if one doesn't already exist,
+          returning both an opaque `session_token` and `session_jwt` for this session. Remember that the `session_jwt` will have a fixed lifetime of
+          five minutes regardless of the underlying session duration, and will need to be refreshed over time.
+
+          This value must be a minimum of 5 and a maximum of 527040 minutes (366 days).
+
+          If a `session_token` or `session_jwt` is provided then a successful authentication will continue to extend the session this many minutes.
+
+          If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
+          to use the Stytch session product, you can ignore the session fields in the response.
+          - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
+          `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
+          delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
+          Total custom claims size cannot exceed four kilobytes.
         """  # noqa
-
-        payload: Dict[str, Any] = {
+        data: Dict[str, Any] = {
             "organization_id": organization_id,
         }
-
         if session_token is not None:
-            payload["session_token"] = session_token
+            data["session_token"] = session_token
         if session_jwt is not None:
-            payload["session_jwt"] = session_jwt
+            data["session_jwt"] = session_jwt
         if session_duration_minutes is not None:
-            payload["session_duration_minutes"] = session_duration_minutes
+            data["session_duration_minutes"] = session_duration_minutes
         if session_custom_claims is not None:
-            payload["session_custom_claims"] = session_custom_claims
+            data["session_custom_claims"] = session_custom_claims
 
-        url = self.api_base.route_with_sub_url(self.sub_url, "exchange")
-
-        res = await self.async_client.post(url, json=payload)
+        url = self.api_base.url_for("/v1/b2b/sessions/exchange", data)
+        res = await self.async_client.post(url, data)
         return ExchangeResponse.from_json(res.response.status, res.json)
+
+    def get_jwks(
+        self,
+        project_id: str,
+    ) -> GetJWKSResponse:
+        """Get the JSON Web Key Set (JWKS) for a project.
+
+        Fields:
+          - project_id: The `project_id` to get the JWKS for.
+        """  # noqa
+        data: Dict[str, Any] = {
+            "project_id": project_id,
+        }
+
+        url = self.api_base.url_for("/v1/b2b/sessions/jwks/{project_id}", data)
+        res = self.sync_client.get(url, data)
+        return GetJWKSResponse.from_json(res.response.status_code, res.json)
+
+    async def get_jwks_async(
+        self,
+        project_id: str,
+    ) -> GetJWKSResponse:
+        """Get the JSON Web Key Set (JWKS) for a project.
+
+        Fields:
+          - project_id: The `project_id` to get the JWKS for.
+        """  # noqa
+        data: Dict[str, Any] = {
+            "project_id": project_id,
+        }
+
+        url = self.api_base.url_for("/v1/b2b/sessions/jwks/{project_id}", data)
+        res = await self.async_client.get(url, data)
+        return GetJWKSResponse.from_json(res.response.status, res.json)
```

### Comparing `stytch-6.9.0/stytch/b2b/models/discovery_intermediate_sessions.py` & `stytch-7.0.0/stytch/b2b/models/passwords_session.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-#!/usr/bin/env python3
+# !!!
+# WARNING: This file is autogenerated
+# Only modify code within MANUAL() sections
+# or your changes may be overwritten later!
+# !!!
 
-from typing import Optional
-
-from stytch.b2b.core.models import B2BStytchSession, Member, Organization
-from stytch.core.models import ResponseBase
-
-
-class ExchangeResponse(ResponseBase):
-    """Response fields beyond those defined in `ResponseBase`:
+from __future__ import annotations
 
-    - `member_id`: The UUID of the new Member that was created.
-
-    - `session_token`: A secret token for a given Stytch Session. Read more about session_token in our Session management guide.
-
-    - `session_jwt`: The JSON Web Token (JWT) for a given Stytch Session. Read more about session_token in our Session management guide.
+from typing import Optional
 
-    - `member_session`: The B2BStytchSession object.
+from stytch.b2b.models.organizations import Member, Organization
+from stytch.b2b.models.sessions import MemberSession
+from stytch.core.response_base import ResponseBase
 
-    - `member`: The [Member](https://stytch.com/docs/b2b/api/member-object) object.
 
-    - `organization`: The [Organization](https://stytch.com/docs/b2b/api/organization-object) object.
+class ResetResponse(ResponseBase):
+    """Response type for `Sessions.reset`.
+    Fields:
+      - member_id: Globally unique UUID that identifies a specific Member.
+      - member: The [Member object](https://stytch.com/docs/b2b/api/member-object).
+      - organization: The [Organization object](https://stytch.com/docs/b2b/api/organization-object).
+      - member_session: The [Session object](https://stytch.com/docs/b2b/api/session-object).
     """  # noqa
 
     member_id: str
-    member_session: Optional[B2BStytchSession]
-    session_token: str
-    session_jwt: str
     member: Member
     organization: Organization
+    member_session: Optional[MemberSession] = None
```

### Comparing `stytch-6.9.0/stytch/b2b/models/discovery_organizations.py` & `stytch-7.0.0/stytch/b2b/models/discovery_intermediate_sessions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,32 @@
-#!/usr/bin/env python3
-
-from typing import List, Optional
-
-from stytch.b2b.core.models import (
-    B2BStytchSession,
-    DiscoveredOrganization,
-    Member,
-    Organization,
-)
-from stytch.core.models import ResponseBase
-
-
-class ListResponse(ResponseBase):
-    """Response fields beyond those defined in `ResponseBase`:
-
-    - `email_address`: The email address associated with the intermediate session token.
-
-    - `discovered_organizations`: An array of `discovered_organization` objects tied to the `intermediate_session_token`. See the [Discovered Organization Object](https://stytch.com/docs/b2b/api/discovered-organization-object) for complete details.
-    """  # noqa
-
-    email_address: str
-    discovered_organizations: List[DiscoveredOrganization]
-
-
-class CreateResponse(ResponseBase):
-    """Response fields beyond those defined in `ResponseBase`:
-
-    - `member_id`: The UUID of the new Member that was created.
-
-    - `session_token`: A secret token for a given Stytch Session. Read more about session_token in our Session management guide.
-
-    - `session_jwt`: The JSON Web Token (JWT) for a given Stytch Session. Read more about session_token in our Session management guide.
-
-    - `member_session`: The B2BStytchSession object.
-
-    - `member`: The [Member](https://stytch.com/docs/b2b/api/member-object) object.
-
-    - `organization`: The [Organization](https://stytch.com/docs/b2b/api/organization-object) object.
+# !!!
+# WARNING: This file is autogenerated
+# Only modify code within MANUAL() sections
+# or your changes may be overwritten later!
+# !!!
+
+from __future__ import annotations
+
+from typing import Optional
+
+from stytch.b2b.models.organizations import Member, Organization
+from stytch.b2b.models.sessions import MemberSession
+from stytch.core.response_base import ResponseBase
+
+
+class ExchangeResponse(ResponseBase):
+    """Response type for `IntermediateSessions.exchange`.
+    Fields:
+      - member_id: Globally unique UUID that identifies a specific Member.
+      - session_token: A secret token for a given Stytch Session.
+      - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
+      - member: The [Member object](https://stytch.com/docs/b2b/api/member-object).
+      - organization: The [Organization object](https://stytch.com/docs/b2b/api/organization-object).
+      - member_session: The [Session object](https://stytch.com/docs/b2b/api/session-object).
     """  # noqa
 
     member_id: str
-    member_session: Optional[B2BStytchSession]
     session_token: str
     session_jwt: str
     member: Member
     organization: Organization
+    member_session: Optional[MemberSession] = None
```

### Comparing `stytch-6.9.0/stytch/b2b/models/magic_links_discovery.py` & `stytch-7.0.0/stytch/b2b/models/magic_links_discovery.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,36 @@
-#!/usr/bin/env python3
+# !!!
+# WARNING: This file is autogenerated
+# Only modify code within MANUAL() sections
+# or your changes may be overwritten later!
+# !!!
+
+from __future__ import annotations
 
 from typing import List
 
-from stytch.b2b.core.models import DiscoveredOrganization
-from stytch.core.models import ResponseBase
+from stytch.b2b.models.discovery import DiscoveredOrganization
+from stytch.core.response_base import ResponseBase
 
 
 class AuthenticateResponse(ResponseBase):
-    """Response fields beyond those defined in `ResponseBase`:
+    """Response type for `Discovery.authenticate`.
+    Fields:
+      - intermediate_session_token: The Intermediate Session Token. This token does not belong to a specific instance of a member, but may be exchanged for an existing Member Session or used to create a new organization.
+      - email_address: The email address.
+      - discovered_organizations: An array of `discovered_organization` objects tied to the `intermediate_session_token`, `session_token`, or `session_jwt`. See the [Discovered Organization Object](https://stytch.com/docs/b2b/api/discovered-organization-object) for complete details.
+
+      Note that Organizations will only appear here under any of the following conditions:
+      1. The end user is already a Member of the Organization.
+      2. The end user is invited to the Organization.
+      3. The end user can join the Organization because:
 
-    - `intermediate_session_token`: The Intermediate Session Token. This token does not belong to a specific instance of a member, but may be exchanged for an existing Member Session or used to create a new organization.
+          a) The Organization allows JIT provisioning.
 
-    - `email_address`: The email address associated with the intermediate session token.
+          b) The Organizations' allowed domains list contains the Member's email domain.
 
-    - `discovered_organizations`: An array of `discovered_organization` objects tied to the `intermediate_session_token`. See the [Discovered Organization Object](https://stytch.com/docs/b2b/api/discovered-organization-object) for complete details.
+          c) The Organization has at least one other Member with a verified email address with the same domain as the end user (to prevent phishing attacks).
     """  # noqa
 
     intermediate_session_token: str
     email_address: str
     discovered_organizations: List[DiscoveredOrganization]
```

### Comparing `stytch-6.9.0/stytch/b2b/models/magic_links_email.py` & `stytch-7.0.0/stytch/b2b/models/magic_links_email.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,52 @@
-#!/usr/bin/env python3
+# !!!
+# WARNING: This file is autogenerated
+# Only modify code within MANUAL() sections
+# or your changes may be overwritten later!
+# !!!
 
+from __future__ import annotations
 
-from stytch.b2b.core.models import Member, Organization
-from stytch.core.models import ResponseBase
+import enum
 
+from stytch.b2b.models.organizations import Member, Organization
+from stytch.core.response_base import ResponseBase
 
-class LoginOrSignupResponse(ResponseBase):
-    """Response fields beyond those defined in `ResponseBase`:
 
-    - `member_id`: Globally unique UUID that identifies a specific Member in the Stytch API. The member_id is critical to perform operations on a Member, so be sure to preserve this value.
+class InviteRequestLocale(enum.Enum):
+    EN = "en"
+    ES = "es"
+    PTBR = "pt-br"
+
 
-    - `member_created`: A flag indicating `true` if a new Member object was created and `false` if the Member object already existed.
+class LoginOrSignupRequestLocale(enum.Enum):
+    EN = "en"
+    ES = "es"
+    PTBR = "pt-br"
 
-    - `member`: The Member object.
 
-    - `organization`: The Organization object.
+class InviteResponse(ResponseBase):
+    """Response type for `Email.invite`.
+    Fields:
+      - member_id: Globally unique UUID that identifies a specific Member.
+      - member: The [Member object](https://stytch.com/docs/b2b/api/member-object).
+      - organization: The [Organization object](https://stytch.com/docs/b2b/api/organization-object).
     """  # noqa
 
     member_id: str
-    member_created: bool
     member: Member
     organization: Organization
 
 
-class InviteResponse(ResponseBase):
-    """Response fields beyond those defined in `ResponseBase`:
-
-    - `member_id`: Globally unique UUID that identifies a specific Member. The member_id is critical to perform operations on a Member, so be sure to preserve this value.
-    - `member`: The Member object.
-    - `organization`: The Organization object.
+class LoginOrSignupResponse(ResponseBase):
+    """Response type for `Email.login_or_signup`.
+    Fields:
+      - member_id: Globally unique UUID that identifies a specific Member.
+      - member_created: A flag indicating `true` if a new Member object was created and `false` if the Member object already existed.
+      - member: The [Member object](https://stytch.com/docs/b2b/api/member-object).
+      - organization: The [Organization object](https://stytch.com/docs/b2b/api/organization-object).
     """  # noqa
 
     member_id: str
+    member_created: bool
     member: Member
     organization: Organization
```

### Comparing `stytch-6.9.0/stytch/b2b/models/passwords_existing_password.py` & `stytch-7.0.0/stytch/b2b/models/passwords_existing_password.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-#!/usr/bin/env python3
+# !!!
+# WARNING: This file is autogenerated
+# Only modify code within MANUAL() sections
+# or your changes may be overwritten later!
+# !!!
+
+from __future__ import annotations
 
 from typing import Optional
 
-from stytch.b2b.core.models import B2BStytchSession, Member, Organization
-from stytch.core.models import ResponseBase
+from stytch.b2b.models.organizations import Member, Organization
+from stytch.b2b.models.sessions import MemberSession
+from stytch.core.response_base import ResponseBase
 
 
 class ResetResponse(ResponseBase):
-    """Response fields beyond those defined in `ResponseBase`:
-
-    - `member_session`: The B2BStytchSession object.
-
-    - `session_token`: A secret token for a given Stytch Session. Read more about session_token in our Session management guide.
-
-    - `session_jwt`: The JSON Web Token (JWT) for a given Stytch Session. Read more about session_token in our Session Management guide.
-
-    - `organization_id`: Globally unique UUID that identifies a specific Organization in the Stytch API. The organization_id is critical to perform operations on an Organization so be sure to preserve this value.
-
-    - `member`: The Member object.
-
-    - `member_id`: Globally unique UUID that identifies a specific Member in the Stytch API. The member_id is critical to perform operations on a Member, so be sure to preserve this value.
-
-    - `organization`: The Organization object.
+    """Response type for `ExistingPassword.reset`.
+    Fields:
+      - member_id: Globally unique UUID that identifies a specific Member.
+      - member: The [Member object](https://stytch.com/docs/b2b/api/member-object).
+      - session_token: A secret token for a given Stytch Session.
+      - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
+      - organization: The [Organization object](https://stytch.com/docs/b2b/api/organization-object).
+      - member_session: The [Session object](https://stytch.com/docs/b2b/api/session-object).
     """  # noqa
 
-    member: Member
     member_id: str
-    organization_id: str
-    organization: Organization
+    member: Member
     session_token: str
     session_jwt: str
-    member_session: Optional[B2BStytchSession]
+    organization: Organization
+    member_session: Optional[MemberSession] = None
```

### Comparing `stytch-6.9.0/stytch/core/http/client.py` & `stytch-7.0.0/stytch/core/http/client.py`

 * *Files identical despite different names*

### Comparing `stytch-6.9.0/stytch.egg-info/PKG-INFO` & `stytch-7.0.0/stytch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stytch
-Version: 6.9.0
+Version: 7.0.0
 Summary: Stytch python client
 Download-URL: https://github.com/stytchauth/stytch-python
 Author: Stytch
 Author-email: hello@stytch.com
 License: MIT
 Keywords: stytch,user,authentication
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stytch-6.9.0/test/test_integration.py` & `stytch-7.0.0/test/test_integration.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     TEST_USERS_NAME,
 )
 from test.integration_base import CreatedTestUser, IntegrationTestBase
 
 
 class SyncIntegrationTest(IntegrationTestBase, unittest.TestCase):
     def test_crypto_wallets(self) -> None:
-        api = self.client.crypto_wallets
+        api = self.b2c_client.crypto_wallets
 
         self.assertTrue(
             api.authenticate_start(
                 crypto_wallet_type=TEST_CRYPTO_WALLET_TYPE,
                 crypto_wallet_address=TEST_CRYPTO_WALLET_ADDRESS,
             ).is_success
         )
@@ -37,15 +37,15 @@
                 crypto_wallet_type=TEST_CRYPTO_WALLET_TYPE,
                 crypto_wallet_address=TEST_CRYPTO_WALLET_ADDRESS,
                 signature=TEST_CRYPTO_SIGNATURE,
             ).is_success
         )
 
     def test_magic_links(self) -> None:
-        api = self.client.magic_links
+        api = self.b2c_client.magic_links
 
         self.assertTrue(api.authenticate(token=TEST_MAGIC_TOKEN).is_success)
 
         with self.skip_if_stytcherror(
             subtest_name="create_endpoint",
             skip_reason="Not approved for embedded magic links",
             error_message_pattern="requires approval before using",
@@ -63,20 +63,29 @@
             self.assertTrue(api.email.revoke_invite(email=TEST_MAGIC_EMAIL).is_success)
             self.assertTrue(
                 api.email.login_or_create(email=TEST_MAGIC_EMAIL).is_success
             )
             self.assertTrue(api.email.send(TEST_MAGIC_EMAIL).is_success)
 
     def test_oauth(self) -> None:
-        api = self.client.oauth
+        api = self.b2c_client.oauth
+
+        with self.skip_if_stytcherror(
+            subtest_name="attach",
+            skip_reason="No OAuth config set up",
+            error_message_pattern="OAuth config",
+        ):
+            with self._get_temporary_user() as user:
+                assert isinstance(user, CreatedTestUser)
+                self.assertTrue(api.attach(provider="google", user_id=user.user_id))
 
         self.assertTrue(api.authenticate(token=TEST_OAUTH_TOKEN).is_success)
 
     def test_otp(self) -> None:
-        api = self.client.otps
+        api = self.b2c_client.otps
 
         with self.subTest("email"):
             self.assertTrue(api.email.login_or_create(email=TEST_OTP_EMAIL).is_success)
             email_send_response = api.email.send(email=TEST_OTP_EMAIL)
             self.assertTrue(email_send_response.is_success)
             self.assertTrue(
                 api.authenticate(
@@ -105,91 +114,68 @@
             self.assertTrue(
                 api.authenticate(
                     method_id=whatsapp_send_response.phone_id, code=TEST_OTP_CODE
                 ).is_success
             )
 
     def test_passwords(self) -> None:
-        api = self.client.passwords
+        api = self.b2c_client.passwords
 
         with self._get_temporary_user(create=False) as user:
             self.assertTrue(api.strength_check(password=user.old_password).is_success)
             create_response = api.create(email=user.email, password=user.old_password)
             self.assertTrue(create_response.is_success)
             authenticate_response = api.authenticate(
                 email=user.email, password=user.old_password
             )
             self.assertTrue(authenticate_response.is_success)
             # Remember to manually delete since we manually created!
-            self.client.users.delete(create_response.user_id)
+            self.b2c_client.users.delete(create_response.user_id)
 
         # Migrate an existing user created via magic link
         with self._get_temporary_user(via_magic_link=True) as user:
             self.assertTrue(
                 api.migrate(
                     email=user.email,
                     hash=TEST_PW_HASH,
                     hash_type=TEST_PW_HASH_TYPE,
                 ).is_success
             )
 
-        with self.skip_if_stytcherror(
-            subtest_name="email",
-            skip_reason="No login_redirect_url set up",
-            error_message_pattern="There are no .* URLs",
-        ):
-            # Can't test: there's no reset token that can be used for testing the API
-            self.skipTest("No reset token to use for testing")
-            with self._get_temporary_user() as user:
-                reset_start_response = api.email.reset_start(email=user.email)
-                self.assertTrue(reset_start_response.is_success)
-                # TODO: We don't have a sample reset token (see skipTest above)
-                self.assertTrue(
-                    api.email.reset(token="", password=user.new_password).is_success
-                )
+        # NOTE: email and sessions sub-APIS are not tested since there's no reset token
+        # defined in test resources
         with self.subTest("existing_password"):
             with self._get_temporary_user() as user:
                 self.assertTrue(
                     api.existing_password.reset(
                         email=user.email,
                         existing_password=user.old_password,
                         new_password=user.new_password,
                     ).is_success
                 )
-        with self.subTest("session"):
-            # Can't test: there's no sesison token that can be used for testing the API
-            self.skipTest("No session token to use for testing")
-            with self._get_temporary_user() as user:
-                # TODO: We don't have a sample session token (see skipTest above)
-                self.assertTrue(
-                    api.session.reset(
-                        session_token="",
-                        password=user.new_password,
-                    ).is_success
-                )
 
     def test_sessions(self) -> None:
-        api = self.client.sessions
+        api = self.b2c_client.sessions
 
         with self._get_temporary_user() as user:
             # TODO: With @overload, it should be possible to let
             # the type checker infer this statically. I tried, but
             # it was a bit complicated since it's not a simple type,
             # but actually returning a Generator from a @contextmanager
             assert isinstance(user, CreatedTestUser)
             self.assertTrue(api.get(user_id=user.user_id).is_success)
             self.assertTrue(
                 api.authenticate(session_token=TEST_SESSION_TOKEN).is_success
             )
             # Can't test revoke -- it doesn't support the TEST_SESSION_TOKEN
             # self.assertTrue(api.revoke(session_token=TEST_SESSION_TOKEN).is_success)
-            self.assertTrue(api.jwks(project_id=self.project_id).is_success)
+            self.assertTrue(api.get_jwks(project_id=self.project_id).is_success)
 
     def test_totps(self) -> None:
-        api = self.client.totps
+        api = self.b2c_client.totps
 
         self.assertTrue(api.create(user_id=TEST_TOTP_USER_ID).is_success)
         self.assertTrue(
             api.authenticate(
                 user_id=TEST_TOTP_USER_ID, totp_code=TEST_TOTP_CODE
             ).is_success
         )
@@ -200,32 +186,31 @@
             ).is_success
         )
 
     def test_users(self) -> None:
         # NOTE: the various `delete_XXX` can't easily be tested (yet)
         # since it would require we first create the user with each of those
         # methods/auth factors present (and possibly authenticated?).
-        api = self.client.users
+        api = self.b2c_client.users
 
         with self._get_temporary_user(create=False) as user:
             create_resp = api.create(email=user.email)
             self.assertTrue(create_resp.is_success)
-            self.assertTrue(api.get_pending().is_success)
             self.assertTrue(api.search(limit=10).is_success)
             self.assertTrue(
                 api.update(
                     user_id=create_resp.user_id,
                     name=TEST_USERS_NAME,
                 ).is_success
             )
             self.assertTrue(api.get(user_id=create_resp.user_id).is_success)
             self.assertTrue(api.delete(user_id=create_resp.user_id).is_success)
 
     def test_webauthn(self) -> None:
-        api = self.client.webauthn
+        api = self.b2c_client.webauthn
         # Can't test: webauthn requires calling browser functions
         # It would probably work if we had some way of using test API
         # sample values (like a sample public_key_credential for testing)
         self.skipTest("webauthn cannot be tested from this client")
 
         with self._get_temporary_user() as user:
             assert isinstance(user, CreatedTestUser)
```

### Comparing `stytch-6.9.0/test/test_integration_async.py` & `stytch-7.0.0/test/test_integration_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     IsolatedAsyncioTestCase = unittest.TestCase
 else:
     from unittest import IsolatedAsyncioTestCase
 
 
 class AsyncIntegrationTest(IntegrationTestBase, IsolatedAsyncioTestCase):
     async def test_crypto_wallets_async(self) -> None:
-        api = self.client.crypto_wallets
+        api = self.b2c_client.crypto_wallets
 
         self.assertTrue(
             (
                 await api.authenticate_start_async(
                     crypto_wallet_type=TEST_CRYPTO_WALLET_TYPE,
                     crypto_wallet_address=TEST_CRYPTO_WALLET_ADDRESS,
                 )
@@ -48,15 +48,15 @@
                     crypto_wallet_address=TEST_CRYPTO_WALLET_ADDRESS,
                     signature=TEST_CRYPTO_SIGNATURE,
                 )
             ).is_success
         )
 
     async def test_magic_links_async(self) -> None:
-        api = self.client.magic_links
+        api = self.b2c_client.magic_links
 
         self.assertTrue(
             (await api.authenticate_async(token=TEST_MAGIC_TOKEN)).is_success
         )
 
         with self.skip_if_stytcherror(
             subtest_name="create_endpoint",
@@ -84,22 +84,22 @@
                 (
                     await api.email.login_or_create_async(email=TEST_MAGIC_EMAIL)
                 ).is_success
             )
             self.assertTrue((await api.email.send_async(TEST_MAGIC_EMAIL)).is_success)
 
     async def test_oauth_async(self) -> None:
-        api = self.client.oauth
+        api = self.b2c_client.oauth
 
         self.assertTrue(
             (await api.authenticate_async(token=TEST_OAUTH_TOKEN)).is_success
         )
 
     async def test_otp_async(self) -> None:
-        api = self.client.otps
+        api = self.b2c_client.otps
 
         with self.subTest("email"):
             self.assertTrue(
                 (await api.email.login_or_create_async(email=TEST_OTP_EMAIL)).is_success
             )
             email_send_response = await api.email.send_async(email=TEST_OTP_EMAIL)
             self.assertTrue(email_send_response.is_success)
@@ -146,30 +146,30 @@
                     await api.authenticate_async(
                         method_id=whatsapp_send_response.phone_id, code=TEST_OTP_CODE
                     )
                 ).is_success
             )
 
     async def test_passwords_async(self) -> None:
-        api = self.client.passwords
+        api = self.b2c_client.passwords
 
         async with self._get_temporary_user_async(create=False) as user:
             self.assertTrue(
                 (await api.strength_check_async(password=user.old_password)).is_success
             )
             create_response = await api.create_async(
                 email=user.email, password=user.old_password
             )
             self.assertTrue(create_response.is_success)
             authenticate_response = await api.authenticate_async(
                 email=user.email, password=user.old_password
             )
             self.assertTrue(authenticate_response.is_success)
             # Remember to manually delete since we manually created!
-            await self.client.users.delete_async(create_response.user_id)
+            await self.b2c_client.users.delete_async(create_response.user_id)
 
         # Migrate an existing user created via magic link
         async with self._get_temporary_user_async(via_magic_link=True) as user:
             self.assertTrue(
                 (
                     await api.migrate_async(
                         email=user.email,
@@ -213,23 +213,23 @@
         with self.subTest("session"):
             # Can't test: there's no sesison token that can be used for testing the API
             self.skipTest("No session token to use for testing")
             async with self._get_temporary_user_async() as user:
                 # TODO: We don't have a sample session token (see skipTest above)
                 self.assertTrue(
                     (
-                        await api.session.reset_async(
+                        await api.sessions.reset_async(
                             session_token="",
                             password=user.new_password,
                         )
                     ).is_success
                 )
 
     async def test_sessions_async(self) -> None:
-        api = self.client.sessions
+        api = self.b2c_client.sessions
 
         async with self._get_temporary_user_async() as user:
             # TODO: With @overload, it should be possible to let
             # the type checker infer this statically. I tried, but
             # it was a bit complicated since it's not a simple type,
             # but actually returning a Generator from a @contextmanager
             assert isinstance(user, CreatedTestUser)
@@ -238,19 +238,19 @@
                 (
                     await api.authenticate_async(session_token=TEST_SESSION_TOKEN)
                 ).is_success
             )
             # Can't test revoke -- it doesn't support the TEST_SESSION_TOKEN
             # self.assertTrue(api.revoke(session_token=TEST_SESSION_TOKEN).is_success)
             self.assertTrue(
-                (await api.jwks_async(project_id=self.project_id)).is_success
+                (await api.get_jwks_async(project_id=self.project_id)).is_success
             )
 
     async def test_totps_async(self) -> None:
-        api = self.client.totps
+        api = self.b2c_client.totps
 
         self.assertTrue((await api.create_async(user_id=TEST_TOTP_USER_ID)).is_success)
         self.assertTrue(
             (
                 await api.authenticate_async(
                     user_id=TEST_TOTP_USER_ID, totp_code=TEST_TOTP_CODE
                 )
@@ -267,20 +267,19 @@
             ).is_success
         )
 
     async def test_users_async(self) -> None:
         # NOTE: the various `delete_XXX` can't easily be tested (yet)
         # since it would require we first create the user with each of those
         # methods/auth factors present (and possibly authenticated?).
-        api = self.client.users
+        api = self.b2c_client.users
 
         async with self._get_temporary_user_async(create=False) as user:
             create_resp = await api.create_async(email=user.email)
             self.assertTrue(create_resp.is_success)
-            self.assertTrue((await api.get_pending_async()).is_success)
             self.assertTrue((await api.search_async(limit=10)).is_success)
             self.assertTrue(
                 (
                     await api.update_async(
                         user_id=create_resp.user_id,
                         name=TEST_USERS_NAME,
                     )
@@ -290,15 +289,15 @@
                 (await api.get_async(user_id=create_resp.user_id)).is_success
             )
             self.assertTrue(
                 (await api.delete_async(user_id=create_resp.user_id)).is_success
             )
 
     async def test_webauthn_async(self) -> None:
-        api = self.client.webauthn
+        api = self.b2c_client.webauthn
         # Can't test: webauthn requires calling browser functions
         # It would probably work if we had some way of using test API
         # sample values (like a sample public_key_credential for testing)
         self.skipTest("webauthn cannot be tested from this client")
 
         async with self._get_temporary_user_async() as user:
             assert isinstance(user, CreatedTestUser)
```

