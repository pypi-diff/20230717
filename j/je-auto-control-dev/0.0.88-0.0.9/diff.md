# Comparing `tmp/je_auto_control_dev-0.0.88.tar.gz` & `tmp/je_auto_control_dev-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "je_auto_control_dev-0.0.88.tar", last modified: Mon Jul 17 02:32:51 2023, max compression
+gzip compressed data, was "dist\je_auto_control_dev-0.0.9.tar", last modified: Sat Mar 26 16:27:30 2022, max compression
```

## Comparing `je_auto_control_dev-0.0.88.tar` & `je_auto_control_dev-0.0.9.tar`

### file list

```diff
@@ -1,162 +1,120 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.628442 je_auto_control_dev-0.0.88/
--rw-rw-rw-   0        0        0     3780 2023-07-17 02:32:51.623352 je_auto_control_dev-0.0.88/PKG-INFO
--rw-rw-rw-   0        0        0     2975 2023-05-30 02:56:01.000000 je_auto_control_dev-0.0.88/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:50.991127 je_auto_control_dev-0.0.88/je_auto_control/
--rw-rw-rw-   0        0        0     6458 2023-06-01 01:55:14.000000 je_auto_control_dev-0.0.88/je_auto_control/__init__.py
--rw-rw-rw-   0        0        0     2355 2023-04-25 09:06:42.000000 je_auto_control_dev-0.0.88/je_auto_control/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:50.993164 je_auto_control_dev-0.0.88/je_auto_control/linux_with_x11/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/linux_with_x11/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:50.996199 je_auto_control_dev-0.0.88/je_auto_control/linux_with_x11/core/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/linux_with_x11/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.014309 je_auto_control_dev-0.0.88/je_auto_control/linux_with_x11/core/utils/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/linux_with_x11/core/utils/__init__.py
--rw-rw-rw-   0        0        0      467 2023-06-13 01:38:53.000000 je_auto_control_dev-0.0.88/je_auto_control/linux_with_x11/core/utils/x11_linux_display.py
--rw-rw-rw-   0        0        0    14539 2023-06-17 09:28:03.000000 je_auto_control_dev-0.0.88/je_auto_control/linux_with_x11/core/utils/x11_linux_vk.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.022714 je_auto_control_dev-0.0.88/je_auto_control/linux_with_x11/keyboard/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/linux_with_x11/keyboard/__init__.py
--rw-rw-rw-   0        0        0      828 2023-06-17 09:28:03.000000 je_auto_control_dev-0.0.88/je_auto_control/linux_with_x11/keyboard/x11_linux_keyboard_control.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.036484 je_auto_control_dev-0.0.88/je_auto_control/linux_with_x11/listener/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/linux_with_x11/listener/__init__.py
--rw-rw-rw-   0        0        0     5554 2023-06-13 01:38:29.000000 je_auto_control_dev-0.0.88/je_auto_control/linux_with_x11/listener/x11_linux_listener.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.048138 je_auto_control_dev-0.0.88/je_auto_control/linux_with_x11/mouse/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/linux_with_x11/mouse/__init__.py
--rw-rw-rw-   0        0        0     2393 2023-05-22 01:10:31.000000 je_auto_control_dev-0.0.88/je_auto_control/linux_with_x11/mouse/x11_linux_mouse_control.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.062277 je_auto_control_dev-0.0.88/je_auto_control/linux_with_x11/record/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/linux_with_x11/record/__init__.py
--rw-rw-rw-   0        0        0     1563 2023-04-10 02:15:44.000000 je_auto_control_dev-0.0.88/je_auto_control/linux_with_x11/record/x11_linux_record.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.073375 je_auto_control_dev-0.0.88/je_auto_control/linux_with_x11/screen/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/linux_with_x11/screen/__init__.py
--rw-rw-rw-   0        0        0      533 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/linux_with_x11/screen/x11_linux_screen.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.078225 je_auto_control_dev-0.0.88/je_auto_control/osx/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/osx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.084311 je_auto_control_dev-0.0.88/je_auto_control/osx/core/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/osx/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.097437 je_auto_control_dev-0.0.88/je_auto_control/osx/core/utils/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/osx/core/utils/__init__.py
--rw-rw-rw-   0        0        0     3157 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/osx/core/utils/osx_vk.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.122098 je_auto_control_dev-0.0.88/je_auto_control/osx/keyboard/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/osx/keyboard/__init__.py
--rw-rw-rw-   0        0        0     3017 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/osx/keyboard/osx_keyboard.py
--rw-rw-rw-   0        0        0      446 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/osx/keyboard/osx_keyboard_check.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.131459 je_auto_control_dev-0.0.88/je_auto_control/osx/listener/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/osx/listener/__init__.py
--rw-rw-rw-   0        0        0     1519 2023-04-10 02:15:44.000000 je_auto_control_dev-0.0.88/je_auto_control/osx/listener/osx_listener.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.141543 je_auto_control_dev-0.0.88/je_auto_control/osx/mouse/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/osx/mouse/__init__.py
--rw-rw-rw-   0        0        0     3500 2023-05-22 01:10:31.000000 je_auto_control_dev-0.0.88/je_auto_control/osx/mouse/osx_mouse.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.153680 je_auto_control_dev-0.0.88/je_auto_control/osx/record/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/osx/record/__init__.py
--rw-rw-rw-   0        0        0      957 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/osx/record/osx_record.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.165271 je_auto_control_dev-0.0.88/je_auto_control/osx/screen/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/osx/screen/__init__.py
--rw-rw-rw-   0        0        0      495 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/osx/screen/osx_screen.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.171388 je_auto_control_dev-0.0.88/je_auto_control/utils/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.181368 je_auto_control_dev-0.0.88/je_auto_control/utils/callback/
--rw-rw-rw-   0        0        0        0 2023-03-31 01:55:17.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/callback/__init__.py
--rw-rw-rw-   0        0        0     7800 2023-06-19 06:41:34.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/callback/callback_function_executor.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.194360 je_auto_control_dev-0.0.88/je_auto_control/utils/critical_exit/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/critical_exit/__init__.py
--rw-rw-rw-   0        0        0     1524 2023-04-10 02:15:44.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/critical_exit/critcal_exit.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.216346 je_auto_control_dev-0.0.88/je_auto_control/utils/exception/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/exception/__init__.py
--rw-rw-rw-   0        0        0     2870 2023-06-08 09:14:35.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0     1663 2023-03-31 02:15:20.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.226555 je_auto_control_dev-0.0.88/je_auto_control/utils/executor/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/executor/__init__.py
--rw-rw-rw-   0        0        0     9446 2023-07-17 02:28:39.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/executor/action_executor.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.237670 je_auto_control_dev-0.0.88/je_auto_control/utils/file_process/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/file_process/__init__.py
--rw-rw-rw-   0        0        0      758 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/file_process/get_dir_file_list.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.267291 je_auto_control_dev-0.0.88/je_auto_control/utils/generate_report/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/generate_report/__init__.py
--rw-rw-rw-   0        0        0     4975 2023-06-19 06:50:46.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/generate_report/generate_html_report.py
--rw-rw-rw-   0        0        0     3415 2023-06-19 08:53:36.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/generate_report/generate_json_report.py
--rw-rw-rw-   0        0        0     2114 2023-06-19 06:50:46.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/generate_report/generate_xml_report.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.286311 je_auto_control_dev-0.0.88/je_auto_control/utils/image/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/image/__init__.py
--rw-rw-rw-   0        0        0      532 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/image/screenshot.py
--rw-rw-rw-   0        0        0     1151 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/image/template_detection.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.291832 je_auto_control_dev-0.0.88/je_auto_control/utils/json/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/json/__init__.py
--rw-rw-rw-   0        0        0     1477 2023-06-19 06:56:53.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/json/json_file.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.300937 je_auto_control_dev-0.0.88/je_auto_control/utils/logging/
--rw-rw-rw-   0        0        0        0 2023-06-08 03:44:59.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/logging/__init__.py
--rw-rw-rw-   0        0        0      579 2023-06-12 07:11:50.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/logging/loggin_instance.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.308176 je_auto_control_dev-0.0.88/je_auto_control/utils/package_manager/
--rw-rw-rw-   0        0        0        0 2023-04-06 01:15:41.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/package_manager/__init__.py
--rw-rw-rw-   0        0        0     3644 2023-06-19 09:13:36.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/package_manager/package_manager_class.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.318829 je_auto_control_dev-0.0.88/je_auto_control/utils/project/
--rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/project/__init__.py
--rw-rw-rw-   0        0        0     3030 2023-06-13 06:53:21.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/project/create_project_structure.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.332858 je_auto_control_dev-0.0.88/je_auto_control/utils/project/template/
--rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/project/template/__init__.py
--rw-rw-rw-   0        0        0      639 2023-04-10 08:38:18.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/project/template/template_executor.py
--rw-rw-rw-   0        0        0     2517 2023-04-10 07:40:39.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/project/template/template_keyword.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.345375 je_auto_control_dev-0.0.88/je_auto_control/utils/scheduler/
--rw-rw-rw-   0        0        0        0 2023-05-31 01:17:46.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/scheduler/__init__.py
--rw-rw-rw-   0        0        0    11468 2023-07-17 02:27:57.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/scheduler/extend_apscheduler.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.353199 je_auto_control_dev-0.0.88/je_auto_control/utils/shell_process/
--rw-rw-rw-   0        0        0        0 2023-05-29 01:48:49.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/shell_process/__init__.py
--rw-rw-rw-   0        0        0     5226 2023-06-13 06:53:21.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/shell_process/shell_exec.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.364462 je_auto_control_dev-0.0.88/je_auto_control/utils/socket_server/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/socket_server/__init__.py
--rw-rw-rw-   0        0        0     2329 2023-06-19 07:21:50.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/socket_server/auto_control_socket_server.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.372657 je_auto_control_dev-0.0.88/je_auto_control/utils/start_exe/
--rw-rw-rw-   0        0        0        0 2023-05-29 01:48:49.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/start_exe/__init__.py
--rw-rw-rw-   0        0        0      822 2023-06-19 07:21:50.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/start_exe/start_another_process.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.382169 je_auto_control_dev-0.0.88/je_auto_control/utils/test_record/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/test_record/__init__.py
--rw-rw-rw-   0        0        0     1059 2023-06-13 06:39:14.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/test_record/record_test_class.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.395518 je_auto_control_dev-0.0.88/je_auto_control/utils/timeout/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/timeout/__init__.py
--rw-rw-rw-   0        0        0      659 2023-06-19 07:40:40.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/timeout/multiprocess_timeout.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.401609 je_auto_control_dev-0.0.88/je_auto_control/utils/xml/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/xml/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.410589 je_auto_control_dev-0.0.88/je_auto_control/utils/xml/change_xml_structure/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/xml/change_xml_structure/__init__.py
--rw-rw-rw-   0        0        0     2498 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/xml/change_xml_structure/change_xml_structure.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.420585 je_auto_control_dev-0.0.88/je_auto_control/utils/xml/xml_file/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/xml/xml_file/__init__.py
--rw-rw-rw-   0        0        0     2369 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/utils/xml/xml_file/xml_file.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.428256 je_auto_control_dev-0.0.88/je_auto_control/windows/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/windows/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.433263 je_auto_control_dev-0.0.88/je_auto_control/windows/core/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/windows/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.460620 je_auto_control_dev-0.0.88/je_auto_control/windows/core/utils/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/windows/core/utils/__init__.py
--rw-rw-rw-   0        0        0     2388 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/windows/core/utils/win32_ctype_input.py
--rw-rw-rw-   0        0        0      584 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/windows/core/utils/win32_keypress_check.py
--rw-rw-rw-   0        0        0     5810 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/windows/core/utils/win32_vk.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.473609 je_auto_control_dev-0.0.88/je_auto_control/windows/keyboard/
--rw-rw-rw-   0        0        0        4 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/windows/keyboard/__init__.py
--rw-rw-rw-   0        0        0     1259 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/windows/keyboard/win32_ctype_keyboard_control.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.496220 je_auto_control_dev-0.0.88/je_auto_control/windows/listener/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/windows/listener/__init__.py
--rw-rw-rw-   0        0        0     2538 2023-04-10 02:15:44.000000 je_auto_control_dev-0.0.88/je_auto_control/windows/listener/win32_keyboard_listener.py
--rw-rw-rw-   0        0        0     3065 2023-04-07 08:14:40.000000 je_auto_control_dev-0.0.88/je_auto_control/windows/listener/win32_mouse_listener.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.504237 je_auto_control_dev-0.0.88/je_auto_control/windows/mouse/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/windows/mouse/__init__.py
--rw-rw-rw-   0        0        0     4170 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/windows/mouse/win32_ctype_mouse_control.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.518283 je_auto_control_dev-0.0.88/je_auto_control/windows/record/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/windows/record/__init__.py
--rw-rw-rw-   0        0        0     2182 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/windows/record/win32_record.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.530835 je_auto_control_dev-0.0.88/je_auto_control/windows/screen/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/windows/screen/__init__.py
--rw-rw-rw-   0        0        0      568 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/windows/screen/win32_screen.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.586372 je_auto_control_dev-0.0.88/je_auto_control/wrapper/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:06.000000 je_auto_control_dev-0.0.88/je_auto_control/wrapper/__init__.py
--rw-rw-rw-   0        0        0     8157 2023-06-13 03:21:38.000000 je_auto_control_dev-0.0.88/je_auto_control/wrapper/auto_control_image.py
--rw-rw-rw-   0        0        0    14111 2023-06-13 03:24:01.000000 je_auto_control_dev-0.0.88/je_auto_control/wrapper/auto_control_keyboard.py
--rw-rw-rw-   0        0        0    11484 2023-06-13 03:43:27.000000 je_auto_control_dev-0.0.88/je_auto_control/wrapper/auto_control_mouse.py
--rw-rw-rw-   0        0        0     1964 2023-06-13 03:46:16.000000 je_auto_control_dev-0.0.88/je_auto_control/wrapper/auto_control_record.py
--rw-rw-rw-   0        0        0     2445 2023-06-13 03:50:56.000000 je_auto_control_dev-0.0.88/je_auto_control/wrapper/auto_control_screen.py
--rw-rw-rw-   0        0        0    58693 2023-06-13 03:50:56.000000 je_auto_control_dev-0.0.88/je_auto_control/wrapper/platform_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:32:51.618475 je_auto_control_dev-0.0.88/je_auto_control_dev.egg-info/
--rw-rw-rw-   0        0        0     3780 2023-07-17 02:32:50.000000 je_auto_control_dev-0.0.88/je_auto_control_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5256 2023-07-17 02:32:50.000000 je_auto_control_dev-0.0.88/je_auto_control_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 02:32:50.000000 je_auto_control_dev-0.0.88/je_auto_control_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      124 2023-07-17 02:32:50.000000 je_auto_control_dev-0.0.88/je_auto_control_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-17 02:32:50.000000 je_auto_control_dev-0.0.88/je_auto_control_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1310 2023-07-17 02:32:28.000000 je_auto_control_dev-0.0.88/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-17 02:32:51.632438 je_auto_control_dev-0.0.88/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:30.000000 je_auto_control_dev-0.0.9/
+-rw-rw-rw-   0        0        0     1085 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1672 2022-03-26 16:27:30.000000 je_auto_control_dev-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1044 2022-03-20 19:17:34.000000 je_auto_control_dev-0.0.9/README.md
+-rw-rw-rw-   0        0        0     1120 2022-03-26 16:27:27.000000 je_auto_control_dev-0.0.9/dev_setup.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:29.000000 je_auto_control_dev-0.0.9/je_auto_control/
+-rw-rw-rw-   0        0        0     3079 2022-03-25 17:19:44.000000 je_auto_control_dev-0.0.9/je_auto_control/__init__.py
+-rw-rw-rw-   0        0        0      470 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/__main__.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:29.000000 je_auto_control_dev-0.0.9/je_auto_control/linux_with_x11/
+-rw-rw-rw-   0        0        0        0 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/linux_with_x11/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:29.000000 je_auto_control_dev-0.0.9/je_auto_control/linux_with_x11/core/
+-rw-rw-rw-   0        0        0        0 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/linux_with_x11/core/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:29.000000 je_auto_control_dev-0.0.9/je_auto_control/linux_with_x11/core/utils/
+-rw-rw-rw-   0        0        0       72 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/linux_with_x11/core/utils/__init__.py
+-rw-rw-rw-   0        0        0      389 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/linux_with_x11/core/utils/x11_linux_display.py
+-rw-rw-rw-   0        0        0    15472 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/linux_with_x11/core/utils/x11_linux_vk.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:29.000000 je_auto_control_dev-0.0.9/je_auto_control/linux_with_x11/keyboard/
+-rw-rw-rw-   0        0        0        0 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/linux_with_x11/keyboard/__init__.py
+-rw-rw-rw-   0        0        0     1015 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/linux_with_x11/keyboard/x11_linux_keyboard_control.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:29.000000 je_auto_control_dev-0.0.9/je_auto_control/linux_with_x11/listener/
+-rw-rw-rw-   0        0        0        0 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/linux_with_x11/listener/__init__.py
+-rw-rw-rw-   0        0        0     5651 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/linux_with_x11/listener/x11_linux_listener.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:29.000000 je_auto_control_dev-0.0.9/je_auto_control/linux_with_x11/mouse/
+-rw-rw-rw-   0        0        0        0 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/linux_with_x11/mouse/__init__.py
+-rw-rw-rw-   0        0        0     2267 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/linux_with_x11/mouse/x11_linux_mouse_control.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:29.000000 je_auto_control_dev-0.0.9/je_auto_control/linux_with_x11/record/
+-rw-rw-rw-   0        0        0        0 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/linux_with_x11/record/__init__.py
+-rw-rw-rw-   0        0        0     1761 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/linux_with_x11/record/x11_linux_record.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:29.000000 je_auto_control_dev-0.0.9/je_auto_control/linux_with_x11/screen/
+-rw-rw-rw-   0        0        0        0 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/linux_with_x11/screen/__init__.py
+-rw-rw-rw-   0        0        0      487 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/linux_with_x11/screen/x11_linux_screen.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:29.000000 je_auto_control_dev-0.0.9/je_auto_control/osx/
+-rw-rw-rw-   0        0        0        0 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/osx/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:29.000000 je_auto_control_dev-0.0.9/je_auto_control/osx/core/
+-rw-rw-rw-   0        0        0        2 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/osx/core/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:29.000000 je_auto_control_dev-0.0.9/je_auto_control/osx/core/utils/
+-rw-rw-rw-   0        0        0       55 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/osx/core/utils/__init__.py
+-rw-rw-rw-   0        0        0     3162 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/osx/core/utils/osx_vk.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:29.000000 je_auto_control_dev-0.0.9/je_auto_control/osx/keyboard/
+-rw-rw-rw-   0        0        0        2 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/osx/keyboard/__init__.py
+-rw-rw-rw-   0        0        0     2999 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/osx/keyboard/osx_keyboard.py
+-rw-rw-rw-   0        0        0      439 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/osx/keyboard/osx_keyboard_check.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:29.000000 je_auto_control_dev-0.0.9/je_auto_control/osx/listener/
+-rw-rw-rw-   0        0        0        0 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/osx/listener/__init__.py
+-rw-rw-rw-   0        0        0     1569 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/osx/listener/osx_listener.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:29.000000 je_auto_control_dev-0.0.9/je_auto_control/osx/mouse/
+-rw-rw-rw-   0        0        0        0 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/osx/mouse/__init__.py
+-rw-rw-rw-   0        0        0     3360 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/osx/mouse/osx_mouse.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:29.000000 je_auto_control_dev-0.0.9/je_auto_control/osx/record/
+-rw-rw-rw-   0        0        0        0 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/osx/record/__init__.py
+-rw-rw-rw-   0        0        0     1035 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/osx/record/osx_record.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:29.000000 je_auto_control_dev-0.0.9/je_auto_control/osx/screen/
+-rw-rw-rw-   0        0        0        0 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/osx/screen/__init__.py
+-rw-rw-rw-   0        0        0      449 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/osx/screen/osx_screen.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:29.000000 je_auto_control_dev-0.0.9/je_auto_control/utils/
+-rw-rw-rw-   0        0        0        2 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:29.000000 je_auto_control_dev-0.0.9/je_auto_control/utils/critical_exit/
+-rw-rw-rw-   0        0        0        2 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/utils/critical_exit/__init__.py
+-rw-rw-rw-   0        0        0     1466 2022-03-20 09:07:16.000000 je_auto_control_dev-0.0.9/je_auto_control/utils/critical_exit/critcal_exit.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:29.000000 je_auto_control_dev-0.0.9/je_auto_control/utils/exception/
+-rw-rw-rw-   0        0        0        2 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0     1967 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/utils/exception/exception_tag.py
+-rw-rw-rw-   0        0        0      892 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:29.000000 je_auto_control_dev-0.0.9/je_auto_control/utils/executor/
+-rw-rw-rw-   0        0        0        0 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/utils/executor/__init__.py
+-rw-rw-rw-   0        0        0     3466 2022-03-26 16:19:48.000000 je_auto_control_dev-0.0.9/je_auto_control/utils/executor/action_executor.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:29.000000 je_auto_control_dev-0.0.9/je_auto_control/utils/image/
+-rw-rw-rw-   0        0        0        0 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/utils/image/__init__.py
+-rw-rw-rw-   0        0        0      440 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/utils/image/screenshot.py
+-rw-rw-rw-   0        0        0     1092 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/utils/image/template_detection.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:29.000000 je_auto_control_dev-0.0.9/je_auto_control/utils/json/
+-rw-rw-rw-   0        0        0        0 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/utils/json/__init__.py
+-rw-rw-rw-   0        0        0     1390 2022-03-20 11:24:03.000000 je_auto_control_dev-0.0.9/je_auto_control/utils/json/json_file.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:29.000000 je_auto_control_dev-0.0.9/je_auto_control/utils/test_record/
+-rw-rw-rw-   0        0        0        0 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/utils/test_record/__init__.py
+-rw-rw-rw-   0        0        0      680 2022-03-26 15:30:37.000000 je_auto_control_dev-0.0.9/je_auto_control/utils/test_record/record_test_class.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:29.000000 je_auto_control_dev-0.0.9/je_auto_control/utils/timeout/
+-rw-rw-rw-   0        0        0        2 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/utils/timeout/__init__.py
+-rw-rw-rw-   0        0        0      640 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/utils/timeout/multiprocess_timeout.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:29.000000 je_auto_control_dev-0.0.9/je_auto_control/windows/
+-rw-rw-rw-   0        0        0        2 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/windows/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:29.000000 je_auto_control_dev-0.0.9/je_auto_control/windows/core/
+-rw-rw-rw-   0        0        0        2 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/windows/core/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:30.000000 je_auto_control_dev-0.0.9/je_auto_control/windows/core/utils/
+-rw-rw-rw-   0        0        0       59 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/windows/core/utils/__init__.py
+-rw-rw-rw-   0        0        0     2187 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/windows/core/utils/win32_ctype_input.py
+-rw-rw-rw-   0        0        0      566 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/windows/core/utils/win32_keypress_check.py
+-rw-rw-rw-   0        0        0     4979 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/windows/core/utils/win32_vk.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:30.000000 je_auto_control_dev-0.0.9/je_auto_control/windows/keyboard/
+-rw-rw-rw-   0        0        0        4 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/windows/keyboard/__init__.py
+-rw-rw-rw-   0        0        0     1209 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/windows/keyboard/win32_ctype_keyboard_control.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:30.000000 je_auto_control_dev-0.0.9/je_auto_control/windows/listener/
+-rw-rw-rw-   0        0        0        0 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/windows/listener/__init__.py
+-rw-rw-rw-   0        0        0     2632 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/windows/listener/win32_keyboard_listener.py
+-rw-rw-rw-   0        0        0     3154 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/windows/listener/win32_mouse_listener.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:30.000000 je_auto_control_dev-0.0.9/je_auto_control/windows/mouse/
+-rw-rw-rw-   0        0        0        0 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/windows/mouse/__init__.py
+-rw-rw-rw-   0        0        0     4098 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/windows/mouse/win32_ctype_mouse_control.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:30.000000 je_auto_control_dev-0.0.9/je_auto_control/windows/record/
+-rw-rw-rw-   0        0        0        2 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/windows/record/__init__.py
+-rw-rw-rw-   0        0        0     2246 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/windows/record/win32_record.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:30.000000 je_auto_control_dev-0.0.9/je_auto_control/windows/screen/
+-rw-rw-rw-   0        0        0       62 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/windows/screen/__init__.py
+-rw-rw-rw-   0        0        0      484 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/windows/screen/win32_screen.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:30.000000 je_auto_control_dev-0.0.9/je_auto_control/wrapper/
+-rw-rw-rw-   0        0        0        2 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/wrapper/__init__.py
+-rw-rw-rw-   0        0        0     5007 2022-03-26 15:03:54.000000 je_auto_control_dev-0.0.9/je_auto_control/wrapper/auto_control_image.py
+-rw-rw-rw-   0        0        0     7269 2022-03-26 16:22:17.000000 je_auto_control_dev-0.0.9/je_auto_control/wrapper/auto_control_keyboard.py
+-rw-rw-rw-   0        0        0     8077 2022-03-26 16:27:27.000000 je_auto_control_dev-0.0.9/je_auto_control/wrapper/auto_control_mouse.py
+-rw-rw-rw-   0        0        0     1757 2022-03-26 16:27:27.000000 je_auto_control_dev-0.0.9/je_auto_control/wrapper/auto_control_record.py
+-rw-rw-rw-   0        0        0     1533 2022-03-26 16:27:27.000000 je_auto_control_dev-0.0.9/je_auto_control/wrapper/auto_control_screen.py
+-rw-rw-rw-   0        0        0    58298 2022-03-19 16:29:14.000000 je_auto_control_dev-0.0.9/je_auto_control/wrapper/platform_wrapper.py
+drwxrwxrwx   0        0        0        0 2022-03-26 16:27:30.000000 je_auto_control_dev-0.0.9/je_auto_control_dev.egg-info/
+-rw-rw-rw-   0        0        0     1672 2022-03-26 16:27:29.000000 je_auto_control_dev-0.0.9/je_auto_control_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3681 2022-03-26 16:27:29.000000 je_auto_control_dev-0.0.9/je_auto_control_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-03-26 16:27:29.000000 je_auto_control_dev-0.0.9/je_auto_control_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2022-03-26 16:27:29.000000 je_auto_control_dev-0.0.9/je_auto_control_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2022-03-26 16:27:29.000000 je_auto_control_dev-0.0.9/je_auto_control_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-03-26 16:27:30.000000 je_auto_control_dev-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1112 2022-03-20 16:04:14.000000 je_auto_control_dev-0.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `je_auto_control_dev-0.0.88/je_auto_control/linux_with_x11/keyboard/x11_linux_keyboard_control.py` & `je_auto_control_dev-0.0.9/je_auto_control/linux_with_x11/keyboard/x11_linux_keyboard_control.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 import sys
 import time
 
-from je_auto_control.utils.exception.exception_tags import linux_import_error
 from je_auto_control.utils.exception.exceptions import AutoControlException
+from je_auto_control.utils.exception.exception_tag import linux_import_error
 
 if sys.platform not in ["linux", "linux2"]:
     raise AutoControlException(linux_import_error)
 
 from je_auto_control.linux_with_x11.core.utils.x11_linux_display import display
 from Xlib.ext.xtest import fake_input
 from Xlib import X
 
 
-def press_key(keycode: int) -> None:
+def press_key(keycode: int):
     """
     :param keycode which keycode we want to press
     """
-    time.sleep(0.01)
-    fake_input(display, X.KeyPress, keycode)
-    display.sync()
+    try:
+        time.sleep(0.01)
+        fake_input(display, X.KeyPress, keycode)
+        display.sync()
+    except struct.error as error:
+        print(repr(error), file=sys.stderr)
 
 
-def release_key(keycode: int) -> None:
+def release_key(keycode: int):
     """
     :param keycode which keycode we want to release
     """
-    time.sleep(0.01)
-    fake_input(display, X.KeyRelease, keycode)
-    display.sync()
+    try:
+        time.sleep(0.01)
+        fake_input(display, X.KeyRelease, keycode)
+        display.sync()
+    except struct.error as error:
+        print(repr(error), file=sys.stderr)
```

### Comparing `je_auto_control_dev-0.0.88/je_auto_control/linux_with_x11/listener/x11_linux_listener.py` & `je_auto_control_dev-0.0.9/je_auto_control/linux_with_x11/listener/x11_linux_listener.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import sys
-from queue import Queue
 
-from je_auto_control.utils.exception.exception_tags import linux_import_error
-from je_auto_control.utils.exception.exception_tags import listener_error
 from je_auto_control.utils.exception.exceptions import AutoControlException
+from je_auto_control.utils.exception.exception_tag import linux_import_error
+from je_auto_control.utils.exception.exception_tag import listener_error
+
 
 if sys.platform not in ["linux", "linux2"]:
     raise AutoControlException(linux_import_error)
 
+import Xlib.threaded
+
 from Xlib.display import Display
 from Xlib import X
 from Xlib.ext import record
 from Xlib.protocol import rq
 
 from threading import Thread
 
@@ -19,38 +21,38 @@
 current_display = Display()
 
 
 class KeypressHandler(Thread):
 
     def __init__(self, default_daemon: bool = True):
         """
-        default damon is true
+        setDaemon : default damon is true
         still listener : continue listener keycode ?
         event_key_code : now current key code default is 0
         """
         super().__init__()
-        self.daemon = default_daemon
+        self.setDaemon(default_daemon)
         self.still_listener = True
         self.record_flag = False
         self.record_queue = None
         self.event_keycode = 0
         self.event_position = 0, 0
 
     # two times because press and release
-    def check_is_press(self, keycode: int) -> bool:
+    def check_is_press(self, keycode: int):
         """
         :param keycode we want to check
         """
         if keycode == self.event_keycode:
             self.event_keycode = 0
             return True
         else:
             return False
 
-    def run(self, reply) -> None:
+    def run(self, reply):
         """
         :param reply listener return data
         get data
         while data not null and still listener
             get event
 
         """
@@ -64,48 +66,48 @@
                         self.event_position = event.root_x, event.root_y
                         if self.record_flag is True:
                             temp = (event.type, event.detail, event.root_x, event.root_y)
                             self.record_queue.put(temp)
         except AutoControlException:
             raise AutoControlException(listener_error)
 
-    def record(self, record_queue) -> None:
+    def record(self, record_queue):
         """
         :param record_queue the queue test_record action
         """
         self.record_flag = True
         self.record_queue = record_queue
 
-    def stop_record(self) -> Queue:
+    def stop_record(self):
         self.record_flag = False
         return self.record_queue
 
 
 class XWindowsKeypressListener(Thread):
 
     def __init__(self, default_daemon=True):
         """
         :param default_daemon default kill when program down
         create handler
         set root
         """
         super().__init__()
-        self.daemon = default_daemon
+        self.setDaemon(default_daemon)
         self.still_listener = True
         self.handler = KeypressHandler()
         self.root = current_display.screen().root
         self.context = None
 
-    def check_is_press(self, keycode: int) -> bool:
+    def check_is_press(self, keycode: int):
         """
         :param keycode check this keycode is press?
         """
         return self.handler.check_is_press(keycode)
 
-    def run(self) -> None:
+    def run(self):
         """
         while still listener
             get context
             set handler
             set test_record
             get event
         """
@@ -126,44 +128,52 @@
                             'errors': (0, 0),
                             'client_started': False,
                             'client_died': False,
                         }])
                     current_display.record_enable_context(self.context, self.handler.run)
                     current_display.record_free_context(self.context)
                 # keep running this to get event
-                self.root.display.next_event()
+                next_event = self.root.display.next_event()
             except AutoControlException:
                 raise AutoControlException(listener_error)
             finally:
                 self.handler.still_listener = False
                 self.still_listener = False
 
-    def record(self, record_queue) -> None:
+    def record(self, record_queue):
         self.handler.record(record_queue)
 
-    def stop_record(self) -> Queue:
+    def stop_record(self):
         return self.handler.stop_record()
 
 
 xwindows_listener = XWindowsKeypressListener()
 xwindows_listener.start()
 
 
-def check_key_is_press(keycode: int) -> bool:
+def check_key_is_press(keycode: int):
     """
     :param keycode check this keycode is press?
     """
     return xwindows_listener.check_is_press(keycode)
 
 
-def x11_linux_record(record_queue) -> None:
+def x11_linux_record(record_queue):
     """
     :param record_queue the queue test_record action
     """
     xwindows_listener.record(record_queue)
 
 
-def x11_linux_stop_record() -> Queue:
+def x11_linux_stop_record():
     """
     stop test_record action
     """
     return xwindows_listener.stop_record()
+
+
+if __name__ == "__main__":
+    from queue import Queue
+    test_queue = Queue()
+    xwindows_listener.record(test_queue)
+    while True:
+        pass
```

### Comparing `je_auto_control_dev-0.0.88/je_auto_control/linux_with_x11/mouse/x11_linux_mouse_control.py` & `je_auto_control_dev-0.0.9/je_auto_control/linux_with_x11/mouse/x11_linux_mouse_control.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import sys
 import time
-from typing import Tuple
 
-from je_auto_control.utils.exception.exception_tags import linux_import_error
 from je_auto_control.utils.exception.exceptions import AutoControlException
+from je_auto_control.utils.exception.exception_tag import linux_import_error
 
 if sys.platform not in ["linux", "linux2"]:
     raise AutoControlException(linux_import_error)
 
 from Xlib import X
 from Xlib.ext.xtest import fake_input
 
@@ -18,68 +17,67 @@
 x11_linux_mouse_right = 3
 x11_linux_scroll_direction_up = 4
 x11_linux_scroll_direction_down = 5
 x11_linux_scroll_direction_left = 6
 x11_linux_scroll_direction_right = 7
 
 
-def position() -> Tuple[int, int]:
+def position():
     """
     get mouse current position
     """
     coord = display.screen().root.query_pointer()._data
     return coord["root_x"], coord["root_y"]
 
 
-def set_position(x: int, y: int) -> None:
+def set_position(x: int, y: int):
     """
     :param x we want to set mouse x position
     :param y we want to set mouse y position
     """
     time.sleep(0.01)
     fake_input(display, X.MotionNotify, x=x, y=y)
     display.sync()
 
 
-def press_mouse(mouse_keycode: int) -> None:
+def press_mouse(mouse_keycode: int):
     """
     :param mouse_keycode mouse keycode we want to press
     """
     time.sleep(0.01)
     fake_input(display, X.ButtonPress, mouse_keycode)
     display.sync()
 
 
-def release_mouse(mouse_keycode: int) -> None:
+def release_mouse(mouse_keycode: int):
     """
     :param mouse_keycode which mouse keycode we want to release
     """
     time.sleep(0.01)
     fake_input(display, X.ButtonRelease, mouse_keycode)
     display.sync()
 
 
-def click_mouse(mouse_keycode: int, x=None, y=None) -> None:
+def click_mouse(mouse_keycode: int, x=None, y=None):
     """
     :param mouse_keycode which mouse keycode we want to click
     :param x set mouse x position
     :param y set mouse y position
     """
     if x and y is not None:
         set_position(x, y)
     press_mouse(mouse_keycode)
     release_mouse(mouse_keycode)
 
 
-def scroll(scroll_value: int, scroll_direction: int) -> None:
+def scroll(scroll_value: int, scroll_direction: int):
     """"
     :param scroll_value scroll unit
     :param scroll_direction what direction you want to scroll
     scroll_direction = 4 : direction up
     scroll_direction = 5 : direction down
     scroll_direction = 6 : direction left
     scroll_direction = 7 : direction right
     """
-    total = 0
     for i in range(scroll_value):
         click_mouse(scroll_direction)
-        total = total + i
+
```

### Comparing `je_auto_control_dev-0.0.88/je_auto_control/linux_with_x11/record/x11_linux_record.py` & `je_auto_control_dev-0.0.9/je_auto_control/linux_with_x11/record/x11_linux_record.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 import sys
-from typing import Any
 
-from je_auto_control.utils.exception.exception_tags import linux_import_error
 from je_auto_control.utils.exception.exceptions import AutoControlException
+from je_auto_control.utils.exception.exception_tag import linux_import_error
 
 if sys.platform not in ["linux", "linux2"]:
     raise AutoControlException(linux_import_error)
 
+from Xlib import X
+
 from je_auto_control.linux_with_x11.listener.x11_linux_listener import x11_linux_record
 from je_auto_control.linux_with_x11.listener.x11_linux_listener import x11_linux_stop_record
 
 from queue import Queue
 
-type_dict = {5: "mouse", 3: "type_keyboard"}
+type_dict = {5: "mouse", 3: "type_key"}
 detail_dict = {1: "mouse_left", 2: "mouse_middle", 3: "mouse_right"}
 
 
 class X11LinuxRecorder(object):
     """
     test_record controller
     """
-
     def __init__(self):
         self.record_queue = None
         self.result_queue = None
 
-    def record(self) -> None:
+    def record(self):
         """
         create a new queue and start test_record
         """
         self.record_queue = Queue()
         x11_linux_record(self.record_queue)
 
-    def stop_record(self) -> Queue[Any]:
+    def stop_record(self):
         """
         stop test_record
         make a format action queue
         """
         self.result_queue = x11_linux_stop_record()
         action_queue = Queue()
         for details in self.result_queue.queue:
@@ -44,7 +44,18 @@
                 action_queue.put((detail_dict.get(details[1]), details[2], details[3]))
             elif details[0] == 3:
                 action_queue.put((type_dict.get(details[0]), details[1]))
         return action_queue
 
 
 x11_linux_recoder = X11LinuxRecorder()
+
+
+if __name__ == "__main__":
+    x11_record = X11LinuxRecorder()
+    x11_record.record()
+    from time import sleep
+    sleep(10)
+    temp = x11_record.stop_record()
+    for action in temp.queue:
+        print(action)
+
```

### Comparing `je_auto_control_dev-0.0.88/je_auto_control/osx/core/utils/osx_vk.py` & `je_auto_control_dev-0.0.9/je_auto_control/osx/core/utils/osx_vk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import sys
 
-from je_auto_control.utils.exception.exception_tags import osx_import_error
+from je_auto_control.utils.exception.exception_tag import osx_import_error
 from je_auto_control.utils.exception.exceptions import AutoControlException
 
 if sys.platform not in ["darwin"]:
     raise AutoControlException(osx_import_error)
 
-# osx keyboard virtual keycode
-
+"""
+osx keyboard virtual keycode
+"""
 osx_key_a = osx_key_A = 0x00
 osx_key_s = osx_key_S = 0x01
 osx_key_d = osx_key_D = 0x02
 osx_key_f = osx_key_F = 0x03
 osx_key_h = osx_key_H = 0x04
 osx_key_g = osx_key_G = 0x05
 osx_key_z = osx_key_Z = 0x06
```

### Comparing `je_auto_control_dev-0.0.88/je_auto_control/osx/keyboard/osx_keyboard.py` & `je_auto_control_dev-0.0.9/je_auto_control/osx/keyboard/osx_keyboard.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import sys
 
-from je_auto_control.utils.exception.exception_tags import osx_import_error
+from je_auto_control.utils.exception.exception_tag import osx_import_error
 from je_auto_control.utils.exception.exceptions import AutoControlException
 
 if sys.platform not in ["darwin"]:
     raise AutoControlException(osx_import_error)
 
+import time
+
 import AppKit
 import Quartz
 
 from je_auto_control.osx.core.utils.osx_vk import osx_key_shift
 
 special_key_table = {
     "key_sound_up": 0,
@@ -35,15 +37,15 @@
     "key_rewind": 20,
     "key_illumination_up": 21,
     "key_illumination_down": 22,
     "key_illumination_toggle": 23,
 }
 
 
-def normal_key(keycode: int, is_shift: bool, is_down: bool) -> None:
+def normal_key(keycode: int, is_shift: bool, is_down: bool):
     """
     :param keycode which keycode we want to press or release
     :param is_shift use shift key ?
     :param is_down is_down true = press; false = release
     create event
     post event
     """
@@ -61,15 +63,15 @@
             is_down
         )
         Quartz.CGEventPost(Quartz.kCGHIDEventTap, event)
     except ValueError as error:
         print(repr(error), file=sys.stderr)
 
 
-def special_key(keycode: int, is_shift: bool) -> None:
+def special_key(keycode: int, is_shift: bool):
     """
     :param keycode which keycode we want to press or release
     :param is_shift use shift key ?
     create event
     post event
     """
     keycode = special_key_table[keycode]
@@ -83,26 +85,26 @@
         8,
         (keycode << 16) | ((0xa if is_shift else 0xb) << 8),
         -1
     )
     Quartz.CGEventPost(0, event)
 
 
-def press_key(keycode: int, is_shift: bool) -> None:
+def press_key(keycode: int, is_shift: bool):
     """
     :param keycode which keycode we want to press
     :param is_shift is shift press?
     """
     if keycode in special_key_table:
         special_key(keycode, is_shift)
     else:
         normal_key(keycode, is_shift, True)
 
 
-def release_key(keycode: int, is_shift: bool) -> None:
+def release_key(keycode: int, is_shift: bool):
     """
     :param keycode which keycode we want to release
     :param is_shift is shift press?
     """
     if keycode in special_key_table:
         special_key(keycode, is_shift)
     else:
```

### Comparing `je_auto_control_dev-0.0.88/je_auto_control/osx/listener/osx_listener.py` & `je_auto_control_dev-0.0.9/je_auto_control/osx/listener/osx_listener.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,61 @@
 import sys
 
-from je_auto_control.utils.exception.exception_tags import osx_import_error
+from je_auto_control.utils.exception.exception_tag import osx_import_error
 from je_auto_control.utils.exception.exceptions import AutoControlException
 
 if sys.platform not in ["darwin"]:
     raise AutoControlException(osx_import_error)
 
+
 from Cocoa import *
+import time
 from Foundation import *
 from PyObjCTools import AppHelper
 
 from queue import Queue
 
+
 record_queue = Queue()
 
 app = NSApplication.sharedApplication()
 
 
 class AppDelegate(NSObject):
     def applicationDidFinishLaunching_(self, aNotification):
         NSEvent.addGlobalMonitorForEventsMatchingMask_handler_(NSEventMaskKeyDown, keyboard_handler)
         NSEvent.addGlobalMonitorForEventsMatchingMask_handler_(NSEventMaskLeftMouseDown, mouse_left_handler)
         NSEvent.addGlobalMonitorForEventsMatchingMask_handler_(NSEventMaskRightMouseDown, mouse_right_handler)
 
 
-def mouse_left_handler(event) -> None:
+def mouse_left_handler(event):
     loc = NSEvent.mouseLocation()
     record_queue.put(("mouse_left", loc.x, loc.y))
 
 
-def mouse_right_handler(event) -> None:
+def mouse_right_handler(event):
     loc = NSEvent.mouseLocation()
     record_queue.put(("mouse_right", loc.x, loc.y))
 
 
-def keyboard_handler(event) -> None:
+def keyboard_handler(event):
     if int(event.keyCode()) == 98:
         pass
     else:
-        record_queue.put(("type_keyboard", int(hex(event.keyCode()), 16)))
+        record_queue.put(("type_key", int(hex(event.keyCode()), 16)))
         print(event)
 
 
-def osx_record() -> None:
+def osx_record():
+    record_queue = Queue()
     delegate = AppDelegate.alloc().init()
     app.setDelegate_(delegate)
     AppHelper.runEventLoop()
 
 
-def osx_stop_record() -> Queue:
+def osx_stop_record():
     return record_queue
+
+
+if __name__ == "__main__":
+    osx_record()
+
```

### Comparing `je_auto_control_dev-0.0.88/je_auto_control/osx/mouse/osx_mouse.py` & `je_auto_control_dev-0.0.9/je_auto_control/osx/mouse/osx_mouse.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,80 +1,80 @@
 import sys
-from typing import Tuple
 
-from je_auto_control.utils.exception.exception_tags import osx_import_error
+
+from je_auto_control.utils.exception.exception_tag import osx_import_error
 from je_auto_control.utils.exception.exceptions import AutoControlException
 
 if sys.platform not in ["darwin"]:
     raise AutoControlException(osx_import_error)
 
 import time
 
 import Quartz
 
 from je_auto_control.osx.core.utils.osx_vk import osx_mouse_left
 from je_auto_control.osx.core.utils.osx_vk import osx_mouse_middle
 from je_auto_control.osx.core.utils.osx_vk import osx_mouse_right
 
 
-def position() -> Tuple[int, int]:
+def position():
     """
     get mouse current position
     """
-    return Quartz.NSEvent.mouseLocation().x, Quartz.NSEvent.mouseLocation().y
+    return (Quartz.NSEvent.mouseLocation().x, Quartz.NSEvent.mouseLocation().y)
 
 
-def mouse_event(event, x: int, y: int, mouse_button: int) -> None:
+def mouse_event(event, x: int, y: int, mouse_button: int):
     """
     :param event which event we want to use
     :param x event x
     :param y event y
     :param mouse_button which mouse button will use event
     """
     curr_event = Quartz.CGEventCreateMouseEvent(None, event, (x, y), mouse_button)
     Quartz.CGEventPost(Quartz.kCGHIDEventTap, curr_event)
 
 
-def set_position(x: int, y: int) -> None:
+def set_position(x: int, y: int):
     """
     :param x we want to set mouse x position
     :param y we want to set mouse y position
     """
     mouse_event(Quartz.kCGEventMouseMoved, x, y, 0)
 
 
-def press_mouse(x: int, y: int, mouse_button: int) -> None:
+def press_mouse(x: int, y: int, mouse_button: int):
     """
     :param x event x
     :param y event y
     :param mouse_button which mouse button press
     """
     if mouse_button is osx_mouse_left:
         mouse_event(Quartz.kCGEventLeftMouseDown, x, y, Quartz.kCGMouseButtonLeft)
     elif mouse_button is osx_mouse_middle:
         mouse_event(Quartz.kCGEventOtherMouseDown, x, y, Quartz.kCGMouseButtonCenter)
     elif mouse_button is osx_mouse_right:
         mouse_event(Quartz.kCGEventRightMouseDown, x, y, Quartz.kCGMouseButtonRight)
 
 
-def release_mouse(x: int, y: int, mouse_button: int) -> None:
+def release_mouse(x: int, y: int, mouse_button: int):
     """
     :param x event x
     :param y event y
     :param mouse_button which mouse button release
     """
     if mouse_button is osx_mouse_left:
         mouse_event(Quartz.kCGEventLeftMouseUp, x, y, Quartz.kCGMouseButtonLeft)
     elif mouse_button is osx_mouse_middle:
         mouse_event(Quartz.kCGEventOtherMouseUp, x, y, Quartz.kCGMouseButtonCenter)
     elif mouse_button is osx_mouse_right:
         mouse_event(Quartz.kCGEventRightMouseUp, x, y, Quartz.kCGMouseButtonRight)
 
 
-def click_mouse(x: int, y: int, mouse_button: int) -> None:
+def click_mouse(x: int, y: int, mouse_button: int):
     """
     :param x event x
     :param y event y
     :param mouse_button which mouse button click
     """
     if mouse_button is osx_mouse_left:
         press_mouse(x, y, mouse_button)
@@ -86,22 +86,20 @@
         release_mouse(x, y, mouse_button)
     elif mouse_button is osx_mouse_right:
         press_mouse(x, y, mouse_button)
         time.sleep(.001)
         release_mouse(x, y, mouse_button)
 
 
-def scroll(scroll_value: int) -> None:
+def scroll(scroll_value: int):
     """
     :param scroll_value scroll count
     """
     scroll_value = int(scroll_value)
-    total = 0
     for do_scroll in range(abs(scroll_value)):
         scroll_event = Quartz.CGEventCreateScrollWheelEvent(
             None,
             0,
             1,
             1 if scroll_value >= 0 else -1
         )
         Quartz.CGEventPost(Quartz.kCGHIDEventTap, scroll_event)
-        total = total + do_scroll
```

### Comparing `je_auto_control_dev-0.0.88/je_auto_control/osx/record/osx_record.py` & `je_auto_control_dev-0.0.9/je_auto_control/osx/record/osx_record.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 import sys
-from queue import Queue
 
-from je_auto_control.utils.exception.exception_tags import osx_import_error
+
+from je_auto_control.utils.exception.exception_tag import osx_import_error
 from je_auto_control.utils.exception.exceptions import AutoControlException
 
 if sys.platform not in ["darwin"]:
     raise AutoControlException(osx_import_error)
 
 from je_auto_control.osx.listener.osx_listener import osx_record
 from je_auto_control.osx.listener.osx_listener import osx_stop_record
 
 from je_auto_control.utils.exception.exceptions import AutoControlJsonActionException
 
 
 class OSXRecorder(object):
 
-    def __init__(self):
-        self.record_flag = False
-
-    def record(self) -> None:
-        self.record_flag = True
+    def record(self):
         osx_record()
 
-    def stop_record(self) -> Queue:
+    def stop_record(self):
         record_queue = osx_stop_record()
-        self.record_flag = False
         if record_queue is None:
             raise AutoControlJsonActionException
         return osx_stop_record()
 
 
 osx_recorder = OSXRecorder()
+
+if __name__ == "__main__":
+    test_osx_recorder = OSXRecorder()
+    test_osx_recorder.record()
+    temp = test_osx_recorder.stop_record()
+    print(temp)
+    for action in temp.queue:
+        print(action)
+    while True:
+        pass
```

### Comparing `je_auto_control_dev-0.0.88/je_auto_control/utils/critical_exit/critcal_exit.py` & `je_auto_control_dev-0.0.9/je_auto_control/utils/critical_exit/critcal_exit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 import _thread
 import sys
 from threading import Thread
 
-from je_auto_control.wrapper.auto_control_keyboard import keyboard_keys_table
+from je_auto_control.wrapper.auto_control_keyboard import keys_table
 from je_auto_control.wrapper.platform_wrapper import keyboard_check
 
 
 class CriticalExit(Thread):
     """
     use to make program interrupt
     """
 
     def __init__(self, default_daemon: bool = True):
         """
         default interrupt is keyboard F7 key
         :param default_daemon bool thread setDaemon
         """
         super().__init__()
-        self.daemon = default_daemon
-        self._exit_check_key: int = keyboard_keys_table.get("f7")
+        self.setDaemon(default_daemon)
+        self._exit_check_key = keys_table.get("f7")
 
-    def set_critical_key(self, keycode: [int, str] = None) -> None:
+    def set_critical_key(self, keycode: [int, str] = None):
         """
         set interrupt key
         :param keycode interrupt key
         """
-        if isinstance(keycode, int):
+        if type(keycode) is int:
             self._exit_check_key = keycode
         else:
-            self._exit_check_key = keyboard_keys_table.get(keycode)
+            self._exit_check_key = keys_table.get(keycode)
 
-    def run(self) -> None:
+    def run(self):
         """
         listener keycode _exit_check_key to interrupt
         """
         try:
             while True:
                 if keyboard_check.check_key_is_press(self._exit_check_key):
                     _thread.interrupt_main()
         except Exception as error:
             print(repr(error), file=sys.stderr)
 
-    def init_critical_exit(self) -> None:
+    def init_critical_exit(self):
         """
         should only use this to start critical exit
         may this function will add more
         """
         critical_thread = self
         critical_thread.start()
```

### Comparing `je_auto_control_dev-0.0.88/je_auto_control/utils/exception/exception_tags.py` & `je_auto_control_dev-0.0.9/je_auto_control/utils/exception/exception_tag.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,63 +1,46 @@
 # error tags
-je_auto_control_error: str = "Auto control error"
-je_auto_control_critical_exit_error: str = "Auto control critical exit error"
+je_auto_control_error = "Auto control error"
+je_auto_control_critical_exit_error = "Auto control critical exit error"
 # os tags
-linux_import_error: str = "should be only loaded on linux"
-osx_import_error: str = "should be only loaded on MacOS"
-windows_import_error: str = "should be only loaded on windows"
-macos_record_error: str = "macos cant use recorder"
+linux_import_error = "should be only loaded on linux"
+osx_import_error = "should be only loaded on MacOS"
+windows_import_error = "should be only loaded on windows"
+macos_record_error = "macos can't use recorder"
 # keyboard tags
-keyboard_error: str = "Auto control keyboard error"
-keyboard_press_key: str = "keyboard press key error"
-keyboard_release_key: str = "keyboard release key error"
-keyboard_type_key: str = "keyboard type key error"
-keyboard_write: str = "keyboard write error"
-keyboard_write_cant_find: str = "keyboard write error cant find key"
-keyboard_hotkey: str = "keyboard hotkey error"
+keyboard_error = "Auto control keyboard error"
+keyboard_press_key = "keyboard press key error"
+keyboard_release_key = "keyboard release key error"
+keyboard_type_key = "keyboard type key error"
+keyboard_write = "keyboard write error"
+keyboard_write_cant_find = "keyboard write error can't find key"
+keyboard_hotkey = "keyboard hotkey error"
 # mouse tags
-mouse_error: str = "Auto control mouse error"
-mouse_get_position: str = "mouse get position error"
-mouse_set_position: str = "mouse set position error"
-mouse_press_mouse: str = "mouse press mouse error"
-mouse_release_mouse: str = "mouse release key error"
-mouse_click_mouse: str = "mouse click mouse error"
-mouse_scroll: str = "mouse scroll error"
-mouse_wrong_value: str = "mouse value error"
+mouse_error = "Auto control mouse error"
+mouse_get_position = "mouse get position error"
+mouse_set_position = "mouse set position error"
+mouse_press_mouse = "mouse press mouse error"
+mouse_release_mouse = "mouse release key error"
+mouse_click_mouse = "mouse click mouse error"
+mouse_scroll = "mouse scroll error"
+mouse_wrong_value = "mouse value error"
 # screen tags
-screen_error: str = "Auto control screen error"
-screen_get_size: str = "screen get size error"
-screen_screenshot: str = "screen screenshot error"
+screen_error = "Auto control screen error"
+screen_get_size = "screen get size error"
+screen_screenshot = "screen screenshot error"
 # table tags
-table_cant_find_key: str = "cant find key error"
+table_cant_find_key = "can't find key error"
 # image tags
-cant_find_image: str = "cant find image"
-find_image_error_variable: str = "variable error"
+cant_find_image = "can't find image"
+find_image_error_variable = "variable error"
 # listener tags
-listener_error: str = "Auto control listener error"
+listener_error = "Auto control listener error"
 # test_record tags
-record_queue_error: str = "cant get test_record queue its none are you using stop test_record before test_record"
-record_not_found_action_error: str = "test_record action not found"
-# json tag
-cant_execute_action_error: str = "cant execute action"
-cant_generate_json_report: str = "can't generate json report"
-cant_find_json_error: str = "cant find json file"
-cant_save_json_error: str = "cant save json file"
-action_is_null_error: str = "json action is null"
+record_queue_error = "can't get test_record queue it's none are you using stop test_record before test_record"
+record_not_found_action_error = "test_record action not found"
+# json action file tag
+cant_execute_action_error = "can't execute action"
+cant_find_json_error = "can't find json file"
+cant_save_json_error = "can't save json file"
+action_is_null_error = "json action is null"
 # timeout tag
-timeout_need_on_main_error: str = "should put timeout function on main"
-# HTML
-html_generate_no_data_tag: str = "record is None"
-# add command
-add_command_exception: str = "command value type should be as method or function"
-# executor
-executor_list_error: str = "executor receive wrong data list is none or wrong type"
-# argparse
-argparse_get_wrong_data: str = "argparse receive wrong data"
-# XML
-cant_read_xml_error: str = "can't read xml"
-xml_type_error: str = "xml type error"
-# Callback executor
-get_bad_trigger_method: str = "get bad trigger method, only accept kwargs and args"
-get_bad_trigger_function: str = "get bad trigger function only accept function in event_dict"
-# Can't find file
-can_not_find_file: str = "Can not find file"
+timeout_need_on_main_error = "should put timeout function on main"
```

### Comparing `je_auto_control_dev-0.0.88/je_auto_control/utils/exception/exceptions.py` & `je_auto_control_dev-0.0.9/je_auto_control/utils/exception/exceptions.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Keyboard
 
 
 class AutoControlKeyboardException(AutoControlException):
     pass
 
 
-class AutoControlCantFindKeyException(AutoControlKeyboardException):
+class AutoControlCantFindKeyException(AutoControlException):
     pass
 
 
 # Mouse
 
 
 class AutoControlMouseException(AutoControlException):
@@ -40,65 +40,23 @@
 
 class AutoControlRecordException(AutoControlException):
     pass
 
 
 # Execute action
 
-class AutoControlExecuteActionException(AutoControlException):
-    pass
-
-
-class AutoControlJsonActionException(AutoControlExecuteActionException):
-    pass
-
-
-class AutoControlActionNullException(AutoControlExecuteActionException):
-    pass
-
 
-class AutoControlActionException(AutoControlExecuteActionException):
+class AutoControlJsonActionException(AutoControlException):
     pass
 
 
-class AutoControlAddCommandException(AutoControlExecuteActionException):
+class AutoControlActionNullException(AutoControlException):
     pass
 
 
-class AutoControlArgparseException(AutoControlExecuteActionException):
+class AutoControlActionException(AutoControlException):
     pass
 
 
 # timeout
 class AutoControlTimeoutException(AutoControlException):
     pass
-
-
-# html exception
-
-class AutoControlHTMLException(AutoControlException):
-    pass
-
-
-# Json Exception
-
-class AutoControlJsonException(AutoControlException):
-    pass
-
-
-class AutoControlGenerateJsonReportException(AutoControlJsonException):
-    pass
-
-
-# XML
-
-class XMLException(AutoControlException):
-    pass
-
-
-class XMLTypeException(XMLException):
-    pass
-
-
-# Execute callback
-class CallbackExecutorException(AutoControlException):
-    pass
```

### Comparing `je_auto_control_dev-0.0.88/je_auto_control/utils/image/template_detection.py` & `je_auto_control_dev-0.0.9/je_auto_control/utils/image/template_detection.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-from typing import List
-
 from PIL import ImageGrab
 from je_open_cv import template_detection
 
 
-def find_image(image, detect_threshold: float = 1, draw_image: bool = False) -> List[int]:
+def find_image(image, detect_threshold: float = 1, draw_image: bool = False):
     """
     :param image which image we want to find on screen
     :param detect_threshold detect precision 0.0 ~ 1.0; 1 is absolute equal
     :param draw_image draw detect tag on return image
     """
     grab_image = ImageGrab.grab()
     return template_detection.find_object(image=grab_image, template=image,
                                           detect_threshold=detect_threshold, draw_image=draw_image)
 
 
-def find_image_multi(image, detect_threshold: float = 1, draw_image: bool = False) -> List[List[int]]:
+def find_image_multi(image, detect_threshold: float = 1, draw_image: bool = False):
     """
     :param image which image we want to find on screen
     :param detect_threshold detect precision 0.0 ~ 1.0; 1 is absolute equal
     :param draw_image draw detect tag on return image
     """
     grab_image = ImageGrab.grab()
     return template_detection.find_multi_object(image=grab_image, template=image,
```

### Comparing `je_auto_control_dev-0.0.88/je_auto_control/utils/json/json_file.py` & `je_auto_control_dev-0.0.9/je_auto_control/utils/json/json_file.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 import json
 from pathlib import Path
 from threading import Lock
-from typing import List, Dict
 
-from je_auto_control.utils.exception.exception_tags import cant_find_json_error
-from je_auto_control.utils.exception.exception_tags import cant_save_json_error
 from je_auto_control.utils.exception.exceptions import AutoControlJsonActionException
+from je_auto_control.utils.exception.exception_tag import cant_save_json_error
+from je_auto_control.utils.exception.exception_tag import cant_find_json_error
 
-_lock = Lock()
+lock = Lock()
 
 
-def read_action_json(json_file_path: str) -> List[List[Dict[str, Dict[str, str]]]]:
+def read_action_json(json_file_path: str):
     """
     use to read action file
     :param json_file_path json file's path to read
     """
-    _lock.acquire()
     try:
+        lock.acquire()
         file_path = Path(json_file_path)
         if file_path.exists() and file_path.is_file():
             with open(json_file_path) as read_file:
                 return json.loads(read_file.read())
     except AutoControlJsonActionException:
         raise AutoControlJsonActionException(cant_find_json_error)
     finally:
-        _lock.release()
+        lock.release()
 
 
-def write_action_json(json_save_path: str, action_json: list) -> None:
+def write_action_json(json_save_path: str, action_json: list):
     """
     use to save action file
     :param json_save_path  json save path
     :param action_json the json str include action to write
     """
-    _lock.acquire()
     try:
+        lock.acquire()
         with open(json_save_path, "w+") as file_to_write:
-            file_to_write.write(json.dumps(action_json, indent=4))
+            file_to_write.write(json.dumps(action_json))
     except AutoControlJsonActionException:
         raise AutoControlJsonActionException(cant_save_json_error)
     finally:
-        _lock.release()
+        lock.release()
+
```

### Comparing `je_auto_control_dev-0.0.88/je_auto_control/utils/timeout/multiprocess_timeout.py` & `je_auto_control_dev-0.0.9/je_auto_control/utils/timeout/multiprocess_timeout.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from multiprocessing import Process
-
-from je_auto_control.utils.exception.exception_tags import timeout_need_on_main_error
 from je_auto_control.utils.exception.exceptions import AutoControlTimeoutException
+from je_auto_control.utils.exception.exception_tag import timeout_need_on_main_error
 
 
-def multiprocess_timeout(check_function, time: int) -> str:
+def multiprocess_timeout(check_function, time: int):
     try:
-        new_process: Process = Process(target=check_function)
+        new_process = Process(target=check_function)
         new_process.start()
         new_process.join(timeout=time)
     except AutoControlTimeoutException:
         raise AutoControlTimeoutException(timeout_need_on_main_error)
     new_process.terminate()
     if new_process.exitcode is None:
         return "timeout"
```

### Comparing `je_auto_control_dev-0.0.88/je_auto_control/windows/core/utils/win32_ctype_input.py` & `je_auto_control_dev-0.0.9/je_auto_control/windows/core/utils/win32_ctype_input.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,72 +1,74 @@
 import sys
 
-from je_auto_control.utils.exception.exception_tags import windows_import_error
+from je_auto_control.utils.exception.exception_tag import windows_import_error
 from je_auto_control.utils.exception.exceptions import AutoControlException
 
 if sys.platform not in ["win32", "cygwin", "msys"]:
     raise AutoControlException(windows_import_error)
 
 import ctypes
 from ctypes import wintypes
-from je_auto_control.windows.core.utils.win32_vk import win32_EventF_UNICODE, win32_VkToVSC
+from ctypes import windll
+from je_auto_control.windows.core.utils.win32_vk import *
 
 user32 = ctypes.WinDLL('user32', use_last_error=True)
 
 wintypes.ULONG_PTR = wintypes.WPARAM
 
-Mouse: int = 0
-Keyboard: int = 1
-Hardware: int = 2
+Mouse = 0
+Keyboard = 1
+Hardware = 2
 
 
 class MouseInput(ctypes.Structure):
-    _fields_: tuple = (("dx", wintypes.LONG),
-                       ("dy", wintypes.LONG),
-                       ("mouseData", wintypes.DWORD),
-                       ("dwFlags", wintypes.DWORD),
-                       ("time", wintypes.DWORD),
-                       ("dwExtraInfo", ctypes.c_void_p))
+    _fields_ = (("dx", wintypes.LONG),
+                ("dy", wintypes.LONG),
+                ("mouseData", wintypes.DWORD),
+                ("dwFlags", wintypes.DWORD),
+                ("time", wintypes.DWORD),
+                ("dwExtraInfo", ctypes.c_void_p))
 
 
 class KeyboardInput(ctypes.Structure):
-    _fields_: tuple = (("wVk", wintypes.WORD),
-                       ("wScan", wintypes.WORD),
-                       ("dwFlags", wintypes.DWORD),
-                       ("time", wintypes.DWORD),
-                       ("dwExtraInfo", ctypes.c_void_p))
+    _fields_ = (("wVk", wintypes.WORD),
+                ("wScan", wintypes.WORD),
+                ("dwFlags", wintypes.DWORD),
+                ("time", wintypes.DWORD),
+                ("dwExtraInfo", ctypes.c_void_p))
 
     def __init__(self, *args, **kwds):
         super(KeyboardInput, self).__init__(*args, **kwds)
         if not self.dwFlags & win32_EventF_UNICODE:
             self.wScan = user32.MapVirtualKeyExW(self.wVk, win32_VkToVSC, 0)
 
 
 class HardwareInput(ctypes.Structure):
-    _fields_: tuple = (("uMsg", wintypes.DWORD),
-                       ("wParamL", wintypes.WORD),
-                       ("wParamH", wintypes.WORD))
+    _fields_ = (("uMsg", wintypes.DWORD),
+                ("wParamL", wintypes.WORD),
+                ("wParamH", wintypes.WORD))
 
 
 class Input(ctypes.Structure):
-    class INPUTUnion(ctypes.Union):
-        _fields_: tuple = (("ki", KeyboardInput),
-                           ("mi", MouseInput),
-                           ("hi", HardwareInput))
+    class INPUT_Union(ctypes.Union):
+        _fields_ = (("ki", KeyboardInput),
+                    ("mi", MouseInput),
+                    ("hi", HardwareInput))
 
-    _anonymous_: tuple = ("_input",)
-    _fields_: tuple = (("type", wintypes.DWORD),
-                       ("_input", INPUTUnion))
+    _anonymous_ = ("_input",)
+    _fields_ = (("type", wintypes.DWORD),
+                ("_input", INPUT_Union))
 
 
-def _check_count(result, func, args) -> list:
+LPINPUT = ctypes.POINTER(Input)
+
+
+def _check_count(result, func, args):
     if result == 0:
         raise ctypes.WinError(ctypes.get_last_error())
     return args
 
 
-LPINPUT: ctypes.POINTER = ctypes.POINTER(Input)
-
-SendInput: user32.SendInput = user32.SendInput
+SendInput = user32.SendInput
 
 user32.SendInput.errcheck = _check_count
 user32.SendInput.arg_types = (wintypes.UINT, ctypes.c_void_p, ctypes.c_int)
```

### Comparing `je_auto_control_dev-0.0.88/je_auto_control/windows/core/utils/win32_keypress_check.py` & `je_auto_control_dev-0.0.9/je_auto_control/windows/core/utils/win32_keypress_check.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import sys
 
-from je_auto_control.utils.exception.exception_tags import windows_import_error
+from je_auto_control.utils.exception.exception_tag import windows_import_error
 from je_auto_control.utils.exception.exceptions import AutoControlException
 
 if sys.platform not in ["win32", "cygwin", "msys"]:
     raise AutoControlException(windows_import_error)
 
 import ctypes
 
 
-def check_key_is_press(keycode: [int, str]) -> bool:
-    if isinstance(keycode, int):
-        temp: int = ctypes.windll.user32.GetKeyState(keycode)
+def check_key_is_press(keycode: [int, str]):
+    if type(keycode) is int:
+        temp = ctypes.windll.user32.GetKeyState(keycode)
     else:
         temp = ctypes.windll.user32.GetKeyState(ord(keycode))
     if temp > 1:
         return True
     return False
```

### Comparing `je_auto_control_dev-0.0.88/je_auto_control/windows/keyboard/win32_ctype_keyboard_control.py` & `je_auto_control_dev-0.0.9/je_auto_control/windows/keyboard/win32_ctype_keyboard_control.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import sys
 
-from je_auto_control.utils.exception.exception_tags import windows_import_error
+from je_auto_control.utils.exception.exception_tag import windows_import_error
 from je_auto_control.utils.exception.exceptions import AutoControlException
 
 if sys.platform not in ["win32", "cygwin", "msys"]:
     raise AutoControlException(windows_import_error)
 
 from je_auto_control.windows.core.utils.win32_ctype_input import Input
 from je_auto_control.windows.core.utils.win32_ctype_input import Keyboard
 from je_auto_control.windows.core.utils.win32_ctype_input import KeyboardInput
 from je_auto_control.windows.core.utils.win32_ctype_input import SendInput
 from je_auto_control.windows.core.utils.win32_ctype_input import ctypes
-from je_auto_control.windows.core.utils.win32_vk import win32_EventF_KEYUP
+from je_auto_control.windows.core.utils.win32_ctype_input import win32_EventF_KEYUP
 
 
-def press_key(keycode: int) -> None:
+def press_key(keycode: int):
     """
     :param keycode which keycode we want to press
     """
-    keyboard = Input(type=Keyboard, ki=KeyboardInput(wVk=keycode))
-    SendInput(1, ctypes.byref(keyboard), ctypes.sizeof(keyboard))
+    x = Input(type=Keyboard, ki=KeyboardInput(wVk=keycode))
+    SendInput(1, ctypes.byref(x), ctypes.sizeof(x))
 
 
-def release_key(keycode: int) -> None:
+def release_key(keycode: int):
     """
     :param keycode which keycode we want to release
     """
-    keyboard = Input(type=Keyboard, ki=KeyboardInput(wVk=keycode, dwFlags=win32_EventF_KEYUP))
-    SendInput(1, ctypes.byref(keyboard), ctypes.sizeof(keyboard))
+    x = Input(type=Keyboard, ki=KeyboardInput(wVk=keycode, dwFlags=win32_EventF_KEYUP))
+    SendInput(1, ctypes.byref(x), ctypes.sizeof(x))
```

### Comparing `je_auto_control_dev-0.0.88/je_auto_control/windows/mouse/win32_ctype_mouse_control.py` & `je_auto_control_dev-0.0.9/je_auto_control/windows/mouse/win32_ctype_mouse_control.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,111 +1,110 @@
 import sys
-from typing import Tuple
 
-from je_auto_control.utils.exception.exception_tags import windows_import_error
+from je_auto_control.utils.exception.exception_tag import windows_import_error
 from je_auto_control.utils.exception.exceptions import AutoControlException
 
 if sys.platform not in ["win32", "cygwin", "msys"]:
     raise AutoControlException(windows_import_error)
 
 from je_auto_control.windows.core.utils.win32_ctype_input import Input
-from je_auto_control.windows.core.utils.win32_vk import win32_LEFTDOWN
-from je_auto_control.windows.core.utils.win32_vk import win32_LEFTUP
-from je_auto_control.windows.core.utils.win32_vk import win32_MIDDLEDOWN
-from je_auto_control.windows.core.utils.win32_vk import win32_MIDDLEUP
+from je_auto_control.windows.core.utils.win32_ctype_input import win32_LEFTDOWN
+from je_auto_control.windows.core.utils.win32_ctype_input import win32_LEFTUP
+from je_auto_control.windows.core.utils.win32_ctype_input import win32_MIDDLEDOWN
+from je_auto_control.windows.core.utils.win32_ctype_input import win32_MIDDLEUP
 from je_auto_control.windows.core.utils.win32_ctype_input import Mouse
 from je_auto_control.windows.core.utils.win32_ctype_input import MouseInput
-from je_auto_control.windows.core.utils.win32_vk import win32_RIGHTDOWN
-from je_auto_control.windows.core.utils.win32_vk import win32_RIGHTUP
+from je_auto_control.windows.core.utils.win32_ctype_input import win32_RIGHTDOWN
+from je_auto_control.windows.core.utils.win32_ctype_input import win32_RIGHTUP
 from je_auto_control.windows.core.utils.win32_ctype_input import SendInput
-from je_auto_control.windows.core.utils.win32_vk import win32_XBUTTON1
-from je_auto_control.windows.core.utils.win32_vk import win32_XBUTTON2
-from je_auto_control.windows.core.utils.win32_vk import win32_DOWN
-from je_auto_control.windows.core.utils.win32_vk import win32_XUP
-from ctypes import windll
+from je_auto_control.windows.core.utils.win32_ctype_input import win32_XBUTTON1
+from je_auto_control.windows.core.utils.win32_ctype_input import win32_XBUTTON2
+from je_auto_control.windows.core.utils.win32_ctype_input import win32_DOWN
+from je_auto_control.windows.core.utils.win32_ctype_input import win32_XUP
+from je_auto_control.windows.core.utils.win32_ctype_input import windll
 from je_auto_control.windows.core.utils.win32_ctype_input import wintypes
 from je_auto_control.windows.core.utils.win32_vk import win32_WHEEL
 from je_auto_control.windows.core.utils.win32_ctype_input import ctypes
-from je_auto_control.windows.screen.win32_screen import size
+from je_auto_control.windows.screen import size
 
-win32_mouse_left: Tuple = (win32_LEFTUP, win32_LEFTDOWN, 0)
-win32_mouse_middle: Tuple = (win32_MIDDLEUP, win32_MIDDLEDOWN, 0)
-win32_mouse_right: Tuple = (win32_RIGHTUP, win32_RIGHTDOWN, 0)
-win32_mouse_x1: Tuple = (win32_XUP, win32_DOWN, win32_XBUTTON1)
-win32_mouse_x2: Tuple = (win32_XUP, win32_DOWN, win32_XBUTTON2)
+win32_mouse_left = (win32_LEFTUP, win32_LEFTDOWN, 0)
+win32_mouse_middle = (win32_MIDDLEUP, win32_MIDDLEDOWN, 0)
+win32_mouse_right = (win32_RIGHTUP, win32_RIGHTDOWN, 0)
+win32_mouse_x1 = (win32_XUP, win32_DOWN, win32_XBUTTON1)
+win32_mouse_x2 = (win32_XUP, win32_DOWN, win32_XBUTTON2)
 
-_get_cursor_pos: windll.user32.GetCursorPos = windll.user32.GetCursorPos
-_set_cursor_pos: windll.user32.SetCursorPos = windll.user32.SetCursorPos
+_get_cursor_pos = windll.user32.GetCursorPos
+_set_cursor_pos = windll.user32.SetCursorPos
 
 
-def mouse_event(event, x: int, y: int, dwData: int = 0) -> None:
+def mouse_event(event, x: int, y: int, dwData: int = 0):
     """
     :param event which event we use
     :param x event x
     :param y event y
     :param dwData still 0
     """
     width, height = size()
-    converted_x = 65536 * x // width + 1
-    converted_y = 65536 * y // height + 1
-    ctypes.windll.user32.mouse_event(event, ctypes.c_long(converted_x), ctypes.c_long(converted_y), dwData, 0)
+    convertedX = 65536 * x // width + 1
+    convertedY = 65536 * y // height + 1
+    ctypes.windll.user32.mouse_event(event, ctypes.c_long(convertedX), ctypes.c_long(convertedY), dwData, 0)
 
 
-def position() -> [Tuple[int, int], None]:
+def position():
     """
     get mouse position
     """
     point = wintypes.POINT()
     if _get_cursor_pos(ctypes.byref(point)):
         return point.x, point.y
     else:
         return None
 
 
-def set_position(x: int, y: int) -> None:
+def set_position(x: int, y: int):
     """
     :param x set mouse position x
     :param y set mouse position y
     """
     pos = x, y
     _set_cursor_pos(*pos)
 
 
-def press_mouse(press_button: int) -> None:
+def press_mouse(press_button: int):
     """
     :param press_button which button we want to press
     """
     SendInput(1, ctypes.byref(
-        Input(type=Mouse, _input=Input.INPUTUnion(
+        Input(type=Mouse, _input=Input.INPUT_Union(
             mi=MouseInput(dwFlags=press_button[1], mouseData=press_button[2])))),
               ctypes.sizeof(Input))
 
 
-def release_mouse(release_button: int) -> None:
+def release_mouse(release_button: int):
     """
     :param release_button which button we want to release
     """
     SendInput(1, ctypes.byref(
-        Input(type=Mouse, _input=Input.INPUTUnion(
+        Input(type=Mouse, _input=Input.INPUT_Union(
             mi=MouseInput(dwFlags=release_button[0], mouseData=release_button[2])))),
               ctypes.sizeof(Input))
 
 
-def click_mouse(mouse_keycode: int, x: int = None, y: int = None) -> None:
+def click_mouse(mouse_keycode: int, x: int = None, y: int = None):
     """
     :param mouse_keycode which mouse keycode we want to click
     :param x mouse x position
     :param y mouse y position
     """
     if x and y is not None:
         set_position(x, y)
     press_mouse(mouse_keycode)
     release_mouse(mouse_keycode)
 
 
-def scroll(scroll_value: int, x: int = None, y: int = None) -> None:
+def scroll(scroll_value: int, x: int = None, y: int = None):
     """
     :param scroll_value scroll count
     :param x scroll x
     :param y scroll y
     """
     mouse_event(win32_WHEEL, x, y, dwData=scroll_value)
```

### Comparing `je_auto_control_dev-0.0.88/je_auto_control/windows/record/win32_record.py` & `je_auto_control_dev-0.0.9/je_auto_control/windows/record/win32_record.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,57 +1,66 @@
 import sys
 
-from je_auto_control.utils.exception.exception_tags import windows_import_error
+from je_auto_control.utils.exception.exception_tag import windows_import_error
 from je_auto_control.utils.exception.exceptions import AutoControlException
 
 if sys.platform not in ["win32", "cygwin", "msys"]:
     raise AutoControlException(windows_import_error)
 
 from je_auto_control.windows.listener.win32_keyboard_listener import Win32KeyboardListener
 from je_auto_control.windows.listener.win32_mouse_listener import Win32MouseListener
 
 from queue import Queue
 
 
 class Win32Recorder(object):
 
     def __init__(self):
-        self.mouse_record_listener: [None, Win32MouseListener] = None
-        self.keyboard_record_listener: [None, Win32KeyboardListener] = None
-        self.record_queue: [None, Queue] = None
-        self.result_queue: [None, Queue] = None
+        self.mouse_record_listener = None
+        self.keyboard_record_listener = None
+        self.record_queue = None
+        self.result_queue = None
 
-    def record(self) -> None:
+    def record(self):
         self.mouse_record_listener = Win32MouseListener()
         self.keyboard_record_listener = Win32KeyboardListener()
         self.record_queue = Queue()
         self.mouse_record_listener.record(self.record_queue)
         self.keyboard_record_listener.record(self.record_queue)
 
-    def stop_record(self) -> Queue:
+    def stop_record(self):
         self.result_queue = self.mouse_record_listener.stop_record()
         self.result_queue = self.keyboard_record_listener.stop_record()
         self.record_queue = None
         return self.result_queue
 
-    def record_mouse(self) -> None:
+    def record_mouse(self):
         self.mouse_record_listener = Win32MouseListener()
         self.record_queue = Queue()
         self.mouse_record_listener.record(self.record_queue)
 
-    def stop_record_mouse(self) -> Queue:
+    def stop_record_mouse(self):
         self.result_queue = self.mouse_record_listener.stop_record()
         self.record_queue = None
         return self.result_queue
 
-    def record_keyboard(self) -> None:
+    def record_keyboard(self):
         self.keyboard_record_listener = Win32KeyboardListener()
         self.record_queue = Queue()
-        self.keyboard_record_listener.record(self.record_queue)
+        self.keyboard_record_listener.record(record_queue)
 
-    def stop_record_keyboard(self) -> Queue:
+    def stop_record_keyboard(self):
         self.result_queue = self.keyboard_record_listener.stop_record()
         self.record_queue = None
         return self.result_queue
 
 
 win32_recorder = Win32Recorder()
+
+if __name__ == "__main__":
+    win32_recorder = Win32Recorder()
+    win32_recorder.record()
+    from time import sleep
+
+    sleep(10)
+    for i in win32_recorder.stop_record().queue:
+        print(i)
```

### Comparing `je_auto_control_dev-0.0.88/je_auto_control/wrapper/auto_control_record.py` & `je_auto_control_dev-0.0.9/je_auto_control/wrapper/auto_control_record.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 import sys
 
-from je_auto_control.utils.exception.exception_tags import macos_record_error
+from je_auto_control.utils.executor.action_executor import execute_action
+from je_auto_control.utils.exception.exception_tag import macos_record_error
 from je_auto_control.utils.exception.exceptions import AutoControlException
 from je_auto_control.utils.exception.exceptions import AutoControlJsonActionException
-from je_auto_control.utils.logging.loggin_instance import auto_control_logger
-from je_auto_control.utils.test_record.record_test_class import record_action_to_list
 from je_auto_control.wrapper.platform_wrapper import recorder
+from je_auto_control.utils.test_record.record_test_class import record_total
 
 
-def record() -> None:
+def record():
     """
     start record keyboard and mouse event until stop_record
     """
-    auto_control_logger.info("record")
     try:
         if sys.platform == "darwin":
             raise AutoControlException(macos_record_error)
-        record_action_to_list("record", None)
+        record_total("record", None)
         return recorder.record()
     except Exception as error:
-        record_action_to_list("record", None, repr(error))
-        auto_control_logger.error(f"record, failed: {repr(error)}")
+        record_total("record", None, repr(error))
+        print(repr(error), file=sys.stderr)
 
 
-def stop_record() -> list:
+def stop_record():
     """
     stop current record
     """
-    auto_control_logger.info("stop_record")
     try:
         if sys.platform == "darwin":
             raise AutoControlException(macos_record_error)
         action_queue = recorder.stop_record()
         if action_queue is None:
             raise AutoControlJsonActionException
         action_list = list(action_queue.queue)
         new_list = list()
         for action in action_list:
-            if action[0] == "type_keyboard":
+            if action[0] == "type_key":
                 new_list.append([action[0], dict([["keycode", action[1]]])])
             else:
                 new_list.append([action[0], dict(zip(["mouse_keycode", "x", "y"], [action[0], action[1], action[2]]))])
-        record_action_to_list("stop_record", None)
+        record_total("stop_record", None)
         return new_list
     except Exception as error:
-        record_action_to_list("stop_record", None, repr(error))
-        auto_control_logger.error(f"stop_record, failed: {repr(error)}")
+        record_total("stop_record", None, repr(error))
+        print(repr(error), file=sys.stderr)
+
```

### Comparing `je_auto_control_dev-0.0.88/je_auto_control/wrapper/auto_control_screen.py` & `je_auto_control_dev-0.0.9/je_auto_control/wrapper/auto_control_screen.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,55 +1,44 @@
 import sys
-from typing import Tuple, List
 
 import cv2
 import numpy as np
 
-from je_auto_control.utils.exception.exception_tags import screen_get_size
-from je_auto_control.utils.exception.exception_tags import screen_screenshot
-from je_auto_control.utils.exception.exceptions import AutoControlScreenException
 from je_auto_control.utils.image.screenshot import pil_screenshot
-from je_auto_control.utils.logging.loggin_instance import auto_control_logger
-from je_auto_control.utils.test_record.record_test_class import record_action_to_list
+from je_auto_control.utils.exception.exception_tag import screen_get_size
+from je_auto_control.utils.exception.exception_tag import screen_screenshot
+from je_auto_control.utils.exception.exceptions import AutoControlScreenException
 from je_auto_control.wrapper.platform_wrapper import screen
+from je_auto_control.utils.test_record.record_test_class import record_total
 
 
-def screen_size() -> Tuple[int, int]:
+def size():
     """
     get screen size
     """
-    auto_control_logger.info("screen_size")
     try:
         try:
-            record_action_to_list("size", None)
+            record_total("size", None)
             return screen.size()
         except AutoControlScreenException:
-            auto_control_logger.error(f"screen_size, failed: {repr(AutoControlScreenException(screen_get_size))}")
             raise AutoControlScreenException(screen_get_size)
     except Exception as error:
-        record_action_to_list("size", None, repr(error))
-        auto_control_logger.error(f"screen_size, failed: {repr(error)}")
+        record_total("size", None, repr(error))
+        print(repr(error), file=sys.stderr)
 
 
-def screenshot(file_path: str = None, screen_region: list = None) -> List[int]:
+def screenshot(file_path: str = None, region: list = None):
     """
     use to capture current screen image
     :param file_path screenshot file save path
-    :param screen_region screenshot screen_region
+    :param region screenshot region
     """
-    auto_control_logger.info(f"screen_size, file_path: {file_path}, screen_region: {screen_region}")
     param = locals()
     try:
         try:
-            record_action_to_list("screenshot", param)
-            return cv2.cvtColor(
-                np.array(pil_screenshot(file_path=file_path, screen_region=screen_region)), cv2.COLOR_RGB2BGR)
-        except AutoControlScreenException as error:
-            auto_control_logger.info(
-                f"screen_size, file_path: {file_path}, screen_region: {screen_region}, "
-                f"failed: {AutoControlScreenException(screen_screenshot + ' ' + repr(error))}")
-            raise AutoControlScreenException(screen_screenshot + " " + repr(error))
+            record_total("screenshot", param)
+            return cv2.cvtColor(np.array(pil_screenshot(file_path=file_path, region=region)), cv2.COLOR_RGB2BGR)
+        except AutoControlScreenException:
+            raise AutoControlScreenException(screen_screenshot)
     except Exception as error:
-        record_action_to_list("screenshot", None, repr(error))
-        auto_control_logger.info(
-            f"screen_size, file_path: {file_path}, screen_region: {screen_region}, "
-            f"failed: {repr(error)}")
+        record_total("screenshot", None, repr(error))
+        print(repr(error), file=sys.stderr)
```

### Comparing `je_auto_control_dev-0.0.88/je_auto_control/wrapper/platform_wrapper.py` & `je_auto_control_dev-0.0.9/je_auto_control/wrapper/platform_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import sys
 
 from je_auto_control.utils.exception.exceptions import AutoControlException
-from je_auto_control.utils.logging.loggin_instance import auto_control_logger
 
 if sys.platform in ["win32", "cygwin", "msys"]:
     from je_auto_control.windows.core.utils.win32_vk import win32_ABSOLUTE
     from je_auto_control.windows.core.utils.win32_vk import win32_EventF_EXTENDEDKEY
     from je_auto_control.windows.core.utils.win32_vk import win32_EventF_KEYUP
     from je_auto_control.windows.core.utils.win32_vk import win32_EventF_SCANCODE
     from je_auto_control.windows.core.utils.win32_vk import win32_EventF_UNICODE
@@ -480,26 +479,26 @@
     from je_auto_control.linux_with_x11.mouse import x11_linux_mouse_control
     from je_auto_control.linux_with_x11.screen import x11_linux_screen
     from je_auto_control.linux_with_x11.record.x11_linux_record import x11_linux_recoder
 
 else:
     raise AutoControlException("unknown operating system")
 
-keyboard_keys_table = None
-mouse_keys_table = None
-special_mouse_keys_table = None
+keys_table = None
+mouse_table = None
+special_table = None
 keyboard = None
 keyboard_check = None
 mouse = None
 screen = None
 recorder = None
 
 if sys.platform in ["win32", "cygwin", "msys"]:
-    auto_control_logger.info("Load Windows Setting")
-    keyboard_keys_table = {
+
+    keys_table = {
         "absolute": win32_ABSOLUTE,
         "eventf_extendedkey": win32_EventF_EXTENDEDKEY,
         "eventf_keyup": win32_EventF_KEYUP,
         "eventf_scancode": win32_EventF_SCANCODE,
         "eventf_unicode": win32_EventF_UNICODE,
         "hwheel": win32_HWHEEL,
         "leftdown": win32_LEFTDOWN,
@@ -685,33 +684,33 @@
         "X": win32_keyX,
         "x": win32_keyX,
         "Y": win32_keyY,
         "y": win32_keyY,
         "Z": win32_keyZ,
         "z": win32_keyZ,
     }
-    mouse_keys_table = {
-        "mouse_left": win32_mouse_left,
-        "mouse_middle": win32_mouse_middle,
-        "mouse_right": win32_mouse_right,
-        "mouse_x1": win32_mouse_x1,
-        "mouse_x2": win32_mouse_x2
+    mouse_table = {
+     "mouse_left": win32_mouse_left,
+     "mouse_middle": win32_mouse_middle,
+     "mouse_right": win32_mouse_right,
+     "mouse_x1": win32_mouse_x1,
+     "mouse_x2": win32_mouse_x2
     }
     keyboard = win32_ctype_keyboard_control
     keyboard_check = win32_keypress_check
     mouse = win32_ctype_mouse_control
     screen = win32_screen
     recorder = win32_recorder
 
-    if None in [keyboard_keys_table, mouse_keys_table, keyboard_check, keyboard, mouse, screen, recorder]:
+    if None in [keys_table, mouse_table, keyboard_check, keyboard, mouse, screen, recorder]:
         raise AutoControlException("Can't init auto control")
 
 elif sys.platform in ["darwin"]:
-    auto_control_logger.info("Load MacOS Setting")
-    keyboard_keys_table = {
+
+    keys_table = {
         "a": osx_key_a,
         "A": osx_key_A,
         "b": osx_key_b,
         "B": osx_key_B,
         "c": osx_key_c,
         "C": osx_key_C,
         "d": osx_key_d,
@@ -851,29 +850,29 @@
         "right": osx_key_right,
         "down": osx_key_down,
         "up": osx_key_up,
         "yen": osx_key_yen,
         "eisu": osx_key_eisu,
         "kana": osx_key_kana,
     }
-    mouse_keys_table = {
+    mouse_table = {
         "mouse_left": osx_mouse_left,
         "mouse_middle": osx_mouse_middle,
         "mouse_right": osx_mouse_right,
     }
     keyboard = osx_keyboard
     keyboard_check = osx_keyboard_check
     mouse = osx_mouse
     screen = osx_screen
-    if None in [keyboard_keys_table, mouse_keys_table, keyboard_check, keyboard, mouse, screen]:
+    if None in [keys_table, mouse_table, keyboard_check, keyboard, mouse, screen]:
         raise AutoControlException("Can't init auto control")
 
 elif sys.platform in ["linux", "linux2"]:
-    auto_control_logger.info("Load Linux x11 Setting")
-    keyboard_keys_table = {
+
+    keys_table = {
         "backspace": x11_linux_key_backspace,
         "\b": x11_linux_key_slash_b,
         "tab": x11_linux_key_tab,
         "enter": x11_linux_key_enter,
         "return": x11_linux_key_return,
         "shift": x11_linux_key_shift,
         "ctrl": x11_linux_key_ctrl,
@@ -1048,28 +1047,28 @@
         "5": x11_linux_key_5,
         "6": x11_linux_key_6,
         "7": x11_linux_key_7,
         "8": x11_linux_key_8,
         "9": x11_linux_key_9,
         "0": x11_linux_key_0,
     }
-    mouse_keys_table = {
+    mouse_table = {
         "mouse_left": x11_linux_mouse_left,
         "mouse_middle": x11_linux_mouse_middle,
         "mouse_right": x11_linux_mouse_right
     }
-    special_mouse_keys_table = {
+    special_table = {
         "scroll_up": x11_linux_scroll_direction_up,
         "scroll_down": x11_linux_scroll_direction_down,
         "scroll_left": x11_linux_scroll_direction_left,
         "scroll_right": x11_linux_scroll_direction_right
     }
     keyboard = x11_linux_keyboard_control
     keyboard_check = x11_linux_listener
     mouse = x11_linux_mouse_control
     screen = x11_linux_screen
     recorder = x11_linux_recoder
-    if None in [keyboard_keys_table, mouse_keys_table, special_mouse_keys_table, keyboard, mouse, screen, recorder]:
+    if None in [keys_table, mouse_table, special_table, keyboard, mouse, screen, recorder]:
         raise AutoControlException("Can't init auto control")
 
-if None in [keyboard_keys_table, mouse_keys_table, keyboard, mouse, screen]:
+if None in [keys_table, mouse_table, keyboard, mouse, screen]:
     raise AutoControlException("Can't init auto control")
```

### Comparing `je_auto_control_dev-0.0.88/je_auto_control_dev.egg-info/SOURCES.txt` & `je_auto_control_dev-0.0.9/je_auto_control_dev.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+LICENSE
 README.md
-pyproject.toml
+dev_setup.py
+setup.py
 je_auto_control/__init__.py
 je_auto_control/__main__.py
 je_auto_control/linux_with_x11/__init__.py
 je_auto_control/linux_with_x11/core/__init__.py
 je_auto_control/linux_with_x11/core/utils/__init__.py
 je_auto_control/linux_with_x11/core/utils/x11_linux_display.py
 je_auto_control/linux_with_x11/core/utils/x11_linux_vk.py
@@ -29,60 +31,30 @@
 je_auto_control/osx/mouse/__init__.py
 je_auto_control/osx/mouse/osx_mouse.py
 je_auto_control/osx/record/__init__.py
 je_auto_control/osx/record/osx_record.py
 je_auto_control/osx/screen/__init__.py
 je_auto_control/osx/screen/osx_screen.py
 je_auto_control/utils/__init__.py
-je_auto_control/utils/callback/__init__.py
-je_auto_control/utils/callback/callback_function_executor.py
 je_auto_control/utils/critical_exit/__init__.py
 je_auto_control/utils/critical_exit/critcal_exit.py
 je_auto_control/utils/exception/__init__.py
-je_auto_control/utils/exception/exception_tags.py
+je_auto_control/utils/exception/exception_tag.py
 je_auto_control/utils/exception/exceptions.py
 je_auto_control/utils/executor/__init__.py
 je_auto_control/utils/executor/action_executor.py
-je_auto_control/utils/file_process/__init__.py
-je_auto_control/utils/file_process/get_dir_file_list.py
-je_auto_control/utils/generate_report/__init__.py
-je_auto_control/utils/generate_report/generate_html_report.py
-je_auto_control/utils/generate_report/generate_json_report.py
-je_auto_control/utils/generate_report/generate_xml_report.py
 je_auto_control/utils/image/__init__.py
 je_auto_control/utils/image/screenshot.py
 je_auto_control/utils/image/template_detection.py
 je_auto_control/utils/json/__init__.py
 je_auto_control/utils/json/json_file.py
-je_auto_control/utils/logging/__init__.py
-je_auto_control/utils/logging/loggin_instance.py
-je_auto_control/utils/package_manager/__init__.py
-je_auto_control/utils/package_manager/package_manager_class.py
-je_auto_control/utils/project/__init__.py
-je_auto_control/utils/project/create_project_structure.py
-je_auto_control/utils/project/template/__init__.py
-je_auto_control/utils/project/template/template_executor.py
-je_auto_control/utils/project/template/template_keyword.py
-je_auto_control/utils/scheduler/__init__.py
-je_auto_control/utils/scheduler/extend_apscheduler.py
-je_auto_control/utils/shell_process/__init__.py
-je_auto_control/utils/shell_process/shell_exec.py
-je_auto_control/utils/socket_server/__init__.py
-je_auto_control/utils/socket_server/auto_control_socket_server.py
-je_auto_control/utils/start_exe/__init__.py
-je_auto_control/utils/start_exe/start_another_process.py
 je_auto_control/utils/test_record/__init__.py
 je_auto_control/utils/test_record/record_test_class.py
 je_auto_control/utils/timeout/__init__.py
 je_auto_control/utils/timeout/multiprocess_timeout.py
-je_auto_control/utils/xml/__init__.py
-je_auto_control/utils/xml/change_xml_structure/__init__.py
-je_auto_control/utils/xml/change_xml_structure/change_xml_structure.py
-je_auto_control/utils/xml/xml_file/__init__.py
-je_auto_control/utils/xml/xml_file/xml_file.py
 je_auto_control/windows/__init__.py
 je_auto_control/windows/core/__init__.py
 je_auto_control/windows/core/utils/__init__.py
 je_auto_control/windows/core/utils/win32_ctype_input.py
 je_auto_control/windows/core/utils/win32_keypress_check.py
 je_auto_control/windows/core/utils/win32_vk.py
 je_auto_control/windows/keyboard/__init__.py
```

