# Comparing `tmp/switbuilder_core-0.0.3.tar.gz` & `tmp/switbuilder_core-0.0.4.tar.gz`

## Comparing `switbuilder_core-0.0.3.tar` & `switbuilder_core-0.0.4.tar`

### file list

```diff
@@ -1,97 +1,99 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/.DS_Store
--rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/build.sh
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/requirements.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/.idea/.gitignore
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/.idea/core.iml
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/.idea/misc.xml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/.idea/vcs.xml
--rw-r--r--   0        0        0    28901 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/.idea/workspace.xml
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/action/__init__.py
--rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/action/activity_handler.py
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/action/activity_handler_abc.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/action/activity_router.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/action/dependencies.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/action/exceptions.py
--rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/action/schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/channel/__init__.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/channel/schemas.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/channel/service.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/channel/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/conversation/__init__.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/conversation/schemas.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/conversation/service.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/conversation/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/constants.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/exception.py
--rw-r--r--   0        0        0    11454 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/schemas.py
--rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/service.py
--rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/__init__.py
--rw-r--r--   0        0        0    13670 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/tests.py
--rw-r--r--   0        0        0   306291 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/email/cid_image_email.json
--rw-r--r--   0        0        0  1499842 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/email/email_with_attachment.json
--rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/email/empty_receiver_email.json
--rw-r--r--   0        0        0    43739 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/email/html_email.json
--rw-r--r--   0        0        0    64730 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/email/invalid_swit_image.json
--rw-r--r--   0        0        0   631221 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/email/large_cid_image_email.json
--rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/email/plain_text_email.json
--rw-r--r--   0        0        0    34901 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/html/example1.html
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/html/example2.html
--rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/html/example3.html
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/html/example4.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/membership/__init__.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/membership/schemas.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/membership/service.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/membership/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/project/__init__.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/project/schemas.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/project/service.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/project/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/task/__init__.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/task/schemas.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/task/service.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/task/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/workspace/__init__.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/workspace/schemas.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/workspace/service.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/workspace/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/auth/__init__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/auth/constants.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/auth/dependencies.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/auth/exception.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/auth/models.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/auth/repository.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/auth/router.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/auth/schemas.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/auth/service.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/auth/utils.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/Icon.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/__init__.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/button.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/collection_entry.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/container.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/divider.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/file.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/header.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/html_frame.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/image.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/input.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/select.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/select_item.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/signIn_page.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/static_action.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/tabs.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/text_paragraph.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/textarea.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/view.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/.gitignore
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/README.md
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/.DS_Store
+-rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/build.sh
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/.idea/.gitignore
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/.idea/core.iml
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/.idea/misc.xml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/.idea/vcs.xml
+-rw-r--r--   0        0        0    29277 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/.idea/workspace.xml
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/__init__.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/constants.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/logger.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/lokalise.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/type.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/action/__init__.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/action/activity_handler_abc.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/action/activity_router.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/action/dependencies.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/action/exceptions.py
+-rw-r--r--   0        0        0     7341 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/action/schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/channel/__init__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/channel/schemas.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/channel/service.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/channel/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/conversation/__init__.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/conversation/schemas.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/conversation/service.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/conversation/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/constants.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/exception.py
+-rw-r--r--   0        0        0    11454 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/schemas.py
+-rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/service.py
+-rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/__init__.py
+-rw-r--r--   0        0        0    13670 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/tests.py
+-rw-r--r--   0        0        0   306291 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/email/cid_image_email.json
+-rw-r--r--   0        0        0  1499842 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/email/email_with_attachment.json
+-rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/email/empty_receiver_email.json
+-rw-r--r--   0        0        0    43739 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/email/html_email.json
+-rw-r--r--   0        0        0    64730 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/email/invalid_swit_image.json
+-rw-r--r--   0        0        0   631221 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/email/large_cid_image_email.json
+-rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/email/plain_text_email.json
+-rw-r--r--   0        0        0    34901 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/html/example1.html
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/html/example2.html
+-rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/html/example3.html
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/html/example4.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/membership/__init__.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/membership/schemas.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/membership/service.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/membership/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/project/__init__.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/project/schemas.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/project/service.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/project/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/task/__init__.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/task/schemas.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/task/service.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/task/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/workspace/__init__.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/workspace/schemas.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/workspace/service.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/apis/v1/workspace/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/auth/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/auth/constants.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/auth/dependencies.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/auth/exception.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/auth/models.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/auth/repository.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/auth/router.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/auth/schemas.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/auth/service.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/auth/utils.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/Icon.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/__init__.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/button.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/collection_entry.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/container.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/divider.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/file.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/header.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/html_frame.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/image.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/input.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/select.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/select_item.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/signIn_page.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/static_action.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/tabs.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/text_paragraph.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/switcore/ui/textarea.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/.gitignore
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/README.md
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 switbuilder_core-0.0.4/PKG-INFO
```

### Comparing `switbuilder_core-0.0.3/.DS_Store` & `switbuilder_core-0.0.4/.DS_Store`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.3/requirements.txt` & `switbuilder_core-0.0.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.3/.idea/workspace.xml` & `switbuilder_core-0.0.4/.idea/workspace.xml`

 * *Files 0% similar despite different names*

#### Comparing `switbuilder_core-0.0.3/.idea/workspace.xml` & `switbuilder_core-0.0.4/.idea/workspace.xml`

```diff
@@ -7,15 +7,14 @@
     <list default="true" id="7747ff4f-b6a5-4206-b1a9-45990956cc9c" name="Changes" comment="">
       <change afterPath="$PROJECT_DIR$/.gitignore" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/build.sh" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/switcore/__init__.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/switcore/action/__init__.py" afterDir="false"/>
-      <change afterPath="$PROJECT_DIR$/switcore/action/activity_handler.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/switcore/action/activity_handler_abc.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/switcore/action/activity_router.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/switcore/action/dependencies.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/switcore/action/exceptions.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/switcore/action/schemas.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/switcore/apis/__init__.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/switcore/apis/v1/__init__.py" afterDir="false"/>
@@ -68,14 +67,18 @@
       <change afterPath="$PROJECT_DIR$/switcore/auth/exception.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/switcore/auth/models.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/switcore/auth/repository.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/switcore/auth/router.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/switcore/auth/schemas.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/switcore/auth/service.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/switcore/auth/utils.py" afterDir="false"/>
+      <change afterPath="$PROJECT_DIR$/switcore/constants.py" afterDir="false"/>
+      <change afterPath="$PROJECT_DIR$/switcore/logger.py" afterDir="false"/>
+      <change afterPath="$PROJECT_DIR$/switcore/lokalise.py" afterDir="false"/>
+      <change afterPath="$PROJECT_DIR$/switcore/type.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/switcore/ui/Icon.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/switcore/ui/__init__.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/switcore/ui/button.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/switcore/ui/collection_entry.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/switcore/ui/container.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/switcore/ui/divider.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/switcore/ui/file.py" afterDir="false"/>
@@ -86,15 +89,14 @@
       <change afterPath="$PROJECT_DIR$/switcore/ui/select.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/switcore/ui/select_item.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/switcore/ui/signIn_page.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/switcore/ui/static_action.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/switcore/ui/tabs.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/switcore/ui/text_paragraph.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/switcore/ui/textarea.py" afterDir="false"/>
-      <change afterPath="$PROJECT_DIR$/switcore/ui/view.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
@@ -115,15 +117,15 @@
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
   <component name="PropertiesComponent"><![CDATA[{
   "keyToString": {
     "RunOnceActivity.ShowReadmeOnStart": "true",
     "WebServerToolWindowFactoryState": "false",
-    "com.google.cloudcode.ide_session_index": "20230717_0003",
+    "com.google.cloudcode.ide_session_index": "20230717_0006",
     "last_opened_file_path": "/Users/el/PycharmProjects/core/switcore",
     "node.js.detected.package.eslint": "true",
     "node.js.detected.package.tslint": "true",
     "node.js.selected.package.eslint": "(autodetect)",
     "node.js.selected.package.tslint": "(autodetect)",
     "settings.editor.selected.configurable": "preferences.lookFeel",
     "vue.rearranger.settings.migration": "true"
@@ -447,18 +449,29 @@
       <workItem from="1689250625591" duration="36000"/>
       <workItem from="1689250806915" duration="2161000"/>
       <workItem from="1689287326456" duration="22000"/>
       <workItem from="1689287357011" duration="77000"/>
       <workItem from="1689287435257" duration="46000"/>
       <workItem from="1689287487514" duration="1547000"/>
       <workItem from="1689309026861" duration="1964000"/>
-      <workItem from="1689550354850" duration="1404000"/>
+      <workItem from="1689550354850" duration="5819000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
+  <component name="Vcs.Log.Tabs.Properties">
+    <option name="TAB_STATES">
+      <map>
+        <entry key="MAIN">
+          <value>
+            <State/>
+          </value>
+        </entry>
+      </map>
+    </option>
+  </component>
   <component name="com.intellij.coverage.CoverageDataManagerImpl">
     <SUITE FILE_PATH="coverage/core$.coverage" NAME=" Coverage Results" MODIFIED="1686548968679" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/ui/swit_response"/>
   </component>
 </project>
```

### Comparing `switbuilder_core-0.0.3/.idea/inspectionProfiles/Project_Default.xml` & `switbuilder_core-0.0.4/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.3/switcore/action/activity_router.py` & `switbuilder_core-0.0.4/switcore/action/activity_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections import defaultdict
 
-from src.type import DrawerHandler
+from switcore.type import DrawerHandler
 
 
 class PathResolver:
 
     def __init__(self, id: str, paths: list[str]) -> None:
         self._id: str = id
         self.paths: list[str] = paths
```

### Comparing `switbuilder_core-0.0.3/switcore/action/schemas.py` & `switbuilder_core-0.0.4/switcore/action/schemas.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 import base64
 import bz2
 import json
 from datetime import datetime
 from enum import Enum
-from typing import Any
+from typing import Any, Container
 from typing import Optional, Dict, List
 
 from pydantic import BaseModel
 from pydantic import validator
 
-from src.action.exceptions import InvalidStateException
-from src.ui.button import Button
-from src.ui.collection_entry import CollectionEntry
-from src.ui.container import Container
-from src.ui.divider import Divider
-from src.ui.file import File
-from src.ui.header import Header
-from src.ui.html_frame import HtmlFrame
-from src.ui.image import Image
-from src.ui.input import Input
-from src.ui.select import Select
-from src.ui.signIn_page import SignInPage
-from src.ui.tabs import Tabs
-from src.ui.text_paragraph import TextParagraph
-from src.ui.textarea import Textarea
+from switcore.action.exceptions import InvalidStateException
+from switcore.ui.button import Button
+from switcore.ui.collection_entry import CollectionEntry
+from switcore.ui.divider import Divider
+from switcore.ui.file import File
+from switcore.ui.header import Header
+from switcore.ui.html_frame import HtmlFrame
+from switcore.ui.image import Image
+from switcore.ui.input import Input
+from switcore.ui.select import Select
+from switcore.ui.signIn_page import SignInPage
+from switcore.ui.tabs import Tabs
+from switcore.ui.text_paragraph import TextParagraph
+from switcore.ui.textarea import Textarea
 
 
 class UserInfo(BaseModel):
     user_id: str
     organization_id: str
```

### Comparing `switbuilder_core-0.0.3/switcore/apis/v1/channel/service.py` & `switbuilder_core-0.0.4/switcore/apis/v1/channel/service.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from schemas import Channel
+from switcore.action.schemas import SwitRequest
+from switcore.apis.v1.channel.utils import get_channels_url
 
 
 def get_channel_or_null(channels: list[Channel], channel_id: str) -> Channel | None:
     ret = None
     for channel in channels:
         if channel.id == channel_id:
             ret = channel
             break
 
     return ret
 
 
 async def get_all_channels_recursive(
-        action_request: ActionRequest,
+        action_request: SwitRequest,
         workspace_id: str,
         offset: str | None = None
 ) -> list[Channel]:
     params: dict = {
         "limit": 50,
         "workspace_id": workspace_id,
     }
```

### Comparing `switbuilder_core-0.0.3/switcore/apis/v1/conversation/schemas.py` & `switbuilder_core-0.0.4/switcore/apis/v1/conversation/schemas.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.3/switcore/apis/v1/conversation/service.py` & `switbuilder_core-0.0.4/switcore/apis/v1/conversation/service.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.3/switcore/apis/v1/imap/exception.py` & `switbuilder_core-0.0.4/switcore/apis/v1/imap/exception.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.3/switcore/apis/v1/imap/schemas.py` & `switbuilder_core-0.0.4/switcore/apis/v1/imap/schemas.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.3/switcore/apis/v1/imap/service.py` & `switbuilder_core-0.0.4/switcore/apis/v1/imap/service.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.3/switcore/apis/v1/imap/utils.py` & `switbuilder_core-0.0.4/switcore/apis/v1/imap/utils.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/tests.py` & `switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/tests.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/email/cid_image_email.json` & `switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/email/cid_image_email.json`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/email/email_with_attachment.json` & `switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/email/email_with_attachment.json`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/email/empty_receiver_email.json` & `switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/email/empty_receiver_email.json`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/email/html_email.json` & `switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/email/html_email.json`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/email/invalid_swit_image.json` & `switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/email/invalid_swit_image.json`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/email/large_cid_image_email.json` & `switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/email/large_cid_image_email.json`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/email/plain_text_email.json` & `switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/email/plain_text_email.json`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/html/example1.html` & `switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/html/example1.html`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/html/example3.html` & `switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/html/example3.html`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/html/example4.html` & `switbuilder_core-0.0.4/switcore/apis/v1/imap/tests/html/example4.html`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.3/switcore/apis/v1/membership/schemas.py` & `switbuilder_core-0.0.4/switcore/apis/v1/membership/schemas.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.3/switcore/apis/v1/membership/service.py` & `switbuilder_core-0.0.4/switcore/apis/v1/membership/service.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.3/switcore/apis/v1/project/service.py` & `switbuilder_core-0.0.4/switcore/apis/v1/project/service.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.3/switcore/apis/v1/task/schemas.py` & `switbuilder_core-0.0.4/switcore/apis/v1/task/schemas.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.3/switcore/apis/v1/task/service.py` & `switbuilder_core-0.0.4/switcore/apis/v1/task/service.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.3/switcore/apis/v1/workspace/schemas.py` & `switbuilder_core-0.0.4/switcore/apis/v1/workspace/schemas.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.3/switcore/apis/v1/workspace/service.py` & `switbuilder_core-0.0.4/switcore/apis/v1/workspace/service.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.3/switcore/auth/dependencies.py` & `switbuilder_core-0.0.4/switcore/auth/dependencies.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-from typing import Optional
+import os
 
 from fastapi import Request, Depends
-from httpx_oauth.integrations.fastapi import OAuth2AuthorizeCallback
-from httpx_oauth.oauth2 import OAuth2
+from fastapi.security import OAuth2
 
-from src.auth.utils import get_swit_openapi_base_url
-from src.config import settings
+from switcore.auth.utils import get_swit_openapi_base_url
 
 
 async def get_swit_oauth2() -> OAuth2:
+    print(os.getenv('SWIT_CLIENT_ID'))
     return OAuth2(
         client_id=settings.SWIT_CLIENT_ID,
         client_secret=settings.SWIT_CLIENT_SECRET,
         authorize_endpoint=f"{get_swit_openapi_base_url()}/oauth/authorize",
         access_token_endpoint=f"{get_swit_openapi_base_url()}/oauth/token",
         refresh_token_endpoint=f"{get_swit_openapi_base_url()}/oauth/token",
         name="swit",
```

### Comparing `switbuilder_core-0.0.3/switcore/auth/repository.py` & `switbuilder_core-0.0.4/switcore/auth/repository.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.3/switcore/auth/service.py` & `switbuilder_core-0.0.4/switcore/auth/service.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.3/switcore/ui/collection_entry.py` & `switbuilder_core-0.0.4/switcore/ui/collection_entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pydantic import BaseModel
 
-from src.ui.static_action import StaticAction
+from switcore.ui.static_action import StaticAction
 
 
 class TextStyle(BaseModel):
     bold: bool = False
     color: str
     size: str
     max_lines: int
```

### Comparing `switbuilder_core-0.0.3/switcore/ui/file.py` & `switbuilder_core-0.0.4/switcore/ui/file.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pydantic import BaseModel
 from enum import Enum
 
-from src.ui.static_action import StaticAction
+from switcore.ui.static_action import StaticAction
 
 
 class FileType(str, Enum):
     image = "image"
     video = "video"
     document = "document"
     pdf = "pdf"
```

### Comparing `switbuilder_core-0.0.3/pyproject.toml` & `switbuilder_core-0.0.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "switbuilder-core"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name = "ur-team", email = "el.lee@swit.io" },
 ]
 description = "this is a switbuilder core package"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `switbuilder_core-0.0.3/PKG-INFO` & `switbuilder_core-0.0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: switbuilder-core
-Version: 0.0.3
+Version: 0.0.4
 Summary: this is a switbuilder core package
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: ur-team <el.lee@swit.io>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

