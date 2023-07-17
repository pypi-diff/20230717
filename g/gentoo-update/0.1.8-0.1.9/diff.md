# Comparing `tmp/gentoo-update-0.1.8.tar.gz` & `tmp/gentoo-update-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentoo-update-0.1.8.tar", last modified: Mon Jul 10 07:03:51 2023, max compression
+gzip compressed data, was "gentoo-update-0.1.9.tar", last modified: Mon Jul 17 20:44:07 2023, max compression
```

## Comparing `gentoo-update-0.1.8.tar` & `gentoo-update-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:03:51.525594 gentoo-update-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-10 07:03:39.000000 gentoo-update-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-10 07:03:39.000000 gentoo-update-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-10 07:03:51.525594 gentoo-update-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-10 07:03:39.000000 gentoo-update-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:03:51.525594 gentoo-update-0.1.8/gentoo_update/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-10 07:03:39.000000 gentoo-update-0.1.8/gentoo_update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 07:03:39.000000 gentoo-update-0.1.8/gentoo_update/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-07-10 07:03:39.000000 gentoo-update-0.1.8/gentoo_update/gentoo_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-07-10 07:03:39.000000 gentoo-update-0.1.8/gentoo_update/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:03:51.525594 gentoo-update-0.1.8/gentoo_update/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7390 2023-07-10 07:03:39.000000 gentoo-update-0.1.8/gentoo_update/scripts/updater.sh
--rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-07-10 07:03:39.000000 gentoo-update-0.1.8/gentoo_update/shell_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:03:51.525594 gentoo-update-0.1.8/gentoo_update.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-10 07:03:51.000000 gentoo-update-0.1.8/gentoo_update.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-10 07:03:51.000000 gentoo-update-0.1.8/gentoo_update.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 07:03:51.000000 gentoo-update-0.1.8/gentoo_update.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-10 07:03:51.000000 gentoo-update-0.1.8/gentoo_update.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 07:03:51.000000 gentoo-update-0.1.8/gentoo_update.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-10 07:03:51.525594 gentoo-update-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-10 07:03:39.000000 gentoo-update-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:03:51.525594 gentoo-update-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-10 07:03:39.000000 gentoo-update-0.1.8/tests/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:44:07.736160 gentoo-update-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-17 20:43:56.000000 gentoo-update-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-17 20:43:56.000000 gentoo-update-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-17 20:44:07.736160 gentoo-update-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-17 20:43:56.000000 gentoo-update-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:44:07.736160 gentoo-update-0.1.9/gentoo_update/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-17 20:43:56.000000 gentoo-update-0.1.9/gentoo_update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 20:43:56.000000 gentoo-update-0.1.9/gentoo_update/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-07-17 20:43:56.000000 gentoo-update-0.1.9/gentoo_update/gentoo_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-07-17 20:43:56.000000 gentoo-update-0.1.9/gentoo_update/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-07-17 20:43:56.000000 gentoo-update-0.1.9/gentoo_update/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:44:07.736160 gentoo-update-0.1.9/gentoo_update/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7396 2023-07-17 20:43:56.000000 gentoo-update-0.1.9/gentoo_update/scripts/updater.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-07-17 20:43:56.000000 gentoo-update-0.1.9/gentoo_update/shell_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:44:07.736160 gentoo-update-0.1.9/gentoo_update.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-17 20:44:07.000000 gentoo-update-0.1.9/gentoo_update.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-17 20:44:07.000000 gentoo-update-0.1.9/gentoo_update.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 20:44:07.000000 gentoo-update-0.1.9/gentoo_update.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-17 20:44:07.000000 gentoo-update-0.1.9/gentoo_update.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-17 20:44:07.000000 gentoo-update-0.1.9/gentoo_update.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-17 20:44:07.736160 gentoo-update-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-17 20:43:56.000000 gentoo-update-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:44:07.736160 gentoo-update-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-17 20:43:56.000000 gentoo-update-0.1.9/tests/test_updater.py
```

### Comparing `gentoo-update-0.1.8/LICENSE` & `gentoo-update-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gentoo-update-0.1.8/PKG-INFO` & `gentoo-update-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gentoo-update
-Version: 0.1.8
+Version: 0.1.9
 Summary: Gentoo Linux updater
 Home-page: https://github.com/Lab-Brat/gentoo_update
 Author: Lab-Brat
 Author-email: labbrat_social@pm.me
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gentoo-update-0.1.8/README.md` & `gentoo-update-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `gentoo-update-0.1.8/gentoo_update/parser.py` & `gentoo-update-0.1.9/gentoo_update/parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import re
-from pprint import pprint
 from typing import Dict, List, Tuple
 
 
 class Parser:
     def __init__(self, log_file: str) -> None:
         """
         Initialize the Parser with a log file.
@@ -70,23 +69,100 @@
             pretend_status = True
             pretend_details = None
             return {
                 "pretend_status": pretend_status,
                 "pretend_details": pretend_details,
             }
         else:
-            pretend_status = {"pretend_status": False}
+            pretend_status = False
             # function to parse errors during emerge --pretend
-            # pretend_details = parse_pretend_details(section_content)
-            pretend_details = {"error_type": "", "error_details": ""}
+            pretend_details = self.parse_pretend_details(section_content)
             return {
                 "pretend_status": pretend_status,
                 "pretend_details": pretend_details,
             }
 
+    def _parse_pretend_get_blocked_details(
+        self, error_content: List[str]
+    ) -> List[str]:
+        """
+        Parse details of blocked package error.
+
+        Parameters:
+            error_content (List[str]): Lines from log marked as ERROR by logger.
+
+        Returns:
+            List[str]: Parsed packages tht cause the error.
+        """
+        blocked_packages = []
+        for line in error_content:
+            match_package_pattern = re.search(r"^\((.+?)\)", line)
+            if match_package_pattern:
+                blocked_packages.append(match_package_pattern.group(1))
+
+        return blocked_packages
+
+    def _parse_pretend_get_error_type(
+        self, error_content
+    ) -> Tuple[str, str, List[str]]:
+        """
+        Parse error type and error details.
+
+        Parameters:
+            error_content (List[str]): Lines from log marked as ERROR by logger.
+
+        Returns:
+            Tuple[str, str, List[str]]: Return error type, error definition as strings
+                and error details as a list of strings.
+        """
+        error_type = "undefined"
+        error_definition = "undefined"
+        error_details = "undefined"
+
+        for line in error_content:
+            if "Blocked Packages" in line:
+                error_type = "Blocked Packages"
+                error_details = self._parse_pretend_get_blocked_details(
+                    error_content
+                )
+
+        for line in error_content:
+            if line[0] == "*":
+                error_definition += f"{line[2:]} "
+
+        return (error_type, error_definition, error_details)
+
+    def parse_pretend_details(self, section_content: List[str]) -> Dict:
+        """
+        Parse information about the emerge pretend from logs.
+
+        Parameters:
+            section_content (List[str]): A list where each item is
+                one line of logs from a section.
+
+        Returns:
+            List[Dict]: A list of dictionaries where each item is
+                a named dictionary containing useful information for the report.
+        """
+        error_index = section_content.index(
+            "emerge pretend has failed, exiting"
+        )
+        error_content = [
+            line for line in section_content[error_index + 1 :] if line
+        ]
+
+        error_type, _, error_details = self._parse_pretend_get_error_type(
+            error_content
+        )
+        pretend_details = {
+            "error_type": error_type,
+            "error_details": error_details,
+        }
+        return pretend_details
+
     def parse_update_system_section(self, section_content: List[str]) -> Dict:
         """
         Function to parse the "update system" section of the log data.
 
         Parameters:
             section_content (List[str]): A list of strings that contains
                     the content of the "update system" section.
@@ -97,23 +173,25 @@
         """
         update_type = section_content[1].split()[1]
         if "update was successful" in section_content:
             update_status = True
             package_list = self.parse_update_details(section_content)
             update_details = {"updated_packages": package_list}
             return {
+                "update_type": update_type,
                 "update_status": update_status,
                 "update_details": update_details,
             }
         else:
             update_status = False
             # function to parse emerge update errors
             # update_details = parse_update_error_details(section_content, type)
             update_details = {"updated_packages": [], "errors": []}
             return {
+                "update_type": update_type,
                 "update_status": update_status,
                 "update_details": update_details,
             }
 
     def _parse_update_get_packages_names(
         self, name_and_version: str
     ) -> Tuple[str, str]:
@@ -160,15 +238,15 @@
             List[Dict]: A list of dictionaries where each item is
                 a named dictionary containing useful information for the report.
         """
         ebuild_info_pattern = r"\[(.+?)\]"
         package_strings = [
             line
             for line in section_content
-            if re.search(ebuild_info_pattern, line)
+            if re.search(ebuild_info_pattern, line) and line != "[ ok ]"
         ]
         packages = []
         for line in package_strings:
             chunks = re.findall(r'\S+=".*?"|\[.*?\]|\S+', line)
             package_name, new_version = self._parse_update_get_packages_names(
                 chunks[1]
             )
@@ -250,86 +328,7 @@
                 )
             elif "calculate_disk_usage" in section:
                 info["disk_usage"][section] = self.parse_disk_usage_info(
                     section_content
                 )
 
         return info
-
-    def create_failed_report(
-        self, update_info: List[Dict], disk_usage_info: Dict
-    ) -> List[str]:
-        """
-        Create a report when update failes.
-
-        Parameters:
-            update_info (List[Dict]): Update information parsed by
-                self.parse_update_details.
-            disk_usage_inf (Dict): Disk usage information parsed by
-                self.parse_disk_usage_info.
-
-        Returns:
-            List: A list of strings that comprise the failed update report.
-        """
-        # do failed report processing
-        return []
-
-    def create_successful_report(
-        self, update_info: List[Dict], disk_usage_info: Dict
-    ) -> List[str]:
-        """
-        Create a report when update succeeds.
-
-        Parameters:
-            update_info (List[Dict]): Update information parsed by
-                self.parse_update_details.
-            disk_usage_inf (Dict): Disk usage information parsed by
-                self.parse_disk_usage_info.
-
-        Returns:
-            List: A list of strings that comprise the successful update report.
-        """
-        report = [
-            "==========> Gentoo Update Report <==========",
-            "update status: SUCCESS",
-        ]
-        updated_packages = update_info["update_details"]["updated_packages"]
-        if updated_packages:
-            report.append(r"processed packages:")
-            for package in updated_packages:
-                package_name = list(package.keys())[0]
-                new_version = package[package_name]["New Version"]
-                old_version = package[package_name]["Old Version"]
-                report.append(
-                    f"--- {package_name} {old_version}->{new_version}"
-                )
-            report.append("")
-
-            disk_usage_before = disk_usage_info["calculate_disk_usage_1"]
-            disk_usage_after = disk_usage_info["calculate_disk_usage_2"]
-            disk_usage_stats = (
-                "Disk Usage Stats:\n"
-                f"Free Space {disk_usage_before['Free']} => {disk_usage_after['Free']}\n"
-                f"Used Space {disk_usage_before['Used']} => {disk_usage_after['Used']}\n"
-                f"Used pc(%) {disk_usage_before['Percent used']} => {disk_usage_after['Percent used']}\n"
-            )
-            report.append(disk_usage_stats)
-
-        return report
-
-    def create_report(self) -> List[str]:
-        """
-        Create a report.
-
-        Returns:
-            List: A list of strings that comprise the update report.
-        """
-        info = self.extract_info_for_report()
-        update_info = info["update_system"]
-        disk_usage_info = info["disk_usage"]
-        update_success = update_info["update_status"]
-        if update_success:
-            report = self.create_successful_report(update_info, disk_usage_info)
-            return report
-        else:
-            report = self.create_failed_report(update_info, disk_usage_info)
-            return report
```

### Comparing `gentoo-update-0.1.8/gentoo_update/scripts/updater.sh` & `gentoo-update-0.1.9/gentoo_update/scripts/updater.sh`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     while read -r line; do
         if [[ "${line}" = \#* ]] || [[ -z "${line}" ]]; then
             continue
         fi
 
         mount_point=$(echo "${line}" | awk '{print $2}')
 
-        if [[ ${mount_point} = "/tmp" || ${mount_point} = "swap" ]]; then
+        if [[ ${mount_point} = "/tmp" || "${mount_point}" = "swap" ]]; then
             continue
         fi
 
         if [[ ! -d "${mount_point}" ]]; then
             echo "Warning: mount point ${mount_point} does not exist."
             continue
         fi
@@ -38,15 +38,15 @@
         mount_point_found=true
 
         df -h "${mount_point}" |
             awk -v OFS=", " 'NR==2 {print "Disk usage for " "'"${mount_point}"'"" ===> Total=" $2, "Used=" $3, "Free=" $4, "Percent used=" $5}'
 
     done </etc/fstab
 
-    if [[ $mount_point_found == false ]]; then
+    if [[ "${mount_point_found}" == false ]]; then
         df -h "/" |
             awk -v OFS=", " 'NR==2 {print "Disk usage for " "/"" ===> Total=" $2, "Used=" $3, "Free=" $4, "Percent used=" $5}'
     fi
 }
 
 function check_disk_usage_before_update() {
     echo -e "\n{{ CALCULATE DISK USAGE 1 }}\n"
```

### Comparing `gentoo-update-0.1.8/gentoo_update/shell_runner.py` & `gentoo-update-0.1.9/gentoo_update/shell_runner.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,90 +1,29 @@
 import os
 import sys
 import logging
 import subprocess
-import pprint
-from configparser import ConfigParser
 from datetime import datetime
-from typing import Tuple, List
-from .parser import Parser
+from typing import List
 
 
 class ShellRunner:
-    def __init__(self, quiet: str, report: str) -> None:
+    def __init__(self, quiet: str, log_dir: str, log_dir_messages: str) -> None:
         self.quiet = True if quiet == "y" else False
 
         self.timestamp = datetime.now().strftime("%Y-%m-%d-%H-%M")
-        self.make_conf = self.make_conf_reader()
-        self.log_dir, self.log_dir_messages = self.initiate_log_directory()
-
-        self.report = True if report == "y" else False
-        if self.report:
-            self.show_last_report()
+        self.log_dir = log_dir
+        self.log_dir_messages = log_dir_messages
 
         self.log_filename = f"{self.log_dir}/log_{self.timestamp}"
         self.logger = self.initiate_logger()
 
         self.script_dir = os.path.join(os.path.dirname(__file__), "scripts")
         self.script_path = os.path.join(self.script_dir, "updater.sh")
 
-    def make_conf_reader(self) -> ConfigParser:
-        """
-        Read /etc/portage/make.conf with configparser.
-
-        Returns:
-            configparser.ConfigParser: ConfigParser object.
-        """
-        config = ConfigParser()
-        with open("/etc/portage/make.conf") as config_string:
-            config.read_string("[DEFAULT]\n" + config_string.read())
-        return config
-
-    def initiate_log_directory(self) -> Tuple[str, List[str]]:
-        """
-        Create log directory if it does not exist.
-        If PORTAGE_LOGDIR is not set, use the default directory.
-
-        Returns:
-            str: Log directory path.
-            List[str]: List of messages to be logged.
-        """
-        try:
-            log_dir = self.make_conf["DEFAULT"]["PORTAGE_LOGDIR"]
-        except KeyError:
-            log_dir = ""
-
-        log_dir_messages = []
-        if log_dir == "":
-            log_dir = "/var/log/portage/gentoo-update"
-            log_dir_messages.append(
-                f"PORTAGE_LOGDIR not set, using default: {log_dir}"
-            )
-        else:
-            log_dir = log_dir.replace('"', "")
-            log_dir = f"{log_dir}/gentoo-update"
-            log_dir_messages.append(f"PORTAGE_LOGDIR set, using: {log_dir}")
-
-        if not os.path.exists(log_dir):
-            os.mkdir(log_dir)
-            log_dir_messages.append(f"Created log directory: {log_dir}")
-
-        return log_dir, log_dir_messages
-
-    def show_last_report(self):
-        """
-        Show report for the last log located in $PORTAGE_LOGDIR.
-        """
-        files = os.listdir(self.log_dir)
-        paths = [os.path.join(self.log_dir, basename) for basename in files]
-        last_log = max(paths, key=os.path.getctime)
-        report = Parser(last_log).extract_info_for_report()
-        pprint.pprint(report)
-        sys.exit(0)
-
     def initiate_logger(self) -> logging.Logger:
         """
         Create a logger with two handlers:
             1. terminal output
             2. file output
         Both handlers have the same logging level (INFO)
         and share the same formatter.
@@ -217,16 +156,19 @@
         final_message = f"gentoo-update is done! Log:file: {self.log_filename}"
         self.logger.info(final_message)
         if self.quiet:
             print(final_message)
 
     def __del__(self) -> None:
         """
-        Closed all file handlers after ShellRunner is closed.
+        Close all file handlers after ShellRunner is closed.
         """
         try:
             if self.logger:
                 for handler in self.logger.handlers:
-                    handler.close()
-                    self.logger.removeHandler(handler)
+                    try:
+                        handler.close()
+                        self.logger.removeHandler(handler)
+                    except:
+                        "Log Handler Error: Could not close handler"
         except AttributeError:
-            pass
+            print("Log Hanlder Error: Logger object was not defined")
```

### Comparing `gentoo-update-0.1.8/gentoo_update.egg-info/PKG-INFO` & `gentoo-update-0.1.9/gentoo_update.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gentoo-update
-Version: 0.1.8
+Version: 0.1.9
 Summary: Gentoo Linux updater
 Home-page: https://github.com/Lab-Brat/gentoo_update
 Author: Lab-Brat
 Author-email: labbrat_social@pm.me
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gentoo-update-0.1.8/setup.cfg` & `gentoo-update-0.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `gentoo-update-0.1.8/tests/test_updater.py` & `gentoo-update-0.1.9/tests/test_updater.py`

 * *Files identical despite different names*

