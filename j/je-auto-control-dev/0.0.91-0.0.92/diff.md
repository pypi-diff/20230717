# Comparing `tmp/je_auto_control_dev-0.0.91.tar.gz` & `tmp/je_auto_control_dev-0.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "je_auto_control_dev-0.0.91.tar", last modified: Mon Jul 17 06:32:56 2023, max compression
+gzip compressed data, was "je_auto_control_dev-0.0.92.tar", last modified: Mon Jul 17 09:36:10 2023, max compression
```

## Comparing `je_auto_control_dev-0.0.91.tar` & `je_auto_control_dev-0.0.92.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.389573 je_auto_control_dev-0.0.91/
--rw-rw-rw-   0        0        0     3780 2023-07-17 06:32:56.386541 je_auto_control_dev-0.0.91/PKG-INFO
--rw-rw-rw-   0        0        0     2975 2023-05-30 02:56:01.000000 je_auto_control_dev-0.0.91/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.727708 je_auto_control_dev-0.0.91/je_auto_control/
--rw-rw-rw-   0        0        0     6485 2023-07-17 06:17:59.000000 je_auto_control_dev-0.0.91/je_auto_control/__init__.py
--rw-rw-rw-   0        0        0     2355 2023-04-25 09:06:42.000000 je_auto_control_dev-0.0.91/je_auto_control/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.729669 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.734012 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/core/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.749915 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/core/utils/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/core/utils/__init__.py
--rw-rw-rw-   0        0        0      386 2023-07-17 06:24:07.000000 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/core/utils/x11_linux_display.py
--rw-rw-rw-   0        0        0    14539 2023-06-17 09:28:03.000000 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/core/utils/x11_linux_vk.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.760465 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/keyboard/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/keyboard/__init__.py
--rw-rw-rw-   0        0        0      828 2023-06-17 09:28:03.000000 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/keyboard/x11_linux_keyboard_control.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.771489 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/listener/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/listener/__init__.py
--rw-rw-rw-   0        0        0     5554 2023-06-13 01:38:29.000000 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/listener/x11_linux_listener.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.782654 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/mouse/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/mouse/__init__.py
--rw-rw-rw-   0        0        0     2393 2023-05-22 01:10:31.000000 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/mouse/x11_linux_mouse_control.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.792177 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/record/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/record/__init__.py
--rw-rw-rw-   0        0        0     1563 2023-04-10 02:15:44.000000 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/record/x11_linux_record.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.801459 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/screen/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/screen/__init__.py
--rw-rw-rw-   0        0        0      533 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/screen/x11_linux_screen.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.805374 je_auto_control_dev-0.0.91/je_auto_control/osx/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/osx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.809923 je_auto_control_dev-0.0.91/je_auto_control/osx/core/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/osx/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.818642 je_auto_control_dev-0.0.91/je_auto_control/osx/core/utils/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/osx/core/utils/__init__.py
--rw-rw-rw-   0        0        0     3157 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/osx/core/utils/osx_vk.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.840325 je_auto_control_dev-0.0.91/je_auto_control/osx/keyboard/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/osx/keyboard/__init__.py
--rw-rw-rw-   0        0        0     3017 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/osx/keyboard/osx_keyboard.py
--rw-rw-rw-   0        0        0      446 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/osx/keyboard/osx_keyboard_check.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.846347 je_auto_control_dev-0.0.91/je_auto_control/osx/listener/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/osx/listener/__init__.py
--rw-rw-rw-   0        0        0     1519 2023-04-10 02:15:44.000000 je_auto_control_dev-0.0.91/je_auto_control/osx/listener/osx_listener.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.865160 je_auto_control_dev-0.0.91/je_auto_control/osx/mouse/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/osx/mouse/__init__.py
--rw-rw-rw-   0        0        0     3500 2023-05-22 01:10:31.000000 je_auto_control_dev-0.0.91/je_auto_control/osx/mouse/osx_mouse.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.871215 je_auto_control_dev-0.0.91/je_auto_control/osx/record/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/osx/record/__init__.py
--rw-rw-rw-   0        0        0      957 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/osx/record/osx_record.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.880905 je_auto_control_dev-0.0.91/je_auto_control/osx/screen/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/osx/screen/__init__.py
--rw-rw-rw-   0        0        0      495 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/osx/screen/osx_screen.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.886801 je_auto_control_dev-0.0.91/je_auto_control/utils/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.898485 je_auto_control_dev-0.0.91/je_auto_control/utils/callback/
--rw-rw-rw-   0        0        0        0 2023-03-31 01:55:17.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/callback/__init__.py
--rw-rw-rw-   0        0        0     7800 2023-06-19 06:41:34.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/callback/callback_function_executor.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.910078 je_auto_control_dev-0.0.91/je_auto_control/utils/critical_exit/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/critical_exit/__init__.py
--rw-rw-rw-   0        0        0     1524 2023-04-10 02:15:44.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/critical_exit/critcal_exit.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.930733 je_auto_control_dev-0.0.91/je_auto_control/utils/exception/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/exception/__init__.py
--rw-rw-rw-   0        0        0     2870 2023-06-08 09:14:35.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0     1663 2023-03-31 02:15:20.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.937783 je_auto_control_dev-0.0.91/je_auto_control/utils/executor/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/executor/__init__.py
--rw-rw-rw-   0        0        0    10153 2023-07-17 03:36:53.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/executor/action_executor.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.948454 je_auto_control_dev-0.0.91/je_auto_control/utils/file_process/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/file_process/__init__.py
--rw-rw-rw-   0        0        0      758 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/file_process/get_dir_file_list.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.973847 je_auto_control_dev-0.0.91/je_auto_control/utils/generate_report/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/generate_report/__init__.py
--rw-rw-rw-   0        0        0     4938 2023-07-17 06:30:47.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/generate_report/generate_html_report.py
--rw-rw-rw-   0        0        0     3415 2023-06-19 08:53:36.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/generate_report/generate_json_report.py
--rw-rw-rw-   0        0        0     2090 2023-07-17 06:31:02.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/generate_report/generate_xml_report.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.989705 je_auto_control_dev-0.0.91/je_auto_control/utils/image/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/image/__init__.py
--rw-rw-rw-   0        0        0      532 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/image/screenshot.py
--rw-rw-rw-   0        0        0     1151 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/image/template_detection.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.001425 je_auto_control_dev-0.0.91/je_auto_control/utils/json/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/json/__init__.py
--rw-rw-rw-   0        0        0     1477 2023-06-19 06:56:53.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/json/json_file.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.012324 je_auto_control_dev-0.0.91/je_auto_control/utils/logging/
--rw-rw-rw-   0        0        0        0 2023-06-08 03:44:59.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/logging/__init__.py
--rw-rw-rw-   0        0        0      579 2023-06-12 07:11:50.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/logging/loggin_instance.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.022367 je_auto_control_dev-0.0.91/je_auto_control/utils/package_manager/
--rw-rw-rw-   0        0        0        0 2023-04-06 01:15:41.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/package_manager/__init__.py
--rw-rw-rw-   0        0        0     3644 2023-06-19 09:13:36.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/package_manager/package_manager_class.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.029467 je_auto_control_dev-0.0.91/je_auto_control/utils/project/
--rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/project/__init__.py
--rw-rw-rw-   0        0        0     3030 2023-06-13 06:53:21.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/project/create_project_structure.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.043968 je_auto_control_dev-0.0.91/je_auto_control/utils/project/template/
--rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/project/template/__init__.py
--rw-rw-rw-   0        0        0      639 2023-04-10 08:38:18.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/project/template/template_executor.py
--rw-rw-rw-   0        0        0     2517 2023-04-10 07:40:39.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/project/template/template_keyword.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.056007 je_auto_control_dev-0.0.91/je_auto_control/utils/scheduler/
--rw-rw-rw-   0        0        0        0 2023-05-31 01:17:46.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/scheduler/__init__.py
--rw-rw-rw-   0        0        0    11468 2023-07-17 02:27:57.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/scheduler/extend_apscheduler.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.070593 je_auto_control_dev-0.0.91/je_auto_control/utils/shell_process/
--rw-rw-rw-   0        0        0        0 2023-05-29 01:48:49.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/shell_process/__init__.py
--rw-rw-rw-   0        0        0     5226 2023-06-13 06:53:21.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/shell_process/shell_exec.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.084372 je_auto_control_dev-0.0.91/je_auto_control/utils/socket_server/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/socket_server/__init__.py
--rw-rw-rw-   0        0        0     2329 2023-06-19 07:21:50.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/socket_server/auto_control_socket_server.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.097568 je_auto_control_dev-0.0.91/je_auto_control/utils/start_exe/
--rw-rw-rw-   0        0        0        0 2023-05-29 01:48:49.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/start_exe/__init__.py
--rw-rw-rw-   0        0        0      822 2023-06-19 07:21:50.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/start_exe/start_another_process.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.116733 je_auto_control_dev-0.0.91/je_auto_control/utils/test_record/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/test_record/__init__.py
--rw-rw-rw-   0        0        0     1059 2023-06-13 06:39:14.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/test_record/record_test_class.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.135830 je_auto_control_dev-0.0.91/je_auto_control/utils/timeout/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/timeout/__init__.py
--rw-rw-rw-   0        0        0      659 2023-06-19 07:40:40.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/timeout/multiprocess_timeout.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.140362 je_auto_control_dev-0.0.91/je_auto_control/utils/xml/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/xml/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.151801 je_auto_control_dev-0.0.91/je_auto_control/utils/xml/change_xml_structure/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/xml/change_xml_structure/__init__.py
--rw-rw-rw-   0        0        0     2498 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/xml/change_xml_structure/change_xml_structure.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.167512 je_auto_control_dev-0.0.91/je_auto_control/utils/xml/xml_file/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/xml/xml_file/__init__.py
--rw-rw-rw-   0        0        0     2369 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/xml/xml_file/xml_file.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.176416 je_auto_control_dev-0.0.91/je_auto_control/windows/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.183444 je_auto_control_dev-0.0.91/je_auto_control/windows/core/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.217914 je_auto_control_dev-0.0.91/je_auto_control/windows/core/utils/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/core/utils/__init__.py
--rw-rw-rw-   0        0        0     2388 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/core/utils/win32_ctype_input.py
--rw-rw-rw-   0        0        0      584 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/core/utils/win32_keypress_check.py
--rw-rw-rw-   0        0        0     5804 2023-07-17 06:26:04.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/core/utils/win32_vk.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.234458 je_auto_control_dev-0.0.91/je_auto_control/windows/keyboard/
--rw-rw-rw-   0        0        0        4 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/keyboard/__init__.py
--rw-rw-rw-   0        0        0     1259 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/keyboard/win32_ctype_keyboard_control.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.249334 je_auto_control_dev-0.0.91/je_auto_control/windows/listener/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/listener/__init__.py
--rw-rw-rw-   0        0        0     2538 2023-04-10 02:15:44.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/listener/win32_keyboard_listener.py
--rw-rw-rw-   0        0        0     3065 2023-04-07 08:14:40.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/listener/win32_mouse_listener.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.264197 je_auto_control_dev-0.0.91/je_auto_control/windows/mouse/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/mouse/__init__.py
--rw-rw-rw-   0        0        0     4170 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/mouse/win32_ctype_mouse_control.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.280430 je_auto_control_dev-0.0.91/je_auto_control/windows/record/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/record/__init__.py
--rw-rw-rw-   0        0        0     2182 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/record/win32_record.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.294519 je_auto_control_dev-0.0.91/je_auto_control/windows/screen/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/screen/__init__.py
--rw-rw-rw-   0        0        0      568 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/screen/win32_screen.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.346670 je_auto_control_dev-0.0.91/je_auto_control/wrapper/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/wrapper/__init__.py
--rw-rw-rw-   0        0        0     8157 2023-06-13 03:21:38.000000 je_auto_control_dev-0.0.91/je_auto_control/wrapper/auto_control_image.py
--rw-rw-rw-   0        0        0    14111 2023-06-13 03:24:01.000000 je_auto_control_dev-0.0.91/je_auto_control/wrapper/auto_control_keyboard.py
--rw-rw-rw-   0        0        0    11484 2023-06-13 03:43:27.000000 je_auto_control_dev-0.0.91/je_auto_control/wrapper/auto_control_mouse.py
--rw-rw-rw-   0        0        0     1957 2023-07-17 06:14:02.000000 je_auto_control_dev-0.0.91/je_auto_control/wrapper/auto_control_record.py
--rw-rw-rw-   0        0        0     2433 2023-07-17 06:26:57.000000 je_auto_control_dev-0.0.91/je_auto_control/wrapper/auto_control_screen.py
--rw-rw-rw-   0        0        0    58693 2023-06-13 03:50:56.000000 je_auto_control_dev-0.0.91/je_auto_control/wrapper/platform_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.382537 je_auto_control_dev-0.0.91/je_auto_control_dev.egg-info/
--rw-rw-rw-   0        0        0     3780 2023-07-17 06:32:55.000000 je_auto_control_dev-0.0.91/je_auto_control_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5256 2023-07-17 06:32:55.000000 je_auto_control_dev-0.0.91/je_auto_control_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 06:32:55.000000 je_auto_control_dev-0.0.91/je_auto_control_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      124 2023-07-17 06:32:55.000000 je_auto_control_dev-0.0.91/je_auto_control_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-17 06:32:55.000000 je_auto_control_dev-0.0.91/je_auto_control_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1310 2023-07-17 06:31:28.000000 je_auto_control_dev-0.0.91/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-17 06:32:56.390583 je_auto_control_dev-0.0.91/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.569200 je_auto_control_dev-0.0.92/
+-rw-rw-rw-   0        0        0     3780 2023-07-17 09:36:10.568210 je_auto_control_dev-0.0.92/PKG-INFO
+-rw-rw-rw-   0        0        0     2975 2023-05-30 02:56:01.000000 je_auto_control_dev-0.0.92/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.016602 je_auto_control_dev-0.0.92/je_auto_control/
+-rw-rw-rw-   0        0        0     6485 2023-07-17 09:33:39.000000 je_auto_control_dev-0.0.92/je_auto_control/__init__.py
+-rw-rw-rw-   0        0        0     2355 2023-07-17 09:33:56.000000 je_auto_control_dev-0.0.92/je_auto_control/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.021123 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.024119 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/core/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.056163 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/core/utils/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/core/utils/__init__.py
+-rw-rw-rw-   0        0        0      386 2023-07-17 06:24:07.000000 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/core/utils/x11_linux_display.py
+-rw-rw-rw-   0        0        0    14539 2023-06-17 09:28:03.000000 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/core/utils/x11_linux_vk.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.069723 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/keyboard/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/keyboard/__init__.py
+-rw-rw-rw-   0        0        0      828 2023-06-17 09:28:03.000000 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/keyboard/x11_linux_keyboard_control.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.080378 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/listener/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/listener/__init__.py
+-rw-rw-rw-   0        0        0     5554 2023-06-13 01:38:29.000000 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/listener/x11_linux_listener.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.090256 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/mouse/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/mouse/__init__.py
+-rw-rw-rw-   0        0        0     2393 2023-05-22 01:10:31.000000 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/mouse/x11_linux_mouse_control.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.100800 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/record/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/record/__init__.py
+-rw-rw-rw-   0        0        0     1575 2023-07-17 09:22:52.000000 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/record/x11_linux_record.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.108662 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/screen/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/screen/__init__.py
+-rw-rw-rw-   0        0        0      533 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/screen/x11_linux_screen.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.112668 je_auto_control_dev-0.0.92/je_auto_control/osx/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/osx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.118501 je_auto_control_dev-0.0.92/je_auto_control/osx/core/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/osx/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.128065 je_auto_control_dev-0.0.92/je_auto_control/osx/core/utils/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/osx/core/utils/__init__.py
+-rw-rw-rw-   0        0        0     3157 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/osx/core/utils/osx_vk.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.144054 je_auto_control_dev-0.0.92/je_auto_control/osx/keyboard/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/osx/keyboard/__init__.py
+-rw-rw-rw-   0        0        0     3017 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/osx/keyboard/osx_keyboard.py
+-rw-rw-rw-   0        0        0      446 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/osx/keyboard/osx_keyboard_check.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.152307 je_auto_control_dev-0.0.92/je_auto_control/osx/listener/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/osx/listener/__init__.py
+-rw-rw-rw-   0        0        0     1528 2023-07-17 09:22:52.000000 je_auto_control_dev-0.0.92/je_auto_control/osx/listener/osx_listener.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.162123 je_auto_control_dev-0.0.92/je_auto_control/osx/mouse/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/osx/mouse/__init__.py
+-rw-rw-rw-   0        0        0     3500 2023-05-22 01:10:31.000000 je_auto_control_dev-0.0.92/je_auto_control/osx/mouse/osx_mouse.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.170942 je_auto_control_dev-0.0.92/je_auto_control/osx/record/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/osx/record/__init__.py
+-rw-rw-rw-   0        0        0      957 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/osx/record/osx_record.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.180044 je_auto_control_dev-0.0.92/je_auto_control/osx/screen/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/osx/screen/__init__.py
+-rw-rw-rw-   0        0        0      495 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/osx/screen/osx_screen.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.185049 je_auto_control_dev-0.0.92/je_auto_control/utils/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.191358 je_auto_control_dev-0.0.92/je_auto_control/utils/callback/
+-rw-rw-rw-   0        0        0        0 2023-03-31 01:55:17.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/callback/__init__.py
+-rw-rw-rw-   0        0        0     7917 2023-07-17 09:31:18.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/callback/callback_function_executor.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.200400 je_auto_control_dev-0.0.92/je_auto_control/utils/critical_exit/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/critical_exit/__init__.py
+-rw-rw-rw-   0        0        0     1524 2023-04-10 02:15:44.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/critical_exit/critcal_exit.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.217020 je_auto_control_dev-0.0.92/je_auto_control/utils/exception/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0     2870 2023-06-08 09:14:35.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0     1663 2023-03-31 02:15:20.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.222971 je_auto_control_dev-0.0.92/je_auto_control/utils/executor/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/executor/__init__.py
+-rw-rw-rw-   0        0        0    10300 2023-07-17 09:33:34.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/executor/action_executor.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.231310 je_auto_control_dev-0.0.92/je_auto_control/utils/file_process/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/file_process/__init__.py
+-rw-rw-rw-   0        0        0      758 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/file_process/get_dir_file_list.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.245842 je_auto_control_dev-0.0.92/je_auto_control/utils/generate_report/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/generate_report/__init__.py
+-rw-rw-rw-   0        0        0     4938 2023-07-17 09:34:19.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/generate_report/generate_html_report.py
+-rw-rw-rw-   0        0        0     3415 2023-07-17 09:34:23.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/generate_report/generate_json_report.py
+-rw-rw-rw-   0        0        0     2090 2023-07-17 09:34:26.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/generate_report/generate_xml_report.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.261382 je_auto_control_dev-0.0.92/je_auto_control/utils/image/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/image/__init__.py
+-rw-rw-rw-   0        0        0      532 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/image/screenshot.py
+-rw-rw-rw-   0        0        0     1151 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/image/template_detection.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.273152 je_auto_control_dev-0.0.92/je_auto_control/utils/json/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/json/__init__.py
+-rw-rw-rw-   0        0        0     1477 2023-06-19 06:56:53.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/json/json_file.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.284537 je_auto_control_dev-0.0.92/je_auto_control/utils/logging/
+-rw-rw-rw-   0        0        0        0 2023-06-08 03:44:59.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/logging/__init__.py
+-rw-rw-rw-   0        0        0      579 2023-06-12 07:11:50.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/logging/loggin_instance.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.294191 je_auto_control_dev-0.0.92/je_auto_control/utils/package_manager/
+-rw-rw-rw-   0        0        0        0 2023-04-06 01:15:41.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/package_manager/__init__.py
+-rw-rw-rw-   0        0        0     3644 2023-06-19 09:13:36.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/package_manager/package_manager_class.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.304366 je_auto_control_dev-0.0.92/je_auto_control/utils/project/
+-rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/project/__init__.py
+-rw-rw-rw-   0        0        0     3030 2023-06-13 06:53:21.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/project/create_project_structure.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.319145 je_auto_control_dev-0.0.92/je_auto_control/utils/project/template/
+-rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/project/template/__init__.py
+-rw-rw-rw-   0        0        0      639 2023-04-10 08:38:18.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/project/template/template_executor.py
+-rw-rw-rw-   0        0        0     2649 2023-07-17 09:30:46.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/project/template/template_keyword.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.328074 je_auto_control_dev-0.0.92/je_auto_control/utils/scheduler/
+-rw-rw-rw-   0        0        0        0 2023-05-31 01:17:46.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/scheduler/__init__.py
+-rw-rw-rw-   0        0        0    11468 2023-07-17 02:27:57.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/scheduler/extend_apscheduler.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.339055 je_auto_control_dev-0.0.92/je_auto_control/utils/shell_process/
+-rw-rw-rw-   0        0        0        0 2023-05-29 01:48:49.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/shell_process/__init__.py
+-rw-rw-rw-   0        0        0     5226 2023-06-13 06:53:21.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/shell_process/shell_exec.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.344328 je_auto_control_dev-0.0.92/je_auto_control/utils/socket_server/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/socket_server/__init__.py
+-rw-rw-rw-   0        0        0     2329 2023-06-19 07:21:50.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/socket_server/auto_control_socket_server.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.354776 je_auto_control_dev-0.0.92/je_auto_control/utils/start_exe/
+-rw-rw-rw-   0        0        0        0 2023-05-29 01:48:49.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/start_exe/__init__.py
+-rw-rw-rw-   0        0        0      822 2023-06-19 07:21:50.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/start_exe/start_another_process.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.363314 je_auto_control_dev-0.0.92/je_auto_control/utils/test_record/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/test_record/__init__.py
+-rw-rw-rw-   0        0        0     1059 2023-06-13 06:39:14.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/test_record/record_test_class.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.376368 je_auto_control_dev-0.0.92/je_auto_control/utils/timeout/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/timeout/__init__.py
+-rw-rw-rw-   0        0        0      659 2023-06-19 07:40:40.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/timeout/multiprocess_timeout.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.379428 je_auto_control_dev-0.0.92/je_auto_control/utils/xml/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/xml/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.389996 je_auto_control_dev-0.0.92/je_auto_control/utils/xml/change_xml_structure/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/xml/change_xml_structure/__init__.py
+-rw-rw-rw-   0        0        0     2498 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/xml/change_xml_structure/change_xml_structure.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.399166 je_auto_control_dev-0.0.92/je_auto_control/utils/xml/xml_file/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/xml/xml_file/__init__.py
+-rw-rw-rw-   0        0        0     2369 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/xml/xml_file/xml_file.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.405165 je_auto_control_dev-0.0.92/je_auto_control/windows/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.410440 je_auto_control_dev-0.0.92/je_auto_control/windows/core/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.439770 je_auto_control_dev-0.0.92/je_auto_control/windows/core/utils/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/core/utils/__init__.py
+-rw-rw-rw-   0        0        0     2388 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/core/utils/win32_ctype_input.py
+-rw-rw-rw-   0        0        0      584 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/core/utils/win32_keypress_check.py
+-rw-rw-rw-   0        0        0     5804 2023-07-17 06:26:04.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/core/utils/win32_vk.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.453271 je_auto_control_dev-0.0.92/je_auto_control/windows/keyboard/
+-rw-rw-rw-   0        0        0        4 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/keyboard/__init__.py
+-rw-rw-rw-   0        0        0     1259 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/keyboard/win32_ctype_keyboard_control.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.463779 je_auto_control_dev-0.0.92/je_auto_control/windows/listener/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/listener/__init__.py
+-rw-rw-rw-   0        0        0     2541 2023-07-17 09:22:52.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/listener/win32_keyboard_listener.py
+-rw-rw-rw-   0        0        0     3074 2023-07-17 09:18:18.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/listener/win32_mouse_listener.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.473815 je_auto_control_dev-0.0.92/je_auto_control/windows/mouse/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/mouse/__init__.py
+-rw-rw-rw-   0        0        0     4170 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/mouse/win32_ctype_mouse_control.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.486376 je_auto_control_dev-0.0.92/je_auto_control/windows/record/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/record/__init__.py
+-rw-rw-rw-   0        0        0     2182 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/record/win32_record.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.496195 je_auto_control_dev-0.0.92/je_auto_control/windows/screen/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/screen/__init__.py
+-rw-rw-rw-   0        0        0      568 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/screen/win32_screen.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.525205 je_auto_control_dev-0.0.92/je_auto_control/wrapper/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/wrapper/__init__.py
+-rw-rw-rw-   0        0        0     8157 2023-07-17 09:34:45.000000 je_auto_control_dev-0.0.92/je_auto_control/wrapper/auto_control_image.py
+-rw-rw-rw-   0        0        0    14111 2023-07-17 09:34:52.000000 je_auto_control_dev-0.0.92/je_auto_control/wrapper/auto_control_keyboard.py
+-rw-rw-rw-   0        0        0    11484 2023-07-17 09:34:57.000000 je_auto_control_dev-0.0.92/je_auto_control/wrapper/auto_control_mouse.py
+-rw-rw-rw-   0        0        0     1957 2023-07-17 09:35:02.000000 je_auto_control_dev-0.0.92/je_auto_control/wrapper/auto_control_record.py
+-rw-rw-rw-   0        0        0     2442 2023-07-17 09:24:58.000000 je_auto_control_dev-0.0.92/je_auto_control/wrapper/auto_control_screen.py
+-rw-rw-rw-   0        0        0    58693 2023-07-17 09:21:08.000000 je_auto_control_dev-0.0.92/je_auto_control/wrapper/platform_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.562084 je_auto_control_dev-0.0.92/je_auto_control_dev.egg-info/
+-rw-rw-rw-   0        0        0     3780 2023-07-17 09:36:09.000000 je_auto_control_dev-0.0.92/je_auto_control_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5256 2023-07-17 09:36:09.000000 je_auto_control_dev-0.0.92/je_auto_control_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 09:36:09.000000 je_auto_control_dev-0.0.92/je_auto_control_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      124 2023-07-17 09:36:09.000000 je_auto_control_dev-0.0.92/je_auto_control_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-17 09:36:09.000000 je_auto_control_dev-0.0.92/je_auto_control_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1310 2023-07-17 09:35:43.000000 je_auto_control_dev-0.0.92/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-17 09:36:10.570199 je_auto_control_dev-0.0.92/setup.cfg
```

### Comparing `je_auto_control_dev-0.0.91/PKG-INFO` & `je_auto_control_dev-0.0.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je_auto_control_dev
-Version: 0.0.91
+Version: 0.0.92
 Summary: GUI Automation Framework
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/AutoControl
 Project-URL: Documentation, https://autocontrol.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/AutoControl
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `je_auto_control_dev-0.0.91/README.md` & `je_auto_control_dev-0.0.92/README.md`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/__init__.py` & `je_auto_control_dev-0.0.92/je_auto_control/__init__.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/__main__.py` & `je_auto_control_dev-0.0.92/je_auto_control/__main__.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/core/utils/x11_linux_vk.py` & `je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/core/utils/x11_linux_vk.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/keyboard/x11_linux_keyboard_control.py` & `je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/keyboard/x11_linux_keyboard_control.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/listener/x11_linux_listener.py` & `je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/listener/x11_linux_listener.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/mouse/x11_linux_mouse_control.py` & `je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/mouse/x11_linux_mouse_control.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/record/x11_linux_record.py` & `je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/record/x11_linux_record.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     raise AutoControlException(linux_import_error)
 
 from je_auto_control.linux_with_x11.listener.x11_linux_listener import x11_linux_record
 from je_auto_control.linux_with_x11.listener.x11_linux_listener import x11_linux_stop_record
 
 from queue import Queue
 
-type_dict = {5: "mouse", 3: "type_keyboard"}
-detail_dict = {1: "mouse_left", 2: "mouse_middle", 3: "mouse_right"}
+type_dict = {5: "mouse", 3: "AC_type_keyboard"}
+detail_dict = {1: "AC_mouse_left", 2: "AC_mouse_middle", 3: "AC_mouse_right"}
 
 
 class X11LinuxRecorder(object):
     """
     test_record controller
     """
```

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/screen/x11_linux_screen.py` & `je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/screen/x11_linux_screen.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/osx/core/utils/osx_vk.py` & `je_auto_control_dev-0.0.92/je_auto_control/osx/core/utils/osx_vk.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/osx/keyboard/osx_keyboard.py` & `je_auto_control_dev-0.0.92/je_auto_control/osx/keyboard/osx_keyboard.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/osx/listener/osx_listener.py` & `je_auto_control_dev-0.0.92/je_auto_control/osx/listener/osx_listener.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,27 +22,27 @@
         NSEvent.addGlobalMonitorForEventsMatchingMask_handler_(NSEventMaskKeyDown, keyboard_handler)
         NSEvent.addGlobalMonitorForEventsMatchingMask_handler_(NSEventMaskLeftMouseDown, mouse_left_handler)
         NSEvent.addGlobalMonitorForEventsMatchingMask_handler_(NSEventMaskRightMouseDown, mouse_right_handler)
 
 
 def mouse_left_handler(event) -> None:
     loc = NSEvent.mouseLocation()
-    record_queue.put(("mouse_left", loc.x, loc.y))
+    record_queue.put(("AC_mouse_left", loc.x, loc.y))
 
 
 def mouse_right_handler(event) -> None:
     loc = NSEvent.mouseLocation()
-    record_queue.put(("mouse_right", loc.x, loc.y))
+    record_queue.put(("AC_mouse_right", loc.x, loc.y))
 
 
 def keyboard_handler(event) -> None:
     if int(event.keyCode()) == 98:
         pass
     else:
-        record_queue.put(("type_keyboard", int(hex(event.keyCode()), 16)))
+        record_queue.put(("AC_type_keyboard", int(hex(event.keyCode()), 16)))
         print(event)
 
 
 def osx_record() -> None:
     delegate = AppDelegate.alloc().init()
     app.setDelegate_(delegate)
     AppHelper.runEventLoop()
```

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/osx/mouse/osx_mouse.py` & `je_auto_control_dev-0.0.92/je_auto_control/osx/mouse/osx_mouse.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/osx/record/osx_record.py` & `je_auto_control_dev-0.0.92/je_auto_control/osx/record/osx_record.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/utils/callback/callback_function_executor.py` & `je_auto_control_dev-0.0.92/je_auto_control/utils/callback/callback_function_executor.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,70 +57,70 @@
 
 
 class CallbackFunctionExecutor(object):
 
     def __init__(self):
         self.event_dict: dict = {
             # mouse
-            "mouse_left": click_mouse,
-            "mouse_right": click_mouse,
-            "mouse_middle": click_mouse,
-            "click_mouse": click_mouse,
-            "get_mouse_table": get_mouse_table,
-            "get_mouse_position": get_mouse_position,
-            "press_mouse": press_mouse,
-            "release_mouse": release_mouse,
-            "mouse_scroll": mouse_scroll,
-            "set_mouse_position": set_mouse_position,
-            "get_special_table": get_special_table,
+            "AC_mouse_left": click_mouse,
+            "AC_mouse_right": click_mouse,
+            "AC_mouse_middle": click_mouse,
+            "AC_click_mouse": click_mouse,
+            "AC_get_mouse_table": get_mouse_table,
+            "AC_get_mouse_position": get_mouse_position,
+            "AC_press_mouse": press_mouse,
+            "AC_release_mouse": release_mouse,
+            "AC_mouse_scroll": mouse_scroll,
+            "AC_set_mouse_position": set_mouse_position,
+            "AC_get_special_table": get_special_table,
             # keyboard
-            "get_keyboard_keys_table": get_keyboard_keys_table,
-            "type_keyboard": type_keyboard,
-            "press_keyboard_key": press_keyboard_key,
-            "release_keyboard_key": release_keyboard_key,
-            "check_key_is_press": check_key_is_press,
-            "write": write,
-            "hotkey": hotkey,
+            "AC_get_keyboard_keys_table": get_keyboard_keys_table,
+            "AC_type_keyboard": type_keyboard,
+            "AC_press_keyboard_key": press_keyboard_key,
+            "AC_release_keyboard_key": release_keyboard_key,
+            "AC_check_key_is_press": check_key_is_press,
+            "AC_write": write,
+            "AC_hotkey": hotkey,
             # image
-            "locate_all_image": locate_all_image,
-            "locate_image_center": locate_image_center,
-            "locate_and_click": locate_and_click,
+            "AC_locate_all_image": locate_all_image,
+            "AC_locate_image_center": locate_image_center,
+            "AC_locate_and_click": locate_and_click,
             # screen
-            "screen_size": screen_size,
-            "screenshot": screenshot,
+            "AC_screen_size": screen_size,
+            "AC_screenshot": screenshot,
             # test record
-            "set_record_enable": test_record_instance.set_record_enable,
+            "AC_set_record_enable": test_record_instance.set_record_enable,
             # only generate
-            "generate_html": generate_html,
-            "generate_json": generate_json,
-            "generate_xml": generate_xml,
+            "AC_generate_html": generate_html,
+            "AC_generate_json": generate_json,
+            "AC_generate_xml": generate_xml,
             # generate report
-            "generate_html_report": generate_html_report,
-            "generate_json_report": generate_json_report,
-            "generate_xml_report": generate_xml_report,
+            "AC_generate_html_report": generate_html_report,
+            "AC_generate_json_report": generate_json_report,
+            "AC_generate_xml_report": generate_xml_report,
             # record
-            "record": record,
-            "stop_record": stop_record,
+            "AC_record": record,
+            "AC_stop_record": stop_record,
             # execute
-            "execute_action": execute_action,
-            "execute_files": execute_files,
+            "AC_execute_action": execute_action,
+            "AC_execute_files": execute_files,
             "create_template_dir": create_project_dir,
             "get_dir_files_as_list": get_dir_files_as_list,
             "pil_screenshot": pil_screenshot,
             "read_action_json": read_action_json,
             "write_action_json": write_action_json,
             "start_autocontrol_socket_server": start_autocontrol_socket_server,
-            "add_package_to_executor": package_manager.add_package_to_executor,
-            "add_package_to_callback_executor": package_manager.add_package_to_callback_executor,
+            "AC_add_package_to_executor": package_manager.add_package_to_executor,
+            "AC_add_package_to_callback_executor": package_manager.add_package_to_callback_executor,
             # project
-            "create_project": create_project_dir,
+            "AC_create_project": create_project_dir,
             # Shell
-            "shell_command": ShellManager().exec_shell,
+            "AC_shell_command": ShellManager().exec_shell,
             # Another process
-            "execute_process": start_exe,
+            "AC_execute_process": start_exe,
         }
 
     def callback_function(
             self,
             trigger_function_name: str,
             callback_function: Callable,
             callback_function_param: [dict, None] = None,
```

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/utils/critical_exit/critcal_exit.py` & `je_auto_control_dev-0.0.92/je_auto_control/utils/critical_exit/critcal_exit.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/utils/exception/exception_tags.py` & `je_auto_control_dev-0.0.92/je_auto_control/utils/exception/exception_tags.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/utils/exception/exceptions.py` & `je_auto_control_dev-0.0.92/je_auto_control/utils/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/utils/executor/action_executor.py` & `je_auto_control_dev-0.0.92/je_auto_control/utils/executor/action_executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,73 +36,73 @@
 
 
 class Executor(object):
 
     def __init__(self):
         self.event_dict: dict = {
             # mouse
-            "mouse_left": click_mouse,
-            "mouse_right": click_mouse,
-            "mouse_middle": click_mouse,
-            "click_mouse": click_mouse,
-            "get_mouse_table": get_mouse_table,
-            "get_mouse_position": get_mouse_position,
-            "press_mouse": press_mouse,
-            "release_mouse": release_mouse,
-            "mouse_scroll": mouse_scroll,
-            "set_mouse_position": set_mouse_position,
-            "get_special_table": get_special_table,
+            "AC_mouse_left": click_mouse,
+            "AC_mouse_right": click_mouse,
+            "AC_mouse_middle": click_mouse,
+            "AC_click_mouse": click_mouse,
+            "AC_get_mouse_table": get_mouse_table,
+            "AC_get_mouse_position": get_mouse_position,
+            "AC_press_mouse": press_mouse,
+            "AC_release_mouse": release_mouse,
+            "AC_mouse_scroll": mouse_scroll,
+            "AC_set_mouse_position": set_mouse_position,
+            "AC_get_special_table": get_special_table,
             # keyboard
-            "get_keyboard_keys_table": get_keyboard_keys_table,
-            "type_keyboard": type_keyboard,
-            "press_keyboard_key": press_keyboard_key,
-            "release_keyboard_key": release_keyboard_key,
-            "check_key_is_press": check_key_is_press,
-            "write": write,
-            "hotkey": hotkey,
+            "AC_get_keyboard_keys_table": get_keyboard_keys_table,
+            "AC_type_keyboard": type_keyboard,
+            "AC_press_keyboard_key": press_keyboard_key,
+            "AC_release_keyboard_key": release_keyboard_key,
+            "AC_check_key_is_press": check_key_is_press,
+            "AC_write": write,
+            "AC_hotkey": hotkey,
             # image
-            "locate_all_image": locate_all_image,
-            "locate_image_center": locate_image_center,
-            "locate_and_click": locate_and_click,
+            "AC_locate_all_image": locate_all_image,
+            "AC_locate_image_center": locate_image_center,
+            "AC_locate_and_click": locate_and_click,
             # screen
-            "screen_size": screen_size,
-            "screenshot": screenshot,
+            "AC_screen_size": screen_size,
+            "AC_screenshot": screenshot,
             # test record
-            "set_record_enable": test_record_instance.set_record_enable,
+            "AC_set_record_enable": test_record_instance.set_record_enable,
             # only generate
-            "generate_html": generate_html,
-            "generate_json": generate_json,
-            "generate_xml": generate_xml,
+            "AC_generate_html": generate_html,
+            "AC_generate_json": generate_json,
+            "AC_generate_xml": generate_xml,
             # generate report
-            "generate_html_report": generate_html_report,
-            "generate_json_report": generate_json_report,
-            "generate_xml_report": generate_xml_report,
+            "AC_generate_html_report": generate_html_report,
+            "AC_generate_json_report": generate_json_report,
+            "AC_generate_xml_report": generate_xml_report,
             # record
-            "record": record,
-            "stop_record": stop_record,
+            "AC_record": record,
+            "AC_stop_record": stop_record,
             # execute
-            "execute_action": self.execute_action,
-            "execute_files": self.execute_files,
-            "add_package_to_executor": package_manager.add_package_to_executor,
-            "add_package_to_callback_executor": package_manager.add_package_to_callback_executor,
+            "AC_execute_action": self.execute_action,
+            "AC_execute_files": self.execute_files,
+            "AC_add_package_to_executor": package_manager.add_package_to_executor,
+            "AC_add_package_to_callback_executor": package_manager.add_package_to_callback_executor,
             # project
-            "create_project": create_project_dir,
+            "AC_create_project": create_project_dir,
             # Shell
-            "shell_command": ShellManager().exec_shell,
+            "AC_shell_command": ShellManager().exec_shell,
             # Another process
-            "execute_process": start_exe,
+            "AC_execute_process": start_exe,
             # Scheduler
-            "scheduler_event_trigger": self.scheduler_event_trigger,
-            "remove_blocking_scheduler_job": scheduler_manager.remove_blocking_job,
-            "remove_nonblocking_scheduler_job": scheduler_manager.remove_nonblocking_job,
-            "start_blocking_scheduler": scheduler_manager.start_block_scheduler,
-            "start_nonblocking_scheduler": scheduler_manager.start_nonblocking_scheduler,
-            "start_all_scheduler": scheduler_manager.start_all_scheduler,
-            "shutdown_blocking_scheduler": scheduler_manager.shutdown_blocking_scheduler,
-            "shutdown_nonblocking_scheduler": scheduler_manager.shutdown_nonblocking_scheduler,
+            "AC_scheduler_event_trigger": self.scheduler_event_trigger,
+            "AC_remove_blocking_scheduler_job": scheduler_manager.remove_blocking_job,
+            "AC_remove_nonblocking_scheduler_job": scheduler_manager.remove_nonblocking_job,
+            "AC_start_blocking_scheduler": scheduler_manager.start_block_scheduler,
+            "AC_start_nonblocking_scheduler": scheduler_manager.start_nonblocking_scheduler,
+            "AC_start_all_scheduler": scheduler_manager.start_all_scheduler,
+            "AC_shutdown_blocking_scheduler": scheduler_manager.shutdown_blocking_scheduler,
+            "AC_shutdown_nonblocking_scheduler": scheduler_manager.shutdown_nonblocking_scheduler,
         }
         # get all builtin function and add to event dict
         for function in getmembers(builtins, isbuiltin):
             self.event_dict.update({str(function[0]): function[1]})
 
     def _execute_event(self, action: list) -> Any:
         event = self.event_dict.get(action[0])
@@ -130,28 +130,28 @@
         execute_record_dict = dict()
         try:
             if len(action_list) > 0 or isinstance(action_list, list):
                 pass
             else:
                 raise AutoControlActionNullException(action_is_null_error)
         except Exception as error:
-            record_action_to_list("execute_action", action_list, repr(error))
+            record_action_to_list("AC_execute_action", action_list, repr(error))
             auto_control_logger.info(
                 f"execute_action, action_list: {action_list}, "
                 f"failed: {repr(error)}")
         for action in action_list:
             try:
                 event_response = self._execute_event(action)
                 execute_record = "execute: " + str(action)
                 execute_record_dict.update({execute_record: event_response})
             except Exception as error:
                 auto_control_logger.info(
                     f"execute_action, action_list: {action_list}, "
                     f"action: {action}, failed: {repr(error)}")
-                record_action_to_list("execute_action", None, repr(error))
+                record_action_to_list("AC_execute_action", None, repr(error))
                 execute_record = "execute: " + str(action)
                 execute_record_dict.update({execute_record: repr(error)})
         for key, value in execute_record_dict.items():
             print(key, flush=True)
             print(value, flush=True)
         return execute_record_dict
```

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/utils/file_process/get_dir_file_list.py` & `je_auto_control_dev-0.0.92/je_auto_control/utils/file_process/get_dir_file_list.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/utils/generate_report/generate_html_report.py` & `je_auto_control_dev-0.0.92/je_auto_control/utils/generate_report/generate_html_report.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/utils/generate_report/generate_json_report.py` & `je_auto_control_dev-0.0.92/je_auto_control/utils/generate_report/generate_json_report.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/utils/generate_report/generate_xml_report.py` & `je_auto_control_dev-0.0.92/je_auto_control/utils/generate_report/generate_xml_report.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/utils/image/screenshot.py` & `je_auto_control_dev-0.0.92/je_auto_control/utils/image/screenshot.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/utils/image/template_detection.py` & `je_auto_control_dev-0.0.92/je_auto_control/utils/image/template_detection.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/utils/json/json_file.py` & `je_auto_control_dev-0.0.92/je_auto_control/utils/json/json_file.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/utils/logging/loggin_instance.py` & `je_auto_control_dev-0.0.92/je_auto_control/utils/logging/loggin_instance.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/utils/package_manager/package_manager_class.py` & `je_auto_control_dev-0.0.92/je_auto_control/utils/package_manager/package_manager_class.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/utils/project/create_project_structure.py` & `je_auto_control_dev-0.0.92/je_auto_control/utils/project/create_project_structure.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/utils/project/template/template_executor.py` & `je_auto_control_dev-0.0.92/je_auto_control/utils/project/template/template_executor.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/utils/project/template/template_keyword.py` & `je_auto_control_dev-0.0.92/je_auto_control/utils/project/template/template_keyword.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 template_keyword_1: list = [
-    ["set_record_enable", [True]],
-    ["write", {"write_string": "Hello World"}],
-    ["type_keyboard", {"keycode": "return"}],
-    ["write", {"write_string": "If you want Windows write upcase string"}],
-    ["type_keyboard", {"keycode": "return"}],
-    ["write", {"write_string": "you need to press shift first"}],
-    ["type_keyboard", {"keycode": "return"}],
-    ["press_keyboard_key", {"keycode": "shift"}],
-    ["write", {"write_string": "UPCASEE"}],
-    ["release_keyboard_key", {"keycode": "shift"}],
-    ["type_keyboard", {"keycode": "return"}],
-    ["write", {"write_string": "this is example how to use keyword"}],
-    ["write", {"write_string": " and add module to executor"}],
-    ["type_keyboard", {"keycode": "return"}],
-    ["write", {"write_string": "now i will add time module and sleep 3 sec"}],
-    ["add_package_to_executor", ["time"]],
+    ["AC_set_record_enable", [True]],
+    ["AC_write", {"write_string": "Hello World"}],
+    ["AC_type_keyboard", {"keycode": "return"}],
+    ["AC_write", {"write_string": "If you want Windows write upcase string"}],
+    ["AC_type_keyboard", {"keycode": "return"}],
+    ["AC_write", {"write_string": "you need to press shift first"}],
+    ["AC_type_keyboard", {"keycode": "return"}],
+    ["AC_press_keyboard_key", {"keycode": "shift"}],
+    ["AC_write", {"write_string": "UPCASEE"}],
+    ["AC_release_keyboard_key", {"keycode": "shift"}],
+    ["AC_type_keyboard", {"keycode": "return"}],
+    ["AC_write", {"write_string": "this is example how to use keyword"}],
+    ["AC_write", {"write_string": " and add module to executor"}],
+    ["AC_type_keyboard", {"keycode": "return"}],
+    ["AC_write", {"write_string": "now i will add time module and sleep 3 sec"}],
+    ["AC_add_package_to_executor", ["time"]],
     ["time_sleep", [3]],
-    ["type_keyboard", {"keycode": "return"}],
-    ["write", {"write_string": "also you can use builtin function on executor like print"}],
+    ["AC_type_keyboard", {"keycode": "return"}],
+    ["AC_write", {"write_string": "also you can use builtin function on executor like print"}],
     ["print", ["Google Bye World"]],
-    ["type_keyboard", {"keycode": "return"}],
-    ["write", {"write_string": "and i will create an html report for you"}],
-    ["generate_html_report"],
-    ["type_keyboard", {"keycode": "return"}]
+    ["AC_type_keyboard", {"keycode": "return"}],
+    ["AC_write", {"write_string": "and i will create an html report for you"}],
+    ["AC_generate_html_report"],
+    ["AC_type_keyboard", {"keycode": "return"}]
 ]
 
 template_keyword_2: list = [
-    ["set_record_enable", [True]],
-    ["write", {"write_string": "in this keyword file we will change the mouse position"}],
-    ["type_keyboard", {"keycode": "return"}],
-    ["set_mouse_position", [500, 500]],
-    ["set_mouse_position", {"x": 100, "y": 100}],
-    ["set_mouse_position", [600, 600]],
-    ["set_mouse_position", {"x": 100, "y": 100}],
-    ["set_mouse_position", [400, 400]],
-    ["set_mouse_position", {"x": 100, "y": 100}],
-    ["set_mouse_position", [300, 300]],
-    ["set_mouse_position", {"x": 100, "y": 100}],
-    ["set_mouse_position", [200, 200]],
-    ["set_mouse_position", {"x": 100, "y": 100}],
-    ["set_mouse_position", [700, 700]],
-    ["set_mouse_position", {"x": 100, "y": 100}],
-    ["set_mouse_position", [800, 800]],
-    ["set_mouse_position", {"x": 100, "y": 100}],
-    ["write", {"write_string": "now i will create an json report for you"}],
-    ["type_keyboard", {"keycode": "return"}],
-    ["generate_json_report"]
+    ["AC_set_record_enable", [True]],
+    ["AC_write", {"write_string": "in this keyword file we will change the mouse position"}],
+    ["AC_type_keyboard", {"keycode": "return"}],
+    ["AC_set_mouse_position", [500, 500]],
+    ["AC_set_mouse_position", {"x": 100, "y": 100}],
+    ["AC_set_mouse_position", [600, 600]],
+    ["AC_set_mouse_position", {"x": 100, "y": 100}],
+    ["AC_set_mouse_position", [400, 400]],
+    ["AC_set_mouse_position", {"x": 100, "y": 100}],
+    ["AC_set_mouse_position", [300, 300]],
+    ["AC_set_mouse_position", {"x": 100, "y": 100}],
+    ["AC_set_mouse_position", [200, 200]],
+    ["AC_set_mouse_position", {"x": 100, "y": 100}],
+    ["AC_set_mouse_position", [700, 700]],
+    ["AC_set_mouse_position", {"x": 100, "y": 100}],
+    ["AC_set_mouse_position", [800, 800]],
+    ["AC_set_mouse_position", {"x": 100, "y": 100}],
+    ["AC_write", {"write_string": "now i will create an json report for you"}],
+    ["AC_type_keyboard", {"keycode": "return"}],
+    ["AC_generate_json_report"]
 ]
 
 bad_template_1 = [
-    ["set_record_enable", [True]],
-    ["add_package_to_executor", ["os"]],
+    ["AC_set_record_enable", [True]],
+    ["AC_add_package_to_executor", ["os"]],
     ["os_system", ["python --version"]],
     ["os_system", ["python -m pip --version"]],
 ]
```

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/utils/scheduler/extend_apscheduler.py` & `je_auto_control_dev-0.0.92/je_auto_control/utils/scheduler/extend_apscheduler.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/utils/shell_process/shell_exec.py` & `je_auto_control_dev-0.0.92/je_auto_control/utils/shell_process/shell_exec.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/utils/socket_server/auto_control_socket_server.py` & `je_auto_control_dev-0.0.92/je_auto_control/utils/socket_server/auto_control_socket_server.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/utils/start_exe/start_another_process.py` & `je_auto_control_dev-0.0.92/je_auto_control/utils/start_exe/start_another_process.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/utils/test_record/record_test_class.py` & `je_auto_control_dev-0.0.92/je_auto_control/utils/test_record/record_test_class.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/utils/timeout/multiprocess_timeout.py` & `je_auto_control_dev-0.0.92/je_auto_control/utils/timeout/multiprocess_timeout.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/utils/xml/change_xml_structure/change_xml_structure.py` & `je_auto_control_dev-0.0.92/je_auto_control/utils/xml/change_xml_structure/change_xml_structure.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/utils/xml/xml_file/xml_file.py` & `je_auto_control_dev-0.0.92/je_auto_control/utils/xml/xml_file/xml_file.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/windows/core/utils/win32_ctype_input.py` & `je_auto_control_dev-0.0.92/je_auto_control/windows/core/utils/win32_ctype_input.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/windows/core/utils/win32_keypress_check.py` & `je_auto_control_dev-0.0.92/je_auto_control/windows/core/utils/win32_keypress_check.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/windows/core/utils/win32_vk.py` & `je_auto_control_dev-0.0.92/je_auto_control/windows/core/utils/win32_vk.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/windows/keyboard/win32_ctype_keyboard_control.py` & `je_auto_control_dev-0.0.92/je_auto_control/windows/keyboard/win32_ctype_keyboard_control.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/windows/listener/win32_keyboard_listener.py` & `je_auto_control_dev-0.0.92/je_auto_control/windows/listener/win32_keyboard_listener.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
     def _win32_hook_proc(self, code, w_param, l_param) -> _user32.CallNextHookEx:
         if w_param is not _wm_keydown:
             return _user32.CallNextHookEx(self.hooked, code, w_param, l_param)
         if self.record_flag is True:
             # int to hex
             temp = hex(l_param[0] & 0xFFFFFFFF)
-            self.record_queue.put(("type_keyboard", int(temp, 16)))
+            self.record_queue.put(("AC_type_keyboard", int(temp, 16)))
         return _user32.CallNextHookEx(self.hooked, code, w_param, l_param)
 
     def _start_listener(self) -> None:
         pointer = _get_function_pointer(self._win32_hook_proc)
         self._set_win32_hook(pointer)
         message = MSG()
         _user32.GetMessageA(byref(message), 0, 0, 0)
```

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/windows/listener/win32_mouse_listener.py` & `je_auto_control_dev-0.0.92/je_auto_control/windows/listener/win32_mouse_listener.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,21 +56,21 @@
         self.hooked = None
 
     def _win32_hook_proc(self, code, w_param, l_param) -> _user32.CallNextHookEx:
         if w_param not in _wm_mouse_key_code:
             return _user32.CallNextHookEx(self.hooked, code, w_param, l_param)
         if w_param == _wm_mouse_key_code[0] and self.record_flag is True:
             x, y = position()
-            self.record_queue.put(("mouse_left", x, y))
+            self.record_queue.put(("AC_mouse_left", x, y))
         elif w_param == _wm_mouse_key_code[1] and self.record_flag is True:
             x, y = position()
-            self.record_queue.put(("mouse_right", x, y))
+            self.record_queue.put(("AC_mouse_right", x, y))
         elif w_param == _wm_mouse_key_code[2] and self.record_flag is True:
             x, y = position()
-            self.record_queue.put(("mouse_middle", x, y))
+            self.record_queue.put(("AC_mouse_middle", x, y))
         return _user32.CallNextHookEx(self.hooked, code, w_param, l_param)
 
     def _start_listener(self) -> None:
         pointer = _get_function_pointer(self._win32_hook_proc)
         self._set_win32_hook(pointer)
         message = MSG()
         _user32.GetMessageA(byref(message), 0, 0, 0)
```

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/windows/mouse/win32_ctype_mouse_control.py` & `je_auto_control_dev-0.0.92/je_auto_control/windows/mouse/win32_ctype_mouse_control.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/windows/record/win32_record.py` & `je_auto_control_dev-0.0.92/je_auto_control/windows/record/win32_record.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/windows/screen/win32_screen.py` & `je_auto_control_dev-0.0.92/je_auto_control/windows/screen/win32_screen.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/wrapper/auto_control_image.py` & `je_auto_control_dev-0.0.92/je_auto_control/wrapper/auto_control_image.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/wrapper/auto_control_keyboard.py` & `je_auto_control_dev-0.0.92/je_auto_control/wrapper/auto_control_keyboard.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/wrapper/auto_control_mouse.py` & `je_auto_control_dev-0.0.92/je_auto_control/wrapper/auto_control_mouse.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/wrapper/auto_control_record.py` & `je_auto_control_dev-0.0.92/je_auto_control/wrapper/auto_control_record.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/wrapper/auto_control_screen.py` & `je_auto_control_dev-0.0.92/je_auto_control/wrapper/auto_control_screen.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from je_auto_control.wrapper.platform_wrapper import screen
 
 
 def screen_size() -> Tuple[int, int]:
     """
     get screen size
     """
-    auto_control_logger.info("screen_size")
+    auto_control_logger.info("AC_screen_size")
     try:
         try:
             record_action_to_list("size", None)
             return screen.size()
         except AutoControlScreenException:
             auto_control_logger.error(f"screen_size, failed: {repr(AutoControlScreenException(screen_get_size))}")
             raise AutoControlScreenException(screen_get_size)
@@ -35,20 +35,20 @@
     :param file_path screenshot file save path
     :param screen_region screenshot screen_region
     """
     auto_control_logger.info(f"screen_size, file_path: {file_path}, screen_region: {screen_region}")
     param = locals()
     try:
         try:
-            record_action_to_list("screenshot", param)
+            record_action_to_list("AC_screenshot", param)
             return cv2.cvtColor(
                 np.array(pil_screenshot(file_path=file_path, screen_region=screen_region)), cv2.COLOR_RGB2BGR)
         except AutoControlScreenException as error:
             auto_control_logger.info(
                 f"screen_size, file_path: {file_path}, screen_region: {screen_region}, "
                 f"failed: {AutoControlScreenException(screen_screenshot + ' ' + repr(error))}")
             raise AutoControlScreenException(screen_screenshot + " " + repr(error))
     except Exception as error:
-        record_action_to_list("screenshot", None, repr(error))
+        record_action_to_list("AC_screenshot", None, repr(error))
         auto_control_logger.info(
             f"screen_size, file_path: {file_path}, screen_region: {screen_region}, "
             f"failed: {repr(error)}")
```

### Comparing `je_auto_control_dev-0.0.91/je_auto_control/wrapper/platform_wrapper.py` & `je_auto_control_dev-0.0.92/je_auto_control/wrapper/platform_wrapper.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/je_auto_control_dev.egg-info/PKG-INFO` & `je_auto_control_dev-0.0.92/je_auto_control_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je-auto-control-dev
-Version: 0.0.91
+Version: 0.0.92
 Summary: GUI Automation Framework
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/AutoControl
 Project-URL: Documentation, https://autocontrol.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/AutoControl
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `je_auto_control_dev-0.0.91/je_auto_control_dev.egg-info/SOURCES.txt` & `je_auto_control_dev-0.0.92/je_auto_control_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.91/pyproject.toml` & `je_auto_control_dev-0.0.92/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is dev version
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "je_auto_control_dev"
-version = "0.0.91"
+version = "0.0.92"
 authors = [
     { name = "JE-Chen", email = "jechenmailman@gmail.com" },
 ]
 description = "GUI Automation Framework"
 requires-python = ">=3.8"
 license = { text = "MIT" }
 dependencies = [
```

