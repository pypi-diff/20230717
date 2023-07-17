# Comparing `tmp/matrix-nio-0.8.0.tar.gz` & `tmp/matrix-nio-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/matrix-nio-0.8.0.tar", last modified: Fri Feb 21 15:30:04 2020, max compression
+gzip compressed data, was "dist/matrix-nio-0.9.0.tar", last modified: Thu Feb 27 16:47:08 2020, max compression
```

## Comparing `matrix-nio-0.8.0.tar` & `matrix-nio-0.9.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 poljar    (1000) poljar    (1000)        0 2020-02-21 15:30:04.306733 matrix-nio-0.8.0/
--rw-r--r--   0 poljar    (1000) poljar    (1000)       17 2020-01-09 10:01:32.000000 matrix-nio-0.8.0/MANIFEST.in
--rw-r--r--   0 poljar    (1000) poljar    (1000)      605 2020-01-09 10:01:32.000000 matrix-nio-0.8.0/Makefile
--rw-r--r--   0 poljar    (1000) poljar    (1000)     4229 2020-02-21 15:30:04.306733 matrix-nio-0.8.0/PKG-INFO
--rw-r--r--   0 poljar    (1000) poljar    (1000)     3073 2020-01-09 10:01:32.000000 matrix-nio-0.8.0/README.md
-drwxr-xr-x   0 poljar    (1000) poljar    (1000)        0 2020-02-21 15:30:04.303400 matrix-nio-0.8.0/matrix_nio.egg-info/
--rw-r--r--   0 poljar    (1000) poljar    (1000)     4229 2020-02-21 15:30:04.000000 matrix-nio-0.8.0/matrix_nio.egg-info/PKG-INFO
--rw-r--r--   0 poljar    (1000) poljar    (1000)     1133 2020-02-21 15:30:04.000000 matrix-nio-0.8.0/matrix_nio.egg-info/SOURCES.txt
--rw-r--r--   0 poljar    (1000) poljar    (1000)        1 2020-02-21 15:30:04.000000 matrix-nio-0.8.0/matrix_nio.egg-info/dependency_links.txt
--rw-r--r--   0 poljar    (1000) poljar    (1000)        1 2020-02-14 14:23:13.000000 matrix-nio-0.8.0/matrix_nio.egg-info/not-zip-safe
--rw-r--r--   0 poljar    (1000) poljar    (1000)      247 2020-02-21 15:30:04.000000 matrix-nio-0.8.0/matrix_nio.egg-info/requires.txt
--rw-r--r--   0 poljar    (1000) poljar    (1000)        4 2020-02-21 15:30:04.000000 matrix-nio-0.8.0/matrix_nio.egg-info/top_level.txt
-drwxr-xr-x   0 poljar    (1000) poljar    (1000)        0 2020-02-21 15:30:04.306733 matrix-nio-0.8.0/nio/
--rw-r--r--   0 poljar    (1000) poljar    (1000)      291 2020-01-09 10:01:32.000000 matrix-nio-0.8.0/nio/__init__.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)     1415 2020-01-09 10:01:32.000000 matrix-nio-0.8.0/nio/_compat.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)    45018 2020-02-16 18:24:07.000000 matrix-nio-0.8.0/nio/api.py
-drwxr-xr-x   0 poljar    (1000) poljar    (1000)        0 2020-02-21 15:30:04.306733 matrix-nio-0.8.0/nio/client/
--rw-r--r--   0 poljar    (1000) poljar    (1000)      228 2020-01-09 10:01:32.000000 matrix-nio-0.8.0/nio/client/__init__.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)    79588 2020-02-16 18:24:07.000000 matrix-nio-0.8.0/nio/client/async_client.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)    44406 2020-02-15 12:10:25.000000 matrix-nio-0.8.0/nio/client/base_client.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)    43950 2020-02-10 10:01:46.000000 matrix-nio-0.8.0/nio/client/http_client.py
-drwxr-xr-x   0 poljar    (1000) poljar    (1000)        0 2020-02-21 15:30:04.306733 matrix-nio-0.8.0/nio/crypto/
--rw-r--r--   0 poljar    (1000) poljar    (1000)     1165 2020-01-09 10:01:32.000000 matrix-nio-0.8.0/nio/crypto/__init__.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)     4754 2020-01-09 10:01:32.000000 matrix-nio-0.8.0/nio/crypto/async_attachments.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)     4776 2020-01-09 10:01:32.000000 matrix-nio-0.8.0/nio/crypto/attachments.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)     4499 2020-01-09 10:01:32.000000 matrix-nio-0.8.0/nio/crypto/key_export.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)      929 2020-01-09 10:01:32.000000 matrix-nio-0.8.0/nio/crypto/log.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)     6230 2020-01-09 10:01:32.000000 matrix-nio-0.8.0/nio/crypto/memorystores.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)    83732 2020-02-14 12:46:15.000000 matrix-nio-0.8.0/nio/crypto/olm_machine.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)    23727 2020-02-10 10:01:46.000000 matrix-nio-0.8.0/nio/crypto/sas.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)    11209 2020-01-09 10:01:32.000000 matrix-nio-0.8.0/nio/crypto/sessions.py
-drwxr-xr-x   0 poljar    (1000) poljar    (1000)        0 2020-02-21 15:30:04.306733 matrix-nio-0.8.0/nio/event_builders/
--rw-r--r--   0 poljar    (1000) poljar    (1000)      386 2020-01-09 10:01:32.000000 matrix-nio-0.8.0/nio/event_builders/__init__.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)     1782 2020-01-09 10:01:32.000000 matrix-nio-0.8.0/nio/event_builders/direct_messages.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)     1128 2020-01-09 10:01:32.000000 matrix-nio-0.8.0/nio/event_builders/event_builder.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)     5681 2020-01-09 10:01:32.000000 matrix-nio-0.8.0/nio/event_builders/state_events.py
-drwxr-xr-x   0 poljar    (1000) poljar    (1000)        0 2020-02-21 15:30:04.306733 matrix-nio-0.8.0/nio/events/
--rw-r--r--   0 poljar    (1000) poljar    (1000)      461 2020-01-09 10:01:32.000000 matrix-nio-0.8.0/nio/events/__init__.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)     3569 2020-01-09 10:01:32.000000 matrix-nio-0.8.0/nio/events/account_data.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)     2629 2020-01-09 10:01:32.000000 matrix-nio-0.8.0/nio/events/ephemeral.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)     6640 2020-01-09 10:01:32.000000 matrix-nio-0.8.0/nio/events/invite_events.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)     6518 2020-01-09 10:01:32.000000 matrix-nio-0.8.0/nio/events/misc.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)    45822 2020-02-21 09:25:29.000000 matrix-nio-0.8.0/nio/events/room_events.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)    17159 2020-01-09 10:01:32.000000 matrix-nio-0.8.0/nio/events/to_device.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)     1602 2020-01-09 10:01:32.000000 matrix-nio-0.8.0/nio/exceptions.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)    17848 2020-01-09 10:01:32.000000 matrix-nio-0.8.0/nio/http.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)      894 2020-01-09 10:01:32.000000 matrix-nio-0.8.0/nio/log.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)     6974 2020-01-09 10:01:32.000000 matrix-nio-0.8.0/nio/monitors.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)    46255 2020-02-16 18:24:07.000000 matrix-nio-0.8.0/nio/responses.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)    15508 2020-01-09 10:01:32.000000 matrix-nio-0.8.0/nio/rooms.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)    55844 2020-02-21 09:25:29.000000 matrix-nio-0.8.0/nio/schemas.py
-drwxr-xr-x   0 poljar    (1000) poljar    (1000)        0 2020-02-21 15:30:04.306733 matrix-nio-0.8.0/nio/store/
--rw-r--r--   0 poljar    (1000) poljar    (1000)     1396 2020-01-09 10:01:32.000000 matrix-nio-0.8.0/nio/store/__init__.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)    45975 2020-01-09 10:01:32.000000 matrix-nio-0.8.0/nio/store/database.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)     5169 2020-02-10 10:01:46.000000 matrix-nio-0.8.0/nio/store/file_trustdb.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)      930 2020-01-09 10:01:32.000000 matrix-nio-0.8.0/nio/store/log.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)     8101 2020-01-09 10:01:32.000000 matrix-nio-0.8.0/nio/store/models.py
--rw-r--r--   0 poljar    (1000) poljar    (1000)      133 2020-02-21 15:30:04.306733 matrix-nio-0.8.0/setup.cfg
--rw-r--r--   0 poljar    (1000) poljar    (1000)     1236 2020-02-21 15:21:17.000000 matrix-nio-0.8.0/setup.py
+drwxr-xr-x   0 poljar    (1000) poljar    (1000)        0 2020-02-27 16:47:08.226969 matrix-nio-0.9.0/
+-rw-r--r--   0 poljar    (1000) poljar    (1000)       17 2020-01-09 10:01:32.000000 matrix-nio-0.9.0/MANIFEST.in
+-rw-r--r--   0 poljar    (1000) poljar    (1000)      605 2020-01-09 10:01:32.000000 matrix-nio-0.9.0/Makefile
+-rw-r--r--   0 poljar    (1000) poljar    (1000)     4229 2020-02-27 16:47:08.226969 matrix-nio-0.9.0/PKG-INFO
+-rw-r--r--   0 poljar    (1000) poljar    (1000)     3073 2020-01-09 10:01:32.000000 matrix-nio-0.9.0/README.md
+drwxr-xr-x   0 poljar    (1000) poljar    (1000)        0 2020-02-27 16:47:08.226969 matrix-nio-0.9.0/matrix_nio.egg-info/
+-rw-r--r--   0 poljar    (1000) poljar    (1000)     4229 2020-02-27 16:47:08.000000 matrix-nio-0.9.0/matrix_nio.egg-info/PKG-INFO
+-rw-r--r--   0 poljar    (1000) poljar    (1000)     1133 2020-02-27 16:47:08.000000 matrix-nio-0.9.0/matrix_nio.egg-info/SOURCES.txt
+-rw-r--r--   0 poljar    (1000) poljar    (1000)        1 2020-02-27 16:47:08.000000 matrix-nio-0.9.0/matrix_nio.egg-info/dependency_links.txt
+-rw-r--r--   0 poljar    (1000) poljar    (1000)        1 2020-02-14 14:23:13.000000 matrix-nio-0.9.0/matrix_nio.egg-info/not-zip-safe
+-rw-r--r--   0 poljar    (1000) poljar    (1000)      247 2020-02-27 16:47:08.000000 matrix-nio-0.9.0/matrix_nio.egg-info/requires.txt
+-rw-r--r--   0 poljar    (1000) poljar    (1000)        4 2020-02-27 16:47:08.000000 matrix-nio-0.9.0/matrix_nio.egg-info/top_level.txt
+drwxr-xr-x   0 poljar    (1000) poljar    (1000)        0 2020-02-27 16:47:08.226969 matrix-nio-0.9.0/nio/
+-rw-r--r--   0 poljar    (1000) poljar    (1000)      291 2020-01-09 10:01:32.000000 matrix-nio-0.9.0/nio/__init__.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)     1415 2020-01-09 10:01:32.000000 matrix-nio-0.9.0/nio/_compat.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)    45018 2020-02-16 18:24:07.000000 matrix-nio-0.9.0/nio/api.py
+drwxr-xr-x   0 poljar    (1000) poljar    (1000)        0 2020-02-27 16:47:08.226969 matrix-nio-0.9.0/nio/client/
+-rw-r--r--   0 poljar    (1000) poljar    (1000)      228 2020-01-09 10:01:32.000000 matrix-nio-0.9.0/nio/client/__init__.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)    79588 2020-02-16 18:24:07.000000 matrix-nio-0.9.0/nio/client/async_client.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)    44406 2020-02-15 12:10:25.000000 matrix-nio-0.9.0/nio/client/base_client.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)    43950 2020-02-10 10:01:46.000000 matrix-nio-0.9.0/nio/client/http_client.py
+drwxr-xr-x   0 poljar    (1000) poljar    (1000)        0 2020-02-27 16:47:08.226969 matrix-nio-0.9.0/nio/crypto/
+-rw-r--r--   0 poljar    (1000) poljar    (1000)     1165 2020-01-09 10:01:32.000000 matrix-nio-0.9.0/nio/crypto/__init__.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)     4754 2020-01-09 10:01:32.000000 matrix-nio-0.9.0/nio/crypto/async_attachments.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)     4776 2020-01-09 10:01:32.000000 matrix-nio-0.9.0/nio/crypto/attachments.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)     4499 2020-01-09 10:01:32.000000 matrix-nio-0.9.0/nio/crypto/key_export.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)      929 2020-01-09 10:01:32.000000 matrix-nio-0.9.0/nio/crypto/log.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)     6230 2020-01-09 10:01:32.000000 matrix-nio-0.9.0/nio/crypto/memorystores.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)    87525 2020-02-27 16:35:00.000000 matrix-nio-0.9.0/nio/crypto/olm_machine.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)    23727 2020-02-10 10:01:46.000000 matrix-nio-0.9.0/nio/crypto/sas.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)    11574 2020-02-27 13:35:51.000000 matrix-nio-0.9.0/nio/crypto/sessions.py
+drwxr-xr-x   0 poljar    (1000) poljar    (1000)        0 2020-02-27 16:47:08.226969 matrix-nio-0.9.0/nio/event_builders/
+-rw-r--r--   0 poljar    (1000) poljar    (1000)      386 2020-01-09 10:01:32.000000 matrix-nio-0.9.0/nio/event_builders/__init__.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)     2503 2020-02-27 16:01:35.000000 matrix-nio-0.9.0/nio/event_builders/direct_messages.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)     1128 2020-01-09 10:01:32.000000 matrix-nio-0.9.0/nio/event_builders/event_builder.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)     5681 2020-01-09 10:01:32.000000 matrix-nio-0.9.0/nio/event_builders/state_events.py
+drwxr-xr-x   0 poljar    (1000) poljar    (1000)        0 2020-02-27 16:47:08.226969 matrix-nio-0.9.0/nio/events/
+-rw-r--r--   0 poljar    (1000) poljar    (1000)      461 2020-01-09 10:01:32.000000 matrix-nio-0.9.0/nio/events/__init__.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)     3569 2020-01-09 10:01:32.000000 matrix-nio-0.9.0/nio/events/account_data.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)     2629 2020-01-09 10:01:32.000000 matrix-nio-0.9.0/nio/events/ephemeral.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)     6640 2020-01-09 10:01:32.000000 matrix-nio-0.9.0/nio/events/invite_events.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)     6518 2020-01-09 10:01:32.000000 matrix-nio-0.9.0/nio/events/misc.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)    46471 2020-02-27 15:21:02.000000 matrix-nio-0.9.0/nio/events/room_events.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)    17159 2020-01-09 10:01:32.000000 matrix-nio-0.9.0/nio/events/to_device.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)     1602 2020-01-09 10:01:32.000000 matrix-nio-0.9.0/nio/exceptions.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)    17848 2020-01-09 10:01:32.000000 matrix-nio-0.9.0/nio/http.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)      894 2020-01-09 10:01:32.000000 matrix-nio-0.9.0/nio/log.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)     6974 2020-01-09 10:01:32.000000 matrix-nio-0.9.0/nio/monitors.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)    46255 2020-02-16 18:24:07.000000 matrix-nio-0.9.0/nio/responses.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)    15508 2020-01-09 10:01:32.000000 matrix-nio-0.9.0/nio/rooms.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)    55844 2020-02-21 09:25:29.000000 matrix-nio-0.9.0/nio/schemas.py
+drwxr-xr-x   0 poljar    (1000) poljar    (1000)        0 2020-02-27 16:47:08.226969 matrix-nio-0.9.0/nio/store/
+-rw-r--r--   0 poljar    (1000) poljar    (1000)     1396 2020-01-09 10:01:32.000000 matrix-nio-0.9.0/nio/store/__init__.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)    45975 2020-01-09 10:01:32.000000 matrix-nio-0.9.0/nio/store/database.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)     5169 2020-02-10 10:01:46.000000 matrix-nio-0.9.0/nio/store/file_trustdb.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)      930 2020-01-09 10:01:32.000000 matrix-nio-0.9.0/nio/store/log.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)     8101 2020-01-09 10:01:32.000000 matrix-nio-0.9.0/nio/store/models.py
+-rw-r--r--   0 poljar    (1000) poljar    (1000)      133 2020-02-27 16:47:08.226969 matrix-nio-0.9.0/setup.cfg
+-rw-r--r--   0 poljar    (1000) poljar    (1000)     1236 2020-02-27 16:44:45.000000 matrix-nio-0.9.0/setup.py
```

### Comparing `matrix-nio-0.8.0/Makefile` & `matrix-nio-0.9.0/Makefile`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/PKG-INFO` & `matrix-nio-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matrix-nio
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Python Matrix client library, designed according to sans I/O principles.
 Home-page: https://github.com/poljar/matrix-nio
 Author: Damir Jelić
 Author-email: poljar@termina.org.uk
 License: ISC
 Description: nio  
         ===
```

### Comparing `matrix-nio-0.8.0/README.md` & `matrix-nio-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/matrix_nio.egg-info/PKG-INFO` & `matrix-nio-0.9.0/matrix_nio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matrix-nio
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Python Matrix client library, designed according to sans I/O principles.
 Home-page: https://github.com/poljar/matrix-nio
 Author: Damir Jelić
 Author-email: poljar@termina.org.uk
 License: ISC
 Description: nio  
         ===
```

### Comparing `matrix-nio-0.8.0/matrix_nio.egg-info/SOURCES.txt` & `matrix-nio-0.9.0/matrix_nio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/nio/_compat.py` & `matrix-nio-0.9.0/nio/_compat.py`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/nio/api.py` & `matrix-nio-0.9.0/nio/api.py`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/nio/client/async_client.py` & `matrix-nio-0.9.0/nio/client/async_client.py`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/nio/client/base_client.py` & `matrix-nio-0.9.0/nio/client/base_client.py`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/nio/client/http_client.py` & `matrix-nio-0.9.0/nio/client/http_client.py`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/nio/crypto/__init__.py` & `matrix-nio-0.9.0/nio/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/nio/crypto/async_attachments.py` & `matrix-nio-0.9.0/nio/crypto/async_attachments.py`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/nio/crypto/attachments.py` & `matrix-nio-0.9.0/nio/crypto/attachments.py`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/nio/crypto/key_export.py` & `matrix-nio-0.9.0/nio/crypto/key_export.py`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/nio/crypto/log.py` & `matrix-nio-0.9.0/nio/crypto/log.py`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/nio/crypto/memorystores.py` & `matrix-nio-0.9.0/nio/crypto/memorystores.py`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/nio/crypto/olm_machine.py` & `matrix-nio-0.9.0/nio/crypto/olm_machine.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,16 @@
                           OlmUnverifiedDeviceError, VerificationError)
 from ..responses import (KeysClaimResponse, KeysQueryResponse,
                          KeysUploadResponse, RoomKeyRequestResponse,
                          ToDeviceResponse)
 from ..schemas import Schemas, validate_json
 from ..store import MatrixStore
 from .key_export import decrypt_and_read, encrypt_and_save
-from .sas import Sas, ToDeviceMessage
+from .sas import Sas
+from ..event_builders import ToDeviceMessage, DummyMessage, RoomKeyRequestMessage
 from .sessions import OutgoingKeyRequest
 
 try:
     from json.decoder import JSONDecodeError
 except ImportError:  # pragma: no cover
     JSONDecodeError = ValueError  # type: ignore
 
@@ -172,14 +173,21 @@
         # A list of devices for which we need to start a new Olm session.
         # Matrix clients need to do a one-time key claiming request for the
         # devices in this list. After a new session is created with the device
         # it will be removed from this list and a dummy encrypted message will
         # be queued to be sent as a to-device message.
         self.wedged_devices = list()  # type: List[OlmDevice]
 
+        # A cache of megolm events that failed to decrypt because the Olm
+        # session was wedged and thus the decryption key was missed.
+        # We need to unwedge the session and only then send out key re-requests,
+        # otherwise we might again fail to decrypt the Olm message.
+        self.key_re_requests_events = defaultdict(list)  \
+            # type: DefaultDict[Tuple[str, str], List[MegolmEvent]]
+
         # A mapping from a transaction id to a Sas key verification object. The
         # transaction id uniquely identifies the key verification session.
         self.key_verifications = dict()  # type: Dict[str, Sas]
 
         # A list of to-device messages that need to be sent to the homeserver
         # by the client. This will get populated by common to-device messages
         # for key-requests, interactive device verification and Olm session
@@ -363,15 +371,15 @@
     def _queue_dummy_message(self, session, device):
         olm_dict = self._olm_encrypt(session, device, "m.dummy", {})
 
         logger.info("Queuing a dummy Olm message for device {} of user "
                     "{}".format(device.device_id, device.user_id))
 
         self.outgoing_to_device_messages.append(
-            ToDeviceMessage(
+            DummyMessage(
                 "m.room.encrypted",
                 device.user_id,
                 device.device_id,
                 olm_dict
             )
         )
 
@@ -935,18 +943,44 @@
 
     def _mark_to_device_message_as_sent(self, message):
         """Mark a to-device message as sent.
 
         This removes the to-device message from our outgoing to-device list.
         """
 
-        # TODO if the to-device message was a m.dummy message resend key
-        # requests that were sent to the recipient of the message.
         try:
             self.outgoing_to_device_messages.remove(message)
+
+            if isinstance(message, DummyMessage):
+                # Queue up key requests to be sent out that happened because of
+                # this wedged session.
+                events = self.key_re_requests_events.pop((message.recipient, message.recipient_device), [])
+
+                requested_sessions = []
+
+                for event in events:
+                    # Don't send out key re-requests for the same session twice.
+                    # TODO filter this when putting the events in.
+                    if event.session_id in requested_sessions:
+                        continue
+
+                    message = event.as_key_request(event.sender, self.device_id,
+                                                   event.session_id, event.device_id)
+                    logger.info(f"Queuing a room key re-request for a unwedged "
+                                f"Olm session: {event.sender} {event.sender} "
+                                f"{event.session_id}.")
+                    self.outgoing_to_device_messages.append(message)
+
+                    requested_sessions.append(event.session_id)
+
+            elif isinstance(message, RoomKeyRequestMessage):
+                key_request = OutgoingKeyRequest.from_message(message)
+                self.outgoing_key_requests[message.request_id] = key_request
+                self.store.add_outgoing_key_request(key_request)
+
         except ValueError:
             pass
 
     def handle_response(self, response):
         if isinstance(response, KeysUploadResponse):
             self.account.shared = True
             self.uploaded_key_count = response.signed_curve25519_count
@@ -1406,14 +1440,54 @@
             return True
 
         if event_id != event.event_id or timestamp != event.server_timestamp:
             return False
 
         return True
 
+    def check_if_wedged(self, event: MegolmEvent):
+        """Check if a Megolm event failed decryption because they keys got lost
+        because of a wedged Olm session.
+        """
+        try:
+            device = self.device_store[event.sender][event.device_id]
+        except KeyError:
+            logger.warn(f"Received a undecryptable Megolm event from a unknown "
+                        f"device: {event.sender} {event.device_id}")
+            self.users_for_key_query.add(event.sender)
+            return
+
+        session = self.session_store.get(device.curve25519)
+
+        if not session:
+            logger.warn(f"Received a undecryptable Megolm event from a device "
+                        f"with no Olm sessions: {event.sender} {event.device_id}")
+            return
+
+        session_age = datetime.now() - session.creation_time
+
+        # We received a undecryptable Megolm event from a device that is
+        # currently wedged or has been recently unwedged. If it's recently
+        # unwedged send out a key request, otherwise queue up a key request to
+        # be sent out after we send the dummy message.
+        if (session_age < self._unwedging_interval and
+            event.session_id not in self.outgoing_key_requests):
+            logger.info(f"Received a undecryptable Megolm event from a device "
+                        f"that we recently established an Olm session with: "
+                        f"{event.sender} {event.device_id}.")
+            message = event.as_key_request(event.sender, self.device_id,
+                                           event.session_id, event.device_id)
+            self.outgoing_to_device_messages.append(message)
+
+        if device in self.wedged_devices:
+            logger.info(f"Received a undecryptable Megolm event from a device "
+                        f"that has a wedged Olm session: "
+                        f"{event.sender} {event.device_id}.")
+            self.key_re_requests_events[(device.user_id, device.device_id)].append(event)
+
     def decrypt_megolm_event(self, event, room_id=None):
         # type (MegolmEvent, Optional[str]) -> Union[Event, BadEvent]
         room_id = room_id or event.room_id
 
         if not room_id:
             raise EncryptionError("Event doesn't contain a room id")
 
@@ -1429,14 +1503,15 @@
             message = (
                 "Error decrypting megolm event, no session found "
                 "with session id {} for room {}".format(
                     event.session_id,
                     room_id
                 )
             )
+            self.check_if_wedged(event)
             logger.warn(message)
             raise EncryptionError(message)
 
         try:
             plaintext, message_index = session.decrypt(event.ciphertext)
         except OlmGroupSessionError as e:
             message = "Error decrypting megolm event: {}".format(str(e))
```

### Comparing `matrix-nio-0.8.0/nio/crypto/sas.py` & `matrix-nio-0.9.0/nio/crypto/sas.py`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/nio/crypto/sessions.py` & `matrix-nio-0.9.0/nio/crypto/sessions.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from enum import Enum
 from typing import Dict, List, Optional, Set, Tuple
 
 import attr
 import olm
 
 from ..exceptions import EncryptionError
-from ..event_builders import ToDeviceMessage
+from ..event_builders import ToDeviceMessage, RoomKeyRequestMessage
 
 if False:
     from ..responses import RoomKeyRequestResponse
 
 
 class OlmAccount(olm.Account):
     def __init__(self):
@@ -344,14 +344,25 @@
             response.request_id,
             response.session_id,
             response.room_id,
             response.algorithm
         )
 
     @classmethod
+    def from_message(cls, message):
+        # type: (RoomKeyRequestMessage) -> OutgoingKeyRequest
+        """Create a key request object from a RoomKeyRequestMessage."""
+        return cls(
+            message.request_id,
+            message.session_id,
+            message.room_id,
+            message.algorithm,
+        )
+
+    @classmethod
     def from_database(cls, row):
         """Create a key request object from a database row."""
         return cls.from_response(row)
 
     def as_cancellation(self, user_id, requesting_device_id):
         """Turn the key request into a cancellation to-device message."""
         content = {
```

### Comparing `matrix-nio-0.8.0/nio/event_builders/event_builder.py` & `matrix-nio-0.9.0/nio/event_builders/event_builder.py`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/nio/event_builders/state_events.py` & `matrix-nio-0.9.0/nio/event_builders/state_events.py`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/nio/events/account_data.py` & `matrix-nio-0.9.0/nio/events/account_data.py`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/nio/events/ephemeral.py` & `matrix-nio-0.9.0/nio/events/ephemeral.py`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/nio/events/invite_events.py` & `matrix-nio-0.9.0/nio/events/invite_events.py`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/nio/events/misc.py` & `matrix-nio-0.9.0/nio/events/misc.py`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/nio/events/room_events.py` & `matrix-nio-0.9.0/nio/events/room_events.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from typing import Any, Dict, Optional, Union
 
 import attr
 
 from ..schemas import Schemas
 from .misc import (BadEventType, UnknownBadEvent, validate_or_badevent, verify,
                    BadEvent)
-from ..event_builders import ToDeviceMessage
+from ..event_builders import RoomKeyRequestMessage
 
 
 @attr.s
 class Event(object):
     """Matrix Event class.
 
     This is the base event class, most events inherit from this class.
@@ -309,47 +309,59 @@
 
         event.sender_key = sender_key
         event.session_id = session_id
         event.transaction_id = tx_id
 
         return event
 
-    def as_key_request(self, user_id, requesting_device_id, request_id=None):
-        # type: (str, str, Optional[str]) -> ToDeviceMessage
+    def as_key_request(self, user_id, requesting_device_id, request_id=None, device_id=None):
+        # type: (str, str, Optional[str], Optional[str]) -> RoomKeyRequestMessage
         """Make a to-device message for a room key request.
 
         MegolmEvents are presented to library users only if the library fails
         to decrypt the event because of a missing session key.
 
         A missing key can be requested later on by sending a key request, this
         method creates a ToDeviceMessage that can be sent out if such a request
         should be made.
 
         Args:
             user_id (str): The user id of the user that should receive the key
                 request.
-
+            requesting_device_id (str): The device id of the user that is
+                requesting the key.
+            request_id (str, optional): A unique string identifying the request.
+                Defaults to the session id of the missing megolm session.
+            device_id (str, optional): The device id of the device that should
+                receive the request. Defaults to all the users devices.
         """
+        assert self.session_id
+        request_id = request_id or self.session_id
+
         content = {
             "action": "request",
             "body": {
                 "algorithm": self.algorithm,
                 "session_id": self.session_id,
                 "room_id": self.room_id,
                 "sender_key": self.sender_key
             },
-            "request_id": request_id or self.session_id,
+            "request_id": request_id,
             "requesting_device_id": requesting_device_id,
         }
 
-        return ToDeviceMessage(
+        return RoomKeyRequestMessage(
             "m.room_key_request",
             user_id,
-            "*",
-            content
+            device_id or "*",
+            content,
+            request_id,
+            self.session_id,
+            self.room_id,
+            self.algorithm,
         )
 
 
 @attr.s
 class CallEvent(Event):
     """Base Class for Matrix call signalling events.
```

### Comparing `matrix-nio-0.8.0/nio/events/to_device.py` & `matrix-nio-0.9.0/nio/events/to_device.py`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/nio/exceptions.py` & `matrix-nio-0.9.0/nio/exceptions.py`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/nio/http.py` & `matrix-nio-0.9.0/nio/http.py`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/nio/log.py` & `matrix-nio-0.9.0/nio/log.py`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/nio/monitors.py` & `matrix-nio-0.9.0/nio/monitors.py`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/nio/responses.py` & `matrix-nio-0.9.0/nio/responses.py`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/nio/rooms.py` & `matrix-nio-0.9.0/nio/rooms.py`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/nio/schemas.py` & `matrix-nio-0.9.0/nio/schemas.py`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/nio/store/__init__.py` & `matrix-nio-0.9.0/nio/store/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/nio/store/database.py` & `matrix-nio-0.9.0/nio/store/database.py`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/nio/store/file_trustdb.py` & `matrix-nio-0.9.0/nio/store/file_trustdb.py`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/nio/store/log.py` & `matrix-nio-0.9.0/nio/store/log.py`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/nio/store/models.py` & `matrix-nio-0.9.0/nio/store/models.py`

 * *Files identical despite different names*

### Comparing `matrix-nio-0.8.0/setup.py` & `matrix-nio-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="matrix-nio",
-    version="0.8.0",
+    version="0.9.0",
     url="https://github.com/poljar/matrix-nio",
     author='Damir Jelić',
     author_email="poljar@termina.org.uk",
     description=("A Python Matrix client library, designed according to sans "
                  "I/O principles."),
     long_description=long_description,
     long_description_content_type="text/markdown",
```

