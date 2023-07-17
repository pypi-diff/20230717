# Comparing `tmp/ssh_terminal_manager-0.7.0.tar.gz` & `tmp/ssh_terminal_manager-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_terminal_manager-0.7.0.tar", last modified: Sun Jul 16 06:16:04 2023, max compression
+gzip compressed data, was "ssh_terminal_manager-0.8.0.tar", last modified: Mon Jul 17 06:07:01 2023, max compression
```

## Comparing `ssh_terminal_manager-0.7.0.tar` & `ssh_terminal_manager-0.8.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-16 06:16:04.003744 ssh_terminal_manager-0.7.0/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.7.0/LICENSE
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      820 2023-07-16 06:16:04.003744 ssh_terminal_manager-0.7.0/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      223 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.7.0/README.md
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      802 2023-07-16 06:13:09.000000 ssh_terminal_manager-0.7.0/pyproject.toml
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-16 06:16:04.003744 ssh_terminal_manager-0.7.0/setup.cfg
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-16 06:16:03.999744 ssh_terminal_manager-0.7.0/src/
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-16 06:16:03.999744 ssh_terminal_manager-0.7.0/src/ssh_terminal_manager/
--rw-r--r--   0 adrian    (1000) adrian    (1000)     8529 2023-07-16 04:48:17.000000 ssh_terminal_manager-0.7.0/src/ssh_terminal_manager/__init__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      393 2023-07-15 08:37:34.000000 ssh_terminal_manager-0.7.0/src/ssh_terminal_manager/errors.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-16 06:16:03.999744 ssh_terminal_manager-0.7.0/src/ssh_terminal_manager.egg-info/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      820 2023-07-16 06:16:03.000000 ssh_terminal_manager-0.7.0/src/ssh_terminal_manager.egg-info/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      343 2023-07-16 06:16:03.000000 ssh_terminal_manager-0.7.0/src/ssh_terminal_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-16 06:16:03.000000 ssh_terminal_manager-0.7.0/src/ssh_terminal_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       70 2023-07-16 06:16:03.000000 ssh_terminal_manager-0.7.0/src/ssh_terminal_manager.egg-info/requires.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       21 2023-07-16 06:16:03.000000 ssh_terminal_manager-0.7.0/src/ssh_terminal_manager.egg-info/top_level.txt
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-17 06:07:01.708061 ssh_terminal_manager-0.8.0/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.8.0/LICENSE
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      820 2023-07-17 06:07:01.708061 ssh_terminal_manager-0.8.0/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      223 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.8.0/README.md
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      802 2023-07-17 05:58:51.000000 ssh_terminal_manager-0.8.0/pyproject.toml
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-17 06:07:01.708061 ssh_terminal_manager-0.8.0/setup.cfg
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-17 06:07:01.704061 ssh_terminal_manager-0.8.0/src/
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-17 06:07:01.708061 ssh_terminal_manager-0.8.0/src/ssh_terminal_manager/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     8701 2023-07-17 06:05:19.000000 ssh_terminal_manager-0.8.0/src/ssh_terminal_manager/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      393 2023-07-16 06:39:54.000000 ssh_terminal_manager-0.8.0/src/ssh_terminal_manager/errors.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-17 06:07:01.708061 ssh_terminal_manager-0.8.0/src/ssh_terminal_manager.egg-info/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      820 2023-07-17 06:07:01.000000 ssh_terminal_manager-0.8.0/src/ssh_terminal_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      343 2023-07-17 06:07:01.000000 ssh_terminal_manager-0.8.0/src/ssh_terminal_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-17 06:07:01.000000 ssh_terminal_manager-0.8.0/src/ssh_terminal_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       70 2023-07-17 06:07:01.000000 ssh_terminal_manager-0.8.0/src/ssh_terminal_manager.egg-info/requires.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       21 2023-07-17 06:07:01.000000 ssh_terminal_manager-0.8.0/src/ssh_terminal_manager.egg-info/top_level.txt
```

### Comparing `ssh_terminal_manager-0.7.0/LICENSE` & `ssh_terminal_manager-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ssh_terminal_manager-0.7.0/pyproject.toml` & `ssh_terminal_manager-0.8.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ssh_terminal_manager"
-version = "0.7.0"
+version = "0.8.0"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Use terminal commands to control and monitor remote devices"
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.10"
 classifiers = [
-  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.10",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 keywords = [
   "ssh", 
   "terminal", 
   "command line",
 ]
 dependencies = [
   "icmplib >= 3.0",
   "paramiko >= 3.2.0",
-  "terminal-manager >= 0.7.0",
+  "terminal-manager >= 0.8.0",
   "wakeonlan >= 3.0.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/zhbjsh/ssh-terminal-manager"
 "Bug Tracker" = "https://github.com/zhbjsh/ssh-terminal-manager/issues"
```

### Comparing `ssh_terminal_manager-0.7.0/src/ssh_terminal_manager/__init__.py` & `ssh_terminal_manager-0.8.0/src/ssh_terminal_manager/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,16 +261,21 @@
         try:
             await self.async_connect()
         except SSHConnectError:
             if raise_errors:
                 raise
 
     async def async_turn_on(self) -> None:
-        """Turn on by Wake on LAN."""
+        """Turn on by Wake on LAN.
+
+        Raises:
+            ValueError
+        """
         if self.mac_address is None:
-            return
+            raise ValueError("No MAC Address set")
 
         wakeonlan.send_magic_packet(self.mac_address)
+        self.logger.debug("%s: Magic packet sent to %s", self.name, self.mac_address)
 
     def set_mac_address(self, mac_address: str | None) -> None:
         """Set the MAC address."""
         self._mac_address = mac_address
```

### Comparing `ssh_terminal_manager-0.7.0/src/ssh_terminal_manager.egg-info/PKG-INFO` & `ssh_terminal_manager-0.8.0/src/ssh_terminal_manager.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: ssh-terminal-manager
-Version: 0.7.0
+Version: 0.8.0
 Summary: Use terminal commands to control and monitor remote devices
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/ssh-terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-terminal-manager/issues
 Keywords: ssh,terminal,command line
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SSH Terminal Manager
 
 ## Initialize
```

