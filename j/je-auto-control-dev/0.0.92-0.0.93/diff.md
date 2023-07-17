# Comparing `tmp/je_auto_control_dev-0.0.92.tar.gz` & `tmp/je_auto_control_dev-0.0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "je_auto_control_dev-0.0.92.tar", last modified: Mon Jul 17 09:36:10 2023, max compression
+gzip compressed data, was "je_auto_control_dev-0.0.93.tar", last modified: Mon Jul 17 09:46:04 2023, max compression
```

## Comparing `je_auto_control_dev-0.0.92.tar` & `je_auto_control_dev-0.0.93.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.569200 je_auto_control_dev-0.0.92/
--rw-rw-rw-   0        0        0     3780 2023-07-17 09:36:10.568210 je_auto_control_dev-0.0.92/PKG-INFO
--rw-rw-rw-   0        0        0     2975 2023-05-30 02:56:01.000000 je_auto_control_dev-0.0.92/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.016602 je_auto_control_dev-0.0.92/je_auto_control/
--rw-rw-rw-   0        0        0     6485 2023-07-17 09:33:39.000000 je_auto_control_dev-0.0.92/je_auto_control/__init__.py
--rw-rw-rw-   0        0        0     2355 2023-07-17 09:33:56.000000 je_auto_control_dev-0.0.92/je_auto_control/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.021123 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.024119 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/core/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.056163 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/core/utils/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/core/utils/__init__.py
--rw-rw-rw-   0        0        0      386 2023-07-17 06:24:07.000000 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/core/utils/x11_linux_display.py
--rw-rw-rw-   0        0        0    14539 2023-06-17 09:28:03.000000 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/core/utils/x11_linux_vk.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.069723 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/keyboard/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/keyboard/__init__.py
--rw-rw-rw-   0        0        0      828 2023-06-17 09:28:03.000000 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/keyboard/x11_linux_keyboard_control.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.080378 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/listener/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/listener/__init__.py
--rw-rw-rw-   0        0        0     5554 2023-06-13 01:38:29.000000 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/listener/x11_linux_listener.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.090256 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/mouse/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/mouse/__init__.py
--rw-rw-rw-   0        0        0     2393 2023-05-22 01:10:31.000000 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/mouse/x11_linux_mouse_control.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.100800 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/record/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/record/__init__.py
--rw-rw-rw-   0        0        0     1575 2023-07-17 09:22:52.000000 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/record/x11_linux_record.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.108662 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/screen/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/screen/__init__.py
--rw-rw-rw-   0        0        0      533 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/screen/x11_linux_screen.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.112668 je_auto_control_dev-0.0.92/je_auto_control/osx/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/osx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.118501 je_auto_control_dev-0.0.92/je_auto_control/osx/core/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/osx/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.128065 je_auto_control_dev-0.0.92/je_auto_control/osx/core/utils/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/osx/core/utils/__init__.py
--rw-rw-rw-   0        0        0     3157 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/osx/core/utils/osx_vk.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.144054 je_auto_control_dev-0.0.92/je_auto_control/osx/keyboard/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/osx/keyboard/__init__.py
--rw-rw-rw-   0        0        0     3017 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/osx/keyboard/osx_keyboard.py
--rw-rw-rw-   0        0        0      446 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/osx/keyboard/osx_keyboard_check.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.152307 je_auto_control_dev-0.0.92/je_auto_control/osx/listener/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/osx/listener/__init__.py
--rw-rw-rw-   0        0        0     1528 2023-07-17 09:22:52.000000 je_auto_control_dev-0.0.92/je_auto_control/osx/listener/osx_listener.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.162123 je_auto_control_dev-0.0.92/je_auto_control/osx/mouse/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/osx/mouse/__init__.py
--rw-rw-rw-   0        0        0     3500 2023-05-22 01:10:31.000000 je_auto_control_dev-0.0.92/je_auto_control/osx/mouse/osx_mouse.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.170942 je_auto_control_dev-0.0.92/je_auto_control/osx/record/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/osx/record/__init__.py
--rw-rw-rw-   0        0        0      957 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/osx/record/osx_record.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.180044 je_auto_control_dev-0.0.92/je_auto_control/osx/screen/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/osx/screen/__init__.py
--rw-rw-rw-   0        0        0      495 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/osx/screen/osx_screen.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.185049 je_auto_control_dev-0.0.92/je_auto_control/utils/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.191358 je_auto_control_dev-0.0.92/je_auto_control/utils/callback/
--rw-rw-rw-   0        0        0        0 2023-03-31 01:55:17.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/callback/__init__.py
--rw-rw-rw-   0        0        0     7917 2023-07-17 09:31:18.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/callback/callback_function_executor.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.200400 je_auto_control_dev-0.0.92/je_auto_control/utils/critical_exit/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/critical_exit/__init__.py
--rw-rw-rw-   0        0        0     1524 2023-04-10 02:15:44.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/critical_exit/critcal_exit.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.217020 je_auto_control_dev-0.0.92/je_auto_control/utils/exception/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/exception/__init__.py
--rw-rw-rw-   0        0        0     2870 2023-06-08 09:14:35.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0     1663 2023-03-31 02:15:20.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.222971 je_auto_control_dev-0.0.92/je_auto_control/utils/executor/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/executor/__init__.py
--rw-rw-rw-   0        0        0    10300 2023-07-17 09:33:34.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/executor/action_executor.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.231310 je_auto_control_dev-0.0.92/je_auto_control/utils/file_process/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/file_process/__init__.py
--rw-rw-rw-   0        0        0      758 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/file_process/get_dir_file_list.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.245842 je_auto_control_dev-0.0.92/je_auto_control/utils/generate_report/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/generate_report/__init__.py
--rw-rw-rw-   0        0        0     4938 2023-07-17 09:34:19.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/generate_report/generate_html_report.py
--rw-rw-rw-   0        0        0     3415 2023-07-17 09:34:23.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/generate_report/generate_json_report.py
--rw-rw-rw-   0        0        0     2090 2023-07-17 09:34:26.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/generate_report/generate_xml_report.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.261382 je_auto_control_dev-0.0.92/je_auto_control/utils/image/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/image/__init__.py
--rw-rw-rw-   0        0        0      532 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/image/screenshot.py
--rw-rw-rw-   0        0        0     1151 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/image/template_detection.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.273152 je_auto_control_dev-0.0.92/je_auto_control/utils/json/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/json/__init__.py
--rw-rw-rw-   0        0        0     1477 2023-06-19 06:56:53.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/json/json_file.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.284537 je_auto_control_dev-0.0.92/je_auto_control/utils/logging/
--rw-rw-rw-   0        0        0        0 2023-06-08 03:44:59.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/logging/__init__.py
--rw-rw-rw-   0        0        0      579 2023-06-12 07:11:50.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/logging/loggin_instance.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.294191 je_auto_control_dev-0.0.92/je_auto_control/utils/package_manager/
--rw-rw-rw-   0        0        0        0 2023-04-06 01:15:41.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/package_manager/__init__.py
--rw-rw-rw-   0        0        0     3644 2023-06-19 09:13:36.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/package_manager/package_manager_class.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.304366 je_auto_control_dev-0.0.92/je_auto_control/utils/project/
--rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/project/__init__.py
--rw-rw-rw-   0        0        0     3030 2023-06-13 06:53:21.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/project/create_project_structure.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.319145 je_auto_control_dev-0.0.92/je_auto_control/utils/project/template/
--rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/project/template/__init__.py
--rw-rw-rw-   0        0        0      639 2023-04-10 08:38:18.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/project/template/template_executor.py
--rw-rw-rw-   0        0        0     2649 2023-07-17 09:30:46.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/project/template/template_keyword.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.328074 je_auto_control_dev-0.0.92/je_auto_control/utils/scheduler/
--rw-rw-rw-   0        0        0        0 2023-05-31 01:17:46.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/scheduler/__init__.py
--rw-rw-rw-   0        0        0    11468 2023-07-17 02:27:57.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/scheduler/extend_apscheduler.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.339055 je_auto_control_dev-0.0.92/je_auto_control/utils/shell_process/
--rw-rw-rw-   0        0        0        0 2023-05-29 01:48:49.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/shell_process/__init__.py
--rw-rw-rw-   0        0        0     5226 2023-06-13 06:53:21.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/shell_process/shell_exec.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.344328 je_auto_control_dev-0.0.92/je_auto_control/utils/socket_server/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/socket_server/__init__.py
--rw-rw-rw-   0        0        0     2329 2023-06-19 07:21:50.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/socket_server/auto_control_socket_server.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.354776 je_auto_control_dev-0.0.92/je_auto_control/utils/start_exe/
--rw-rw-rw-   0        0        0        0 2023-05-29 01:48:49.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/start_exe/__init__.py
--rw-rw-rw-   0        0        0      822 2023-06-19 07:21:50.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/start_exe/start_another_process.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.363314 je_auto_control_dev-0.0.92/je_auto_control/utils/test_record/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/test_record/__init__.py
--rw-rw-rw-   0        0        0     1059 2023-06-13 06:39:14.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/test_record/record_test_class.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.376368 je_auto_control_dev-0.0.92/je_auto_control/utils/timeout/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/timeout/__init__.py
--rw-rw-rw-   0        0        0      659 2023-06-19 07:40:40.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/timeout/multiprocess_timeout.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.379428 je_auto_control_dev-0.0.92/je_auto_control/utils/xml/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/xml/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.389996 je_auto_control_dev-0.0.92/je_auto_control/utils/xml/change_xml_structure/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/xml/change_xml_structure/__init__.py
--rw-rw-rw-   0        0        0     2498 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/xml/change_xml_structure/change_xml_structure.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.399166 je_auto_control_dev-0.0.92/je_auto_control/utils/xml/xml_file/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/xml/xml_file/__init__.py
--rw-rw-rw-   0        0        0     2369 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/utils/xml/xml_file/xml_file.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.405165 je_auto_control_dev-0.0.92/je_auto_control/windows/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.410440 je_auto_control_dev-0.0.92/je_auto_control/windows/core/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.439770 je_auto_control_dev-0.0.92/je_auto_control/windows/core/utils/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/core/utils/__init__.py
--rw-rw-rw-   0        0        0     2388 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/core/utils/win32_ctype_input.py
--rw-rw-rw-   0        0        0      584 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/core/utils/win32_keypress_check.py
--rw-rw-rw-   0        0        0     5804 2023-07-17 06:26:04.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/core/utils/win32_vk.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.453271 je_auto_control_dev-0.0.92/je_auto_control/windows/keyboard/
--rw-rw-rw-   0        0        0        4 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/keyboard/__init__.py
--rw-rw-rw-   0        0        0     1259 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/keyboard/win32_ctype_keyboard_control.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.463779 je_auto_control_dev-0.0.92/je_auto_control/windows/listener/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/listener/__init__.py
--rw-rw-rw-   0        0        0     2541 2023-07-17 09:22:52.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/listener/win32_keyboard_listener.py
--rw-rw-rw-   0        0        0     3074 2023-07-17 09:18:18.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/listener/win32_mouse_listener.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.473815 je_auto_control_dev-0.0.92/je_auto_control/windows/mouse/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/mouse/__init__.py
--rw-rw-rw-   0        0        0     4170 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/mouse/win32_ctype_mouse_control.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.486376 je_auto_control_dev-0.0.92/je_auto_control/windows/record/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/record/__init__.py
--rw-rw-rw-   0        0        0     2182 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/record/win32_record.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.496195 je_auto_control_dev-0.0.92/je_auto_control/windows/screen/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/screen/__init__.py
--rw-rw-rw-   0        0        0      568 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/windows/screen/win32_screen.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.525205 je_auto_control_dev-0.0.92/je_auto_control/wrapper/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.92/je_auto_control/wrapper/__init__.py
--rw-rw-rw-   0        0        0     8157 2023-07-17 09:34:45.000000 je_auto_control_dev-0.0.92/je_auto_control/wrapper/auto_control_image.py
--rw-rw-rw-   0        0        0    14111 2023-07-17 09:34:52.000000 je_auto_control_dev-0.0.92/je_auto_control/wrapper/auto_control_keyboard.py
--rw-rw-rw-   0        0        0    11484 2023-07-17 09:34:57.000000 je_auto_control_dev-0.0.92/je_auto_control/wrapper/auto_control_mouse.py
--rw-rw-rw-   0        0        0     1957 2023-07-17 09:35:02.000000 je_auto_control_dev-0.0.92/je_auto_control/wrapper/auto_control_record.py
--rw-rw-rw-   0        0        0     2442 2023-07-17 09:24:58.000000 je_auto_control_dev-0.0.92/je_auto_control/wrapper/auto_control_screen.py
--rw-rw-rw-   0        0        0    58693 2023-07-17 09:21:08.000000 je_auto_control_dev-0.0.92/je_auto_control/wrapper/platform_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:36:10.562084 je_auto_control_dev-0.0.92/je_auto_control_dev.egg-info/
--rw-rw-rw-   0        0        0     3780 2023-07-17 09:36:09.000000 je_auto_control_dev-0.0.92/je_auto_control_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5256 2023-07-17 09:36:09.000000 je_auto_control_dev-0.0.92/je_auto_control_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 09:36:09.000000 je_auto_control_dev-0.0.92/je_auto_control_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      124 2023-07-17 09:36:09.000000 je_auto_control_dev-0.0.92/je_auto_control_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-17 09:36:09.000000 je_auto_control_dev-0.0.92/je_auto_control_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1310 2023-07-17 09:35:43.000000 je_auto_control_dev-0.0.92/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-17 09:36:10.570199 je_auto_control_dev-0.0.92/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.668081 je_auto_control_dev-0.0.93/
+-rw-rw-rw-   0        0        0     3780 2023-07-17 09:46:04.667071 je_auto_control_dev-0.0.93/PKG-INFO
+-rw-rw-rw-   0        0        0     2975 2023-05-30 02:56:01.000000 je_auto_control_dev-0.0.93/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.263737 je_auto_control_dev-0.0.93/je_auto_control/
+-rw-rw-rw-   0        0        0     6485 2023-07-17 09:33:39.000000 je_auto_control_dev-0.0.93/je_auto_control/__init__.py
+-rw-rw-rw-   0        0        0     2355 2023-07-17 09:33:56.000000 je_auto_control_dev-0.0.93/je_auto_control/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.265737 je_auto_control_dev-0.0.93/je_auto_control/linux_with_x11/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/linux_with_x11/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.268739 je_auto_control_dev-0.0.93/je_auto_control/linux_with_x11/core/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/linux_with_x11/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.279494 je_auto_control_dev-0.0.93/je_auto_control/linux_with_x11/core/utils/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/linux_with_x11/core/utils/__init__.py
+-rw-rw-rw-   0        0        0      386 2023-07-17 06:24:07.000000 je_auto_control_dev-0.0.93/je_auto_control/linux_with_x11/core/utils/x11_linux_display.py
+-rw-rw-rw-   0        0        0    14539 2023-06-17 09:28:03.000000 je_auto_control_dev-0.0.93/je_auto_control/linux_with_x11/core/utils/x11_linux_vk.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.284938 je_auto_control_dev-0.0.93/je_auto_control/linux_with_x11/keyboard/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/linux_with_x11/keyboard/__init__.py
+-rw-rw-rw-   0        0        0      828 2023-06-17 09:28:03.000000 je_auto_control_dev-0.0.93/je_auto_control/linux_with_x11/keyboard/x11_linux_keyboard_control.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.290444 je_auto_control_dev-0.0.93/je_auto_control/linux_with_x11/listener/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/linux_with_x11/listener/__init__.py
+-rw-rw-rw-   0        0        0     5554 2023-06-13 01:38:29.000000 je_auto_control_dev-0.0.93/je_auto_control/linux_with_x11/listener/x11_linux_listener.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.297447 je_auto_control_dev-0.0.93/je_auto_control/linux_with_x11/mouse/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/linux_with_x11/mouse/__init__.py
+-rw-rw-rw-   0        0        0     2393 2023-05-22 01:10:31.000000 je_auto_control_dev-0.0.93/je_auto_control/linux_with_x11/mouse/x11_linux_mouse_control.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.302476 je_auto_control_dev-0.0.93/je_auto_control/linux_with_x11/record/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/linux_with_x11/record/__init__.py
+-rw-rw-rw-   0        0        0     1575 2023-07-17 09:22:52.000000 je_auto_control_dev-0.0.93/je_auto_control/linux_with_x11/record/x11_linux_record.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.308478 je_auto_control_dev-0.0.93/je_auto_control/linux_with_x11/screen/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/linux_with_x11/screen/__init__.py
+-rw-rw-rw-   0        0        0      533 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/linux_with_x11/screen/x11_linux_screen.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.311749 je_auto_control_dev-0.0.93/je_auto_control/osx/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/osx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.313746 je_auto_control_dev-0.0.93/je_auto_control/osx/core/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/osx/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.322032 je_auto_control_dev-0.0.93/je_auto_control/osx/core/utils/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/osx/core/utils/__init__.py
+-rw-rw-rw-   0        0        0     3157 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/osx/core/utils/osx_vk.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.335502 je_auto_control_dev-0.0.93/je_auto_control/osx/keyboard/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/osx/keyboard/__init__.py
+-rw-rw-rw-   0        0        0     3017 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/osx/keyboard/osx_keyboard.py
+-rw-rw-rw-   0        0        0      446 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/osx/keyboard/osx_keyboard_check.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.343855 je_auto_control_dev-0.0.93/je_auto_control/osx/listener/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/osx/listener/__init__.py
+-rw-rw-rw-   0        0        0     1528 2023-07-17 09:22:52.000000 je_auto_control_dev-0.0.93/je_auto_control/osx/listener/osx_listener.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.352089 je_auto_control_dev-0.0.93/je_auto_control/osx/mouse/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/osx/mouse/__init__.py
+-rw-rw-rw-   0        0        0     3500 2023-05-22 01:10:31.000000 je_auto_control_dev-0.0.93/je_auto_control/osx/mouse/osx_mouse.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.362605 je_auto_control_dev-0.0.93/je_auto_control/osx/record/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/osx/record/__init__.py
+-rw-rw-rw-   0        0        0      957 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/osx/record/osx_record.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.370545 je_auto_control_dev-0.0.93/je_auto_control/osx/screen/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/osx/screen/__init__.py
+-rw-rw-rw-   0        0        0      495 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/osx/screen/osx_screen.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.375834 je_auto_control_dev-0.0.93/je_auto_control/utils/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.383843 je_auto_control_dev-0.0.93/je_auto_control/utils/callback/
+-rw-rw-rw-   0        0        0        0 2023-03-31 01:55:17.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/callback/__init__.py
+-rw-rw-rw-   0        0        0     7917 2023-07-17 09:31:18.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/callback/callback_function_executor.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.397707 je_auto_control_dev-0.0.93/je_auto_control/utils/critical_exit/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/critical_exit/__init__.py
+-rw-rw-rw-   0        0        0     1524 2023-04-10 02:15:44.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/critical_exit/critcal_exit.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.415156 je_auto_control_dev-0.0.93/je_auto_control/utils/exception/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0     2870 2023-06-08 09:14:35.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0     1663 2023-03-31 02:15:20.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.431256 je_auto_control_dev-0.0.93/je_auto_control/utils/executor/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/executor/__init__.py
+-rw-rw-rw-   0        0        0    10300 2023-07-17 09:33:34.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/executor/action_executor.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.446098 je_auto_control_dev-0.0.93/je_auto_control/utils/file_process/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/file_process/__init__.py
+-rw-rw-rw-   0        0        0      758 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/file_process/get_dir_file_list.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.468699 je_auto_control_dev-0.0.93/je_auto_control/utils/generate_report/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/generate_report/__init__.py
+-rw-rw-rw-   0        0        0     4938 2023-07-17 09:34:19.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/generate_report/generate_html_report.py
+-rw-rw-rw-   0        0        0     3415 2023-07-17 09:34:23.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/generate_report/generate_json_report.py
+-rw-rw-rw-   0        0        0     2090 2023-07-17 09:34:26.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/generate_report/generate_xml_report.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.477103 je_auto_control_dev-0.0.93/je_auto_control/utils/image/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/image/__init__.py
+-rw-rw-rw-   0        0        0      532 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/image/screenshot.py
+-rw-rw-rw-   0        0        0     1151 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/image/template_detection.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.481880 je_auto_control_dev-0.0.93/je_auto_control/utils/json/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/json/__init__.py
+-rw-rw-rw-   0        0        0     1477 2023-06-19 06:56:53.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/json/json_file.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.487882 je_auto_control_dev-0.0.93/je_auto_control/utils/logging/
+-rw-rw-rw-   0        0        0        0 2023-06-08 03:44:59.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/logging/__init__.py
+-rw-rw-rw-   0        0        0      579 2023-06-12 07:11:50.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/logging/loggin_instance.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.495512 je_auto_control_dev-0.0.93/je_auto_control/utils/package_manager/
+-rw-rw-rw-   0        0        0        0 2023-04-06 01:15:41.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/package_manager/__init__.py
+-rw-rw-rw-   0        0        0     3644 2023-06-19 09:13:36.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/package_manager/package_manager_class.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.500530 je_auto_control_dev-0.0.93/je_auto_control/utils/project/
+-rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/project/__init__.py
+-rw-rw-rw-   0        0        0     3030 2023-06-13 06:53:21.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/project/create_project_structure.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.509821 je_auto_control_dev-0.0.93/je_auto_control/utils/project/template/
+-rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/project/template/__init__.py
+-rw-rw-rw-   0        0        0      639 2023-04-10 08:38:18.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/project/template/template_executor.py
+-rw-rw-rw-   0        0        0     2649 2023-07-17 09:30:46.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/project/template/template_keyword.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.515504 je_auto_control_dev-0.0.93/je_auto_control/utils/scheduler/
+-rw-rw-rw-   0        0        0        0 2023-05-31 01:17:46.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/scheduler/__init__.py
+-rw-rw-rw-   0        0        0    11468 2023-07-17 02:27:57.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/scheduler/extend_apscheduler.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.520523 je_auto_control_dev-0.0.93/je_auto_control/utils/shell_process/
+-rw-rw-rw-   0        0        0        0 2023-05-29 01:48:49.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/shell_process/__init__.py
+-rw-rw-rw-   0        0        0     5226 2023-06-13 06:53:21.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/shell_process/shell_exec.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.526045 je_auto_control_dev-0.0.93/je_auto_control/utils/socket_server/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/socket_server/__init__.py
+-rw-rw-rw-   0        0        0     2329 2023-06-19 07:21:50.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/socket_server/auto_control_socket_server.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.532676 je_auto_control_dev-0.0.93/je_auto_control/utils/start_exe/
+-rw-rw-rw-   0        0        0        0 2023-05-29 01:48:49.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/start_exe/__init__.py
+-rw-rw-rw-   0        0        0      822 2023-06-19 07:21:50.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/start_exe/start_another_process.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.537651 je_auto_control_dev-0.0.93/je_auto_control/utils/test_record/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/test_record/__init__.py
+-rw-rw-rw-   0        0        0     1059 2023-06-13 06:39:14.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/test_record/record_test_class.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.541698 je_auto_control_dev-0.0.93/je_auto_control/utils/timeout/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/timeout/__init__.py
+-rw-rw-rw-   0        0        0      659 2023-06-19 07:40:40.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/timeout/multiprocess_timeout.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.544701 je_auto_control_dev-0.0.93/je_auto_control/utils/xml/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/xml/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.549425 je_auto_control_dev-0.0.93/je_auto_control/utils/xml/change_xml_structure/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/xml/change_xml_structure/__init__.py
+-rw-rw-rw-   0        0        0     2498 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/xml/change_xml_structure/change_xml_structure.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.555436 je_auto_control_dev-0.0.93/je_auto_control/utils/xml/xml_file/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/xml/xml_file/__init__.py
+-rw-rw-rw-   0        0        0     2369 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/utils/xml/xml_file/xml_file.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.558944 je_auto_control_dev-0.0.93/je_auto_control/windows/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/windows/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.561474 je_auto_control_dev-0.0.93/je_auto_control/windows/core/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/windows/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.572132 je_auto_control_dev-0.0.93/je_auto_control/windows/core/utils/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/windows/core/utils/__init__.py
+-rw-rw-rw-   0        0        0     2388 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/windows/core/utils/win32_ctype_input.py
+-rw-rw-rw-   0        0        0      584 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/windows/core/utils/win32_keypress_check.py
+-rw-rw-rw-   0        0        0     5804 2023-07-17 06:26:04.000000 je_auto_control_dev-0.0.93/je_auto_control/windows/core/utils/win32_vk.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.578665 je_auto_control_dev-0.0.93/je_auto_control/windows/keyboard/
+-rw-rw-rw-   0        0        0        4 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/windows/keyboard/__init__.py
+-rw-rw-rw-   0        0        0     1259 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/windows/keyboard/win32_ctype_keyboard_control.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.588739 je_auto_control_dev-0.0.93/je_auto_control/windows/listener/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/windows/listener/__init__.py
+-rw-rw-rw-   0        0        0     2541 2023-07-17 09:22:52.000000 je_auto_control_dev-0.0.93/je_auto_control/windows/listener/win32_keyboard_listener.py
+-rw-rw-rw-   0        0        0     3074 2023-07-17 09:18:18.000000 je_auto_control_dev-0.0.93/je_auto_control/windows/listener/win32_mouse_listener.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.596071 je_auto_control_dev-0.0.93/je_auto_control/windows/mouse/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/windows/mouse/__init__.py
+-rw-rw-rw-   0        0        0     4170 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/windows/mouse/win32_ctype_mouse_control.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.602222 je_auto_control_dev-0.0.93/je_auto_control/windows/record/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/windows/record/__init__.py
+-rw-rw-rw-   0        0        0     2182 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/windows/record/win32_record.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.607399 je_auto_control_dev-0.0.93/je_auto_control/windows/screen/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/windows/screen/__init__.py
+-rw-rw-rw-   0        0        0      568 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/windows/screen/win32_screen.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.631476 je_auto_control_dev-0.0.93/je_auto_control/wrapper/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.93/je_auto_control/wrapper/__init__.py
+-rw-rw-rw-   0        0        0     8157 2023-07-17 09:34:45.000000 je_auto_control_dev-0.0.93/je_auto_control/wrapper/auto_control_image.py
+-rw-rw-rw-   0        0        0    14111 2023-07-17 09:34:52.000000 je_auto_control_dev-0.0.93/je_auto_control/wrapper/auto_control_keyboard.py
+-rw-rw-rw-   0        0        0    11484 2023-07-17 09:34:57.000000 je_auto_control_dev-0.0.93/je_auto_control/wrapper/auto_control_mouse.py
+-rw-rw-rw-   0        0        0     1960 2023-07-17 09:45:23.000000 je_auto_control_dev-0.0.93/je_auto_control/wrapper/auto_control_record.py
+-rw-rw-rw-   0        0        0     2442 2023-07-17 09:24:58.000000 je_auto_control_dev-0.0.93/je_auto_control/wrapper/auto_control_screen.py
+-rw-rw-rw-   0        0        0    58693 2023-07-17 09:21:08.000000 je_auto_control_dev-0.0.93/je_auto_control/wrapper/platform_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:46:04.662924 je_auto_control_dev-0.0.93/je_auto_control_dev.egg-info/
+-rw-rw-rw-   0        0        0     3780 2023-07-17 09:46:04.000000 je_auto_control_dev-0.0.93/je_auto_control_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5256 2023-07-17 09:46:04.000000 je_auto_control_dev-0.0.93/je_auto_control_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 09:46:04.000000 je_auto_control_dev-0.0.93/je_auto_control_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      124 2023-07-17 09:46:04.000000 je_auto_control_dev-0.0.93/je_auto_control_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-17 09:46:04.000000 je_auto_control_dev-0.0.93/je_auto_control_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1310 2023-07-17 09:45:38.000000 je_auto_control_dev-0.0.93/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-17 09:46:04.668617 je_auto_control_dev-0.0.93/setup.cfg
```

### Comparing `je_auto_control_dev-0.0.92/PKG-INFO` & `je_auto_control_dev-0.0.93/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je_auto_control_dev
-Version: 0.0.92
+Version: 0.0.93
 Summary: GUI Automation Framework
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/AutoControl
 Project-URL: Documentation, https://autocontrol.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/AutoControl
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `je_auto_control_dev-0.0.92/README.md` & `je_auto_control_dev-0.0.93/README.md`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/__init__.py` & `je_auto_control_dev-0.0.93/je_auto_control/__init__.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/__main__.py` & `je_auto_control_dev-0.0.93/je_auto_control/__main__.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/core/utils/x11_linux_vk.py` & `je_auto_control_dev-0.0.93/je_auto_control/linux_with_x11/core/utils/x11_linux_vk.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/keyboard/x11_linux_keyboard_control.py` & `je_auto_control_dev-0.0.93/je_auto_control/linux_with_x11/keyboard/x11_linux_keyboard_control.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/listener/x11_linux_listener.py` & `je_auto_control_dev-0.0.93/je_auto_control/linux_with_x11/listener/x11_linux_listener.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/mouse/x11_linux_mouse_control.py` & `je_auto_control_dev-0.0.93/je_auto_control/linux_with_x11/mouse/x11_linux_mouse_control.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/record/x11_linux_record.py` & `je_auto_control_dev-0.0.93/je_auto_control/linux_with_x11/record/x11_linux_record.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/linux_with_x11/screen/x11_linux_screen.py` & `je_auto_control_dev-0.0.93/je_auto_control/linux_with_x11/screen/x11_linux_screen.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/osx/core/utils/osx_vk.py` & `je_auto_control_dev-0.0.93/je_auto_control/osx/core/utils/osx_vk.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/osx/keyboard/osx_keyboard.py` & `je_auto_control_dev-0.0.93/je_auto_control/osx/keyboard/osx_keyboard.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/osx/listener/osx_listener.py` & `je_auto_control_dev-0.0.93/je_auto_control/osx/listener/osx_listener.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/osx/mouse/osx_mouse.py` & `je_auto_control_dev-0.0.93/je_auto_control/osx/mouse/osx_mouse.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/osx/record/osx_record.py` & `je_auto_control_dev-0.0.93/je_auto_control/osx/record/osx_record.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/utils/callback/callback_function_executor.py` & `je_auto_control_dev-0.0.93/je_auto_control/utils/callback/callback_function_executor.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/utils/critical_exit/critcal_exit.py` & `je_auto_control_dev-0.0.93/je_auto_control/utils/critical_exit/critcal_exit.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/utils/exception/exception_tags.py` & `je_auto_control_dev-0.0.93/je_auto_control/utils/exception/exception_tags.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/utils/exception/exceptions.py` & `je_auto_control_dev-0.0.93/je_auto_control/utils/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/utils/executor/action_executor.py` & `je_auto_control_dev-0.0.93/je_auto_control/utils/executor/action_executor.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/utils/file_process/get_dir_file_list.py` & `je_auto_control_dev-0.0.93/je_auto_control/utils/file_process/get_dir_file_list.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/utils/generate_report/generate_html_report.py` & `je_auto_control_dev-0.0.93/je_auto_control/utils/generate_report/generate_html_report.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/utils/generate_report/generate_json_report.py` & `je_auto_control_dev-0.0.93/je_auto_control/utils/generate_report/generate_json_report.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/utils/generate_report/generate_xml_report.py` & `je_auto_control_dev-0.0.93/je_auto_control/utils/generate_report/generate_xml_report.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/utils/image/screenshot.py` & `je_auto_control_dev-0.0.93/je_auto_control/utils/image/screenshot.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/utils/image/template_detection.py` & `je_auto_control_dev-0.0.93/je_auto_control/utils/image/template_detection.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/utils/json/json_file.py` & `je_auto_control_dev-0.0.93/je_auto_control/utils/json/json_file.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/utils/logging/loggin_instance.py` & `je_auto_control_dev-0.0.93/je_auto_control/utils/logging/loggin_instance.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/utils/package_manager/package_manager_class.py` & `je_auto_control_dev-0.0.93/je_auto_control/utils/package_manager/package_manager_class.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/utils/project/create_project_structure.py` & `je_auto_control_dev-0.0.93/je_auto_control/utils/project/create_project_structure.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/utils/project/template/template_executor.py` & `je_auto_control_dev-0.0.93/je_auto_control/utils/project/template/template_executor.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/utils/project/template/template_keyword.py` & `je_auto_control_dev-0.0.93/je_auto_control/utils/project/template/template_keyword.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/utils/scheduler/extend_apscheduler.py` & `je_auto_control_dev-0.0.93/je_auto_control/utils/scheduler/extend_apscheduler.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/utils/shell_process/shell_exec.py` & `je_auto_control_dev-0.0.93/je_auto_control/utils/shell_process/shell_exec.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/utils/socket_server/auto_control_socket_server.py` & `je_auto_control_dev-0.0.93/je_auto_control/utils/socket_server/auto_control_socket_server.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/utils/start_exe/start_another_process.py` & `je_auto_control_dev-0.0.93/je_auto_control/utils/start_exe/start_another_process.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/utils/test_record/record_test_class.py` & `je_auto_control_dev-0.0.93/je_auto_control/utils/test_record/record_test_class.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/utils/timeout/multiprocess_timeout.py` & `je_auto_control_dev-0.0.93/je_auto_control/utils/timeout/multiprocess_timeout.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/utils/xml/change_xml_structure/change_xml_structure.py` & `je_auto_control_dev-0.0.93/je_auto_control/utils/xml/change_xml_structure/change_xml_structure.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/utils/xml/xml_file/xml_file.py` & `je_auto_control_dev-0.0.93/je_auto_control/utils/xml/xml_file/xml_file.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/windows/core/utils/win32_ctype_input.py` & `je_auto_control_dev-0.0.93/je_auto_control/windows/core/utils/win32_ctype_input.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/windows/core/utils/win32_keypress_check.py` & `je_auto_control_dev-0.0.93/je_auto_control/windows/core/utils/win32_keypress_check.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/windows/core/utils/win32_vk.py` & `je_auto_control_dev-0.0.93/je_auto_control/windows/core/utils/win32_vk.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/windows/keyboard/win32_ctype_keyboard_control.py` & `je_auto_control_dev-0.0.93/je_auto_control/windows/keyboard/win32_ctype_keyboard_control.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/windows/listener/win32_keyboard_listener.py` & `je_auto_control_dev-0.0.93/je_auto_control/windows/listener/win32_keyboard_listener.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/windows/listener/win32_mouse_listener.py` & `je_auto_control_dev-0.0.93/je_auto_control/windows/listener/win32_mouse_listener.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/windows/mouse/win32_ctype_mouse_control.py` & `je_auto_control_dev-0.0.93/je_auto_control/windows/mouse/win32_ctype_mouse_control.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/windows/record/win32_record.py` & `je_auto_control_dev-0.0.93/je_auto_control/windows/record/win32_record.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/windows/screen/win32_screen.py` & `je_auto_control_dev-0.0.93/je_auto_control/windows/screen/win32_screen.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/wrapper/auto_control_image.py` & `je_auto_control_dev-0.0.93/je_auto_control/wrapper/auto_control_image.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/wrapper/auto_control_keyboard.py` & `je_auto_control_dev-0.0.93/je_auto_control/wrapper/auto_control_keyboard.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/wrapper/auto_control_mouse.py` & `je_auto_control_dev-0.0.93/je_auto_control/wrapper/auto_control_mouse.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/wrapper/auto_control_record.py` & `je_auto_control_dev-0.0.93/je_auto_control/wrapper/auto_control_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             raise AutoControlException(macos_record_error)
         action_queue = recorder.stop_record()
         if action_queue is None:
             raise AutoControlJsonActionException
         action_list = list(action_queue.queue)
         new_list = list()
         for action in action_list:
-            if action[0] == "type_keyboard":
+            if action[0] == "AC_type_keyboard":
                 new_list.append([action[0], dict([["keycode", action[1]]])])
             else:
                 new_list.append([action[0], dict(zip(["mouse_keycode", "x", "y"], [action[0], action[1], action[2]]))])
         record_action_to_list("stop_record", None)
         return new_list
     except Exception as error:
         record_action_to_list("stop_record", None, repr(error))
```

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/wrapper/auto_control_screen.py` & `je_auto_control_dev-0.0.93/je_auto_control/wrapper/auto_control_screen.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control/wrapper/platform_wrapper.py` & `je_auto_control_dev-0.0.93/je_auto_control/wrapper/platform_wrapper.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/je_auto_control_dev.egg-info/PKG-INFO` & `je_auto_control_dev-0.0.93/je_auto_control_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je-auto-control-dev
-Version: 0.0.92
+Version: 0.0.93
 Summary: GUI Automation Framework
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/AutoControl
 Project-URL: Documentation, https://autocontrol.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/AutoControl
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `je_auto_control_dev-0.0.92/je_auto_control_dev.egg-info/SOURCES.txt` & `je_auto_control_dev-0.0.93/je_auto_control_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.92/pyproject.toml` & `je_auto_control_dev-0.0.93/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is dev version
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "je_auto_control_dev"
-version = "0.0.92"
+version = "0.0.93"
 authors = [
     { name = "JE-Chen", email = "jechenmailman@gmail.com" },
 ]
 description = "GUI Automation Framework"
 requires-python = ">=3.8"
 license = { text = "MIT" }
 dependencies = [
```

