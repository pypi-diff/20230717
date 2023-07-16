# Comparing `tmp/mastodon_2_album-0.0.7.tar.gz` & `tmp/mastodon_2_album-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mastodon_2_album-0.0.7.tar", last modified: Tue Jul 11 23:30:53 2023, max compression
+gzip compressed data, was "mastodon_2_album-0.0.9.tar", last modified: Sat Jul 15 03:55:21 2023, max compression
```

## Comparing `mastodon_2_album-0.0.7.tar` & `mastodon_2_album-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-11 23:30:53.000000 mastodon_2_album-0.0.7/
--rw-r--r--   0 user       (501) staff       (20)     1071 2023-02-22 14:28:17.000000 mastodon_2_album-0.0.7/LICENSE
--rw-r--r--   0 user       (501) staff       (20)      759 2023-07-11 23:30:53.000000 mastodon_2_album-0.0.7/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      248 2023-07-11 23:26:41.000000 mastodon_2_album-0.0.7/README.md
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-11 23:30:53.000000 mastodon_2_album-0.0.7/mastodon_2_album/
--rw-r--r--   0 user       (501) staff       (20)     4912 2023-07-11 23:26:15.000000 mastodon_2_album-0.0.7/mastodon_2_album/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-11 23:30:53.000000 mastodon_2_album-0.0.7/mastodon_2_album.egg-info/
--rw-r--r--   0 user       (501) staff       (20)      759 2023-07-11 23:30:53.000000 mastodon_2_album-0.0.7/mastodon_2_album.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      254 2023-07-11 23:30:53.000000 mastodon_2_album-0.0.7/mastodon_2_album.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-07-11 23:30:53.000000 mastodon_2_album-0.0.7/mastodon_2_album.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       18 2023-07-11 23:30:53.000000 mastodon_2_album-0.0.7/mastodon_2_album.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)       17 2023-07-11 23:30:53.000000 mastodon_2_album-0.0.7/mastodon_2_album.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)       38 2023-07-11 23:30:53.000000 mastodon_2_album-0.0.7/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      759 2023-07-11 23:30:45.000000 mastodon_2_album-0.0.7/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-15 03:55:21.000000 mastodon_2_album-0.0.9/
+-rw-r--r--   0 user       (501) staff       (20)     1071 2023-02-22 14:28:17.000000 mastodon_2_album-0.0.9/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)      759 2023-07-15 03:55:21.000000 mastodon_2_album-0.0.9/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      248 2023-07-11 23:26:41.000000 mastodon_2_album-0.0.9/README.md
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-15 03:55:21.000000 mastodon_2_album-0.0.9/mastodon_2_album/
+-rw-r--r--   0 user       (501) staff       (20)     4997 2023-07-15 03:51:07.000000 mastodon_2_album-0.0.9/mastodon_2_album/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-15 03:55:21.000000 mastodon_2_album-0.0.9/mastodon_2_album.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)      759 2023-07-15 03:55:21.000000 mastodon_2_album-0.0.9/mastodon_2_album.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      254 2023-07-15 03:55:21.000000 mastodon_2_album-0.0.9/mastodon_2_album.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-07-15 03:55:21.000000 mastodon_2_album-0.0.9/mastodon_2_album.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       18 2023-07-15 03:55:21.000000 mastodon_2_album-0.0.9/mastodon_2_album.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)       17 2023-07-15 03:55:21.000000 mastodon_2_album-0.0.9/mastodon_2_album.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-07-15 03:55:21.000000 mastodon_2_album-0.0.9/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)      759 2023-07-15 03:55:18.000000 mastodon_2_album-0.0.9/setup.py
```

### Comparing `mastodon_2_album-0.0.7/LICENSE` & `mastodon_2_album-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mastodon_2_album-0.0.7/PKG-INFO` & `mastodon_2_album-0.0.9/mastodon_2_album.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mastodon_2_album
-Version: 0.0.7
+Name: mastodon-2-album
+Version: 0.0.9
 Summary: Return photo list and caption (markdown format) from mastodon.
 Home-page: https://github.com/gaoyunzhi/mastodon_2_album
 Author: Yunzhi Gao
 Author-email: gaoyunzhi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mastodon_2_album-0.0.7/mastodon_2_album/__init__.py` & `mastodon_2_album-0.0.9/mastodon_2_album/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,25 +52,26 @@
     		continue
     	deduped_media_attachments.append(media)
     	media_ids.add(media.id)
     return deduped_media_attachments
 
 def getImages(status):
     media_attachments = getMediaAttachments(status)
-    if not [media for media in media_attachments if media.type == 'image']:
-        return []
-    return [media.url for media in media_attachments]
+    # if not [media for media in media_attachments if media.type == 'image']:
+    #     return []
+    return [media.remote_url or media.url for media in media_attachments]
 
 def getVideo(status):
-    media_attachments = getMediaAttachments(status)
-    if [media for media in media_attachments if media.type == 'image']:
-        return
-    for media in media_attachments:
-        if media.type != 'image':
-            return media.url
+    return
+    # media_attachments = getMediaAttachments(status)
+    # if [media for media in media_attachments if media.type == 'image']:
+    #     return
+    # for media in media_attachments:
+    #     if media.type != 'image':
+    #         return media.remote_url or media.url
 
 def getOriginCap(status):
     try:
         return getContentText(status.reblog)
     except:
         return ''
 
@@ -91,14 +92,15 @@
 def getOrigin(mastodon, status):
     if status.in_reply_to_id:
         origin_status = mastodon.status(status.in_reply_to_id)
         return ' <a href="%s">origin</a>' % origin_status.url
     return ''
 
 def get(mastodon, status):
+    print(status)
     r = Result()
     r.imgs = getImages(status)
     r.video = getVideo(status)
     r.cap_html_v2 = getCap(status) + getOrigin(mastodon, status)
     r.url = getUrl(status)
     return r
```

### Comparing `mastodon_2_album-0.0.7/mastodon_2_album.egg-info/PKG-INFO` & `mastodon_2_album-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mastodon-2-album
-Version: 0.0.7
+Name: mastodon_2_album
+Version: 0.0.9
 Summary: Return photo list and caption (markdown format) from mastodon.
 Home-page: https://github.com/gaoyunzhi/mastodon_2_album
 Author: Yunzhi Gao
 Author-email: gaoyunzhi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mastodon_2_album-0.0.7/setup.py` & `mastodon_2_album-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mastodon_2_album",
-    version="0.0.7",
+    version="0.0.9",
     author="Yunzhi Gao",
     author_email="gaoyunzhi@gmail.com",
     description="Return photo list and caption (markdown format) from mastodon.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gaoyunzhi/mastodon_2_album",
     packages=setuptools.find_packages(),
```

