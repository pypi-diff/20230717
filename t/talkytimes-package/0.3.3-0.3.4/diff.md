# Comparing `tmp/talkytimes_package-0.3.3.tar.gz` & `tmp/talkytimes_package-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytimes_package-0.3.3.tar", last modified: Sun Jul 16 17:10:19 2023, max compression
+gzip compressed data, was "talkytimes_package-0.3.4.tar", last modified: Mon Jul 17 14:22:00 2023, max compression
```

## Comparing `talkytimes_package-0.3.3.tar` & `talkytimes_package-0.3.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 17:10:19.697065 talkytimes_package-0.3.3/
--rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.3.3/LICENSE
--rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0      265 2023-07-16 17:10:19.697065 talkytimes_package-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.3.3/README.md
--rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.3.3/pyproject.toml
--rw-rw-rw-   0        0        0      121 2023-07-16 17:10:19.698067 talkytimes_package-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 17:10:19.675065 talkytimes_package-0.3.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-16 17:10:19.683068 talkytimes_package-0.3.3/src/dynamodb/
--rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.3.3/src/dynamodb/__init__.py
--rw-rw-rw-   0        0        0      483 2023-07-16 06:20:33.000000 talkytimes_package-0.3.3/src/dynamodb/base.py
--rw-rw-rw-   0        0        0     2702 2023-07-16 17:10:02.000000 talkytimes_package-0.3.3/src/dynamodb/dynamodb.py
-drwxrwxrwx   0        0        0        0 2023-07-16 17:10:19.686066 talkytimes_package-0.3.3/src/talkytimes/
--rw-rw-rw-   0        0        0       49 2023-07-16 17:10:16.000000 talkytimes_package-0.3.3/src/talkytimes/__init__.py
--rw-rw-rw-   0        0        0     1236 2023-07-16 08:11:24.000000 talkytimes_package-0.3.3/src/talkytimes/base.py
--rw-rw-rw-   0        0        0     3960 2023-07-16 08:50:22.000000 talkytimes_package-0.3.3/src/talkytimes/talkytimes.py
-drwxrwxrwx   0        0        0        0 2023-07-16 17:10:19.696064 talkytimes_package-0.3.3/src/talkytimes_package.egg-info/
--rw-rw-rw-   0        0        0      265 2023-07-16 17:10:19.000000 talkytimes_package-0.3.3/src/talkytimes_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2023-07-16 17:10:19.000000 talkytimes_package-0.3.3/src/talkytimes_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 17:10:19.000000 talkytimes_package-0.3.3/src/talkytimes_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-16 17:10:19.000000 talkytimes_package-0.3.3/src/talkytimes_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-16 17:10:19.000000 talkytimes_package-0.3.3/src/talkytimes_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 14:22:00.212663 talkytimes_package-0.3.4/
+-rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.3.4/LICENSE
+-rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      265 2023-07-17 14:22:00.212663 talkytimes_package-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.3.4/README.md
+-rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0      121 2023-07-17 14:22:00.213664 talkytimes_package-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 14:22:00.154663 talkytimes_package-0.3.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-17 14:22:00.178662 talkytimes_package-0.3.4/src/dynamodb/
+-rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.3.4/src/dynamodb/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-07-16 06:20:33.000000 talkytimes_package-0.3.4/src/dynamodb/base.py
+-rw-rw-rw-   0        0        0     2684 2023-07-17 14:21:25.000000 talkytimes_package-0.3.4/src/dynamodb/dynamodb.py
+drwxrwxrwx   0        0        0        0 2023-07-17 14:22:00.193663 talkytimes_package-0.3.4/src/talkytimes/
+-rw-rw-rw-   0        0        0       49 2023-07-17 14:21:58.000000 talkytimes_package-0.3.4/src/talkytimes/__init__.py
+-rw-rw-rw-   0        0        0     1236 2023-07-16 08:11:24.000000 talkytimes_package-0.3.4/src/talkytimes/base.py
+-rw-rw-rw-   0        0        0     3960 2023-07-16 08:50:22.000000 talkytimes_package-0.3.4/src/talkytimes/talkytimes.py
+drwxrwxrwx   0        0        0        0 2023-07-17 14:22:00.211662 talkytimes_package-0.3.4/src/talkytimes_package.egg-info/
+-rw-rw-rw-   0        0        0      265 2023-07-17 14:22:00.000000 talkytimes_package-0.3.4/src/talkytimes_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-07-17 14:22:00.000000 talkytimes_package-0.3.4/src/talkytimes_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 14:22:00.000000 talkytimes_package-0.3.4/src/talkytimes_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-17 14:22:00.000000 talkytimes_package-0.3.4/src/talkytimes_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-17 14:22:00.000000 talkytimes_package-0.3.4/src/talkytimes_package.egg-info/top_level.txt
```

### Comparing `talkytimes_package-0.3.3/LICENSE` & `talkytimes_package-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.3.3/src/dynamodb/dynamodb.py` & `talkytimes_package-0.3.4/src/dynamodb/dynamodb.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,30 +50,29 @@
         user_info = json.dumps(
             dict(
                 status=status,
                 messages=messages,
                 emails=emails
             )
         )
-        user = self.get_user(external_id=external_id)
         self.table.update_item(
             ExpressionAttributeNames={
                 '#UI': 'user_info',
             },
             ExpressionAttributeValues={
                 ':user_info': {
                     'S': user_info,
                 },
             },
             Key={
                 'external_id': {
                     'S': external_id,
                 },
-                'user_info': {
-                    'S': user.get("user_info")
+                "user_info": {
+                    'S': json.dumps(dict(status="True", messages="0", emails="0"))
                 }
             },
             ReturnValues='UPDATED_NEW',
             UpdateExpression='SET #UI = :user_info',
         )
 
     def create_or_update(
```

### Comparing `talkytimes_package-0.3.3/src/talkytimes/base.py` & `talkytimes_package-0.3.4/src/talkytimes/base.py`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.3.3/src/talkytimes/talkytimes.py` & `talkytimes_package-0.3.4/src/talkytimes/talkytimes.py`

 * *Files identical despite different names*

