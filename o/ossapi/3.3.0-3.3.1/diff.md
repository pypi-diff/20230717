# Comparing `tmp/ossapi-3.3.0.tar.gz` & `tmp/ossapi-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ossapi-3.3.0.tar", last modified: Sun Jul 16 05:16:59 2023, max compression
+gzip compressed data, was "ossapi-3.3.1.tar", last modified: Mon Jul 17 20:08:19 2023, max compression
```

## Comparing `ossapi-3.3.0.tar` & `ossapi-3.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-07-16 05:16:59.231699 ossapi-3.3.0/
--rw-r--r--   0 tybug      (501) staff       (20)    34523 2023-01-30 05:20:33.000000 ossapi-3.3.0/LICENSE
--rw-r--r--   0 tybug      (501) staff       (20)    10291 2023-07-16 05:16:59.231436 ossapi-3.3.0/PKG-INFO
--rw-r--r--   0 tybug      (501) staff       (20)     9784 2023-07-16 04:59:00.000000 ossapi-3.3.0/README.md
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-07-16 05:16:59.227842 ossapi-3.3.0/ossapi/
--rw-r--r--   0 tybug      (501) staff       (20)     3990 2023-07-16 04:59:00.000000 ossapi-3.3.0/ossapi/__init__.py
--rw-r--r--   0 tybug      (501) staff       (20)      925 2023-04-18 20:48:24.000000 ossapi-3.3.0/ossapi/encoder.py
--rw-r--r--   0 tybug      (501) staff       (20)    17243 2023-07-16 04:59:00.000000 ossapi-3.3.0/ossapi/enums.py
--rw-r--r--   0 tybug      (501) staff       (20)    11982 2023-04-18 20:48:16.000000 ossapi-3.3.0/ossapi/mod.py
--rw-r--r--   0 tybug      (501) staff       (20)    36554 2023-07-16 04:59:00.000000 ossapi-3.3.0/ossapi/models.py
--rw-r--r--   0 tybug      (501) staff       (20)    14955 2023-06-05 19:43:51.000000 ossapi-3.3.0/ossapi/ossapi.py
--rw-r--r--   0 tybug      (501) staff       (20)    87794 2023-07-16 04:59:00.000000 ossapi-3.3.0/ossapi/ossapiv2.py
--rw-r--r--   0 tybug      (501) staff       (20)    92896 2023-07-16 04:59:00.000000 ossapi-3.3.0/ossapi/ossapiv2_async.py
--rw-r--r--   0 tybug      (501) staff       (20)     2639 2023-04-18 20:48:42.000000 ossapi-3.3.0/ossapi/replay.py
--rw-r--r--   0 tybug      (501) staff       (20)     8707 2023-05-28 18:35:43.000000 ossapi-3.3.0/ossapi/utils.py
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-07-16 05:16:59.229058 ossapi-3.3.0/ossapi.egg-info/
--rw-r--r--   0 tybug      (501) staff       (20)    10291 2023-07-16 05:16:59.000000 ossapi-3.3.0/ossapi.egg-info/PKG-INFO
--rw-r--r--   0 tybug      (501) staff       (20)      460 2023-07-16 05:16:59.000000 ossapi-3.3.0/ossapi.egg-info/SOURCES.txt
--rw-r--r--   0 tybug      (501) staff       (20)        1 2023-07-16 05:16:59.000000 ossapi-3.3.0/ossapi.egg-info/dependency_links.txt
--rw-r--r--   0 tybug      (501) staff       (20)       71 2023-07-16 05:16:59.000000 ossapi-3.3.0/ossapi.egg-info/requires.txt
--rw-r--r--   0 tybug      (501) staff       (20)        7 2023-07-16 05:16:59.000000 ossapi-3.3.0/ossapi.egg-info/top_level.txt
--rw-r--r--   0 tybug      (501) staff       (20)      644 2023-07-16 05:00:22.000000 ossapi-3.3.0/pyproject.toml
--rw-r--r--   0 tybug      (501) staff       (20)       38 2023-07-16 05:16:59.231762 ossapi-3.3.0/setup.cfg
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-07-16 05:16:59.231076 ossapi-3.3.0/tests/
--rw-r--r--   0 tybug      (501) staff       (20)     3080 2023-05-27 00:03:28.000000 ossapi-3.3.0/tests/__init__.py
--rw-r--r--   0 tybug      (501) staff       (20)      523 2023-01-28 21:17:50.000000 ossapi-3.3.0/tests/test_cursor.py
--rw-r--r--   0 tybug      (501) staff       (20)    11001 2023-07-16 04:59:00.000000 ossapi-3.3.0/tests/test_endpoints.py
--rw-r--r--   0 tybug      (501) staff       (20)     4039 2023-07-16 04:59:00.000000 ossapi-3.3.0/tests/test_models.py
--rw-r--r--   0 tybug      (501) staff       (20)     1133 2023-07-16 04:59:00.000000 ossapi-3.3.0/tests/test_v1.py
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-07-17 20:08:19.276321 ossapi-3.3.1/
+-rw-r--r--   0 tybug      (501) staff       (20)    34523 2023-01-30 05:20:33.000000 ossapi-3.3.1/LICENSE
+-rw-r--r--   0 tybug      (501) staff       (20)    10465 2023-07-17 20:08:19.276072 ossapi-3.3.1/PKG-INFO
+-rw-r--r--   0 tybug      (501) staff       (20)     9958 2023-07-16 05:35:26.000000 ossapi-3.3.1/README.md
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-07-17 20:08:19.273502 ossapi-3.3.1/ossapi/
+-rw-r--r--   0 tybug      (501) staff       (20)     3990 2023-07-16 04:59:00.000000 ossapi-3.3.1/ossapi/__init__.py
+-rw-r--r--   0 tybug      (501) staff       (20)      925 2023-04-18 20:48:24.000000 ossapi-3.3.1/ossapi/encoder.py
+-rw-r--r--   0 tybug      (501) staff       (20)    17243 2023-07-16 04:59:00.000000 ossapi-3.3.1/ossapi/enums.py
+-rw-r--r--   0 tybug      (501) staff       (20)    11982 2023-07-17 19:16:28.000000 ossapi-3.3.1/ossapi/mod.py
+-rw-r--r--   0 tybug      (501) staff       (20)    36593 2023-07-17 20:07:54.000000 ossapi-3.3.1/ossapi/models.py
+-rw-r--r--   0 tybug      (501) staff       (20)    14955 2023-06-05 19:43:51.000000 ossapi-3.3.1/ossapi/ossapi.py
+-rw-r--r--   0 tybug      (501) staff       (20)    88249 2023-07-17 20:02:29.000000 ossapi-3.3.1/ossapi/ossapiv2.py
+-rw-r--r--   0 tybug      (501) staff       (20)    92896 2023-07-16 04:59:00.000000 ossapi-3.3.1/ossapi/ossapiv2_async.py
+-rw-r--r--   0 tybug      (501) staff       (20)     2639 2023-04-18 20:48:42.000000 ossapi-3.3.1/ossapi/replay.py
+-rw-r--r--   0 tybug      (501) staff       (20)     9237 2023-07-17 20:04:46.000000 ossapi-3.3.1/ossapi/utils.py
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-07-17 20:08:19.274384 ossapi-3.3.1/ossapi.egg-info/
+-rw-r--r--   0 tybug      (501) staff       (20)    10465 2023-07-17 20:08:19.000000 ossapi-3.3.1/ossapi.egg-info/PKG-INFO
+-rw-r--r--   0 tybug      (501) staff       (20)      460 2023-07-17 20:08:19.000000 ossapi-3.3.1/ossapi.egg-info/SOURCES.txt
+-rw-r--r--   0 tybug      (501) staff       (20)        1 2023-07-17 20:08:19.000000 ossapi-3.3.1/ossapi.egg-info/dependency_links.txt
+-rw-r--r--   0 tybug      (501) staff       (20)       71 2023-07-17 20:08:19.000000 ossapi-3.3.1/ossapi.egg-info/requires.txt
+-rw-r--r--   0 tybug      (501) staff       (20)        7 2023-07-17 20:08:19.000000 ossapi-3.3.1/ossapi.egg-info/top_level.txt
+-rw-r--r--   0 tybug      (501) staff       (20)      644 2023-07-17 20:08:08.000000 ossapi-3.3.1/pyproject.toml
+-rw-r--r--   0 tybug      (501) staff       (20)       38 2023-07-17 20:08:19.276367 ossapi-3.3.1/setup.cfg
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-07-17 20:08:19.275709 ossapi-3.3.1/tests/
+-rw-r--r--   0 tybug      (501) staff       (20)     3080 2023-05-27 00:03:28.000000 ossapi-3.3.1/tests/__init__.py
+-rw-r--r--   0 tybug      (501) staff       (20)      523 2023-01-28 21:17:50.000000 ossapi-3.3.1/tests/test_cursor.py
+-rw-r--r--   0 tybug      (501) staff       (20)    11001 2023-07-16 04:59:00.000000 ossapi-3.3.1/tests/test_endpoints.py
+-rw-r--r--   0 tybug      (501) staff       (20)     4039 2023-07-16 04:59:00.000000 ossapi-3.3.1/tests/test_models.py
+-rw-r--r--   0 tybug      (501) staff       (20)     1133 2023-07-16 04:59:00.000000 ossapi-3.3.1/tests/test_v1.py
```

### Comparing `ossapi-3.3.0/LICENSE` & `ossapi-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ossapi-3.3.0/PKG-INFO` & `ossapi-3.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ossapi
-Version: 3.3.0
+Version: 3.3.1
 Summary: Complete python wrapper for osu! api v2 and v1.
 Author-email: Liam DeVoe <orionldevoe@gmail.com>
 Project-URL: Homepage, https://github.com/circleguard/ossapi
 Keywords: osu!,wrapper,api,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -24,14 +24,15 @@
 * [Lazer](#lazer)
 * [Endpoints](#endpoints)
   * [Beatmaps](#endpoints-beatmaps)
   * [Beatmapsets](#endpoints-beatmapsets)
   * [Changelog](#endpoints-changelog)
   * [Chat](#endpoints-chat)
   * [Comments](#endpoints-comments)
+  * [Events](#endpoints-events)
   * [Forums](#endpoints-forums)
   * [Friends](#endpoints-friends)
   * [Home](#endpoints-home)
   * [Matches](#endpoints-matches)
   * [Me](#endpoints-me)
   * [News](#endpoints-news)
   * [OAuth](#endpoints-oauth)
@@ -137,14 +138,16 @@
   * [`api.changelog_listing`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.changelog_listing)
 * Chat<a name="endpoints-chat"></a>
   * [`api.send_announcement`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.send_announcement)
   * [`api.send_pm`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.send_pm)
 * Comments<a name="endpoints-comments"></a>
   * [`api.comment`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.comment)
   * [`api.comments`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.comments)
+* Events<a name="endpoints-events"></a>
+  * [`api.events`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.events)
 * Forums<a name="endpoints-forums"></a>
   * [`api.forum_create_topic`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.forum_create_topic)
   * [`api.forum_edit_post`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.forum_edit_post)
   * [`api.forum_edit_topic`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.forum_edit_topic)
   * [`api.forum_reply`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.forum_reply)
   * [`api.forum_topic`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.forum_topic)
 * Friends<a name="endpoints-friends"></a>
@@ -155,15 +158,15 @@
   * [`api.match`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.match)
   * [`api.matches`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.matches)
 * Me<a name="endpoints-me"></a>
   * [`api.get_me`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.get_me)
 * News<a name="endpoints-news"></a>
   * [`api.news_listing`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.news_listing)
   * [`api.news_post`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.news_post)
-* Oauth<a name="endpoints-oauth"></a>
+* OAuth<a name="endpoints-oauth"></a>
   * [`api.revoke_token`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.revoke_token)
 * Rankings<a name="endpoints-rankings"></a>
   * [`api.ranking`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.ranking)
 * Rooms<a name="endpoints-rooms"></a>
   * [`api.multiplayer_scores`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.multiplayer_scores)
   * [`api.room`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.room)
   * [`api.room_leaderboard`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.room_leaderboard)
```

### Comparing `ossapi-3.3.0/README.md` & `ossapi-3.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 * [Lazer](#lazer)
 * [Endpoints](#endpoints)
   * [Beatmaps](#endpoints-beatmaps)
   * [Beatmapsets](#endpoints-beatmapsets)
   * [Changelog](#endpoints-changelog)
   * [Chat](#endpoints-chat)
   * [Comments](#endpoints-comments)
+  * [Events](#endpoints-events)
   * [Forums](#endpoints-forums)
   * [Friends](#endpoints-friends)
   * [Home](#endpoints-home)
   * [Matches](#endpoints-matches)
   * [Me](#endpoints-me)
   * [News](#endpoints-news)
   * [OAuth](#endpoints-oauth)
@@ -123,14 +124,16 @@
   * [`api.changelog_listing`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.changelog_listing)
 * Chat<a name="endpoints-chat"></a>
   * [`api.send_announcement`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.send_announcement)
   * [`api.send_pm`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.send_pm)
 * Comments<a name="endpoints-comments"></a>
   * [`api.comment`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.comment)
   * [`api.comments`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.comments)
+* Events<a name="endpoints-events"></a>
+  * [`api.events`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.events)
 * Forums<a name="endpoints-forums"></a>
   * [`api.forum_create_topic`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.forum_create_topic)
   * [`api.forum_edit_post`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.forum_edit_post)
   * [`api.forum_edit_topic`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.forum_edit_topic)
   * [`api.forum_reply`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.forum_reply)
   * [`api.forum_topic`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.forum_topic)
 * Friends<a name="endpoints-friends"></a>
@@ -141,15 +144,15 @@
   * [`api.match`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.match)
   * [`api.matches`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.matches)
 * Me<a name="endpoints-me"></a>
   * [`api.get_me`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.get_me)
 * News<a name="endpoints-news"></a>
   * [`api.news_listing`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.news_listing)
   * [`api.news_post`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.news_post)
-* Oauth<a name="endpoints-oauth"></a>
+* OAuth<a name="endpoints-oauth"></a>
   * [`api.revoke_token`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.revoke_token)
 * Rankings<a name="endpoints-rankings"></a>
   * [`api.ranking`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.ranking)
 * Rooms<a name="endpoints-rooms"></a>
   * [`api.multiplayer_scores`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.multiplayer_scores)
   * [`api.room`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.room)
   * [`api.room_leaderboard`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.room_leaderboard)
```

### Comparing `ossapi-3.3.0/ossapi/__init__.py` & `ossapi-3.3.1/ossapi/__init__.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.3.0/ossapi/encoder.py` & `ossapi-3.3.1/ossapi/encoder.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.3.0/ossapi/enums.py` & `ossapi-3.3.1/ossapi/enums.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.3.0/ossapi/mod.py` & `ossapi-3.3.1/ossapi/mod.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,28 +13,28 @@
     1 << 8     : ["HT",    "HalfTime"],
     1 << 9     : ["NC",   "Nightcore"],
     1 << 10    : ["FL",  "Flashlight"],
     1 << 11    : ["AT",    "Autoplay"],
     1 << 12    : ["SO",     "SpunOut"],
     1 << 13    : ["AP",   "Autopilot"],
     1 << 14    : ["PF",     "Perfect"],
-    1 << 15    : ["K4",        "Key4"],
-    1 << 16    : ["K5",        "Key5"],
-    1 << 17    : ["K6",        "Key6"],
-    1 << 18    : ["K7",        "Key7"],
-    1 << 19    : ["K8",        "Key8"],
+    1 << 15    : ["4K",        "Key4"],
+    1 << 16    : ["5K",        "Key5"],
+    1 << 17    : ["6K",        "Key6"],
+    1 << 18    : ["7K",        "Key7"],
+    1 << 19    : ["8K",        "Key8"],
     1 << 20    : ["FI",      "FadeIn"],
     1 << 21    : ["RD",      "Random"],
     1 << 22    : ["CN",      "Cinema"],
     1 << 23    : ["TP",      "Target"],
-    1 << 24    : ["K9",        "Key9"],
+    1 << 24    : ["9K",        "Key9"],
     1 << 25    : ["CO",     "KeyCoop"],
-    1 << 26    : ["K1",        "Key1"],
-    1 << 27    : ["K3",        "Key3"],
-    1 << 28    : ["K2",        "Key2"],
+    1 << 26    : ["1K",        "Key1"],
+    1 << 27    : ["3K",        "Key3"],
+    1 << 28    : ["2K",        "Key2"],
     1 << 29    : ["V2",     "ScoreV2"],
     1 << 30    : ["MR",      "Mirror"]
 }
 
 
 class ModCombination(BaseModel):
     """
```

### Comparing `ossapi-3.3.0/ossapi/models.py` & `ossapi-3.3.1/ossapi/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -873,15 +873,15 @@
 
     # mania attributes
     great_hit_window: Optional[float]
     score_multiplier: Optional[float]
 
 class Events(Model):
     cursor_string: str
-    events: List[Event]
+    events: List[Event] = Field(deserialize_type=List[_Event])
 
 
 # ================
 # Parameter Models
 # ================
 
 # models which aren't used for serialization, but passed to OssapiV2 methods.
```

### Comparing `ossapi-3.3.0/ossapi/ossapi.py` & `ossapi-3.3.1/ossapi/ossapi.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.3.0/ossapi/ossapiv2.py` & `ossapi-3.3.1/ossapi/ossapiv2.py`

 * *Files 0% similar despite different names*

```diff
@@ -803,30 +803,38 @@
             type_hints = get_type_hints(type_)
         except TypeError:
             assert type(type_) is _GenericAlias # pylint: disable=unidiomatic-typecheck
 
             signature_type = get_origin(type_)
             type_hints = get_type_hints(signature_type)
 
+        # field override name to existing attribute name
         field_names = {}
+        # existing attribute name to field deserialize type
+        field_deserialize_types = {}
+        # process Field attributes.
         for name in type_hints:
             # any inherited attributes will be present in the annotations
             # (type_hints) but not actually an attribute of the type. Just skip
             # them for now. TODO I'm pretty sure this is going to cause issues
             # if we ever have a field on a model and then another model
             # inheriting from it; the inheriting model won't have the field
             # picked up here and the override name won't come into play.
             # probably just traverse the mro?
             if not hasattr(type_, name):
                 continue
             value = getattr(type_, name)
             if not isinstance(value, Field):
                 continue
-            if value.name:
+
+            if value.name is not None:
                 field_names[value.name] = name
+            if value.deserialize_type is not None:
+                field_deserialize_types[name] = value.deserialize_type
+
 
         # make a copy so we can modify while iterating
         for key in list(kwargs):
             value = kwargs.pop(key)
             if key in field_names:
                 key = field_names[key]
             kwargs[key] = value
@@ -873,14 +881,17 @@
 
         try:
             val = type_(**kwargs_)
         except TypeError as e:
             raise TypeError(f"type error while instantiating class {type_}: "
                 f"{str(e)}") from e
 
+        for name, deserialize_type in field_deserialize_types.items():
+            val.__annotations__[name] = deserialize_type
+
         return val
 
 
     # =========
     # Endpoints
     # =========
```

### Comparing `ossapi-3.3.0/ossapi/ossapiv2_async.py` & `ossapi-3.3.1/ossapi/ossapiv2_async.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.3.0/ossapi/replay.py` & `ossapi-3.3.1/ossapi/replay.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.3.0/ossapi/utils.py` & `ossapi-3.3.1/ossapi/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,17 +28,27 @@
     """
     if not isinstance(type_, type):
         return False
     return issubclass(type_, BaseModel)
 
 
 class Field:
-    def __init__(self, *, name=None):
+    def __init__(self, *, name=None, deserialize_type=None):
         self.name = name
 
+        # We use annotations for two distinct purposes: deserialization, and
+        # type hints. If the deserialize type does not match the runtime type,
+        # these two annotations are in conflict.
+        #
+        # For instance, events should deserialize as _Event, but have a runtime
+        # type of Event.
+        #
+        # This field allows setting the runtime type via annotations and the
+        # deserialize type via passing this field.
+        self.deserialize_type = deserialize_type
 
 class _Model:
     """
     Base class for all models in ``ossapi``. If you want a model which handles
     its own members and cleanup after instantion, subclass ``BaseModel``
     instead.
     """
```

### Comparing `ossapi-3.3.0/ossapi.egg-info/PKG-INFO` & `ossapi-3.3.1/ossapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ossapi
-Version: 3.3.0
+Version: 3.3.1
 Summary: Complete python wrapper for osu! api v2 and v1.
 Author-email: Liam DeVoe <orionldevoe@gmail.com>
 Project-URL: Homepage, https://github.com/circleguard/ossapi
 Keywords: osu!,wrapper,api,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -24,14 +24,15 @@
 * [Lazer](#lazer)
 * [Endpoints](#endpoints)
   * [Beatmaps](#endpoints-beatmaps)
   * [Beatmapsets](#endpoints-beatmapsets)
   * [Changelog](#endpoints-changelog)
   * [Chat](#endpoints-chat)
   * [Comments](#endpoints-comments)
+  * [Events](#endpoints-events)
   * [Forums](#endpoints-forums)
   * [Friends](#endpoints-friends)
   * [Home](#endpoints-home)
   * [Matches](#endpoints-matches)
   * [Me](#endpoints-me)
   * [News](#endpoints-news)
   * [OAuth](#endpoints-oauth)
@@ -137,14 +138,16 @@
   * [`api.changelog_listing`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.changelog_listing)
 * Chat<a name="endpoints-chat"></a>
   * [`api.send_announcement`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.send_announcement)
   * [`api.send_pm`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.send_pm)
 * Comments<a name="endpoints-comments"></a>
   * [`api.comment`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.comment)
   * [`api.comments`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.comments)
+* Events<a name="endpoints-events"></a>
+  * [`api.events`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.events)
 * Forums<a name="endpoints-forums"></a>
   * [`api.forum_create_topic`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.forum_create_topic)
   * [`api.forum_edit_post`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.forum_edit_post)
   * [`api.forum_edit_topic`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.forum_edit_topic)
   * [`api.forum_reply`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.forum_reply)
   * [`api.forum_topic`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.forum_topic)
 * Friends<a name="endpoints-friends"></a>
@@ -155,15 +158,15 @@
   * [`api.match`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.match)
   * [`api.matches`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.matches)
 * Me<a name="endpoints-me"></a>
   * [`api.get_me`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.get_me)
 * News<a name="endpoints-news"></a>
   * [`api.news_listing`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.news_listing)
   * [`api.news_post`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.news_post)
-* Oauth<a name="endpoints-oauth"></a>
+* OAuth<a name="endpoints-oauth"></a>
   * [`api.revoke_token`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.revoke_token)
 * Rankings<a name="endpoints-rankings"></a>
   * [`api.ranking`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.ranking)
 * Rooms<a name="endpoints-rooms"></a>
   * [`api.multiplayer_scores`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.multiplayer_scores)
   * [`api.room`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.room)
   * [`api.room_leaderboard`](https://circleguard.github.io/ossapi/endpoints.html#ossapi.ossapiv2.Ossapi.room_leaderboard)
```

### Comparing `ossapi-3.3.0/pyproject.toml` & `ossapi-3.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ossapi"
-version = "3.3.0"
+version = "3.3.1"
 description = "Complete python wrapper for osu! api v2 and v1."
 readme = "README.md"
 keywords = ["osu!", "wrapper", "api", "python"]
 authors = [
   {name = "Liam DeVoe", email = "orionldevoe@gmail.com" }
 ]
 classifiers = [
```

### Comparing `ossapi-3.3.0/tests/__init__.py` & `ossapi-3.3.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.3.0/tests/test_cursor.py` & `ossapi-3.3.1/tests/test_cursor.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.3.0/tests/test_endpoints.py` & `ossapi-3.3.1/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.3.0/tests/test_models.py` & `ossapi-3.3.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.3.0/tests/test_v1.py` & `ossapi-3.3.1/tests/test_v1.py`

 * *Files identical despite different names*

