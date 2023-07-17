# Comparing `tmp/youtube_livechat_scraper_ohn0-1.0.0.tar.gz` & `tmp/youtube_livechat_scraper_ohn0-1.0.1.tar.gz`

## Comparing `youtube_livechat_scraper_ohn0-1.0.0.tar` & `youtube_livechat_scraper_ohn0-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.0/.gitattributes
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.0/example.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.0/testing.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.0/builders/continuation_fetcher.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.0/builders/player_state.py
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.0/constants/node_constants.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.0/constants/scraper_constants.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.0/extractors/initial_document_extractor.py
--rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.0/generators/output_generator.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.0/messages/chat_message.py
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.0/messages/membership_gifted_message.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.0/messages/membership_message.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.0/messages/message.py
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.0/messages/pinned_message.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.0/messages/superchat_message.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.0/messages/fragments/content.py
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.0/messages/fragments/emoji.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.0/parsers/livechat_parser.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.0/requestors/continuation_requestor.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.0/requestors/initial_document_requestor.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.0/requestors/livechat_requestor.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.0/requestors/requestor.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.0/requestors/subsequent_requestor.py
--rw-r--r--   0        0        0     7343 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.0/scrapers/livechat_scraper.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.0/scrapers/scraper_initializer.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.0/scrapers/video.py
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.0/tests/request_tester.py
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.0/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.0/LICENSE
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.0/README.md
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.1/.gitattributes
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.1/example.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.1/testing.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.1/builders/continuation_fetcher.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.1/builders/player_state.py
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.1/constants/node_constants.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.1/constants/scraper_constants.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.1/extractors/initial_document_extractor.py
+-rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.1/generators/output_generator.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.1/messages/chat_message.py
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.1/messages/membership_gifted_message.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.1/messages/membership_message.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.1/messages/message.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.1/messages/pinned_message.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.1/messages/superchat_message.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.1/messages/fragments/content.py
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.1/messages/fragments/emoji.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.1/parsers/livechat_parser.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.1/requestors/continuation_requestor.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.1/requestors/initial_document_requestor.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.1/requestors/livechat_requestor.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.1/requestors/requestor.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.1/requestors/subsequent_requestor.py
+-rw-r--r--   0        0        0     7437 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.1/scrapers/livechat_scraper.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.1/scrapers/scraper_initializer.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.1/scrapers/video.py
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.1/tests/request_tester.py
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.1/README.md
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 youtube_livechat_scraper_ohn0-1.0.1/PKG-INFO
```

### Comparing `youtube_livechat_scraper_ohn0-1.0.0/example.py` & `youtube_livechat_scraper_ohn0-1.0.1/example.py`

 * *Files identical despite different names*

### Comparing `youtube_livechat_scraper_ohn0-1.0.0/testing.py` & `youtube_livechat_scraper_ohn0-1.0.1/testing.py`

 * *Files identical despite different names*

### Comparing `youtube_livechat_scraper_ohn0-1.0.0/builders/continuation_fetcher.py` & `youtube_livechat_scraper_ohn0-1.0.1/builders/continuation_fetcher.py`

 * *Files identical despite different names*

### Comparing `youtube_livechat_scraper_ohn0-1.0.0/builders/player_state.py` & `youtube_livechat_scraper_ohn0-1.0.1/builders/player_state.py`

 * *Files identical despite different names*

### Comparing `youtube_livechat_scraper_ohn0-1.0.0/constants/node_constants.py` & `youtube_livechat_scraper_ohn0-1.0.1/constants/node_constants.py`

 * *Files identical despite different names*

### Comparing `youtube_livechat_scraper_ohn0-1.0.0/constants/scraper_constants.py` & `youtube_livechat_scraper_ohn0-1.0.1/constants/scraper_constants.py`

 * *Files identical despite different names*

### Comparing `youtube_livechat_scraper_ohn0-1.0.0/extractors/initial_document_extractor.py` & `youtube_livechat_scraper_ohn0-1.0.1/extractors/initial_document_extractor.py`

 * *Files identical despite different names*

### Comparing `youtube_livechat_scraper_ohn0-1.0.0/generators/output_generator.py` & `youtube_livechat_scraper_ohn0-1.0.1/generators/output_generator.py`

 * *Files identical despite different names*

### Comparing `youtube_livechat_scraper_ohn0-1.0.0/messages/chat_message.py` & `youtube_livechat_scraper_ohn0-1.0.1/messages/chat_message.py`

 * *Files identical despite different names*

### Comparing `youtube_livechat_scraper_ohn0-1.0.0/messages/membership_gifted_message.py` & `youtube_livechat_scraper_ohn0-1.0.1/messages/membership_gifted_message.py`

 * *Files identical despite different names*

### Comparing `youtube_livechat_scraper_ohn0-1.0.0/messages/membership_message.py` & `youtube_livechat_scraper_ohn0-1.0.1/messages/membership_message.py`

 * *Files identical despite different names*

### Comparing `youtube_livechat_scraper_ohn0-1.0.0/messages/message.py` & `youtube_livechat_scraper_ohn0-1.0.1/messages/message.py`

 * *Files identical despite different names*

### Comparing `youtube_livechat_scraper_ohn0-1.0.0/messages/pinned_message.py` & `youtube_livechat_scraper_ohn0-1.0.1/messages/pinned_message.py`

 * *Files identical despite different names*

### Comparing `youtube_livechat_scraper_ohn0-1.0.0/messages/superchat_message.py` & `youtube_livechat_scraper_ohn0-1.0.1/messages/superchat_message.py`

 * *Files identical despite different names*

### Comparing `youtube_livechat_scraper_ohn0-1.0.0/messages/fragments/content.py` & `youtube_livechat_scraper_ohn0-1.0.1/messages/fragments/content.py`

 * *Files identical despite different names*

### Comparing `youtube_livechat_scraper_ohn0-1.0.0/messages/fragments/emoji.py` & `youtube_livechat_scraper_ohn0-1.0.1/messages/fragments/emoji.py`

 * *Files identical despite different names*

### Comparing `youtube_livechat_scraper_ohn0-1.0.0/parsers/livechat_parser.py` & `youtube_livechat_scraper_ohn0-1.0.1/parsers/livechat_parser.py`

 * *Files identical despite different names*

### Comparing `youtube_livechat_scraper_ohn0-1.0.0/requestors/continuation_requestor.py` & `youtube_livechat_scraper_ohn0-1.0.1/requestors/continuation_requestor.py`

 * *Files identical despite different names*

### Comparing `youtube_livechat_scraper_ohn0-1.0.0/requestors/initial_document_requestor.py` & `youtube_livechat_scraper_ohn0-1.0.1/requestors/initial_document_requestor.py`

 * *Files identical despite different names*

### Comparing `youtube_livechat_scraper_ohn0-1.0.0/requestors/livechat_requestor.py` & `youtube_livechat_scraper_ohn0-1.0.1/requestors/livechat_requestor.py`

 * *Files identical despite different names*

### Comparing `youtube_livechat_scraper_ohn0-1.0.0/requestors/requestor.py` & `youtube_livechat_scraper_ohn0-1.0.1/requestors/requestor.py`

 * *Files identical despite different names*

### Comparing `youtube_livechat_scraper_ohn0-1.0.0/requestors/subsequent_requestor.py` & `youtube_livechat_scraper_ohn0-1.0.1/requestors/subsequent_requestor.py`

 * *Files identical despite different names*

### Comparing `youtube_livechat_scraper_ohn0-1.0.0/scrapers/livechat_scraper.py` & `youtube_livechat_scraper_ohn0-1.0.1/scrapers/livechat_scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,17 @@
             self.output_filename = f'{self.video.video_title}_{time.time()}'
             self.end_time = int(initial_content["streamingData"]["formats"][0]["approxDurationMs"])
             self.initialization_successful = True
         except Exception:
             print("error encountered attempting to set initial parameters.")
 
     def __extract_video_id(self):
-        key_start = self.video.video_url.find('=')+1
+        key_start = self.video.video_url.find('watch')+8
+        if key_start <= 8:
+            key_start = self.video.video_url.find("live/")+5
         key_end = key_start + self.video.VIDEO_ID_LENGTH
         self.video.video_id = self.video.video_url[key_start:key_end]
 
     def __clean_filename(self, output_filename):
         for char in self.invalid_characters:
             output_filename = output_filename.replace(char, '')
         return output_filename
```

### Comparing `youtube_livechat_scraper_ohn0-1.0.0/scrapers/scraper_initializer.py` & `youtube_livechat_scraper_ohn0-1.0.1/scrapers/scraper_initializer.py`

 * *Files identical despite different names*

### Comparing `youtube_livechat_scraper_ohn0-1.0.0/tests/request_tester.py` & `youtube_livechat_scraper_ohn0-1.0.1/tests/request_tester.py`

 * *Files identical despite different names*

### Comparing `youtube_livechat_scraper_ohn0-1.0.0/.gitignore` & `youtube_livechat_scraper_ohn0-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `youtube_livechat_scraper_ohn0-1.0.0/LICENSE` & `youtube_livechat_scraper_ohn0-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `youtube_livechat_scraper_ohn0-1.0.0/README.md` & `youtube_livechat_scraper_ohn0-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `youtube_livechat_scraper_ohn0-1.0.0/pyproject.toml` & `youtube_livechat_scraper_ohn0-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "requests", "bs4"]
 build-backend = "hatchling.build"
 
 [project]
 name = "youtube-livechat-scraper-ohn0"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     { name="ohn0", email="silverskinx@gmail.com"},
 ]
 description="Livechat scraper for Youtube video streams"
 readme="README.md"
 requires-python=">=3.10"
 classifiers=[
```

### Comparing `youtube_livechat_scraper_ohn0-1.0.0/PKG-INFO` & `youtube_livechat_scraper_ohn0-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youtube-livechat-scraper-ohn0
-Version: 1.0.0
+Version: 1.0.1
 Summary: Livechat scraper for Youtube video streams
 Project-URL: Homepage, https://github.com/ohn0/youtube-livechat-scraper
 Author-email: ohn0 <silverskinx@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

