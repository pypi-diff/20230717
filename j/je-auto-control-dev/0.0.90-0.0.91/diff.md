# Comparing `tmp/je_auto_control_dev-0.0.90.tar.gz` & `tmp/je_auto_control_dev-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "je_auto_control_dev-0.0.90.tar", last modified: Mon Jul 17 03:48:04 2023, max compression
+gzip compressed data, was "je_auto_control_dev-0.0.91.tar", last modified: Mon Jul 17 06:32:56 2023, max compression
```

## Comparing `je_auto_control_dev-0.0.90.tar` & `je_auto_control_dev-0.0.91.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:04.022188 je_auto_control_dev-0.0.90/
--rw-rw-rw-   0        0        0     3780 2023-07-17 03:48:04.020430 je_auto_control_dev-0.0.90/PKG-INFO
--rw-rw-rw-   0        0        0     2975 2023-05-30 02:56:01.000000 je_auto_control_dev-0.0.90/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:02.595140 je_auto_control_dev-0.0.90/je_auto_control/
--rw-rw-rw-   0        0        0     6458 2023-06-01 01:55:14.000000 je_auto_control_dev-0.0.90/je_auto_control/__init__.py
--rw-rw-rw-   0        0        0     2355 2023-04-25 09:06:42.000000 je_auto_control_dev-0.0.90/je_auto_control/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:02.601478 je_auto_control_dev-0.0.90/je_auto_control/linux_with_x11/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/linux_with_x11/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:02.610519 je_auto_control_dev-0.0.90/je_auto_control/linux_with_x11/core/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/linux_with_x11/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:02.633971 je_auto_control_dev-0.0.90/je_auto_control/linux_with_x11/core/utils/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/linux_with_x11/core/utils/__init__.py
--rw-rw-rw-   0        0        0      467 2023-06-13 01:38:53.000000 je_auto_control_dev-0.0.90/je_auto_control/linux_with_x11/core/utils/x11_linux_display.py
--rw-rw-rw-   0        0        0    14539 2023-06-17 09:28:03.000000 je_auto_control_dev-0.0.90/je_auto_control/linux_with_x11/core/utils/x11_linux_vk.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:02.645502 je_auto_control_dev-0.0.90/je_auto_control/linux_with_x11/keyboard/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/linux_with_x11/keyboard/__init__.py
--rw-rw-rw-   0        0        0      828 2023-06-17 09:28:03.000000 je_auto_control_dev-0.0.90/je_auto_control/linux_with_x11/keyboard/x11_linux_keyboard_control.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:02.668084 je_auto_control_dev-0.0.90/je_auto_control/linux_with_x11/listener/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/linux_with_x11/listener/__init__.py
--rw-rw-rw-   0        0        0     5554 2023-06-13 01:38:29.000000 je_auto_control_dev-0.0.90/je_auto_control/linux_with_x11/listener/x11_linux_listener.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:02.688346 je_auto_control_dev-0.0.90/je_auto_control/linux_with_x11/mouse/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/linux_with_x11/mouse/__init__.py
--rw-rw-rw-   0        0        0     2393 2023-05-22 01:10:31.000000 je_auto_control_dev-0.0.90/je_auto_control/linux_with_x11/mouse/x11_linux_mouse_control.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:02.712673 je_auto_control_dev-0.0.90/je_auto_control/linux_with_x11/record/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/linux_with_x11/record/__init__.py
--rw-rw-rw-   0        0        0     1563 2023-04-10 02:15:44.000000 je_auto_control_dev-0.0.90/je_auto_control/linux_with_x11/record/x11_linux_record.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:02.729718 je_auto_control_dev-0.0.90/je_auto_control/linux_with_x11/screen/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/linux_with_x11/screen/__init__.py
--rw-rw-rw-   0        0        0      533 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/linux_with_x11/screen/x11_linux_screen.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:02.735720 je_auto_control_dev-0.0.90/je_auto_control/osx/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/osx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:02.754215 je_auto_control_dev-0.0.90/je_auto_control/osx/core/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/osx/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:02.837257 je_auto_control_dev-0.0.90/je_auto_control/osx/core/utils/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/osx/core/utils/__init__.py
--rw-rw-rw-   0        0        0     3157 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/osx/core/utils/osx_vk.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:02.877341 je_auto_control_dev-0.0.90/je_auto_control/osx/keyboard/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/osx/keyboard/__init__.py
--rw-rw-rw-   0        0        0     3017 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/osx/keyboard/osx_keyboard.py
--rw-rw-rw-   0        0        0      446 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/osx/keyboard/osx_keyboard_check.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:02.905392 je_auto_control_dev-0.0.90/je_auto_control/osx/listener/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/osx/listener/__init__.py
--rw-rw-rw-   0        0        0     1519 2023-04-10 02:15:44.000000 je_auto_control_dev-0.0.90/je_auto_control/osx/listener/osx_listener.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:02.918356 je_auto_control_dev-0.0.90/je_auto_control/osx/mouse/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/osx/mouse/__init__.py
--rw-rw-rw-   0        0        0     3500 2023-05-22 01:10:31.000000 je_auto_control_dev-0.0.90/je_auto_control/osx/mouse/osx_mouse.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:02.955895 je_auto_control_dev-0.0.90/je_auto_control/osx/record/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/osx/record/__init__.py
--rw-rw-rw-   0        0        0      957 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/osx/record/osx_record.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:02.997075 je_auto_control_dev-0.0.90/je_auto_control/osx/screen/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/osx/screen/__init__.py
--rw-rw-rw-   0        0        0      495 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/osx/screen/osx_screen.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:03.005307 je_auto_control_dev-0.0.90/je_auto_control/utils/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:03.030983 je_auto_control_dev-0.0.90/je_auto_control/utils/callback/
--rw-rw-rw-   0        0        0        0 2023-03-31 01:55:17.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/callback/__init__.py
--rw-rw-rw-   0        0        0     7800 2023-06-19 06:41:34.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/callback/callback_function_executor.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:03.043806 je_auto_control_dev-0.0.90/je_auto_control/utils/critical_exit/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/critical_exit/__init__.py
--rw-rw-rw-   0        0        0     1524 2023-04-10 02:15:44.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/critical_exit/critcal_exit.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:03.069705 je_auto_control_dev-0.0.90/je_auto_control/utils/exception/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/exception/__init__.py
--rw-rw-rw-   0        0        0     2870 2023-06-08 09:14:35.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0     1663 2023-03-31 02:15:20.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:03.091245 je_auto_control_dev-0.0.90/je_auto_control/utils/executor/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/executor/__init__.py
--rw-rw-rw-   0        0        0    10153 2023-07-17 03:36:53.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/executor/action_executor.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:03.110744 je_auto_control_dev-0.0.90/je_auto_control/utils/file_process/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/file_process/__init__.py
--rw-rw-rw-   0        0        0      758 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/file_process/get_dir_file_list.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:03.176454 je_auto_control_dev-0.0.90/je_auto_control/utils/generate_report/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/generate_report/__init__.py
--rw-rw-rw-   0        0        0     4975 2023-06-19 06:50:46.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/generate_report/generate_html_report.py
--rw-rw-rw-   0        0        0     3415 2023-06-19 08:53:36.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/generate_report/generate_json_report.py
--rw-rw-rw-   0        0        0     2114 2023-06-19 06:50:46.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/generate_report/generate_xml_report.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:03.262355 je_auto_control_dev-0.0.90/je_auto_control/utils/image/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/image/__init__.py
--rw-rw-rw-   0        0        0      532 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/image/screenshot.py
--rw-rw-rw-   0        0        0     1151 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/image/template_detection.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:03.288096 je_auto_control_dev-0.0.90/je_auto_control/utils/json/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/json/__init__.py
--rw-rw-rw-   0        0        0     1477 2023-06-19 06:56:53.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/json/json_file.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:03.330873 je_auto_control_dev-0.0.90/je_auto_control/utils/logging/
--rw-rw-rw-   0        0        0        0 2023-06-08 03:44:59.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/logging/__init__.py
--rw-rw-rw-   0        0        0      579 2023-06-12 07:11:50.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/logging/loggin_instance.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:03.371521 je_auto_control_dev-0.0.90/je_auto_control/utils/package_manager/
--rw-rw-rw-   0        0        0        0 2023-04-06 01:15:41.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/package_manager/__init__.py
--rw-rw-rw-   0        0        0     3644 2023-06-19 09:13:36.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/package_manager/package_manager_class.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:03.416747 je_auto_control_dev-0.0.90/je_auto_control/utils/project/
--rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/project/__init__.py
--rw-rw-rw-   0        0        0     3030 2023-06-13 06:53:21.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/project/create_project_structure.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:03.466962 je_auto_control_dev-0.0.90/je_auto_control/utils/project/template/
--rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/project/template/__init__.py
--rw-rw-rw-   0        0        0      639 2023-04-10 08:38:18.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/project/template/template_executor.py
--rw-rw-rw-   0        0        0     2517 2023-04-10 07:40:39.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/project/template/template_keyword.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:03.496265 je_auto_control_dev-0.0.90/je_auto_control/utils/scheduler/
--rw-rw-rw-   0        0        0        0 2023-05-31 01:17:46.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/scheduler/__init__.py
--rw-rw-rw-   0        0        0    11468 2023-07-17 02:27:57.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/scheduler/extend_apscheduler.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:03.517315 je_auto_control_dev-0.0.90/je_auto_control/utils/shell_process/
--rw-rw-rw-   0        0        0        0 2023-05-29 01:48:49.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/shell_process/__init__.py
--rw-rw-rw-   0        0        0     5226 2023-06-13 06:53:21.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/shell_process/shell_exec.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:03.536008 je_auto_control_dev-0.0.90/je_auto_control/utils/socket_server/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/socket_server/__init__.py
--rw-rw-rw-   0        0        0     2329 2023-06-19 07:21:50.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/socket_server/auto_control_socket_server.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:03.562482 je_auto_control_dev-0.0.90/je_auto_control/utils/start_exe/
--rw-rw-rw-   0        0        0        0 2023-05-29 01:48:49.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/start_exe/__init__.py
--rw-rw-rw-   0        0        0      822 2023-06-19 07:21:50.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/start_exe/start_another_process.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:03.588878 je_auto_control_dev-0.0.90/je_auto_control/utils/test_record/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/test_record/__init__.py
--rw-rw-rw-   0        0        0     1059 2023-06-13 06:39:14.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/test_record/record_test_class.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:03.627346 je_auto_control_dev-0.0.90/je_auto_control/utils/timeout/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/timeout/__init__.py
--rw-rw-rw-   0        0        0      659 2023-06-19 07:40:40.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/timeout/multiprocess_timeout.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:03.631877 je_auto_control_dev-0.0.90/je_auto_control/utils/xml/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/xml/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:03.644866 je_auto_control_dev-0.0.90/je_auto_control/utils/xml/change_xml_structure/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/xml/change_xml_structure/__init__.py
--rw-rw-rw-   0        0        0     2498 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/xml/change_xml_structure/change_xml_structure.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:03.660054 je_auto_control_dev-0.0.90/je_auto_control/utils/xml/xml_file/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/xml/xml_file/__init__.py
--rw-rw-rw-   0        0        0     2369 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/utils/xml/xml_file/xml_file.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:03.666857 je_auto_control_dev-0.0.90/je_auto_control/windows/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/windows/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:03.672553 je_auto_control_dev-0.0.90/je_auto_control/windows/core/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/windows/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:03.704821 je_auto_control_dev-0.0.90/je_auto_control/windows/core/utils/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/windows/core/utils/__init__.py
--rw-rw-rw-   0        0        0     2388 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/windows/core/utils/win32_ctype_input.py
--rw-rw-rw-   0        0        0      584 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/windows/core/utils/win32_keypress_check.py
--rw-rw-rw-   0        0        0     5810 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/windows/core/utils/win32_vk.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:03.734395 je_auto_control_dev-0.0.90/je_auto_control/windows/keyboard/
--rw-rw-rw-   0        0        0        4 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/windows/keyboard/__init__.py
--rw-rw-rw-   0        0        0     1259 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/windows/keyboard/win32_ctype_keyboard_control.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:03.780749 je_auto_control_dev-0.0.90/je_auto_control/windows/listener/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/windows/listener/__init__.py
--rw-rw-rw-   0        0        0     2538 2023-04-10 02:15:44.000000 je_auto_control_dev-0.0.90/je_auto_control/windows/listener/win32_keyboard_listener.py
--rw-rw-rw-   0        0        0     3065 2023-04-07 08:14:40.000000 je_auto_control_dev-0.0.90/je_auto_control/windows/listener/win32_mouse_listener.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:03.800486 je_auto_control_dev-0.0.90/je_auto_control/windows/mouse/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/windows/mouse/__init__.py
--rw-rw-rw-   0        0        0     4170 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/windows/mouse/win32_ctype_mouse_control.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:03.831203 je_auto_control_dev-0.0.90/je_auto_control/windows/record/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/windows/record/__init__.py
--rw-rw-rw-   0        0        0     2182 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/windows/record/win32_record.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:03.842923 je_auto_control_dev-0.0.90/je_auto_control/windows/screen/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/windows/screen/__init__.py
--rw-rw-rw-   0        0        0      568 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/windows/screen/win32_screen.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:03.910469 je_auto_control_dev-0.0.90/je_auto_control/wrapper/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.90/je_auto_control/wrapper/__init__.py
--rw-rw-rw-   0        0        0     8157 2023-06-13 03:21:38.000000 je_auto_control_dev-0.0.90/je_auto_control/wrapper/auto_control_image.py
--rw-rw-rw-   0        0        0    14111 2023-06-13 03:24:01.000000 je_auto_control_dev-0.0.90/je_auto_control/wrapper/auto_control_keyboard.py
--rw-rw-rw-   0        0        0    11484 2023-06-13 03:43:27.000000 je_auto_control_dev-0.0.90/je_auto_control/wrapper/auto_control_mouse.py
--rw-rw-rw-   0        0        0     1964 2023-06-13 03:46:16.000000 je_auto_control_dev-0.0.90/je_auto_control/wrapper/auto_control_record.py
--rw-rw-rw-   0        0        0     2445 2023-06-13 03:50:56.000000 je_auto_control_dev-0.0.90/je_auto_control/wrapper/auto_control_screen.py
--rw-rw-rw-   0        0        0    58693 2023-06-13 03:50:56.000000 je_auto_control_dev-0.0.90/je_auto_control/wrapper/platform_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:48:04.010896 je_auto_control_dev-0.0.90/je_auto_control_dev.egg-info/
--rw-rw-rw-   0        0        0     3780 2023-07-17 03:48:01.000000 je_auto_control_dev-0.0.90/je_auto_control_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5256 2023-07-17 03:48:02.000000 je_auto_control_dev-0.0.90/je_auto_control_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 03:48:01.000000 je_auto_control_dev-0.0.90/je_auto_control_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      124 2023-07-17 03:48:01.000000 je_auto_control_dev-0.0.90/je_auto_control_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-17 03:48:01.000000 je_auto_control_dev-0.0.90/je_auto_control_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1310 2023-07-17 03:47:26.000000 je_auto_control_dev-0.0.90/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-17 03:48:04.024198 je_auto_control_dev-0.0.90/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.389573 je_auto_control_dev-0.0.91/
+-rw-rw-rw-   0        0        0     3780 2023-07-17 06:32:56.386541 je_auto_control_dev-0.0.91/PKG-INFO
+-rw-rw-rw-   0        0        0     2975 2023-05-30 02:56:01.000000 je_auto_control_dev-0.0.91/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.727708 je_auto_control_dev-0.0.91/je_auto_control/
+-rw-rw-rw-   0        0        0     6485 2023-07-17 06:17:59.000000 je_auto_control_dev-0.0.91/je_auto_control/__init__.py
+-rw-rw-rw-   0        0        0     2355 2023-04-25 09:06:42.000000 je_auto_control_dev-0.0.91/je_auto_control/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.729669 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.734012 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/core/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.749915 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/core/utils/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/core/utils/__init__.py
+-rw-rw-rw-   0        0        0      386 2023-07-17 06:24:07.000000 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/core/utils/x11_linux_display.py
+-rw-rw-rw-   0        0        0    14539 2023-06-17 09:28:03.000000 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/core/utils/x11_linux_vk.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.760465 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/keyboard/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/keyboard/__init__.py
+-rw-rw-rw-   0        0        0      828 2023-06-17 09:28:03.000000 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/keyboard/x11_linux_keyboard_control.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.771489 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/listener/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/listener/__init__.py
+-rw-rw-rw-   0        0        0     5554 2023-06-13 01:38:29.000000 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/listener/x11_linux_listener.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.782654 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/mouse/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/mouse/__init__.py
+-rw-rw-rw-   0        0        0     2393 2023-05-22 01:10:31.000000 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/mouse/x11_linux_mouse_control.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.792177 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/record/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/record/__init__.py
+-rw-rw-rw-   0        0        0     1563 2023-04-10 02:15:44.000000 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/record/x11_linux_record.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.801459 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/screen/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/screen/__init__.py
+-rw-rw-rw-   0        0        0      533 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/screen/x11_linux_screen.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.805374 je_auto_control_dev-0.0.91/je_auto_control/osx/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/osx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.809923 je_auto_control_dev-0.0.91/je_auto_control/osx/core/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/osx/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.818642 je_auto_control_dev-0.0.91/je_auto_control/osx/core/utils/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/osx/core/utils/__init__.py
+-rw-rw-rw-   0        0        0     3157 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/osx/core/utils/osx_vk.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.840325 je_auto_control_dev-0.0.91/je_auto_control/osx/keyboard/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/osx/keyboard/__init__.py
+-rw-rw-rw-   0        0        0     3017 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/osx/keyboard/osx_keyboard.py
+-rw-rw-rw-   0        0        0      446 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/osx/keyboard/osx_keyboard_check.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.846347 je_auto_control_dev-0.0.91/je_auto_control/osx/listener/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/osx/listener/__init__.py
+-rw-rw-rw-   0        0        0     1519 2023-04-10 02:15:44.000000 je_auto_control_dev-0.0.91/je_auto_control/osx/listener/osx_listener.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.865160 je_auto_control_dev-0.0.91/je_auto_control/osx/mouse/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/osx/mouse/__init__.py
+-rw-rw-rw-   0        0        0     3500 2023-05-22 01:10:31.000000 je_auto_control_dev-0.0.91/je_auto_control/osx/mouse/osx_mouse.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.871215 je_auto_control_dev-0.0.91/je_auto_control/osx/record/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/osx/record/__init__.py
+-rw-rw-rw-   0        0        0      957 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/osx/record/osx_record.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.880905 je_auto_control_dev-0.0.91/je_auto_control/osx/screen/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/osx/screen/__init__.py
+-rw-rw-rw-   0        0        0      495 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/osx/screen/osx_screen.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.886801 je_auto_control_dev-0.0.91/je_auto_control/utils/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.898485 je_auto_control_dev-0.0.91/je_auto_control/utils/callback/
+-rw-rw-rw-   0        0        0        0 2023-03-31 01:55:17.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/callback/__init__.py
+-rw-rw-rw-   0        0        0     7800 2023-06-19 06:41:34.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/callback/callback_function_executor.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.910078 je_auto_control_dev-0.0.91/je_auto_control/utils/critical_exit/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/critical_exit/__init__.py
+-rw-rw-rw-   0        0        0     1524 2023-04-10 02:15:44.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/critical_exit/critcal_exit.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.930733 je_auto_control_dev-0.0.91/je_auto_control/utils/exception/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0     2870 2023-06-08 09:14:35.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0     1663 2023-03-31 02:15:20.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.937783 je_auto_control_dev-0.0.91/je_auto_control/utils/executor/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/executor/__init__.py
+-rw-rw-rw-   0        0        0    10153 2023-07-17 03:36:53.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/executor/action_executor.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.948454 je_auto_control_dev-0.0.91/je_auto_control/utils/file_process/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/file_process/__init__.py
+-rw-rw-rw-   0        0        0      758 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/file_process/get_dir_file_list.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.973847 je_auto_control_dev-0.0.91/je_auto_control/utils/generate_report/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/generate_report/__init__.py
+-rw-rw-rw-   0        0        0     4938 2023-07-17 06:30:47.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/generate_report/generate_html_report.py
+-rw-rw-rw-   0        0        0     3415 2023-06-19 08:53:36.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/generate_report/generate_json_report.py
+-rw-rw-rw-   0        0        0     2090 2023-07-17 06:31:02.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/generate_report/generate_xml_report.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:55.989705 je_auto_control_dev-0.0.91/je_auto_control/utils/image/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/image/__init__.py
+-rw-rw-rw-   0        0        0      532 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/image/screenshot.py
+-rw-rw-rw-   0        0        0     1151 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/image/template_detection.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.001425 je_auto_control_dev-0.0.91/je_auto_control/utils/json/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/json/__init__.py
+-rw-rw-rw-   0        0        0     1477 2023-06-19 06:56:53.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/json/json_file.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.012324 je_auto_control_dev-0.0.91/je_auto_control/utils/logging/
+-rw-rw-rw-   0        0        0        0 2023-06-08 03:44:59.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/logging/__init__.py
+-rw-rw-rw-   0        0        0      579 2023-06-12 07:11:50.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/logging/loggin_instance.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.022367 je_auto_control_dev-0.0.91/je_auto_control/utils/package_manager/
+-rw-rw-rw-   0        0        0        0 2023-04-06 01:15:41.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/package_manager/__init__.py
+-rw-rw-rw-   0        0        0     3644 2023-06-19 09:13:36.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/package_manager/package_manager_class.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.029467 je_auto_control_dev-0.0.91/je_auto_control/utils/project/
+-rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/project/__init__.py
+-rw-rw-rw-   0        0        0     3030 2023-06-13 06:53:21.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/project/create_project_structure.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.043968 je_auto_control_dev-0.0.91/je_auto_control/utils/project/template/
+-rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/project/template/__init__.py
+-rw-rw-rw-   0        0        0      639 2023-04-10 08:38:18.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/project/template/template_executor.py
+-rw-rw-rw-   0        0        0     2517 2023-04-10 07:40:39.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/project/template/template_keyword.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.056007 je_auto_control_dev-0.0.91/je_auto_control/utils/scheduler/
+-rw-rw-rw-   0        0        0        0 2023-05-31 01:17:46.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/scheduler/__init__.py
+-rw-rw-rw-   0        0        0    11468 2023-07-17 02:27:57.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/scheduler/extend_apscheduler.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.070593 je_auto_control_dev-0.0.91/je_auto_control/utils/shell_process/
+-rw-rw-rw-   0        0        0        0 2023-05-29 01:48:49.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/shell_process/__init__.py
+-rw-rw-rw-   0        0        0     5226 2023-06-13 06:53:21.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/shell_process/shell_exec.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.084372 je_auto_control_dev-0.0.91/je_auto_control/utils/socket_server/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/socket_server/__init__.py
+-rw-rw-rw-   0        0        0     2329 2023-06-19 07:21:50.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/socket_server/auto_control_socket_server.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.097568 je_auto_control_dev-0.0.91/je_auto_control/utils/start_exe/
+-rw-rw-rw-   0        0        0        0 2023-05-29 01:48:49.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/start_exe/__init__.py
+-rw-rw-rw-   0        0        0      822 2023-06-19 07:21:50.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/start_exe/start_another_process.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.116733 je_auto_control_dev-0.0.91/je_auto_control/utils/test_record/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/test_record/__init__.py
+-rw-rw-rw-   0        0        0     1059 2023-06-13 06:39:14.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/test_record/record_test_class.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.135830 je_auto_control_dev-0.0.91/je_auto_control/utils/timeout/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/timeout/__init__.py
+-rw-rw-rw-   0        0        0      659 2023-06-19 07:40:40.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/timeout/multiprocess_timeout.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.140362 je_auto_control_dev-0.0.91/je_auto_control/utils/xml/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/xml/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.151801 je_auto_control_dev-0.0.91/je_auto_control/utils/xml/change_xml_structure/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/xml/change_xml_structure/__init__.py
+-rw-rw-rw-   0        0        0     2498 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/xml/change_xml_structure/change_xml_structure.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.167512 je_auto_control_dev-0.0.91/je_auto_control/utils/xml/xml_file/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/xml/xml_file/__init__.py
+-rw-rw-rw-   0        0        0     2369 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/utils/xml/xml_file/xml_file.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.176416 je_auto_control_dev-0.0.91/je_auto_control/windows/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.183444 je_auto_control_dev-0.0.91/je_auto_control/windows/core/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.217914 je_auto_control_dev-0.0.91/je_auto_control/windows/core/utils/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/core/utils/__init__.py
+-rw-rw-rw-   0        0        0     2388 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/core/utils/win32_ctype_input.py
+-rw-rw-rw-   0        0        0      584 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/core/utils/win32_keypress_check.py
+-rw-rw-rw-   0        0        0     5804 2023-07-17 06:26:04.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/core/utils/win32_vk.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.234458 je_auto_control_dev-0.0.91/je_auto_control/windows/keyboard/
+-rw-rw-rw-   0        0        0        4 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/keyboard/__init__.py
+-rw-rw-rw-   0        0        0     1259 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/keyboard/win32_ctype_keyboard_control.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.249334 je_auto_control_dev-0.0.91/je_auto_control/windows/listener/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/listener/__init__.py
+-rw-rw-rw-   0        0        0     2538 2023-04-10 02:15:44.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/listener/win32_keyboard_listener.py
+-rw-rw-rw-   0        0        0     3065 2023-04-07 08:14:40.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/listener/win32_mouse_listener.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.264197 je_auto_control_dev-0.0.91/je_auto_control/windows/mouse/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/mouse/__init__.py
+-rw-rw-rw-   0        0        0     4170 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/mouse/win32_ctype_mouse_control.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.280430 je_auto_control_dev-0.0.91/je_auto_control/windows/record/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/record/__init__.py
+-rw-rw-rw-   0        0        0     2182 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/record/win32_record.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.294519 je_auto_control_dev-0.0.91/je_auto_control/windows/screen/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/screen/__init__.py
+-rw-rw-rw-   0        0        0      568 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/windows/screen/win32_screen.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.346670 je_auto_control_dev-0.0.91/je_auto_control/wrapper/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.91/je_auto_control/wrapper/__init__.py
+-rw-rw-rw-   0        0        0     8157 2023-06-13 03:21:38.000000 je_auto_control_dev-0.0.91/je_auto_control/wrapper/auto_control_image.py
+-rw-rw-rw-   0        0        0    14111 2023-06-13 03:24:01.000000 je_auto_control_dev-0.0.91/je_auto_control/wrapper/auto_control_keyboard.py
+-rw-rw-rw-   0        0        0    11484 2023-06-13 03:43:27.000000 je_auto_control_dev-0.0.91/je_auto_control/wrapper/auto_control_mouse.py
+-rw-rw-rw-   0        0        0     1957 2023-07-17 06:14:02.000000 je_auto_control_dev-0.0.91/je_auto_control/wrapper/auto_control_record.py
+-rw-rw-rw-   0        0        0     2433 2023-07-17 06:26:57.000000 je_auto_control_dev-0.0.91/je_auto_control/wrapper/auto_control_screen.py
+-rw-rw-rw-   0        0        0    58693 2023-06-13 03:50:56.000000 je_auto_control_dev-0.0.91/je_auto_control/wrapper/platform_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:32:56.382537 je_auto_control_dev-0.0.91/je_auto_control_dev.egg-info/
+-rw-rw-rw-   0        0        0     3780 2023-07-17 06:32:55.000000 je_auto_control_dev-0.0.91/je_auto_control_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5256 2023-07-17 06:32:55.000000 je_auto_control_dev-0.0.91/je_auto_control_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 06:32:55.000000 je_auto_control_dev-0.0.91/je_auto_control_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      124 2023-07-17 06:32:55.000000 je_auto_control_dev-0.0.91/je_auto_control_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-17 06:32:55.000000 je_auto_control_dev-0.0.91/je_auto_control_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1310 2023-07-17 06:31:28.000000 je_auto_control_dev-0.0.91/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-17 06:32:56.390583 je_auto_control_dev-0.0.91/setup.cfg
```

### Comparing `je_auto_control_dev-0.0.90/PKG-INFO` & `je_auto_control_dev-0.0.91/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je_auto_control_dev
-Version: 0.0.90
+Version: 0.0.91
 Summary: GUI Automation Framework
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/AutoControl
 Project-URL: Documentation, https://autocontrol.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/AutoControl
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `je_auto_control_dev-0.0.90/README.md` & `je_auto_control_dev-0.0.91/README.md`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/__init__.py` & `je_auto_control_dev-0.0.91/je_auto_control/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 # Scheduler
 from je_auto_control.utils.scheduler.extend_apscheduler import SchedulerManager
 
 __all__ = [
     "click_mouse", "mouse_keys_table", "get_mouse_position", "press_mouse", "release_mouse",
     "mouse_scroll", "set_mouse_position", "special_mouse_keys_table",
     "keyboard_keys_table", "press_keyboard_key", "release_keyboard_key", "type_keyboard", "check_key_is_press",
-    "write", "hotkey", "start_exe", "SchedulerManager",
+    "write", "hotkey", "start_exe", "SchedulerManager", "get_keyboard_keys_table",
     "screen_size", "screenshot", "locate_all_image", "locate_image_center", "locate_and_click",
     "CriticalExit", "AutoControlException", "AutoControlKeyboardException",
     "AutoControlMouseException", "AutoControlCantFindKeyException",
     "AutoControlScreenException", "ImageNotFoundException", "AutoControlJsonActionException",
     "AutoControlRecordException", "AutoControlActionNullException", "AutoControlActionException", "record",
     "stop_record", "read_action_json", "write_action_json", "execute_action", "execute_files", "executor",
     "add_command_to_executor", "multiprocess_timeout", "test_record_instance", "screenshot", "pil_screenshot",
```

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/__main__.py` & `je_auto_control_dev-0.0.91/je_auto_control/__main__.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/linux_with_x11/core/utils/x11_linux_vk.py` & `je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/core/utils/x11_linux_vk.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/linux_with_x11/keyboard/x11_linux_keyboard_control.py` & `je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/keyboard/x11_linux_keyboard_control.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/linux_with_x11/listener/x11_linux_listener.py` & `je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/listener/x11_linux_listener.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/linux_with_x11/mouse/x11_linux_mouse_control.py` & `je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/mouse/x11_linux_mouse_control.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/linux_with_x11/record/x11_linux_record.py` & `je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/record/x11_linux_record.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/linux_with_x11/screen/x11_linux_screen.py` & `je_auto_control_dev-0.0.91/je_auto_control/linux_with_x11/screen/x11_linux_screen.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/osx/core/utils/osx_vk.py` & `je_auto_control_dev-0.0.91/je_auto_control/osx/core/utils/osx_vk.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/osx/keyboard/osx_keyboard.py` & `je_auto_control_dev-0.0.91/je_auto_control/osx/keyboard/osx_keyboard.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/osx/listener/osx_listener.py` & `je_auto_control_dev-0.0.91/je_auto_control/osx/listener/osx_listener.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/osx/mouse/osx_mouse.py` & `je_auto_control_dev-0.0.91/je_auto_control/osx/mouse/osx_mouse.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/osx/record/osx_record.py` & `je_auto_control_dev-0.0.91/je_auto_control/osx/record/osx_record.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/utils/callback/callback_function_executor.py` & `je_auto_control_dev-0.0.91/je_auto_control/utils/callback/callback_function_executor.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/utils/critical_exit/critcal_exit.py` & `je_auto_control_dev-0.0.91/je_auto_control/utils/critical_exit/critcal_exit.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/utils/exception/exception_tags.py` & `je_auto_control_dev-0.0.91/je_auto_control/utils/exception/exception_tags.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/utils/exception/exceptions.py` & `je_auto_control_dev-0.0.91/je_auto_control/utils/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/utils/executor/action_executor.py` & `je_auto_control_dev-0.0.91/je_auto_control/utils/executor/action_executor.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/utils/file_process/get_dir_file_list.py` & `je_auto_control_dev-0.0.91/je_auto_control/utils/file_process/get_dir_file_list.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/utils/generate_report/generate_html_report.py` & `je_auto_control_dev-0.0.91/je_auto_control/utils/generate_report/generate_html_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import sys
-import typing
 from threading import Lock
 
 from je_auto_control.utils.exception.exception_tags import html_generate_no_data_tag
 from je_auto_control.utils.exception.exceptions import AutoControlHTMLException
 from je_auto_control.utils.logging.loggin_instance import auto_control_logger
 from je_auto_control.utils.test_record.record_test_class import test_record_instance
 
@@ -128,18 +126,16 @@
         ]
     )
     return event_str
 
 
 def generate_html() -> str:
     auto_control_logger.info("generate_html")
-    """
-    this function will create html string
-    :return: html_string
-    """
+    """ this function will create html string
+    :return: html_string """
     if len(test_record_instance.test_record_list) == 0:
         raise AutoControlHTMLException(html_generate_no_data_tag)
     else:
         event_str: str = ""
         for record_data in test_record_instance.test_record_list:
             # because data on record_data all is str
             if record_data.get("program_exception") == "None":
```

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/utils/generate_report/generate_json_report.py` & `je_auto_control_dev-0.0.91/je_auto_control/utils/generate_report/generate_json_report.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/utils/generate_report/generate_xml_report.py` & `je_auto_control_dev-0.0.91/je_auto_control/utils/generate_report/generate_xml_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from threading import Lock
+from typing import Tuple, Union
 from xml.dom.minidom import parseString
-from typing import Tuple, Dict, Union
 
 from je_auto_control.utils.generate_report.generate_json_report import generate_json
 from je_auto_control.utils.logging.loggin_instance import auto_control_logger
 from je_auto_control.utils.xml.change_xml_structure.change_xml_structure import dict_to_elements_tree
 
 
 def generate_xml() -> Tuple[Union[str, bytes], Union[str, bytes]]:
@@ -41,14 +41,13 @@
             f"failed: {repr(error)}")
     finally:
         lock.release()
     lock.acquire()
     try:
         with open(xml_file_name + "_success.xml", "w+") as file_to_write:
             file_to_write.write(success_xml)
-            pass
     except Exception as error:
         auto_control_logger.error(
             f"generate_xml_report, xml_file_name: {xml_file_name}, "
             f"failed: {repr(error)}")
     finally:
         lock.release()
```

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/utils/image/screenshot.py` & `je_auto_control_dev-0.0.91/je_auto_control/utils/image/screenshot.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/utils/image/template_detection.py` & `je_auto_control_dev-0.0.91/je_auto_control/utils/image/template_detection.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/utils/json/json_file.py` & `je_auto_control_dev-0.0.91/je_auto_control/utils/json/json_file.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/utils/logging/loggin_instance.py` & `je_auto_control_dev-0.0.91/je_auto_control/utils/logging/loggin_instance.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/utils/package_manager/package_manager_class.py` & `je_auto_control_dev-0.0.91/je_auto_control/utils/package_manager/package_manager_class.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/utils/project/create_project_structure.py` & `je_auto_control_dev-0.0.91/je_auto_control/utils/project/create_project_structure.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/utils/project/template/template_executor.py` & `je_auto_control_dev-0.0.91/je_auto_control/utils/project/template/template_executor.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/utils/project/template/template_keyword.py` & `je_auto_control_dev-0.0.91/je_auto_control/utils/project/template/template_keyword.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/utils/scheduler/extend_apscheduler.py` & `je_auto_control_dev-0.0.91/je_auto_control/utils/scheduler/extend_apscheduler.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/utils/shell_process/shell_exec.py` & `je_auto_control_dev-0.0.91/je_auto_control/utils/shell_process/shell_exec.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/utils/socket_server/auto_control_socket_server.py` & `je_auto_control_dev-0.0.91/je_auto_control/utils/socket_server/auto_control_socket_server.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/utils/start_exe/start_another_process.py` & `je_auto_control_dev-0.0.91/je_auto_control/utils/start_exe/start_another_process.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/utils/test_record/record_test_class.py` & `je_auto_control_dev-0.0.91/je_auto_control/utils/test_record/record_test_class.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/utils/timeout/multiprocess_timeout.py` & `je_auto_control_dev-0.0.91/je_auto_control/utils/timeout/multiprocess_timeout.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/utils/xml/change_xml_structure/change_xml_structure.py` & `je_auto_control_dev-0.0.91/je_auto_control/utils/xml/change_xml_structure/change_xml_structure.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/utils/xml/xml_file/xml_file.py` & `je_auto_control_dev-0.0.91/je_auto_control/utils/xml/xml_file/xml_file.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/windows/core/utils/win32_ctype_input.py` & `je_auto_control_dev-0.0.91/je_auto_control/windows/core/utils/win32_ctype_input.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/windows/core/utils/win32_keypress_check.py` & `je_auto_control_dev-0.0.91/je_auto_control/windows/core/utils/win32_keypress_check.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/windows/core/utils/win32_vk.py` & `je_auto_control_dev-0.0.91/je_auto_control/windows/core/utils/win32_vk.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 
 from je_auto_control.utils.exception.exception_tags import windows_import_error
 from je_auto_control.utils.exception.exceptions import AutoControlException
 
 if sys.platform not in ["win32", "cygwin", "msys"]:
     raise AutoControlException(windows_import_error)
 
-"""
-windows mouse virtual keycode
-"""
+# windows mouse virtual keycode
+
 
 win32_MOVE: int = 0x0001
 win32_LEFTDOWN: int = 0x0002
 win32_LEFTUP: int = 0x0004
 win32_RIGHTDOWN: int = 0x0008
 win32_RIGHTUP: int = 0x0010
 win32_MIDDLEDOWN: int = 0x0020
```

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/windows/keyboard/win32_ctype_keyboard_control.py` & `je_auto_control_dev-0.0.91/je_auto_control/windows/keyboard/win32_ctype_keyboard_control.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/windows/listener/win32_keyboard_listener.py` & `je_auto_control_dev-0.0.91/je_auto_control/windows/listener/win32_keyboard_listener.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/windows/listener/win32_mouse_listener.py` & `je_auto_control_dev-0.0.91/je_auto_control/windows/listener/win32_mouse_listener.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/windows/mouse/win32_ctype_mouse_control.py` & `je_auto_control_dev-0.0.91/je_auto_control/windows/mouse/win32_ctype_mouse_control.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/windows/record/win32_record.py` & `je_auto_control_dev-0.0.91/je_auto_control/windows/record/win32_record.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/windows/screen/win32_screen.py` & `je_auto_control_dev-0.0.91/je_auto_control/windows/screen/win32_screen.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/wrapper/auto_control_image.py` & `je_auto_control_dev-0.0.91/je_auto_control/wrapper/auto_control_image.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/wrapper/auto_control_keyboard.py` & `je_auto_control_dev-0.0.91/je_auto_control/wrapper/auto_control_keyboard.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/wrapper/auto_control_mouse.py` & `je_auto_control_dev-0.0.91/je_auto_control/wrapper/auto_control_mouse.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/wrapper/auto_control_record.py` & `je_auto_control_dev-0.0.91/je_auto_control/wrapper/auto_control_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     start record keyboard and mouse event until stop_record
     """
     auto_control_logger.info("record")
     try:
         if sys.platform == "darwin":
             raise AutoControlException(macos_record_error)
         record_action_to_list("record", None)
-        return recorder.record()
+        recorder.record()
     except Exception as error:
         record_action_to_list("record", None, repr(error))
         auto_control_logger.error(f"record, failed: {repr(error)}")
 
 
 def stop_record() -> list:
     """
```

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/wrapper/auto_control_screen.py` & `je_auto_control_dev-0.0.91/je_auto_control/wrapper/auto_control_screen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import sys
 from typing import Tuple, List
 
 import cv2
 import numpy as np
 
 from je_auto_control.utils.exception.exception_tags import screen_get_size
 from je_auto_control.utils.exception.exception_tags import screen_screenshot
```

### Comparing `je_auto_control_dev-0.0.90/je_auto_control/wrapper/platform_wrapper.py` & `je_auto_control_dev-0.0.91/je_auto_control/wrapper/platform_wrapper.py`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/je_auto_control_dev.egg-info/PKG-INFO` & `je_auto_control_dev-0.0.91/je_auto_control_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je-auto-control-dev
-Version: 0.0.90
+Version: 0.0.91
 Summary: GUI Automation Framework
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/AutoControl
 Project-URL: Documentation, https://autocontrol.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/AutoControl
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `je_auto_control_dev-0.0.90/je_auto_control_dev.egg-info/SOURCES.txt` & `je_auto_control_dev-0.0.91/je_auto_control_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `je_auto_control_dev-0.0.90/pyproject.toml` & `je_auto_control_dev-0.0.91/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is dev version
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "je_auto_control_dev"
-version = "0.0.90"
+version = "0.0.91"
 authors = [
     { name = "JE-Chen", email = "jechenmailman@gmail.com" },
 ]
 description = "GUI Automation Framework"
 requires-python = ">=3.8"
 license = { text = "MIT" }
 dependencies = [
```

