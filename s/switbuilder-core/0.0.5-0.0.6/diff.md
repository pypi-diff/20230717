# Comparing `tmp/switbuilder_core-0.0.5.tar.gz` & `tmp/switbuilder_core-0.0.6.tar.gz`

## Comparing `switbuilder_core-0.0.5.tar` & `switbuilder_core-0.0.6.tar`

### file list

```diff
@@ -1,99 +1,99 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/.DS_Store
--rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/build.sh
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/requirements.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/.idea/.gitignore
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/.idea/core.iml
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/.idea/misc.xml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/.idea/vcs.xml
--rw-r--r--   0        0        0    29277 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/.idea/workspace.xml
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/__init__.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/constants.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/logger.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/lokalise.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/type.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/action/__init__.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/action/activity_handler_abc.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/action/activity_router.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/action/dependencies.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/action/exceptions.py
--rw-r--r--   0        0        0     7341 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/action/schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/channel/__init__.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/channel/schemas.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/channel/service.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/channel/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/conversation/__init__.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/conversation/schemas.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/conversation/service.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/conversation/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/constants.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/exception.py
--rw-r--r--   0        0        0    11454 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/schemas.py
--rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/service.py
--rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/__init__.py
--rw-r--r--   0        0        0    13670 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/tests.py
--rw-r--r--   0        0        0   306291 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/email/cid_image_email.json
--rw-r--r--   0        0        0  1499842 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/email/email_with_attachment.json
--rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/email/empty_receiver_email.json
--rw-r--r--   0        0        0    43739 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/email/html_email.json
--rw-r--r--   0        0        0    64730 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/email/invalid_swit_image.json
--rw-r--r--   0        0        0   631221 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/email/large_cid_image_email.json
--rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/email/plain_text_email.json
--rw-r--r--   0        0        0    34901 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/html/example1.html
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/html/example2.html
--rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/html/example3.html
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/html/example4.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/membership/__init__.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/membership/schemas.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/membership/service.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/membership/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/project/__init__.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/project/schemas.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/project/service.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/project/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/task/__init__.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/task/schemas.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/task/service.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/task/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/workspace/__init__.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/workspace/schemas.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/workspace/service.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/workspace/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/auth/__init__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/auth/constants.py
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/auth/dependencies.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/auth/exception.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/auth/models.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/auth/repository.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/auth/router.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/auth/schemas.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/auth/service.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/auth/utils.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/Icon.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/__init__.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/button.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/collection_entry.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/container.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/divider.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/file.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/header.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/html_frame.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/image.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/input.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/select.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/select_item.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/signIn_page.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/static_action.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/tabs.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/text_paragraph.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/textarea.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/.gitignore
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/README.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/.DS_Store
+-rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/build.sh
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/requirements.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/.idea/.gitignore
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/.idea/core.iml
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/.idea/misc.xml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/.idea/vcs.xml
+-rw-r--r--   0        0        0    29277 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/.idea/workspace.xml
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/__init__.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/constants.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/logger.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/lokalise.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/type.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/action/__init__.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/action/activity_handler_abc.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/action/activity_router.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/action/dependencies.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/action/exceptions.py
+-rw-r--r--   0        0        0     7374 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/action/schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/channel/__init__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/channel/schemas.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/channel/service.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/channel/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/conversation/__init__.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/conversation/schemas.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/conversation/service.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/conversation/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/imap/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/imap/constants.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/imap/exception.py
+-rw-r--r--   0        0        0    11454 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/imap/schemas.py
+-rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/imap/service.py
+-rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/imap/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/imap/tests/__init__.py
+-rw-r--r--   0        0        0    13670 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/imap/tests/tests.py
+-rw-r--r--   0        0        0   306291 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/imap/tests/email/cid_image_email.json
+-rw-r--r--   0        0        0  1499842 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/imap/tests/email/email_with_attachment.json
+-rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/imap/tests/email/empty_receiver_email.json
+-rw-r--r--   0        0        0    43739 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/imap/tests/email/html_email.json
+-rw-r--r--   0        0        0    64730 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/imap/tests/email/invalid_swit_image.json
+-rw-r--r--   0        0        0   631221 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/imap/tests/email/large_cid_image_email.json
+-rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/imap/tests/email/plain_text_email.json
+-rw-r--r--   0        0        0    34901 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/imap/tests/html/example1.html
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/imap/tests/html/example2.html
+-rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/imap/tests/html/example3.html
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/imap/tests/html/example4.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/membership/__init__.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/membership/schemas.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/membership/service.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/membership/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/project/__init__.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/project/schemas.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/project/service.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/project/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/task/__init__.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/task/schemas.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/task/service.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/task/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/workspace/__init__.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/workspace/schemas.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/workspace/service.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/apis/v1/workspace/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/auth/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/auth/constants.py
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/auth/dependencies.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/auth/exception.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/auth/models.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/auth/repository.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/auth/router.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/auth/schemas.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/auth/service.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/auth/utils.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/ui/Icon.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/ui/__init__.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/ui/button.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/ui/collection_entry.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/ui/container.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/ui/divider.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/ui/file.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/ui/header.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/ui/html_frame.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/ui/image.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/ui/input.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/ui/select.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/ui/select_item.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/ui/signIn_page.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/ui/static_action.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/ui/tabs.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/ui/text_paragraph.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/switcore/ui/textarea.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/.gitignore
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/README.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 switbuilder_core-0.0.6/PKG-INFO
```

### Comparing `switbuilder_core-0.0.5/.DS_Store` & `switbuilder_core-0.0.6/.DS_Store`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/requirements.txt` & `switbuilder_core-0.0.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/.idea/workspace.xml` & `switbuilder_core-0.0.6/.idea/workspace.xml`

 * *Files 0% similar despite different names*

#### Comparing `switbuilder_core-0.0.5/.idea/workspace.xml` & `switbuilder_core-0.0.6/.idea/workspace.xml`

```diff
@@ -117,15 +117,15 @@
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
   <component name="PropertiesComponent"><![CDATA[{
   "keyToString": {
     "RunOnceActivity.ShowReadmeOnStart": "true",
     "WebServerToolWindowFactoryState": "false",
-    "com.google.cloudcode.ide_session_index": "20230717_0008",
+    "com.google.cloudcode.ide_session_index": "20230717_0010",
     "last_opened_file_path": "/Users/el/PycharmProjects/core/switcore",
     "node.js.detected.package.eslint": "true",
     "node.js.detected.package.tslint": "true",
     "node.js.selected.package.eslint": "(autodetect)",
     "node.js.selected.package.tslint": "(autodetect)",
     "settings.editor.selected.configurable": "preferences.lookFeel",
     "vue.rearranger.settings.migration": "true"
@@ -449,15 +449,15 @@
       <workItem from="1689250625591" duration="36000"/>
       <workItem from="1689250806915" duration="2161000"/>
       <workItem from="1689287326456" duration="22000"/>
       <workItem from="1689287357011" duration="77000"/>
       <workItem from="1689287435257" duration="46000"/>
       <workItem from="1689287487514" duration="1547000"/>
       <workItem from="1689309026861" duration="1964000"/>
-      <workItem from="1689550354850" duration="8204000"/>
+      <workItem from="1689550354850" duration="8828000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
```

### Comparing `switbuilder_core-0.0.5/.idea/inspectionProfiles/Project_Default.xml` & `switbuilder_core-0.0.6/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/logger.py` & `switbuilder_core-0.0.6/switcore/logger.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/lokalise.py` & `switbuilder_core-0.0.6/switcore/lokalise.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/action/activity_handler_abc.py` & `switbuilder_core-0.0.6/switcore/action/activity_handler_abc.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/action/activity_router.py` & `switbuilder_core-0.0.6/switcore/action/activity_router.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/action/schemas.py` & `switbuilder_core-0.0.6/switcore/action/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import base64
 import bz2
 import json
 from datetime import datetime
 from enum import Enum
-from typing import Any, Container
+from typing import Any
 from typing import Optional, Dict, List
 
 from pydantic import BaseModel
 from pydantic import validator
 
 from switcore.action.exceptions import InvalidStateException
 from switcore.ui.button import Button
@@ -19,14 +19,15 @@
 from switcore.ui.image import Image
 from switcore.ui.input import Input
 from switcore.ui.select import Select
 from switcore.ui.signIn_page import SignInPage
 from switcore.ui.tabs import Tabs
 from switcore.ui.text_paragraph import TextParagraph
 from switcore.ui.textarea import Textarea
+from switcore.ui.container import Container
 
 
 class UserInfo(BaseModel):
     user_id: str
     organization_id: str
```

### Comparing `switbuilder_core-0.0.5/switcore/apis/v1/channel/service.py` & `switbuilder_core-0.0.6/switcore/apis/v1/channel/service.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/apis/v1/conversation/schemas.py` & `switbuilder_core-0.0.6/switcore/apis/v1/conversation/schemas.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/apis/v1/conversation/service.py` & `switbuilder_core-0.0.6/switcore/apis/v1/conversation/service.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/apis/v1/imap/exception.py` & `switbuilder_core-0.0.6/switcore/apis/v1/imap/exception.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/apis/v1/imap/schemas.py` & `switbuilder_core-0.0.6/switcore/apis/v1/imap/schemas.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/apis/v1/imap/service.py` & `switbuilder_core-0.0.6/switcore/apis/v1/imap/service.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/apis/v1/imap/utils.py` & `switbuilder_core-0.0.6/switcore/apis/v1/imap/utils.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/tests.py` & `switbuilder_core-0.0.6/switcore/apis/v1/imap/tests/tests.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/email/cid_image_email.json` & `switbuilder_core-0.0.6/switcore/apis/v1/imap/tests/email/cid_image_email.json`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/email/email_with_attachment.json` & `switbuilder_core-0.0.6/switcore/apis/v1/imap/tests/email/email_with_attachment.json`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/email/empty_receiver_email.json` & `switbuilder_core-0.0.6/switcore/apis/v1/imap/tests/email/empty_receiver_email.json`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/email/html_email.json` & `switbuilder_core-0.0.6/switcore/apis/v1/imap/tests/email/html_email.json`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/email/invalid_swit_image.json` & `switbuilder_core-0.0.6/switcore/apis/v1/imap/tests/email/invalid_swit_image.json`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/email/large_cid_image_email.json` & `switbuilder_core-0.0.6/switcore/apis/v1/imap/tests/email/large_cid_image_email.json`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/email/plain_text_email.json` & `switbuilder_core-0.0.6/switcore/apis/v1/imap/tests/email/plain_text_email.json`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/html/example1.html` & `switbuilder_core-0.0.6/switcore/apis/v1/imap/tests/html/example1.html`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/html/example3.html` & `switbuilder_core-0.0.6/switcore/apis/v1/imap/tests/html/example3.html`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/html/example4.html` & `switbuilder_core-0.0.6/switcore/apis/v1/imap/tests/html/example4.html`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/apis/v1/membership/schemas.py` & `switbuilder_core-0.0.6/switcore/apis/v1/membership/schemas.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/apis/v1/membership/service.py` & `switbuilder_core-0.0.6/switcore/apis/v1/membership/service.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/apis/v1/project/service.py` & `switbuilder_core-0.0.6/switcore/apis/v1/project/service.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/apis/v1/task/schemas.py` & `switbuilder_core-0.0.6/switcore/apis/v1/task/schemas.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/apis/v1/task/service.py` & `switbuilder_core-0.0.6/switcore/apis/v1/task/service.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/apis/v1/workspace/schemas.py` & `switbuilder_core-0.0.6/switcore/apis/v1/workspace/schemas.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/apis/v1/workspace/service.py` & `switbuilder_core-0.0.6/switcore/apis/v1/workspace/service.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/auth/dependencies.py` & `switbuilder_core-0.0.6/switcore/auth/dependencies.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/auth/repository.py` & `switbuilder_core-0.0.6/switcore/auth/repository.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/auth/router.py` & `switbuilder_core-0.0.6/switcore/auth/router.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/auth/service.py` & `switbuilder_core-0.0.6/switcore/auth/service.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/auth/utils.py` & `switbuilder_core-0.0.6/switcore/auth/utils.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/ui/collection_entry.py` & `switbuilder_core-0.0.6/switcore/ui/collection_entry.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/switcore/ui/file.py` & `switbuilder_core-0.0.6/switcore/ui/file.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.5/pyproject.toml` & `switbuilder_core-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "switbuilder-core"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     { name = "ur-team", email = "el.lee@swit.io" },
 ]
 description = "this is a switbuilder core package"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `switbuilder_core-0.0.5/PKG-INFO` & `switbuilder_core-0.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: switbuilder-core
-Version: 0.0.5
+Version: 0.0.6
 Summary: this is a switbuilder core package
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: ur-team <el.lee@swit.io>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

