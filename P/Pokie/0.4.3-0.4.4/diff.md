# Comparing `tmp/Pokie-0.4.3.tar.gz` & `tmp/Pokie-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pokie-0.4.3.tar", last modified: Wed May 31 15:47:22 2023, max compression
+gzip compressed data, was "Pokie-0.4.4.tar", last modified: Mon Jul 17 17:11:27 2023, max compression
```

## Comparing `Pokie-0.4.3.tar` & `Pokie-0.4.4.tar`

### file list

```diff
@@ -1,151 +1,152 @@
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.478436 Pokie-0.4.3/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1315 2023-05-22 13:10:12.000000 Pokie-0.4.3/LICENSE
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      125 2022-11-22 11:02:45.000000 Pokie-0.4.3/MANIFEST.in
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1865 2023-05-31 15:47:22.478436 Pokie-0.4.3/PKG-INFO
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.466436 Pokie-0.4.3/Pokie.egg-info/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1865 2023-05-31 15:47:22.000000 Pokie-0.4.3/Pokie.egg-info/PKG-INFO
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3406 2023-05-31 15:47:22.000000 Pokie-0.4.3/Pokie.egg-info/SOURCES.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        1 2023-05-31 15:47:22.000000 Pokie-0.4.3/Pokie.egg-info/dependency_links.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        1 2022-11-03 11:00:15.000000 Pokie-0.4.3/Pokie.egg-info/not-zip-safe
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      157 2023-05-31 15:47:22.000000 Pokie-0.4.3/Pokie.egg-info/requires.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       12 2023-05-31 15:47:22.000000 Pokie-0.4.3/Pokie.egg-info/top_level.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      619 2023-05-22 13:15:40.000000 Pokie-0.4.3/README.md
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.466436 Pokie-0.4.3/pokie/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       64 2022-11-03 10:59:50.000000 Pokie-0.4.3/pokie/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      116 2022-11-03 11:57:08.000000 Pokie-0.4.3/pokie/__main__.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.470436 Pokie-0.4.3/pokie/codegen/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-11-03 12:16:47.000000 Pokie-0.4.3/pokie/codegen/__init__.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.470436 Pokie-0.4.3/pokie/codegen/pg/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      104 2022-11-07 16:24:37.000000 Pokie-0.4.3/pokie/codegen/pg/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2044 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/codegen/pg/record.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     4238 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/codegen/pg/request.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     4111 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/codegen/pg/spec.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      405 2022-11-07 16:10:53.000000 Pokie-0.4.3/pokie/codegen/spec.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2585 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/codegen/template.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      590 2022-11-07 16:13:57.000000 Pokie-0.4.3/pokie/codegen/textfile.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.470436 Pokie-0.4.3/pokie/config/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-10-01 10:15:02.000000 Pokie-0.4.3/pokie/config/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1982 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/config/template.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1259 2023-05-31 15:18:34.000000 Pokie-0.4.3/pokie/constants.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.470436 Pokie-0.4.3/pokie/contrib/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-10-12 14:05:40.000000 Pokie-0.4.3/pokie/contrib/__init__.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.470436 Pokie-0.4.3/pokie/contrib/auth/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-08-20 16:06:46.000000 Pokie-0.4.3/pokie/contrib/auth/__init__.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.470436 Pokie-0.4.3/pokie/contrib/auth/cli/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      358 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/auth/cli/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)    11699 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/auth/cli/acl.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)    10570 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/auth/cli/user.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       80 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/auth/constants.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.470436 Pokie-0.4.3/pokie/contrib/auth/dto/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       48 2022-10-13 10:50:07.000000 Pokie-0.4.3/pokie/contrib/auth/dto/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      654 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/auth/dto/acl.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      410 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/auth/dto/user.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1491 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/auth/module.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.470436 Pokie-0.4.3/pokie/contrib/auth/plugin/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       29 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/auth/plugin/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2719 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/auth/plugin/db.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.470436 Pokie-0.4.3/pokie/contrib/auth/repository/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-08-20 16:09:00.000000 Pokie-0.4.3/pokie/contrib/auth/repository/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     8672 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/auth/repository/acl.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      989 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/auth/repository/user.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.470436 Pokie-0.4.3/pokie/contrib/auth/service/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       88 2022-10-01 12:37:49.000000 Pokie-0.4.3/pokie/contrib/auth/service/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3396 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/auth/service/acl.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2510 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/auth/service/auth.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2998 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/auth/service/user.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.470436 Pokie-0.4.3/pokie/contrib/auth/sql/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1179 2023-05-30 08:22:14.000000 Pokie-0.4.3/pokie/contrib/auth/sql/001-auth-schema.sql
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.470436 Pokie-0.4.3/pokie/contrib/auth/view/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-08-20 16:10:16.000000 Pokie-0.4.3/pokie/contrib/auth/view/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1660 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/auth/view/account.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.470436 Pokie-0.4.3/pokie/contrib/base/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-10-01 14:59:52.000000 Pokie-0.4.3/pokie/contrib/base/__init__.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.470436 Pokie-0.4.3/pokie/contrib/base/cli/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      326 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/cli/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     5275 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/cli/base.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     7245 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/cli/db.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     6326 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/cli/db_codegen.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3080 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/cli/fixture.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2325 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/cli/job.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      482 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/cli/pytest.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1578 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/cli/tpl_codegen.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      106 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/constants.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.470436 Pokie-0.4.3/pokie/contrib/base/dto/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       51 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/dto/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      329 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/dto/records.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.470436 Pokie-0.4.3/pokie/contrib/base/job/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       26 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/job/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      459 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/job/idle.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1776 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/module.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.474436 Pokie-0.4.3/pokie/contrib/base/repository/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       43 2022-10-12 13:28:57.000000 Pokie-0.4.3/pokie/contrib/base/repository/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      191 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/repository/fixture.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1985 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/repository/settings.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      807 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/repository/validator.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.474436 Pokie-0.4.3/pokie/contrib/base/service/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      128 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/service/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1025 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/service/autorest.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2098 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/service/fixture.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1125 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/service/settings.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2079 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/service/validator.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.474436 Pokie-0.4.3/pokie/contrib/base/sql/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      210 2022-11-02 00:49:04.000000 Pokie-0.4.3/pokie/contrib/base/sql/001-settings.sql
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      138 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/sql/002-fixtures.sql
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.474436 Pokie-0.4.3/pokie/contrib/base/validators/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       46 2022-10-12 13:46:20.000000 Pokie-0.4.3/pokie/contrib/base/validators/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1507 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/base/validators/pk.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.474436 Pokie-0.4.3/pokie/contrib/mail/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/mail/__init__.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.474436 Pokie-0.4.3/pokie/contrib/mail/cli/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       46 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/mail/cli/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1502 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/mail/cli/queue.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       78 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/mail/constants.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.474436 Pokie-0.4.3/pokie/contrib/mail/dto/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       63 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/mail/dto/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      728 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/mail/dto/records.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1466 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/mail/helpers.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.474436 Pokie-0.4.3/pokie/contrib/mail/job/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       32 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/mail/job/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2069 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/mail/job/queue.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      661 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/mail/module.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.474436 Pokie-0.4.3/pokie/contrib/mail/repository/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       76 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/mail/repository/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2823 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/mail/repository/repositories.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.474436 Pokie-0.4.3/pokie/contrib/mail/service/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       84 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/mail/service/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1369 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/mail/service/queue.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      939 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/mail/service/template.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.474436 Pokie-0.4.3/pokie/contrib/mail/sql/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      854 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/contrib/mail/sql/001-mail.sql
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.474436 Pokie-0.4.3/pokie/core/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      139 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/core/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     7229 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/core/application.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      657 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/core/command.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.474436 Pokie-0.4.3/pokie/core/factories/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-10-01 12:07:49.000000 Pokie-0.4.3/pokie/core/factories/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      664 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/core/factories/login.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      887 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/core/factories/pgsql.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      848 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/core/factories/redis.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      475 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/core/module.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      813 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/core/signal.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.474436 Pokie-0.4.3/pokie/http/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       96 2022-11-22 11:02:45.000000 Pokie-0.4.3/pokie/http/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2045 2023-05-31 15:22:30.000000 Pokie-0.4.3/pokie/http/helpers.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      175 2022-10-31 14:57:32.000000 Pokie-0.4.3/pokie/http/response.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3129 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/http/rest.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2165 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/http/routes.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     9475 2023-05-29 17:32:51.000000 Pokie-0.4.3/pokie/http/view.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.474436 Pokie-0.4.3/pokie/plugins/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-10-14 15:27:51.000000 Pokie-0.4.3/pokie/plugins/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      731 2022-11-22 11:02:45.000000 Pokie-0.4.3/pokie/plugins/auth.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.474436 Pokie-0.4.3/pokie/rest/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       69 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/rest/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      652 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/rest/mixin.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2174 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/rest/service.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.478436 Pokie-0.4.3/pokie/util/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-10-01 18:39:00.000000 Pokie-0.4.3/pokie/util/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      775 2023-05-22 13:10:12.000000 Pokie-0.4.3/pokie/util/cli_args.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1576 2023-05-31 15:47:22.478436 Pokie-0.4.3/setup.cfg
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       39 2022-11-03 10:58:29.000000 Pokie-0.4.3/setup.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-05-31 15:47:22.478436 Pokie-0.4.3/tests/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-11-22 11:02:45.000000 Pokie-0.4.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.965400 Pokie-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-17 17:10:55.000000 Pokie-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-17 17:10:55.000000 Pokie-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-17 17:11:27.965400 Pokie-0.4.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.957400 Pokie-0.4.4/Pokie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-17 17:11:27.000000 Pokie-0.4.4/Pokie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-07-17 17:11:27.000000 Pokie-0.4.4/Pokie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 17:11:27.000000 Pokie-0.4.4/Pokie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 17:11:27.000000 Pokie-0.4.4/Pokie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-17 17:11:27.000000 Pokie-0.4.4/Pokie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 17:11:27.000000 Pokie-0.4.4/Pokie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-17 17:10:55.000000 Pokie-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.957400 Pokie-0.4.4/pokie/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.957400 Pokie-0.4.4/pokie/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/codegen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.957400 Pokie-0.4.4/pokie/codegen/pg/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/codegen/pg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/codegen/pg/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/codegen/pg/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/codegen/pg/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/codegen/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/codegen/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/codegen/textfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.957400 Pokie-0.4.4/pokie/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/config/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.957400 Pokie-0.4.4/pokie/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.957400 Pokie-0.4.4/pokie/contrib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.957400 Pokie-0.4.4/pokie/contrib/auth/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/cli/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/cli/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.957400 Pokie-0.4.4/pokie/contrib/auth/dto/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/dto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/dto/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/dto/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.957400 Pokie-0.4.4/pokie/contrib/auth/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/plugin/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.957400 Pokie-0.4.4/pokie/contrib/auth/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8672 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/repository/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/repository/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.961400 Pokie-0.4.4/pokie/contrib/auth/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/service/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/service/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/service/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.961400 Pokie-0.4.4/pokie/contrib/auth/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/sql/001-auth-schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.961400 Pokie-0.4.4/pokie/contrib/auth/view/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/view/account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.961400 Pokie-0.4.4/pokie/contrib/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.961400 Pokie-0.4.4/pokie/contrib/base/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/cli/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/cli/db_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/cli/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/cli/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/cli/pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/cli/tpl_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.961400 Pokie-0.4.4/pokie/contrib/base/dto/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/dto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/dto/records.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.961400 Pokie-0.4.4/pokie/contrib/base/job/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/job/idle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.961400 Pokie-0.4.4/pokie/contrib/base/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/repository/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/repository/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/repository/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.961400 Pokie-0.4.4/pokie/contrib/base/service/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/service/autorest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/service/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/service/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/service/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.961400 Pokie-0.4.4/pokie/contrib/base/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/sql/001-settings.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/sql/002-fixtures.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.961400 Pokie-0.4.4/pokie/contrib/base/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/validators/pk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.961400 Pokie-0.4.4/pokie/contrib/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/mail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.965400 Pokie-0.4.4/pokie/contrib/mail/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/mail/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/mail/cli/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/mail/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.965400 Pokie-0.4.4/pokie/contrib/mail/dto/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/mail/dto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/mail/dto/records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/mail/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.965400 Pokie-0.4.4/pokie/contrib/mail/job/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/mail/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/mail/job/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/mail/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.965400 Pokie-0.4.4/pokie/contrib/mail/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/mail/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/mail/repository/repositories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.965400 Pokie-0.4.4/pokie/contrib/mail/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/mail/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/mail/service/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/mail/service/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.965400 Pokie-0.4.4/pokie/contrib/mail/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/mail/sql/001-mail.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.965400 Pokie-0.4.4/pokie/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/core/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.965400 Pokie-0.4.4/pokie/core/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/core/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/core/factories/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/core/factories/pgsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/core/factories/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/core/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/core/signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.965400 Pokie-0.4.4/pokie/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/http/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/http/http_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/http/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/http/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/http/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/http/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.965400 Pokie-0.4.4/pokie/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/plugins/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.965400 Pokie-0.4.4/pokie/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/rest/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/rest/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.965400 Pokie-0.4.4/pokie/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/util/cli_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-17 17:11:27.965400 Pokie-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-17 17:10:55.000000 Pokie-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.965400 Pokie-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:10:55.000000 Pokie-0.4.4/tests/__init__.py
```

### Comparing `Pokie-0.4.3/LICENSE` & `Pokie-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/PKG-INFO` & `Pokie-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pokie
-Version: 0.4.3
+Version: 0.4.4
 Summary: A high-level Python REST web framework based on Flask, Rick and RickDb.
 Home-page: https://git.oddbit.org/OddBit/pokie
 Author: João Pinheiro
 License: BSD-3-Clause
 Project-URL: Documentation, https://docs.oddbit.org/pokie/
 Project-URL: Source, https://git.oddbit.org/OddBit/pokie
 Classifier: Environment :: Web Environment
```

### Comparing `Pokie-0.4.3/Pokie.egg-info/PKG-INFO` & `Pokie-0.4.4/Pokie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pokie
-Version: 0.4.3
+Version: 0.4.4
 Summary: A high-level Python REST web framework based on Flask, Rick and RickDb.
 Home-page: https://git.oddbit.org/OddBit/pokie
 Author: João Pinheiro
 License: BSD-3-Clause
 Project-URL: Documentation, https://docs.oddbit.org/pokie/
 Project-URL: Source, https://git.oddbit.org/OddBit/pokie
 Classifier: Environment :: Web Environment
```

### Comparing `Pokie-0.4.3/Pokie.egg-info/SOURCES.txt` & `Pokie-0.4.4/Pokie.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 pokie/core/signal.py
 pokie/core/factories/__init__.py
 pokie/core/factories/login.py
 pokie/core/factories/pgsql.py
 pokie/core/factories/redis.py
 pokie/http/__init__.py
 pokie/http/helpers.py
+pokie/http/http_error.py
 pokie/http/response.py
 pokie/http/rest.py
 pokie/http/routes.py
 pokie/http/view.py
 pokie/plugins/__init__.py
 pokie/plugins/auth.py
 pokie/rest/__init__.py
```

### Comparing `Pokie-0.4.3/README.md` & `Pokie-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/codegen/pg/record.py` & `Pokie-0.4.4/pokie/codegen/pg/record.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/codegen/pg/request.py` & `Pokie-0.4.4/pokie/codegen/pg/request.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/codegen/pg/spec.py` & `Pokie-0.4.4/pokie/codegen/pg/spec.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/codegen/template.py` & `Pokie-0.4.4/pokie/codegen/template.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/codegen/textfile.py` & `Pokie-0.4.4/pokie/codegen/textfile.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/config/template.py` & `Pokie-0.4.4/pokie/config/template.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import uuid
 
 from rick.resource.config import StrOrFile
 
 
 class BaseConfigTemplate:
+    # default HTTP Exception Handler - 404 and 500 exceptions
+    HTTP_ERROR_HANDLER = 'pokie.http.HttpErrorHandler'
+
     # list of enabled module names
     MODULES = []
     # if true, all endpoints are authenticated by default
     USE_AUTH = True
     # Autentication plugins to use
     AUTH_PLUGINS = ["pokie.contrib.auth.plugin.DbAuthPlugin"]
```

### Comparing `Pokie-0.4.3/pokie/constants.py` & `Pokie-0.4.4/pokie/constants.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Version
-POKIE_VERSION = ["0", "4", "3"]
+POKIE_VERSION = ["0", "4", "4"]
 
 
 def get_version():
     return ".".join(POKIE_VERSION)
 
 
 # Http Codes
@@ -11,24 +11,28 @@
 HTTP_BADREQ = 400
 HTTP_NOAUTH = 401
 HTTP_FORBIDDEN = 403
 HTTP_NOT_FOUND = 404
 HTTP_INTERNAL_ERROR = 500
 
 # DI Keys
-DI_CONFIG = "config"
-DI_FLASK = "app"
-DI_APP = "main"
-DI_MODULES = "modules"
-DI_SERVICES = "svc_manager"
-DI_DB = "db"
-DI_REDIS = "redis"
-DI_EVENTS = "event_manager"
-DI_TTY = "tty"
-DI_SIGNAL = "signal"
+DI_CONFIG = "config"  # config object
+DI_FLASK = "app"  # flask application
+DI_APP = "main"  # pokie application
+DI_MODULES = "modules"  # module list
+DI_SERVICES = "svc_manager"  # service manager
+DI_DB = "db"  # database client
+DI_REDIS = "redis"  # redis client
+DI_EVENTS = "event_manager"  # event manager
+DI_TTY = "tty"  # console writer
+DI_SIGNAL = "signal"  # signal manager
+DI_HTTP_ERROR_HANDLER = "http_error_handler"  # http exception manager
+
+# Error Handler configuration
+CFG_HTTP_ERROR_HANLDER = "http_error_handler"
 
 # DB Configuration
 CFG_DB_NAME = "db_name"
 CFG_DB_HOST = "db_host"
 CFG_DB_PORT = "db_port"
 CFG_DB_USER = "db_user"
 CFG_DB_PASSWORD = "db_password"
@@ -40,15 +44,14 @@
 CFG_REDIS_PASSWORD = "redis_password"
 CFG_REDIS_DB = "redis_db"
 CFG_REDIS_SSL = "redis_ssl"
 
 # Auth Configuration
 CFG_AUTH_SECRET = "auth_secret"
 
-
 # SMTP Configuration
 CFG_SMTP_HOST = "smtp_host"
 CFG_SMTP_PORT = "smtp_port"
 CFG_SMTP_USE_TLS = "smtp_use_tls"
 CFG_SMTP_USE_SSL = "smtp_use_ssl"
 CFG_SMTP_DEBUG = "smtp_debug"
 CFG_SMTP_USERNAME = "smtp_username"
```

### Comparing `Pokie-0.4.3/pokie/contrib/auth/cli/acl.py` & `Pokie-0.4.4/pokie/contrib/auth/cli/acl.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/auth/cli/user.py` & `Pokie-0.4.4/pokie/contrib/auth/cli/user.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/auth/dto/acl.py` & `Pokie-0.4.4/pokie/contrib/auth/dto/acl.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/auth/module.py` & `Pokie-0.4.4/pokie/contrib/auth/module.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/auth/plugin/db.py` & `Pokie-0.4.4/pokie/contrib/auth/plugin/db.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/auth/repository/acl.py` & `Pokie-0.4.4/pokie/contrib/auth/repository/acl.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/auth/repository/user.py` & `Pokie-0.4.4/pokie/contrib/auth/repository/user.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/auth/service/acl.py` & `Pokie-0.4.4/pokie/contrib/auth/service/acl.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/auth/service/auth.py` & `Pokie-0.4.4/pokie/contrib/auth/service/auth.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/auth/service/user.py` & `Pokie-0.4.4/pokie/contrib/auth/service/user.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/auth/sql/001-auth-schema.sql` & `Pokie-0.4.4/pokie/contrib/auth/sql/001-auth-schema.sql`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/auth/view/account.py` & `Pokie-0.4.4/pokie/contrib/auth/view/account.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/base/cli/base.py` & `Pokie-0.4.4/pokie/contrib/base/cli/base.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/base/cli/db.py` & `Pokie-0.4.4/pokie/contrib/base/cli/db.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/base/cli/db_codegen.py` & `Pokie-0.4.4/pokie/contrib/base/cli/db_codegen.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/base/cli/fixture.py` & `Pokie-0.4.4/pokie/contrib/base/cli/fixture.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/base/cli/job.py` & `Pokie-0.4.4/pokie/contrib/base/cli/job.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/base/cli/tpl_codegen.py` & `Pokie-0.4.4/pokie/contrib/base/cli/tpl_codegen.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/base/module.py` & `Pokie-0.4.4/pokie/contrib/base/module.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/base/repository/settings.py` & `Pokie-0.4.4/pokie/contrib/base/repository/settings.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/base/repository/validator.py` & `Pokie-0.4.4/pokie/contrib/base/repository/validator.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/base/service/autorest.py` & `Pokie-0.4.4/pokie/contrib/base/service/autorest.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/base/service/fixture.py` & `Pokie-0.4.4/pokie/contrib/base/service/fixture.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/base/service/settings.py` & `Pokie-0.4.4/pokie/contrib/base/service/settings.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/base/service/validator.py` & `Pokie-0.4.4/pokie/contrib/base/service/validator.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/base/validators/pk.py` & `Pokie-0.4.4/pokie/contrib/base/validators/pk.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/mail/cli/queue.py` & `Pokie-0.4.4/pokie/contrib/mail/cli/queue.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/mail/dto/records.py` & `Pokie-0.4.4/pokie/contrib/mail/dto/records.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/mail/helpers.py` & `Pokie-0.4.4/pokie/contrib/mail/helpers.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/mail/job/queue.py` & `Pokie-0.4.4/pokie/contrib/mail/job/queue.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/mail/module.py` & `Pokie-0.4.4/pokie/contrib/mail/module.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/mail/repository/repositories.py` & `Pokie-0.4.4/pokie/contrib/mail/repository/repositories.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/mail/service/queue.py` & `Pokie-0.4.4/pokie/contrib/mail/service/queue.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/mail/service/template.py` & `Pokie-0.4.4/pokie/contrib/mail/service/template.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/contrib/mail/sql/001-mail.sql` & `Pokie-0.4.4/pokie/contrib/mail/sql/001-mail.sql`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/core/application.py` & `Pokie-0.4.4/pokie/core/application.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 from argparse import ArgumentParser
 from typing import List
 from collections import OrderedDict
 
 from flask import Flask
 from rick.base import Di, Container, MapLoader
 from rick.event import EventManager
+from rick.mixin import Injectable
 from rick.util.loader import load_class
 from rick.resource.console import ConsoleWriter
 
 from pokie.constants import (
     DI_CONFIG,
     DI_SERVICES,
     DI_FLASK,
     DI_APP,
     DI_EVENTS,
     DI_TTY,
-    DI_SIGNAL,
+    DI_SIGNAL, CFG_HTTP_ERROR_HANLDER, DI_HTTP_ERROR_HANDLER,
 )
 from .module import BaseModule
 from .command import CliCommand
 from pokie.util.cli_args import ArgParser
 from .signal import SignalManager
 
 
@@ -127,14 +128,23 @@
                 for evt_name, evt_details in module_events.items():
                     for priority, handlers in evt_details.items():
                         for handler in handlers:
                             evt_mgr.add_handler(evt_name, handler, int(priority))
 
         self.di.add(DI_EVENTS, evt_mgr)
 
+        # register exception handler
+        if self.cfg.has(CFG_HTTP_ERROR_HANLDER):
+            handler = load_class(self.cfg.get(CFG_HTTP_ERROR_HANLDER), True)
+            if not issubclass(handler, Injectable):
+                raise RuntimeError("build(): HTTP_ERROR_HANDLER class does not extend Injectable")
+            # initialize & register handler
+            handler = handler(self.di)
+            self.di.add(DI_HTTP_ERROR_HANDLER, handler)
+
         # initialize modules
         for _, module in self.modules.items():
             module.build(self)
 
         return self.app
 
     def http(self, **kwargs):
```

### Comparing `Pokie-0.4.3/pokie/core/command.py` & `Pokie-0.4.4/pokie/core/command.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/core/factories/login.py` & `Pokie-0.4.4/pokie/core/factories/login.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/core/factories/pgsql.py` & `Pokie-0.4.4/pokie/core/factories/pgsql.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/core/factories/redis.py` & `Pokie-0.4.4/pokie/core/factories/redis.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/core/signal.py` & `Pokie-0.4.4/pokie/core/signal.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/http/helpers.py` & `Pokie-0.4.4/pokie/http/helpers.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/http/rest.py` & `Pokie-0.4.4/pokie/http/rest.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/http/routes.py` & `Pokie-0.4.4/pokie/http/routes.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/http/view.py` & `Pokie-0.4.4/pokie/http/view.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 import logging
 from typing import Any, Optional, Callable
 from flask import request
 from flask.views import MethodView
 from flask.typing import ResponseReturnValue
 from flask import current_app
 from flask_login import current_user
-from rick.serializer.json import ExtendedJsonEncoder
 from rick.form import RequestRecord
 
-from .response import JsonRequestError, JsonStatus
+from .response import JsonResponse
 from pokie.constants import (
     HTTP_OK,
     HTTP_BADREQ,
     HTTP_INTERNAL_ERROR,
     HTTP_NOAUTH,
     HTTP_FORBIDDEN,
     DI_SERVICES,
@@ -24,17 +23,24 @@
     # allowed HTTP methods
     allow_methods = ["get", "post", "put", "patch", "delete", "head"]
 
     # optional RequestRecord class for request body unmarshall
     # see self.request below
     request_class = None  # type: RequestRecord
 
+    # default response class
+    response_class = JsonResponse
+
+    # default error message
+    msg_error_default = "request failed"
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.di = current_app.di
+        self.logger = current_app.logger
 
         # methods where automatic body deserialization is attempted
         #
         # names must be lowercase
         self.methods_unmarshall_request = ["post", "put", "patch"]
 
         # automatic request de-serialization
@@ -55,15 +61,15 @@
         # optional override of internal options
         for name, value in kwargs.items():
             attr = getattr(self, name, None)
             if attr is not None and not callable(attr):
                 setattr(self, name, value)
 
     def _hook_request(
-            self, method: str, *args: Any, **kwargs: Any
+        self, method: str, *args: Any, **kwargs: Any
     ) -> Optional[ResponseReturnValue]:
         """
         Dispatch hook: de-serialize request
         If body is not json, will use flask form data
 
         :param method: method name in lowercase
         :param args:
@@ -136,15 +142,15 @@
 
             return current_app.ensure_sync(handler)(*args, **kwargs)
         except Exception as e:
             return self.exception_handler(e)
 
     @classmethod
     def view_method(
-            cls, action_method: str, name=None, *class_args: Any, **class_kwargs: Any
+        cls, action_method: str, name=None, *class_args: Any, **class_kwargs: Any
     ) -> Callable:
         """
         Variant of Flask's as_view that supports custom handlers for actions
         :param action_method: method to be called on dispatch 
         :param name: optional route name
         :param class_args: 
         :param class_kwargs: 
@@ -184,74 +190,91 @@
     def exception_handler(self, e) -> ResponseReturnValue:
         """
         Generic exception handler for dispatch
         :param e:
         :return:
         """
         if e is not None:
-            logging.exception(e)
-        if request.is_json:
-            return self.error("bad request")
-        return (
-            "<!doctype html>\n<html lang=en>\n<title>{code} {err}</title>\n<h1>{err}</h1>\n".format(
-                code=HTTP_BADREQ, err="Bad Request"
-            ),
-            HTTP_BADREQ,
-        )
-
-    def json(self, data, code=HTTP_OK):
-        """
-        Adaptation of flask's jsonify using Rick's ExtendedJsonEncoder
-        :param data:
-        :param code:
-        :return:
+            self.logger.exception(e)
+        return self.error("bad request")
+
+    def success(self, data=None, code: int = HTTP_OK):
+        """
+        Returns a success response with optional data payload
+        :param data: optional response data
+        :param code: int
+        :return: Response
         """
-        indent = None
-        separators = (",", ":")
+        cls = self.response_class(data=data, success=True, code=code)
+        return cls.assemble(current_app)
 
-        if current_app.json.compact or current_app.debug:
-            indent = 2
-            separators = (", ", ": ")
-
-        data = json.dumps(
-            data, indent=indent, separators=separators, cls=ExtendedJsonEncoder
-        )
-        return current_app.response_class(
-            data, status=code, mimetype=current_app.json.mimetype
-        )
+    def success_message(self, message: str):
+        """
+        Returns a success response with a string message
+        :param message: str
+        :return: Response
+        """
+        return self.success({"message": message})
 
     def error(self, message=None, code=HTTP_BADREQ):
-        data = JsonStatus(
-            success=False, message=message if message else "operation failed"
-        )
-        return self.json(data, code)
-
-    def request_error(self, req: RequestRecord, code=HTTP_BADREQ):
-        return self.json(
-            JsonRequestError(success=False, formError=req.get_errors()), code
-        )
-
-    def success_message(self, message=""):
-        return self.json(JsonStatus(success=True, message=message))
-
-    def success(self, data=None, code=HTTP_OK):
-        if data is None:
-            return self.json(JsonStatus(success=True, message=""), code=code)
-        return self.json(data, code)
+        """
+        Returns an error response with an optional string message
+        if no message is provided, defaults to PokieView.msg_error_default
+        :param message: str
+        :param code: int
+        :return: Response
+        """
+
+        if message is None:
+            message = self.msg_error_default
+
+        cls = self.response_class(error={"message": message}, success=False, code=code)
+        return cls.assemble(current_app)
+
+    def request_error(self, request_object: RequestRecord, code=HTTP_BADREQ):
+        """
+        Returns a RequestRecord error response
+
+        :param request_object: RequestRecord
+        :param code: int
+        :return: Response
+        """
+        error = {
+            "message": self.msg_error_default,
+            "formError": request_object.get_errors(),
+        }
+        cls = self.response_class(error=error, success=False, code=code)
+        return cls.assemble(current_app)
 
     def empty_body(self):
+        """
+        Error: empty body
+        :return: Request
+        """
         return self.error("empty body", code=HTTP_BADREQ)
 
     def not_found(self):
+        """
+        Error: not found
+        :return: Request
+        """
         return self.error("record not found", code=HTTP_BADREQ)
 
     def forbidden(self):
+        """
+        Error: access denied
+        :return: Request
+        """
         return self.error("access denied", code=HTTP_FORBIDDEN)
 
     def denied(self):
+        """
+        Error: access denied
+        :return: Request
+        """
         return self.error("access denied", code=HTTP_NOAUTH)
 
     def get_service(self, service_name):
         return self.di.get(DI_SERVICES).get(service_name)
 
 
 class PokieAuthView(PokieView):
@@ -263,15 +286,15 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         # auth first
         self.dispatch_hooks = ["_hook_auth"] + self.dispatch_hooks
         self.user = current_user
 
     def _hook_auth(
-            self, method: str, *args: Any, **kwargs: Any
+        self, method: str, *args: Any, **kwargs: Any
     ) -> Optional[ResponseReturnValue]:
         if not current_user.is_authenticated:
             return self.denied()
 
         for acl in self.acl:
             if not self.user.can_access(acl):
                 return self.forbidden()
```

### Comparing `Pokie-0.4.3/pokie/plugins/auth.py` & `Pokie-0.4.4/pokie/plugins/auth.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/rest/mixin.py` & `Pokie-0.4.4/pokie/rest/mixin.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/rest/service.py` & `Pokie-0.4.4/pokie/rest/service.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/pokie/util/cli_args.py` & `Pokie-0.4.4/pokie/util/cli_args.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.3/setup.cfg` & `Pokie-0.4.4/setup.cfg`

 * *Files identical despite different names*

