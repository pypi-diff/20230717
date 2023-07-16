# Comparing `tmp/switbuilder_core-0.0.2.tar.gz` & `tmp/switbuilder_core-0.0.3.tar.gz`

## Comparing `switbuilder_core-0.0.2.tar` & `switbuilder_core-0.0.3.tar`

### file list

```diff
@@ -1,151 +1,97 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/.DS_Store
--rwxr-xr-x   0        0        0       47 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/build.sh
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/database.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/requirements.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/.idea/.gitignore
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/.idea/core.iml
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/.idea/misc.xml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/.idea/vcs.xml
--rw-r--r--   0        0        0    21417 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/.idea/workspace.xml
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/action/ActionId.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/action/__init__.py
--rw-r--r--   0        0        0    18389 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/action/activity_handler.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/action/activity_handler_abc.py
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/action/constants.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/action/dependencies.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/action/exceptions.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/action/router.py
--rw-r--r--   0        0        0     4581 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/action/schemas.py
--rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/action/tests.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/action/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/auth/__init__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/auth/constants.py
--rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/auth/dependencies.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/auth/exception.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/auth/models.py
--rw-r--r--   0        0        0     5916 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/auth/oauth2.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/auth/repository.py
--rw-r--r--   0        0        0     5042 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/auth/router.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/auth/schemas.py
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/auth/service.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/auth/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/channel/__init__.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/channel/schemas.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/channel/service.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/channel/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/conversation/__init__.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/conversation/schemas.py
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/conversation/service.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/conversation/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/emails/__init__.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/emails/service.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/emails/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/constants.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/exception.py
--rw-r--r--   0        0        0    11454 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/schemas.py
--rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/service.py
--rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/tests/__init__.py
--rw-r--r--   0        0        0    13670 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/tests/tests.py
--rw-r--r--   0        0        0   306291 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/tests/email/cid_image_email.json
--rw-r--r--   0        0        0  1499842 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/tests/email/email_with_attachment.json
--rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/tests/email/empty_receiver_email.json
--rw-r--r--   0        0        0    43739 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/tests/email/html_email.json
--rw-r--r--   0        0        0    64730 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/tests/email/invalid_swit_image.json
--rw-r--r--   0        0        0   631221 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/tests/email/large_cid_image_email.json
--rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/tests/email/plain_text_email.json
--rw-r--r--   0        0        0    34901 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/tests/html/example1.html
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/tests/html/example2.html
--rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/tests/html/example3.html
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/tests/html/example4.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/membership/__init__.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/membership/schemas.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/membership/service.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/membership/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/project/__init__.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/project/schemas.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/project/service.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/project/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/task/__init__.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/task/schemas.py
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/task/service.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/task/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/__init__.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/draw_manager_abc.py
--rw-r--r--   0        0        0    25930 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/draw_managers.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/service.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/view.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/collection_entry/Background.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/collection_entry/CollectionEntry.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/collection_entry/MetadataItem.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/collection_entry/StartSection.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/collection_entry/TextContent.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/collection_entry/TextSection.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/collection_entry/TextStyle.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/collection_entry/__init__.py
--rw-r--r--   0        0        0     7475 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/collection_entry/tests.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/common/Button.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/common/Icon.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/common/StaticAction.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/common/__init__.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/container/Container.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/container/__init__.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/divider/Divider.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/divider/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/file/File.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/file/__init__.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/header/ContextMenuItem.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/header/Header.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/header/__init__.py
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/header/tests.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/html_frame/HtmlFrame.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/html_frame/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/image/Image.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/image/__init__.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/input/Input.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/input/__init__.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/input/tests.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/listitem/ListItem.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/listitem/__init__.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/select/Option.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/select/Select.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/select/Style.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/select/__init__.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/select/tests.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/signin/IntegratedService.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/signin/SignInPage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/signin/__init__.py
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/signin/tests.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/swit_response/AttachmentView.py
--rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/swit_response/Body.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/swit_response/Footer.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/swit_response/SwitResponse.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/swit_response/View.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/swit_response/__init__.py
--rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/swit_response/tests.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/text_paragraph/TextParagraph.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/text_paragraph/__init__.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/textarea/Textarea.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/textarea/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/view_draw_managers/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/view_draw_managers/attach_to_task_modal/__init__.py
--rw-r--r--   0        0        0     9100 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/view_draw_managers/attach_to_task_modal/draw_manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/view_draw_managers/convert_to_task_modal/__init__.py
--rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/view_draw_managers/convert_to_task_modal/draw_manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/view_draw_managers/need_authorization_modal/__init__.py
--rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/view_draw_managers/need_authorization_modal/draw_manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/view_draw_managers/share_to_dm_modal/__init__.py
--rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/view_draw_managers/share_to_dm_modal/draw_manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/workspace/__init__.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/workspace/schemas.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/workspace/service.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/workspace/utils.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/.gitignore
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/README.md
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/.DS_Store
+-rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/build.sh
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/.idea/.gitignore
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/.idea/core.iml
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/.idea/misc.xml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/.idea/vcs.xml
+-rw-r--r--   0        0        0    28901 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/.idea/workspace.xml
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/action/__init__.py
+-rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/action/activity_handler.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/action/activity_handler_abc.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/action/activity_router.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/action/dependencies.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/action/exceptions.py
+-rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/action/schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/channel/__init__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/channel/schemas.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/channel/service.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/channel/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/conversation/__init__.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/conversation/schemas.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/conversation/service.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/conversation/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/constants.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/exception.py
+-rw-r--r--   0        0        0    11454 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/schemas.py
+-rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/service.py
+-rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/__init__.py
+-rw-r--r--   0        0        0    13670 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/tests.py
+-rw-r--r--   0        0        0   306291 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/email/cid_image_email.json
+-rw-r--r--   0        0        0  1499842 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/email/email_with_attachment.json
+-rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/email/empty_receiver_email.json
+-rw-r--r--   0        0        0    43739 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/email/html_email.json
+-rw-r--r--   0        0        0    64730 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/email/invalid_swit_image.json
+-rw-r--r--   0        0        0   631221 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/email/large_cid_image_email.json
+-rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/email/plain_text_email.json
+-rw-r--r--   0        0        0    34901 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/html/example1.html
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/html/example2.html
+-rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/html/example3.html
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/html/example4.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/membership/__init__.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/membership/schemas.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/membership/service.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/membership/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/project/__init__.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/project/schemas.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/project/service.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/project/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/task/__init__.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/task/schemas.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/task/service.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/task/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/workspace/__init__.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/workspace/schemas.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/workspace/service.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/apis/v1/workspace/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/auth/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/auth/constants.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/auth/dependencies.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/auth/exception.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/auth/models.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/auth/repository.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/auth/router.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/auth/schemas.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/auth/service.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/auth/utils.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/Icon.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/__init__.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/button.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/collection_entry.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/container.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/divider.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/file.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/header.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/html_frame.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/image.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/input.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/select.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/select_item.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/signIn_page.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/static_action.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/tabs.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/text_paragraph.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/textarea.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/switcore/ui/view.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/.gitignore
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/README.md
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 switbuilder_core-0.0.3/PKG-INFO
```

### Comparing `switbuilder_core-0.0.2/.DS_Store` & `switbuilder_core-0.0.3/.DS_Store`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.2/requirements.txt` & `switbuilder_core-0.0.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.2/.idea/inspectionProfiles/Project_Default.xml` & `switbuilder_core-0.0.3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.2/channel/service.py` & `switbuilder_core-0.0.3/switcore/apis/v1/channel/service.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from action.schemas import ActionRequest
-from channel.schemas import Channel
-from channel.utils import get_channels_url
+from schemas import Channel
 
 
 def get_channel_or_null(channels: list[Channel], channel_id: str) -> Channel | None:
     ret = None
     for channel in channels:
         if channel.id == channel_id:
             ret = channel
```

### Comparing `switbuilder_core-0.0.2/conversation/schemas.py` & `switbuilder_core-0.0.3/switcore/apis/v1/conversation/schemas.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.2/conversation/service.py` & `switbuilder_core-0.0.3/switcore/apis/v1/conversation/service.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import logging
 
-from action.schemas import ActionRequest
-from conversation.schemas import Room
-from conversation.utils import get_rooms_url
+from switcore.apis.v1.conversation.schemas import Room
 
 logger = logging.getLogger()
 
 
 async def get_all_rooms_recursive(
         action_request: ActionRequest,
         offset: str | None = None) -> list[Room]:
```

### Comparing `switbuilder_core-0.0.2/imap/exception.py` & `switbuilder_core-0.0.3/switcore/apis/v1/imap/exception.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.2/imap/schemas.py` & `switbuilder_core-0.0.3/switcore/apis/v1/imap/schemas.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.2/imap/service.py` & `switbuilder_core-0.0.3/switcore/apis/v1/imap/service.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.2/imap/utils.py` & `switbuilder_core-0.0.3/switcore/apis/v1/imap/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import base64
 import datetime
 import re
-import pytz
 from email.header import decode_header
 from email.message import Message
 
 from babel.dates import format_time, format_date
 from bs4 import BeautifulSoup
 
 from action.constants import PlatformTypes
```

### Comparing `switbuilder_core-0.0.2/imap/tests/tests.py` & `switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/tests.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.2/imap/tests/email/cid_image_email.json` & `switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/email/cid_image_email.json`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.2/imap/tests/email/email_with_attachment.json` & `switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/email/email_with_attachment.json`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.2/imap/tests/email/empty_receiver_email.json` & `switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/email/empty_receiver_email.json`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.2/imap/tests/email/html_email.json` & `switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/email/html_email.json`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.2/imap/tests/email/invalid_swit_image.json` & `switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/email/invalid_swit_image.json`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.2/imap/tests/email/large_cid_image_email.json` & `switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/email/large_cid_image_email.json`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.2/imap/tests/email/plain_text_email.json` & `switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/email/plain_text_email.json`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.2/imap/tests/html/example1.html` & `switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/html/example1.html`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.2/imap/tests/html/example3.html` & `switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/html/example3.html`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.2/imap/tests/html/example4.html` & `switbuilder_core-0.0.3/switcore/apis/v1/imap/tests/html/example4.html`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.2/membership/schemas.py` & `switbuilder_core-0.0.3/switcore/apis/v1/membership/schemas.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.2/membership/service.py` & `switbuilder_core-0.0.3/switcore/apis/v1/membership/service.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.2/project/service.py` & `switbuilder_core-0.0.3/switcore/apis/v1/project/service.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.2/task/schemas.py` & `switbuilder_core-0.0.3/switcore/apis/v1/task/schemas.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.2/task/service.py` & `switbuilder_core-0.0.3/switcore/apis/v1/task/service.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 import base64
 import logging
 
-import httpx
-
 from action.schemas import ActionRequest
-from channel.schemas import Channel
-from channel.utils import get_channels_url
 from imap.utils import decode_to_bytes_from_base64
 from logger import logger_decorator
-from project.schemas import Project
-from project.utils import get_projects_url
 from task.schemas import Task
 from task.utils import get_tasks_url, get_convert_to_new_task_url, get_attach_to_task_url
 
 
 def get_task_or_null(tasks: list[Task], task_id: str) -> Task | None:
     ret = None
     for task in tasks:
```

### Comparing `switbuilder_core-0.0.2/workspace/schemas.py` & `switbuilder_core-0.0.3/switcore/apis/v1/workspace/schemas.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.2/workspace/service.py` & `switbuilder_core-0.0.3/switcore/apis/v1/workspace/service.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 import logging
-from typing import Final
-
-import httpx
 
 from action.schemas import ActionRequest
 from workspace.schemas import Workspace
 from workspace.utils import get_workspaces_url
 
 logger = logging.getLogger()
```

### Comparing `switbuilder_core-0.0.2/pyproject.toml` & `switbuilder_core-0.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "switbuilder-core"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name = "ur-team", email = "el.lee@swit.io" },
 ]
-description = "A small example package"
+description = "this is a switbuilder core package"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     'pydantic >= 1.10.9',
```

