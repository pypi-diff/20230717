# Comparing `tmp/je_api_testka_dev-0.0.97.tar.gz` & `tmp/je_api_testka_dev-0.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "je_api_testka_dev-0.0.97.tar", last modified: Mon Jun 19 05:59:05 2023, max compression
+gzip compressed data, was "je_api_testka_dev-0.0.98.tar", last modified: Mon Jul 17 02:22:07 2023, max compression
```

## Comparing `je_api_testka_dev-0.0.97.tar` & `je_api_testka_dev-0.0.98.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 05:59:05.029216 je_api_testka_dev-0.0.97/
--rw-rw-rw-   0        0        0     3074 2023-06-19 05:59:05.028216 je_api_testka_dev-0.0.97/PKG-INFO
--rw-rw-rw-   0        0        0     2270 2023-05-30 02:10:25.000000 je_api_testka_dev-0.0.97/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 05:59:04.795609 je_api_testka_dev-0.0.97/je_api_testka/
--rw-rw-rw-   0        0        0     2957 2023-05-31 05:32:44.000000 je_api_testka_dev-0.0.97/je_api_testka/__init__.py
--rw-rw-rw-   0        0        0     2349 2023-04-25 09:07:47.000000 je_api_testka_dev-0.0.97/je_api_testka/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:59:04.805164 je_api_testka_dev-0.0.97/je_api_testka/requests_wrapper/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.97/je_api_testka/requests_wrapper/__init__.py
--rw-rw-rw-   0        0        0     5676 2023-06-19 05:42:57.000000 je_api_testka_dev-0.0.97/je_api_testka/requests_wrapper/request_method.py
--rw-rw-rw-   0        0        0     3116 2023-06-13 07:15:23.000000 je_api_testka_dev-0.0.97/je_api_testka/requests_wrapper/requests_http_method_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:59:04.807172 je_api_testka_dev-0.0.97/je_api_testka/utils/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:59:04.812684 je_api_testka_dev-0.0.97/je_api_testka/utils/assert_result/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/assert_result/__init__.py
--rw-rw-rw-   0        0        0      942 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/assert_result/result_check.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:59:04.821707 je_api_testka_dev-0.0.97/je_api_testka/utils/callback/
--rw-rw-rw-   0        0        0        0 2023-03-31 09:04:52.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/callback/__init__.py
--rw-rw-rw-   0        0        0     3502 2023-06-19 03:36:07.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/callback/callback_function_executor.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:59:04.830207 je_api_testka_dev-0.0.97/je_api_testka/utils/exception/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/exception/__init__.py
--rw-rw-rw-   0        0        0     3393 2023-04-21 01:54:17.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0     2392 2023-04-21 01:54:17.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:59:04.837233 je_api_testka_dev-0.0.97/je_api_testka/utils/executor/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/executor/__init__.py
--rw-rw-rw-   0        0        0     5973 2023-06-19 03:34:10.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/executor/action_executor.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:59:04.843215 je_api_testka_dev-0.0.97/je_api_testka/utils/file_process/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/file_process/__init__.py
--rw-rw-rw-   0        0        0      734 2023-06-19 03:15:40.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/file_process/get_dir_file_list.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:59:04.857288 je_api_testka_dev-0.0.97/je_api_testka/utils/generate_report/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/generate_report/__init__.py
--rw-rw-rw-   0        0        0     9239 2023-06-19 03:36:07.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/generate_report/html_report_generate.py
--rw-rw-rw-   0        0        0     4289 2023-06-19 03:36:07.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/generate_report/json_report.py
--rw-rw-rw-   0        0        0     2082 2023-06-19 03:36:07.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/generate_report/xml_report.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:59:04.865213 je_api_testka_dev-0.0.97/je_api_testka/utils/get_data_strcture/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/get_data_strcture/__init__.py
--rw-rw-rw-   0        0        0     1623 2023-06-19 05:44:00.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/get_data_strcture/get_api_data.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:59:04.868212 je_api_testka_dev-0.0.97/je_api_testka/utils/json/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/json/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:59:04.876264 je_api_testka_dev-0.0.97/je_api_testka/utils/json/json_file/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/json/json_file/__init__.py
--rw-rw-rw-   0        0        0     1378 2023-06-19 03:31:45.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/json/json_file/json_file.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:59:04.884216 je_api_testka_dev-0.0.97/je_api_testka/utils/json/json_format/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/json/json_format/__init__.py
--rw-rw-rw-   0        0        0     1300 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/json/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:59:04.891294 je_api_testka_dev-0.0.97/je_api_testka/utils/logging/
--rw-rw-rw-   0        0        0        0 2023-06-08 03:44:59.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/logging/__init__.py
--rw-rw-rw-   0        0        0      563 2023-06-13 06:12:30.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/logging/loggin_instance.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:59:04.897303 je_api_testka_dev-0.0.97/je_api_testka/utils/mock_server/
--rw-rw-rw-   0        0        0        0 2023-04-21 01:03:22.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/mock_server/__init__.py
--rw-rw-rw-   0        0        0     1998 2023-06-19 03:36:57.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/mock_server/flask_mock_server.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:59:04.904306 je_api_testka_dev-0.0.97/je_api_testka/utils/package_manager/
--rw-rw-rw-   0        0        0        0 2023-04-06 01:01:22.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/package_manager/__init__.py
--rw-rw-rw-   0        0        0     3593 2023-06-19 03:43:06.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/package_manager/package_manager_class.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:59:04.910826 je_api_testka_dev-0.0.97/je_api_testka/utils/project/
--rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/project/__init__.py
--rw-rw-rw-   0        0        0     3286 2023-06-19 03:59:54.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/project/create_project_structure.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:59:04.921919 je_api_testka_dev-0.0.97/je_api_testka/utils/project/template/
--rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/project/template/__init__.py
--rw-rw-rw-   0        0        0      633 2023-04-17 08:42:18.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/project/template/template_executor.py
--rw-rw-rw-   0        0        0      633 2023-04-17 08:52:06.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/project/template/template_keyword.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:59:04.939836 je_api_testka_dev-0.0.97/je_api_testka/utils/scheduler/
--rw-rw-rw-   0        0        0        0 2023-05-31 01:17:46.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/scheduler/__init__.py
--rw-rw-rw-   0        0        0    10696 2023-06-19 05:58:42.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/scheduler/extend_apscheduler.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:59:04.946823 je_api_testka_dev-0.0.97/je_api_testka/utils/socket_server/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/socket_server/__init__.py
--rw-rw-rw-   0        0        0     2753 2023-06-19 03:55:58.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/socket_server/api_testka_socket_server.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:59:04.956820 je_api_testka_dev-0.0.97/je_api_testka/utils/test_record/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/test_record/__init__.py
--rw-rw-rw-   0        0        0      389 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/test_record/test_record_class.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:59:04.960152 je_api_testka_dev-0.0.97/je_api_testka/utils/xml/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/xml/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:59:04.965150 je_api_testka_dev-0.0.97/je_api_testka/utils/xml/change_xml_structure/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/xml/change_xml_structure/__init__.py
--rw-rw-rw-   0        0        0     2513 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/xml/change_xml_structure/change_xml_structure.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:59:04.976151 je_api_testka_dev-0.0.97/je_api_testka/utils/xml/xml_file/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/xml/xml_file/__init__.py
--rw-rw-rw-   0        0        0     2424 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.97/je_api_testka/utils/xml/xml_file/xml_file.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:59:05.024221 je_api_testka_dev-0.0.97/je_api_testka_dev.egg-info/
--rw-rw-rw-   0        0        0     3074 2023-06-19 05:59:04.000000 je_api_testka_dev-0.0.97/je_api_testka_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2636 2023-06-19 05:59:04.000000 je_api_testka_dev-0.0.97/je_api_testka_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 05:59:04.000000 je_api_testka_dev-0.0.97/je_api_testka_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-19 05:59:04.000000 je_api_testka_dev-0.0.97/je_api_testka_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-19 05:59:04.000000 je_api_testka_dev-0.0.97/je_api_testka_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1172 2023-06-19 05:58:42.000000 je_api_testka_dev-0.0.97/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-19 05:59:05.030219 je_api_testka_dev-0.0.97/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-17 02:22:07.734881 je_api_testka_dev-0.0.98/
+-rw-rw-rw-   0        0        0     3074 2023-07-17 02:22:07.733873 je_api_testka_dev-0.0.98/PKG-INFO
+-rw-rw-rw-   0        0        0     2270 2023-05-30 02:10:25.000000 je_api_testka_dev-0.0.98/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 02:22:07.418664 je_api_testka_dev-0.0.98/je_api_testka/
+-rw-rw-rw-   0        0        0     2957 2023-05-31 05:32:44.000000 je_api_testka_dev-0.0.98/je_api_testka/__init__.py
+-rw-rw-rw-   0        0        0     2349 2023-04-25 09:07:47.000000 je_api_testka_dev-0.0.98/je_api_testka/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:22:07.433143 je_api_testka_dev-0.0.98/je_api_testka/requests_wrapper/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.98/je_api_testka/requests_wrapper/__init__.py
+-rw-rw-rw-   0        0        0     5676 2023-06-19 05:42:57.000000 je_api_testka_dev-0.0.98/je_api_testka/requests_wrapper/request_method.py
+-rw-rw-rw-   0        0        0     3116 2023-06-13 07:15:23.000000 je_api_testka_dev-0.0.98/je_api_testka/requests_wrapper/requests_http_method_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:22:07.435889 je_api_testka_dev-0.0.98/je_api_testka/utils/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:22:07.448010 je_api_testka_dev-0.0.98/je_api_testka/utils/assert_result/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/assert_result/__init__.py
+-rw-rw-rw-   0        0        0      942 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/assert_result/result_check.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:22:07.457160 je_api_testka_dev-0.0.98/je_api_testka/utils/callback/
+-rw-rw-rw-   0        0        0        0 2023-03-31 09:04:52.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/callback/__init__.py
+-rw-rw-rw-   0        0        0     3502 2023-06-19 03:36:07.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/callback/callback_function_executor.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:22:07.468456 je_api_testka_dev-0.0.98/je_api_testka/utils/exception/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0     3393 2023-04-21 01:54:17.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0     2392 2023-04-21 01:54:17.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:22:07.479563 je_api_testka_dev-0.0.98/je_api_testka/utils/executor/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/executor/__init__.py
+-rw-rw-rw-   0        0        0     7228 2023-07-17 02:15:39.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/executor/action_executor.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:22:07.491103 je_api_testka_dev-0.0.98/je_api_testka/utils/file_process/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/file_process/__init__.py
+-rw-rw-rw-   0        0        0      734 2023-06-19 03:15:40.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/file_process/get_dir_file_list.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:22:07.511624 je_api_testka_dev-0.0.98/je_api_testka/utils/generate_report/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/generate_report/__init__.py
+-rw-rw-rw-   0        0        0     9239 2023-06-19 03:36:07.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/generate_report/html_report_generate.py
+-rw-rw-rw-   0        0        0     4289 2023-06-19 03:36:07.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/generate_report/json_report.py
+-rw-rw-rw-   0        0        0     2082 2023-06-19 03:36:07.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/generate_report/xml_report.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:22:07.524340 je_api_testka_dev-0.0.98/je_api_testka/utils/get_data_strcture/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/get_data_strcture/__init__.py
+-rw-rw-rw-   0        0        0     1623 2023-06-19 05:44:00.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/get_data_strcture/get_api_data.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:22:07.528282 je_api_testka_dev-0.0.98/je_api_testka/utils/json/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/json/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:22:07.534950 je_api_testka_dev-0.0.98/je_api_testka/utils/json/json_file/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/json/json_file/__init__.py
+-rw-rw-rw-   0        0        0     1378 2023-06-19 03:31:45.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/json/json_file/json_file.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:22:07.580086 je_api_testka_dev-0.0.98/je_api_testka/utils/json/json_format/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/json/json_format/__init__.py
+-rw-rw-rw-   0        0        0     1300 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/json/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:22:07.595168 je_api_testka_dev-0.0.98/je_api_testka/utils/logging/
+-rw-rw-rw-   0        0        0        0 2023-06-08 03:44:59.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/logging/__init__.py
+-rw-rw-rw-   0        0        0      563 2023-06-13 06:12:30.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/logging/loggin_instance.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:22:07.603663 je_api_testka_dev-0.0.98/je_api_testka/utils/mock_server/
+-rw-rw-rw-   0        0        0        0 2023-04-21 01:03:22.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/mock_server/__init__.py
+-rw-rw-rw-   0        0        0     1998 2023-06-19 03:36:57.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/mock_server/flask_mock_server.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:22:07.610720 je_api_testka_dev-0.0.98/je_api_testka/utils/package_manager/
+-rw-rw-rw-   0        0        0        0 2023-04-06 01:01:22.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/package_manager/__init__.py
+-rw-rw-rw-   0        0        0     3593 2023-06-19 03:43:06.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/package_manager/package_manager_class.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:22:07.624071 je_api_testka_dev-0.0.98/je_api_testka/utils/project/
+-rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/project/__init__.py
+-rw-rw-rw-   0        0        0     3286 2023-06-19 03:59:54.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/project/create_project_structure.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:22:07.636819 je_api_testka_dev-0.0.98/je_api_testka/utils/project/template/
+-rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/project/template/__init__.py
+-rw-rw-rw-   0        0        0      633 2023-04-17 08:42:18.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/project/template/template_executor.py
+-rw-rw-rw-   0        0        0      633 2023-04-17 08:52:06.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/project/template/template_keyword.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:22:07.649048 je_api_testka_dev-0.0.98/je_api_testka/utils/scheduler/
+-rw-rw-rw-   0        0        0        0 2023-05-31 01:17:46.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/scheduler/__init__.py
+-rw-rw-rw-   0        0        0    11468 2023-07-17 01:44:29.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/scheduler/extend_apscheduler.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:22:07.660138 je_api_testka_dev-0.0.98/je_api_testka/utils/socket_server/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/socket_server/__init__.py
+-rw-rw-rw-   0        0        0     2753 2023-06-19 03:55:58.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/socket_server/api_testka_socket_server.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:22:07.668669 je_api_testka_dev-0.0.98/je_api_testka/utils/test_record/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/test_record/__init__.py
+-rw-rw-rw-   0        0        0      389 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/test_record/test_record_class.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:22:07.673227 je_api_testka_dev-0.0.98/je_api_testka/utils/xml/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/xml/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:22:07.683701 je_api_testka_dev-0.0.98/je_api_testka/utils/xml/change_xml_structure/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/xml/change_xml_structure/__init__.py
+-rw-rw-rw-   0        0        0     2513 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/xml/change_xml_structure/change_xml_structure.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:22:07.694994 je_api_testka_dev-0.0.98/je_api_testka/utils/xml/xml_file/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/xml/xml_file/__init__.py
+-rw-rw-rw-   0        0        0     2424 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.98/je_api_testka/utils/xml/xml_file/xml_file.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:22:07.728064 je_api_testka_dev-0.0.98/je_api_testka_dev.egg-info/
+-rw-rw-rw-   0        0        0     3074 2023-07-17 02:22:07.000000 je_api_testka_dev-0.0.98/je_api_testka_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2636 2023-07-17 02:22:07.000000 je_api_testka_dev-0.0.98/je_api_testka_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 02:22:07.000000 je_api_testka_dev-0.0.98/je_api_testka_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-17 02:22:07.000000 je_api_testka_dev-0.0.98/je_api_testka_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-17 02:22:07.000000 je_api_testka_dev-0.0.98/je_api_testka_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1172 2023-07-17 02:21:41.000000 je_api_testka_dev-0.0.98/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-17 02:22:07.735890 je_api_testka_dev-0.0.98/setup.cfg
```

### Comparing `je_api_testka_dev-0.0.97/PKG-INFO` & `je_api_testka_dev-0.0.98/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je_api_testka_dev
-Version: 0.0.97
+Version: 0.0.98
 Summary: Requests Automation Framework
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/APITestka
 Project-URL: Documentation, https://apitestka.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/APITestka
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `je_api_testka_dev-0.0.97/README.md` & `je_api_testka_dev-0.0.98/README.md`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.97/je_api_testka/__init__.py` & `je_api_testka_dev-0.0.98/je_api_testka/__init__.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.97/je_api_testka/__main__.py` & `je_api_testka_dev-0.0.98/je_api_testka/__main__.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.97/je_api_testka/requests_wrapper/request_method.py` & `je_api_testka_dev-0.0.98/je_api_testka/requests_wrapper/request_method.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.97/je_api_testka/requests_wrapper/requests_http_method_wrapper.py` & `je_api_testka_dev-0.0.98/je_api_testka/requests_wrapper/requests_http_method_wrapper.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.97/je_api_testka/utils/assert_result/result_check.py` & `je_api_testka_dev-0.0.98/je_api_testka/utils/assert_result/result_check.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.97/je_api_testka/utils/callback/callback_function_executor.py` & `je_api_testka_dev-0.0.98/je_api_testka/utils/callback/callback_function_executor.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.97/je_api_testka/utils/exception/exception_tags.py` & `je_api_testka_dev-0.0.98/je_api_testka/utils/exception/exception_tags.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.97/je_api_testka/utils/exception/exceptions.py` & `je_api_testka_dev-0.0.98/je_api_testka/utils/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.97/je_api_testka/utils/executor/action_executor.py` & `je_api_testka_dev-0.0.98/je_api_testka/utils/executor/action_executor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import builtins
 import types
 from inspect import getmembers, isbuiltin
-from typing import Dict, Callable, Any, List
+from typing import Dict, Callable, Any, List, Union
 
 from je_api_testka.requests_wrapper.request_method import test_api_method
 from je_api_testka.utils.exception.exception_tags import add_command_exception_tag
 from je_api_testka.utils.exception.exception_tags import executor_data_error, executor_list_error
 from je_api_testka.utils.exception.exceptions import APITesterExecuteException, APIAddCommandException
 from je_api_testka.utils.generate_report.html_report_generate import generate_html
 from je_api_testka.utils.generate_report.html_report_generate import generate_html_report
@@ -13,37 +13,45 @@
 from je_api_testka.utils.generate_report.json_report import generate_json_report
 from je_api_testka.utils.generate_report.xml_report import generate_xml
 from je_api_testka.utils.generate_report.xml_report import generate_xml_report
 from je_api_testka.utils.json.json_file.json_file import read_action_json
 from je_api_testka.utils.logging.loggin_instance import apitestka_logger
 from je_api_testka.utils.mock_server.flask_mock_server import flask_mock_server_instance
 from je_api_testka.utils.package_manager.package_manager_class import package_manager
+from je_api_testka.utils.scheduler.extend_apscheduler import scheduler_manager
 
 
 class Executor(object):
 
     def __init__(self):
         self.event_dict = {
-            # test api
+            # Automation api
             "test_api_method": test_api_method,
             "generate_html": generate_html,
             "generate_html_report": generate_html_report,
             "generate_json": generate_json,
             "generate_json_report": generate_json_report,
             "generate_xml": generate_xml,
             "generate_xml_report": generate_xml_report,
             # Execute
             "execute_action": self.execute_action,
             "execute_files": self.execute_files,
             # Add package
             "add_package_to_executor": package_manager.add_package_to_executor,
             "add_package_to_callback_executor": package_manager.add_package_to_callback_executor,
-            # mock
+            # Mock server
             "flask_mock_server_add_router": flask_mock_server_instance.add_router,
             "start_flask_mock_server": flask_mock_server_instance.start_mock_server,
+            # Scheduler
+            "scheduler_event_trigger": self.scheduler_event_trigger,
+            "remove_blocking_scheduler_job": scheduler_manager.remove_blocking_job,
+            "remove_nonblocking_scheduler_job": scheduler_manager.remove_nonblocking_job,
+            "start_blocking_scheduler": scheduler_manager.start_block_scheduler,
+            "start_nonblocking_scheduler": scheduler_manager.start_nonblocking_scheduler,
+            "start_all_scheduler": scheduler_manager.start_all_scheduler,
         }
         # get all builtin function and add to event dict
         for function in getmembers(builtins, isbuiltin):
             self.event_dict.update({str(function[0]): function[1]})
 
     def _execute_event(self, action: list) -> Any:
         """
@@ -106,14 +114,24 @@
         """
         apitestka_logger.info(f"execute_files, execute_files_list: {execute_files_list}")
         execute_detail_list: list = list()
         for file in execute_files_list:
             execute_detail_list.append(self.execute_action(read_action_json(file)))
         return execute_detail_list
 
+    def scheduler_event_trigger(
+            self, function: str, id: str = None, args: Union[list, tuple] = None,
+            kwargs: dict = None, scheduler_type: str = "nonblocking", wait_type: str = "secondly",
+            wait_value: int = 1, **trigger_args: Any) -> None:
+        if scheduler_type == "nonblocking":
+            scheduler_event = scheduler_manager.nonblocking_scheduler_event_dict.get(wait_type)
+        else:
+            scheduler_event = scheduler_manager.blocking_scheduler_event_dict.get(wait_type)
+        scheduler_event(self.event_dict.get(function), id, args, kwargs, wait_value, **trigger_args)
+
 
 executor = Executor()
 package_manager.executor = executor
 
 
 def add_command_to_executor(command_dict: dict) -> None:
     for command_name, command in command_dict.items():
```

### Comparing `je_api_testka_dev-0.0.97/je_api_testka/utils/file_process/get_dir_file_list.py` & `je_api_testka_dev-0.0.98/je_api_testka/utils/file_process/get_dir_file_list.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.97/je_api_testka/utils/generate_report/html_report_generate.py` & `je_api_testka_dev-0.0.98/je_api_testka/utils/generate_report/html_report_generate.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.97/je_api_testka/utils/generate_report/json_report.py` & `je_api_testka_dev-0.0.98/je_api_testka/utils/generate_report/json_report.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.97/je_api_testka/utils/generate_report/xml_report.py` & `je_api_testka_dev-0.0.98/je_api_testka/utils/generate_report/xml_report.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.97/je_api_testka/utils/get_data_strcture/get_api_data.py` & `je_api_testka_dev-0.0.98/je_api_testka/utils/get_data_strcture/get_api_data.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.97/je_api_testka/utils/json/json_file/json_file.py` & `je_api_testka_dev-0.0.98/je_api_testka/utils/json/json_file/json_file.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.97/je_api_testka/utils/json/json_format/json_process.py` & `je_api_testka_dev-0.0.98/je_api_testka/utils/json/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.97/je_api_testka/utils/logging/loggin_instance.py` & `je_api_testka_dev-0.0.98/je_api_testka/utils/logging/loggin_instance.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.97/je_api_testka/utils/mock_server/flask_mock_server.py` & `je_api_testka_dev-0.0.98/je_api_testka/utils/mock_server/flask_mock_server.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.97/je_api_testka/utils/package_manager/package_manager_class.py` & `je_api_testka_dev-0.0.98/je_api_testka/utils/package_manager/package_manager_class.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.97/je_api_testka/utils/project/create_project_structure.py` & `je_api_testka_dev-0.0.98/je_api_testka/utils/project/create_project_structure.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.97/je_api_testka/utils/project/template/template_executor.py` & `je_api_testka_dev-0.0.98/je_api_testka/utils/project/template/template_executor.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.97/je_api_testka/utils/project/template/template_keyword.py` & `je_api_testka_dev-0.0.98/je_api_testka/utils/project/template/template_keyword.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.97/je_api_testka/utils/scheduler/extend_apscheduler.py` & `je_api_testka_dev-0.0.98/je_api_testka/utils/scheduler/extend_apscheduler.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,28 @@
 
 
 class SchedulerManager(object):
 
     def __init__(self):
         self._blocking_schedulers: BlockingScheduler = BlockingScheduler()
         self._background_schedulers: BackgroundScheduler = BackgroundScheduler()
+        self.blocking_scheduler_event_dict = {
+            "secondly": self.add_interval_blocking_secondly,
+            "minutely": self.add_interval_blocking_minutely,
+            "hourly": self.add_interval_blocking_hourly,
+            "daily": self.add_interval_blocking_daily,
+            "weekly": self.add_interval_blocking_weekly,
+        }
+        self.nonblocking_scheduler_event_dict = {
+            "secondly": self.add_interval_nonblocking_secondly,
+            "minutely": self.add_interval_nonblocking_minutely,
+            "hourly": self.add_interval_nonblocking_hourly,
+            "daily": self.add_interval_nonblocking_daily,
+            "weekly": self.add_interval_nonblocking_weekly,
+        }
 
     def add_blocking_job(
             self, func: Callable, trigger: str = None, args: Union[list, tuple] = None,
             kwargs: dict = None, id: str = None, name: str = None,
             misfire_grace_time: int = undefined, coalesce: bool = undefined, max_instances: int = undefined,
             next_run_time: datetime = undefined, jobstore: str = 'default', executor: str = 'default',
             replace_existing: bool = False, **trigger_args: Any) -> Job:
@@ -192,7 +206,10 @@
         return self._background_schedulers.remove_job(job_id=id, jobstore=jobstore)
 
     def shutdown_blocking_scheduler(self, wait: bool = False) -> None:
         self._blocking_schedulers.shutdown(wait=wait)
 
     def shutdown_nonblocking_scheduler(self, wait: bool = False) -> None:
         self._background_schedulers.shutdown(wait=wait)
+
+
+scheduler_manager = SchedulerManager()
```

### Comparing `je_api_testka_dev-0.0.97/je_api_testka/utils/socket_server/api_testka_socket_server.py` & `je_api_testka_dev-0.0.98/je_api_testka/utils/socket_server/api_testka_socket_server.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.97/je_api_testka/utils/xml/change_xml_structure/change_xml_structure.py` & `je_api_testka_dev-0.0.98/je_api_testka/utils/xml/change_xml_structure/change_xml_structure.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.97/je_api_testka/utils/xml/xml_file/xml_file.py` & `je_api_testka_dev-0.0.98/je_api_testka/utils/xml/xml_file/xml_file.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.97/je_api_testka_dev.egg-info/PKG-INFO` & `je_api_testka_dev-0.0.98/je_api_testka_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je-api-testka-dev
-Version: 0.0.97
+Version: 0.0.98
 Summary: Requests Automation Framework
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/APITestka
 Project-URL: Documentation, https://apitestka.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/APITestka
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `je_api_testka_dev-0.0.97/je_api_testka_dev.egg-info/SOURCES.txt` & `je_api_testka_dev-0.0.98/je_api_testka_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.97/pyproject.toml` & `je_api_testka_dev-0.0.98/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is dev version
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "je_api_testka_dev"
-version = "0.0.97"
+version = "0.0.98"
 authors = [
     { name = "JE-Chen", email = "jechenmailman@gmail.com" },
 ]
 description = "Requests Automation Framework"
 requires-python = ">=3.8"
 license = { text = "MIT" }
 dependencies = [
```

