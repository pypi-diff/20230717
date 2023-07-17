# Comparing `tmp/switbuilder_core-0.0.4.tar.gz` & `tmp/switbuilder_core-0.0.5.tar.gz`

## Comparing `switbuilder_core-0.0.4.tar` & `switbuilder_core-0.0.5.tar`

### file list

```diff
@@ -1,99 +1,99 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/.DS_Store
--rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/build.sh
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/requirements.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/.idea/.gitignore
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/.idea/core.iml
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/.idea/misc.xml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/.idea/vcs.xml
--rw-r--r--   0        0        0    29277 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/.idea/workspace.xml
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/__init__.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/constants.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/logger.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/lokalise.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/type.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/action/__init__.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/action/activity_handler_abc.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/action/activity_router.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/action/dependencies.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/action/exceptions.py
--rw-r--r--   0        0        0     7341 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/action/schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/channel/__init__.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/channel/schemas.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/channel/service.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/channel/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/conversation/__init__.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/conversation/schemas.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/conversation/service.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/conversation/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/constants.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/exception.py
--rw-r--r--   0        0        0    11454 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/schemas.py
--rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/service.py
--rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/__init__.py
--rw-r--r--   0        0        0    13670 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/tests.py
--rw-r--r--   0        0        0   306291 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/email/cid_image_email.json
--rw-r--r--   0        0        0  1499842 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/email/email_with_attachment.json
--rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/email/empty_receiver_email.json
--rw-r--r--   0        0        0    43739 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/email/html_email.json
--rw-r--r--   0        0        0    64730 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/email/invalid_swit_image.json
--rw-r--r--   0        0        0   631221 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/email/large_cid_image_email.json
--rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/email/plain_text_email.json
--rw-r--r--   0        0        0    34901 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/html/example1.html
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/html/example2.html
--rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/html/example3.html
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/html/example4.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/membership/__init__.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/membership/schemas.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/membership/service.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/membership/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/project/__init__.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/project/schemas.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/project/service.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/project/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/task/__init__.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/task/schemas.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/task/service.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/task/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/workspace/__init__.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/workspace/schemas.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/workspace/service.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/workspace/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/auth/__init__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/auth/constants.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/auth/dependencies.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/auth/exception.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/auth/models.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/auth/repository.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/auth/router.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/auth/schemas.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/auth/service.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/auth/utils.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/Icon.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/__init__.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/button.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/collection_entry.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/container.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/divider.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/file.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/header.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/html_frame.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/image.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/input.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/select.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/select_item.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/signIn_page.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/static_action.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/tabs.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/text_paragraph.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/textarea.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/.gitignore
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/README.md
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/.DS_Store
+-rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/build.sh
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/requirements.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/.idea/.gitignore
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/.idea/core.iml
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/.idea/misc.xml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/.idea/vcs.xml
+-rw-r--r--   0        0        0    29277 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/.idea/workspace.xml
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/__init__.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/constants.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/logger.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/lokalise.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/type.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/action/__init__.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/action/activity_handler_abc.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/action/activity_router.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/action/dependencies.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/action/exceptions.py
+-rw-r--r--   0        0        0     7341 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/action/schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/channel/__init__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/channel/schemas.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/channel/service.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/channel/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/conversation/__init__.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/conversation/schemas.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/conversation/service.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/conversation/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/constants.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/exception.py
+-rw-r--r--   0        0        0    11454 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/schemas.py
+-rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/service.py
+-rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/__init__.py
+-rw-r--r--   0        0        0    13670 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/tests.py
+-rw-r--r--   0        0        0   306291 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/email/cid_image_email.json
+-rw-r--r--   0        0        0  1499842 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/email/email_with_attachment.json
+-rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/email/empty_receiver_email.json
+-rw-r--r--   0        0        0    43739 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/email/html_email.json
+-rw-r--r--   0        0        0    64730 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/email/invalid_swit_image.json
+-rw-r--r--   0        0        0   631221 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/email/large_cid_image_email.json
+-rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/email/plain_text_email.json
+-rw-r--r--   0        0        0    34901 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/html/example1.html
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/html/example2.html
+-rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/html/example3.html
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/html/example4.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/membership/__init__.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/membership/schemas.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/membership/service.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/membership/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/project/__init__.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/project/schemas.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/project/service.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/project/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/task/__init__.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/task/schemas.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/task/service.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/task/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/workspace/__init__.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/workspace/schemas.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/workspace/service.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/apis/v1/workspace/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/auth/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/auth/constants.py
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/auth/dependencies.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/auth/exception.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/auth/models.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/auth/repository.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/auth/router.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/auth/schemas.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/auth/service.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/auth/utils.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/Icon.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/__init__.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/button.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/collection_entry.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/container.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/divider.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/file.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/header.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/html_frame.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/image.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/input.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/select.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/select_item.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/signIn_page.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/static_action.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/tabs.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/text_paragraph.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/switcore/ui/textarea.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/.gitignore
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/README.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 switbuilder_core-0.0.5/PKG-INFO
```

### Comparing `switbuilder_core-0.0.4/.DS_Store` & `switbuilder_core-0.0.5/.DS_Store`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/requirements.txt` & `switbuilder_core-0.0.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/.idea/workspace.xml` & `switbuilder_core-0.0.5/.idea/workspace.xml`

 * *Files identical despite different names*

#### Comparing `switbuilder_core-0.0.4/.idea/workspace.xml` & `switbuilder_core-0.0.5/.idea/workspace.xml`

```diff
@@ -117,15 +117,15 @@
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
   <component name="PropertiesComponent"><![CDATA[{
   "keyToString": {
     "RunOnceActivity.ShowReadmeOnStart": "true",
     "WebServerToolWindowFactoryState": "false",
-    "com.google.cloudcode.ide_session_index": "20230717_0006",
+    "com.google.cloudcode.ide_session_index": "20230717_0008",
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
-      <workItem from="1689550354850" duration="5819000"/>
+      <workItem from="1689550354850" duration="8204000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
```

### Comparing `switbuilder_core-0.0.4/.idea/inspectionProfiles/Project_Default.xml` & `switbuilder_core-0.0.5/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/switcore/logger.py` & `switbuilder_core-0.0.5/switcore/logger.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/switcore/action/activity_handler_abc.py` & `switbuilder_core-0.0.5/switcore/action/activity_handler_abc.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/switcore/action/activity_router.py` & `switbuilder_core-0.0.5/switcore/action/activity_router.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/switcore/action/schemas.py` & `switbuilder_core-0.0.5/switcore/action/schemas.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/switcore/apis/v1/channel/service.py` & `switbuilder_core-0.0.5/switcore/apis/v1/channel/service.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/switcore/apis/v1/conversation/schemas.py` & `switbuilder_core-0.0.5/switcore/apis/v1/conversation/schemas.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/switcore/apis/v1/conversation/service.py` & `switbuilder_core-0.0.5/switcore/apis/v1/conversation/service.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/switcore/apis/v1/imap/exception.py` & `switbuilder_core-0.0.5/switcore/apis/v1/imap/exception.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/switcore/apis/v1/imap/schemas.py` & `switbuilder_core-0.0.5/switcore/apis/v1/imap/schemas.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/switcore/apis/v1/imap/service.py` & `switbuilder_core-0.0.5/switcore/apis/v1/imap/service.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/switcore/apis/v1/imap/utils.py` & `switbuilder_core-0.0.5/switcore/apis/v1/imap/utils.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/tests.py` & `switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/tests.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/email/cid_image_email.json` & `switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/email/cid_image_email.json`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/email/email_with_attachment.json` & `switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/email/email_with_attachment.json`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/email/empty_receiver_email.json` & `switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/email/empty_receiver_email.json`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/email/html_email.json` & `switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/email/html_email.json`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/email/invalid_swit_image.json` & `switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/email/invalid_swit_image.json`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/email/large_cid_image_email.json` & `switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/email/large_cid_image_email.json`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/email/plain_text_email.json` & `switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/email/plain_text_email.json`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/html/example1.html` & `switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/html/example1.html`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/html/example3.html` & `switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/html/example3.html`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/html/example4.html` & `switbuilder_core-0.0.5/switcore/apis/v1/imap/tests/html/example4.html`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/switcore/apis/v1/membership/schemas.py` & `switbuilder_core-0.0.5/switcore/apis/v1/membership/schemas.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/switcore/apis/v1/membership/service.py` & `switbuilder_core-0.0.5/switcore/apis/v1/membership/service.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/switcore/apis/v1/project/service.py` & `switbuilder_core-0.0.5/switcore/apis/v1/project/service.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/switcore/apis/v1/task/schemas.py` & `switbuilder_core-0.0.5/switcore/apis/v1/task/schemas.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/switcore/apis/v1/task/service.py` & `switbuilder_core-0.0.5/switcore/apis/v1/task/service.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/switcore/apis/v1/workspace/schemas.py` & `switbuilder_core-0.0.5/switcore/apis/v1/workspace/schemas.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/switcore/apis/v1/workspace/service.py` & `switbuilder_core-0.0.5/switcore/apis/v1/workspace/service.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/switcore/auth/dependencies.py` & `switbuilder_core-0.0.5/switcore/auth/dependencies.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 import os
 
 from fastapi import Request, Depends
-from fastapi.security import OAuth2
+from httpx_oauth.integrations.fastapi import OAuth2AuthorizeCallback
+from httpx_oauth.oauth2 import OAuth2
 
 from switcore.auth.utils import get_swit_openapi_base_url
 
 
 async def get_swit_oauth2() -> OAuth2:
-    print(os.getenv('SWIT_CLIENT_ID'))
+    swit_client_id: str = os.getenv('SWIT_CLIENT_ID', None)
+    swit_client_secret: str = os.getenv('SWIT_CLIENT_SECRET', None)
+
+    assert swit_client_id is not None, "SWIT_CLIENT_ID is not set check .env file"
+    assert swit_client_secret is not None, "SWIT_CLIENT_SECRET is not set check .env file"
+
     return OAuth2(
-        client_id=settings.SWIT_CLIENT_ID,
-        client_secret=settings.SWIT_CLIENT_SECRET,
+        client_id=swit_client_id,
+        client_secret=swit_client_secret,
         authorize_endpoint=f"{get_swit_openapi_base_url()}/oauth/authorize",
         access_token_endpoint=f"{get_swit_openapi_base_url()}/oauth/token",
         refresh_token_endpoint=f"{get_swit_openapi_base_url()}/oauth/token",
         name="swit",
         base_scopes=["app:install"]
     )
 
@@ -23,15 +29,17 @@
         request: Request,
         code: str | None = None,
         code_verifier: str | None = None,
         state: str | None = None,
         error: str | None = None,
         swit_oauth2: OAuth2 = Depends(get_swit_oauth2)
 ):
-    callback = OAuth2AuthorizeCallback(swit_oauth2, redirect_url=settings.BASE_URL + "/auth/callback/bot")
+    base_url: str = os.getenv('BASE_URL', None)
+    assert base_url is not None, "BASE_URL is not set check .env file"
+    callback = OAuth2AuthorizeCallback(swit_oauth2, redirect_url=base_url + "/auth/callback/bot")
 
     return await callback(
         request=request,
         code=code,
         code_verifier=code_verifier,
         state=state,
         error=error
```

### Comparing `switbuilder_core-0.0.4/switcore/auth/repository.py` & `switbuilder_core-0.0.5/switcore/auth/repository.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from fastapi import HTTPException
 from sqlalchemy.orm import Session
 
-from src.auth.models import App
+from switcore.auth.models import App
 
 
 class RepositoryBase:
     def __init__(self, session: Session):
         self.session = session
 
 
@@ -19,15 +19,11 @@
 
     def get_by_id(self, id: int) -> App:
         token = self.session.query(App).get(id)
         if token is None:
             raise HTTPException(status_code=404, detail="Token not found")
         return token
 
-    def get_all(self) -> list[App]:
-        return self.session.query(App).all()
-
     def delete(self, id: int) -> None:
         token = self.get_by_id(id)
         self.session.delete(token)
         self.session.commit()
-
```

### Comparing `switbuilder_core-0.0.4/switcore/auth/router.py` & `switbuilder_core-0.0.5/switcore/auth/router.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,35 @@
+import os
+
 from fastapi import APIRouter, Depends, status, Request
 from fastapi.responses import HTMLResponse, RedirectResponse
-from fastapi.security import OAuth2
+from httpx_oauth.oauth2 import OAuth2
 
 from switcore.auth import dependencies
 
 router = APIRouter()
 
 
 @router.get("/bot", name="auth_bot")
 async def bot_install_oauth2(
         request: Request,  # noqa: F841
         swit_oauth2: OAuth2 = Depends(dependencies.get_swit_oauth2)
 ):
+    base_url: str = os.getenv('BASE_URL', None)
+    assert base_url is not None, "BASE_URL is not set check .env file"
     return RedirectResponse(
         await swit_oauth2.get_authorization_url(
-            redirect_uri=settings.BASE_URL + "/auth/callback/bot",
+            redirect_uri=base_url + "/auth/callback/bot",
             scope=["app:install"]
         ),
         status.HTTP_307_TEMPORARY_REDIRECT
     )
 
 
-@router.get("/callback/bot", name="auth_callback_bot")
-async def bot_install_callback(
-        token_state=Depends(dependencies.get_swit_oauth2_callback_bot),
-        session=Depends(get_db_session)
-):
-    token, state = token_state
-    await auth_service.save_swit_app(session, SwitToken(**token))
-    return HTMLResponse(content="<script>window.close()</script>")
+# @router.get("/callback/bot", name="auth_callback_bot")
+# async def bot_install_callback(
+#         token_state=Depends(dependencies.get_swit_oauth2_callback_bot),
+#         session=Depends(get_db_session)
+# ):
+#     token, state = token_state
+#     await auth_service.save_swit_app(session, SwitToken(**token))
+#     return HTMLResponse(content="<script>window.close()</script>")
```

#### html2text {}

```diff
@@ -1,13 +1,16 @@
-from fastapi import APIRouter, Depends, status, Request from fastapi.responses
-import HTMLResponse, RedirectResponse from fastapi.security import OAuth2 from
-switcore.auth import dependencies router = APIRouter() @router.get("/bot",
-name="auth_bot") async def bot_install_oauth2( request: Request, # noqa: F841
-swit_oauth2: OAuth2 = Depends(dependencies.get_swit_oauth2) ): return
+import os from fastapi import APIRouter, Depends, status, Request from
+fastapi.responses import HTMLResponse, RedirectResponse from httpx_oauth.oauth2
+import OAuth2 from switcore.auth import dependencies router = APIRouter()
+@router.get("/bot", name="auth_bot") async def bot_install_oauth2( request:
+Request, # noqa: F841 swit_oauth2: OAuth2 = Depends
+(dependencies.get_swit_oauth2) ): base_url: str = os.getenv('BASE_URL', None)
+assert base_url is not None, "BASE_URL is not set check .env file" return
 RedirectResponse( await swit_oauth2.get_authorization_url
-( redirect_uri=settings.BASE_URL + "/auth/callback/bot", scope=["app:install"]
-), status.HTTP_307_TEMPORARY_REDIRECT ) @router.get("/callback/bot",
-name="auth_callback_bot") async def bot_install_callback( token_state=Depends
-(dependencies.get_swit_oauth2_callback_bot), session=Depends(get_db_session) ):
-token, state = token_state await auth_service.save_swit_app(session, SwitToken
-(**token)) return HTMLResponse(content="
+( redirect_uri=base_url + "/auth/callback/bot", scope=["app:install"] ),
+status.HTTP_307_TEMPORARY_REDIRECT ) # @router.get("/callback/bot",
+name="auth_callback_bot") # async def bot_install_callback( #
+token_state=Depends(dependencies.get_swit_oauth2_callback_bot), #
+session=Depends(get_db_session) # ): # token, state = token_state # await
+auth_service.save_swit_app(session, SwitToken(**token)) # return HTMLResponse
+(content="
 ")
```

### Comparing `switbuilder_core-0.0.4/switcore/auth/service.py` & `switbuilder_core-0.0.5/switcore/auth/service.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,37 @@
-from typing import Final, Optional
-from urllib import parse
-
-import jwt
-from sqlalchemy.orm import Session
-
-from src.auth.repository import AppRepository
-from src.auth.schemas import SwitToken, Payload
-from src.auth.utils import get_swit_openapi_base_url
-from src.config import settings
-
-
-def get_oauth2_url(
-    scopes: str,
-    redirect_url: str
-) -> str:
-    params: Final[dict] = {
-        "client_id": settings.SWIT_CLIENT_ID,
-        "redirect_uri": settings.BASE_URL + redirect_url,
-        "response_type": "code",
-        "scope": scopes
-    }
-
-    return f"{get_swit_openapi_base_url()}/oauth/authorize?{parse.urlencode(params)}"
-
-
-async def save_swit_app(
-    session: Session,
-    token: SwitToken
-):
-    repository = AppRepository(session)
-    payload = Payload(**jwt.decode(token.access_token, options={"verify_signature": False}))
-    return repository.create(
-        access_token=token.access_token,
-        refresh_token=token.refresh_token,
-        apps_id=payload.apps_id,
-        cmp_id=payload.cmp_id,
-        iss=payload.iss
-    )
-
-
+# from typing import Final, Optional
+# from urllib import parse
+#
+# import jwt
+# from sqlalchemy.orm import Session
+#
+#
+#
+# def get_oauth2_url(
+#     scopes: str,
+#     redirect_url: str
+# ) -> str:
+#     params: Final[dict] = {
+#         "client_id": settings.SWIT_CLIENT_ID,
+#         "redirect_uri": settings.BASE_URL + redirect_url,
+#         "response_type": "code",
+#         "scope": scopes
+#     }
+#
+#     return f"{get_swit_openapi_base_url()}/oauth/authorize?{parse.urlencode(params)}"
+#
+#
+# async def save_swit_app(
+#     session: Session,
+#     token: SwitToken
+# ):
+#     repository = AppRepository(session)
+#     payload = Payload(**jwt.decode(token.access_token, options={"verify_signature": False}))
+#     return repository.create(
+#         access_token=token.access_token,
+#         refresh_token=token.refresh_token,
+#         apps_id=payload.apps_id,
+#         cmp_id=payload.cmp_id,
+#         iss=payload.iss
+#     )
+#
+#
```

### Comparing `switbuilder_core-0.0.4/switcore/ui/collection_entry.py` & `switbuilder_core-0.0.5/switcore/ui/collection_entry.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/switcore/ui/file.py` & `switbuilder_core-0.0.5/switcore/ui/file.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.4/pyproject.toml` & `switbuilder_core-0.0.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [project]
 name = "switbuilder-core"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     { name = "ur-team", email = "el.lee@swit.io" },
 ]
 description = "this is a switbuilder core package"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     'pydantic >= 1.10.9',
     'httpx >=0.24.1',
+    'httpx-oauth >=0.11.2',
     'fastapi >=0.83.0',
     'SQLAlchemy >=1.4.41',
     'PyMySQL >=1.1.0',
 ]
 
 
 [project.urls]
```

### Comparing `switbuilder_core-0.0.4/PKG-INFO` & `switbuilder_core-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: switbuilder-core
-Version: 0.0.4
+Version: 0.0.5
 Summary: this is a switbuilder core package
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: ur-team <el.lee@swit.io>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: fastapi>=0.83.0
+Requires-Dist: httpx-oauth>=0.11.2
 Requires-Dist: httpx>=0.24.1
 Requires-Dist: pydantic>=1.10.9
 Requires-Dist: pymysql>=1.1.0
 Requires-Dist: sqlalchemy>=1.4.41
 Description-Content-Type: text/markdown
 
 this is swit core
```

