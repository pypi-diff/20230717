# Comparing `tmp/tweety-ns-0.8.tar.gz` & `tmp/tweety-ns-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweety-ns-0.8.tar", last modified: Wed Jul  5 11:20:58 2023, max compression
+gzip compressed data, was "tweety-ns-0.9.tar", last modified: Mon Jul 17 19:34:08 2023, max compression
```

## Comparing `tweety-ns-0.8.tar` & `tweety-ns-0.9.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 11:20:58.807665 tweety-ns-0.8/
--rw-rw-rw-   0        0        0     1846 2023-07-05 11:20:58.807665 tweety-ns-0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1137 2023-05-17 13:43:00.000000 tweety-ns-0.8/README.md
--rw-rw-rw-   0        0        0      108 2021-11-15 09:32:36.000000 tweety-ns-0.8/pyproject.toml
--rw-rw-rw-   0        0        0      699 2023-07-05 11:20:58.808663 tweety-ns-0.8/setup.cfg
--rw-rw-rw-   0        0        0      800 2023-07-05 11:17:13.000000 tweety-ns-0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 11:20:58.791461 tweety-ns-0.8/src/
-drwxrwxrwx   0        0        0        0 2023-07-05 11:20:58.798298 tweety-ns-0.8/src/tweety/
--rw-rw-rw-   0        0        0       52 2023-07-05 11:18:41.000000 tweety-ns-0.8/src/tweety/__init__.py
--rw-rw-rw-   0        0        0    10992 2023-07-05 07:31:27.000000 tweety-ns-0.8/src/tweety/bot.py
--rw-rw-rw-   0        0        0    22429 2023-07-04 18:35:58.000000 tweety-ns-0.8/src/tweety/builder.py
-drwxrwxrwx   0        0        0        0 2023-07-05 11:20:58.799309 tweety-ns-0.8/src/tweety/events/
--rw-rw-rw-   0        0        0       42 2023-07-04 06:05:54.000000 tweety-ns-0.8/src/tweety/events/__init__.py
--rw-rw-rw-   0        0        0     1768 2023-07-04 10:00:32.000000 tweety-ns-0.8/src/tweety/events/newmessage.py
--rw-rw-rw-   0        0        0    18739 2023-07-05 09:21:32.000000 tweety-ns-0.8/src/tweety/exceptions_.py
--rw-rw-rw-   0        0        0      282 2022-03-04 06:53:48.000000 tweety-ns-0.8/src/tweety/filters.py
--rw-rw-rw-   0        0        0     7465 2023-07-04 18:35:04.000000 tweety-ns-0.8/src/tweety/http.py
-drwxrwxrwx   0        0        0        0 2023-07-05 11:20:58.803664 tweety-ns-0.8/src/tweety/types/
--rw-rw-rw-   0        0        0       58 2023-03-12 12:43:32.000000 tweety-ns-0.8/src/tweety/types/__init__.py
--rw-rw-rw-   0        0        0     9218 2023-07-05 09:26:20.000000 tweety-ns-0.8/src/tweety/types/inbox.py
--rw-rw-rw-   0        0        0     2631 2023-07-03 12:56:12.000000 tweety-ns-0.8/src/tweety/types/mentions.py
--rw-rw-rw-   0        0        0     2141 2023-07-03 11:20:02.000000 tweety-ns-0.8/src/tweety/types/n_types.py
--rw-rw-rw-   0        0        0     4325 2023-07-01 13:33:55.000000 tweety-ns-0.8/src/tweety/types/search.py
--rw-rw-rw-   0        0        0    30124 2023-07-05 10:13:51.000000 tweety-ns-0.8/src/tweety/types/twDataTypes.py
--rw-rw-rw-   0        0        0     3873 2023-07-05 07:09:50.000000 tweety-ns-0.8/src/tweety/types/usertweet.py
--rw-rw-rw-   0        0        0      584 2023-07-04 06:06:52.000000 tweety-ns-0.8/src/tweety/updates.py
--rw-rw-rw-   0        0        0      677 2023-07-04 06:34:07.000000 tweety-ns-0.8/src/tweety/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-05 11:20:58.806663 tweety-ns-0.8/src/tweety_ns.egg-info/
--rw-rw-rw-   0        0        0     1846 2023-07-05 11:20:58.000000 tweety-ns-0.8/src/tweety_ns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      662 2023-07-05 11:20:58.000000 tweety-ns-0.8/src/tweety_ns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 11:20:58.000000 tweety-ns-0.8/src/tweety_ns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-05 11:20:58.000000 tweety-ns-0.8/src/tweety_ns.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-05 11:20:58.000000 tweety-ns-0.8/src/tweety_ns.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 19:34:08.046963 tweety-ns-0.9/
+-rw-rw-rw-   0        0        0     1855 2023-07-17 19:34:08.046963 tweety-ns-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1146 2023-07-05 12:23:35.000000 tweety-ns-0.9/README.md
+-rw-rw-rw-   0        0        0      108 2021-11-15 09:32:36.000000 tweety-ns-0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      699 2023-07-17 19:34:08.047964 tweety-ns-0.9/setup.cfg
+-rw-rw-rw-   0        0        0      800 2023-07-17 19:33:28.000000 tweety-ns-0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 19:34:07.997765 tweety-ns-0.9/src/
+drwxrwxrwx   0        0        0        0 2023-07-17 19:34:08.021878 tweety-ns-0.9/src/tweety/
+-rw-rw-rw-   0        0        0      230 2023-07-17 19:33:40.000000 tweety-ns-0.9/src/tweety/__init__.py
+-rw-rw-rw-   0        0        0     2316 2023-07-17 19:22:53.000000 tweety-ns-0.9/src/tweety/auth.py
+-rw-rw-rw-   0        0        0    10760 2023-07-17 18:55:39.000000 tweety-ns-0.9/src/tweety/bot.py
+-rw-rw-rw-   0        0        0    30770 2023-07-17 19:26:27.000000 tweety-ns-0.9/src/tweety/builder.py
+drwxrwxrwx   0        0        0        0 2023-07-17 19:34:08.025777 tweety-ns-0.9/src/tweety/events/
+-rw-rw-rw-   0        0        0       42 2023-07-04 06:05:54.000000 tweety-ns-0.9/src/tweety/events/__init__.py
+-rw-rw-rw-   0        0        0     1768 2023-07-04 10:00:32.000000 tweety-ns-0.9/src/tweety/events/newmessage.py
+-rw-rw-rw-   0        0        0    18741 2023-07-17 19:02:14.000000 tweety-ns-0.9/src/tweety/exceptions_.py
+-rw-rw-rw-   0        0        0      282 2022-03-04 06:53:48.000000 tweety-ns-0.9/src/tweety/filters.py
+-rw-rw-rw-   0        0        0     6829 2023-07-17 19:02:14.000000 tweety-ns-0.9/src/tweety/http.py
+-rw-rw-rw-   0        0        0     1257 2023-07-09 18:45:36.000000 tweety-ns-0.9/src/tweety/session.py
+drwxrwxrwx   0        0        0        0 2023-07-17 19:34:08.036784 tweety-ns-0.9/src/tweety/types/
+-rw-rw-rw-   0        0        0       58 2023-03-12 12:43:32.000000 tweety-ns-0.9/src/tweety/types/__init__.py
+-rw-rw-rw-   0        0        0     9218 2023-07-05 09:26:20.000000 tweety-ns-0.9/src/tweety/types/inbox.py
+-rw-rw-rw-   0        0        0     2631 2023-07-03 12:56:12.000000 tweety-ns-0.9/src/tweety/types/mentions.py
+-rw-rw-rw-   0        0        0     3858 2023-07-17 19:07:38.000000 tweety-ns-0.9/src/tweety/types/n_types.py
+-rw-rw-rw-   0        0        0     4325 2023-07-13 14:34:32.000000 tweety-ns-0.9/src/tweety/types/search.py
+-rw-rw-rw-   0        0        0    30235 2023-07-09 18:41:29.000000 tweety-ns-0.9/src/tweety/types/twDataTypes.py
+-rw-rw-rw-   0        0        0     3873 2023-07-05 07:09:50.000000 tweety-ns-0.9/src/tweety/types/usertweet.py
+-rw-rw-rw-   0        0        0      483 2023-07-09 19:15:04.000000 tweety-ns-0.9/src/tweety/updates.py
+-rw-rw-rw-   0        0        0      677 2023-07-04 06:34:07.000000 tweety-ns-0.9/src/tweety/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-17 19:34:08.044963 tweety-ns-0.9/src/tweety_ns.egg-info/
+-rw-rw-rw-   0        0        0     1855 2023-07-17 19:34:07.000000 tweety-ns-0.9/src/tweety_ns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      703 2023-07-17 19:34:07.000000 tweety-ns-0.9/src/tweety_ns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 19:34:07.000000 tweety-ns-0.9/src/tweety_ns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-17 19:34:07.000000 tweety-ns-0.9/src/tweety_ns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-17 19:34:07.000000 tweety-ns-0.9/src/tweety_ns.egg-info/top_level.txt
```

### Comparing `tweety-ns-0.8/PKG-INFO` & `tweety-ns-0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweety-ns
-Version: 0.8
+Version: 0.9
 Summary: An easy Twitter Scraper
 Home-page: https://github.com/mahrtayyab/tweety
 Author: Tayyab Kharl
 Author-email: tayyabmahr@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mahrtayyab/tweety/issues
 Project-URL: Documentation, https://github.com/mahrtayyab/tweety
@@ -37,22 +37,22 @@
 ```
 
 ## Keep synced with latest fixes
 
 ##### **Pip might not be always updated , so to keep everything synced.**
 
 ```bash
-pip install git+https://github.com/mahrtayyab/tweety.git --upgrade --force-reinstall
+pip install https://github.com/mahrtayyab/tweety/archive/main.zip --upgrade --force-reinstall
 ```
 
 ## A Quick Example:
 ```python
   from tweety.bot import Twitter
   
-  app = Twitter("elonmusk")
+  app = Twitter()
   
-  all_tweets = app.get_tweets()
+  all_tweets = app.get_tweets("elonmusk")
   for tweet in all_tweets:
       print(tweet)
 ```
 
 Full Documentation and Changelogs are [here](https://mahrtayyab.github.io/tweety_docs/)
```

### Comparing `tweety-ns-0.8/README.md` & `tweety-ns-0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,22 +18,22 @@
 ```
 
 ## Keep synced with latest fixes
 
 ##### **Pip might not be always updated , so to keep everything synced.**
 
 ```bash
-pip install git+https://github.com/mahrtayyab/tweety.git --upgrade --force-reinstall
+pip install https://github.com/mahrtayyab/tweety/archive/main.zip --upgrade --force-reinstall
 ```
 
 ## A Quick Example:
 ```python
   from tweety.bot import Twitter
   
-  app = Twitter("elonmusk")
+  app = Twitter()
   
-  all_tweets = app.get_tweets()
+  all_tweets = app.get_tweets("elonmusk")
   for tweet in all_tweets:
       print(tweet)
 ```
 
 Full Documentation and Changelogs are [here](https://mahrtayyab.github.io/tweety_docs/)
```

### Comparing `tweety-ns-0.8/setup.cfg` & `tweety-ns-0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 7765 6574 792d 6e73 0d0a 7665   = tweety-ns..ve
-00000020: 7273 696f 6e20 3d20 302e 380d 0a61 7574  rsion = 0.8..aut
+00000020: 7273 696f 6e20 3d20 302e 390d 0a61 7574  rsion = 0.9..aut
 00000030: 686f 7220 3d20 5461 7979 6162 204b 6861  hor = Tayyab Kha
 00000040: 726c 0d0a 6175 7468 6f72 5f65 6d61 696c  rl..author_email
 00000050: 203d 2074 6179 7961 626d 6168 7240 676d   = tayyabmahr@gm
 00000060: 6169 6c2e 636f 6d0d 0a64 6573 6372 6970  ail.com..descrip
 00000070: 7469 6f6e 203d 2041 6e20 6561 7379 2054  tion = An easy T
 00000080: 7769 7474 6572 2053 6372 6170 6572 0d0a  witter Scraper..
 00000090: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
```

### Comparing `tweety-ns-0.8/setup.py` & `tweety-ns-0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='tweety-ns',
     packages=['tweety', 'tweety.types', 'tweety.events'],
-    version='0.8',
+    version='0.9',
     license='MIT',
     description='An easy Twitter Scraper',
     author='Tayyab Kharl',
     author_email='tayyabmahr@gmail.com',
     url='https://github.com/mahrtayyab/tweety',
     keywords=['TWITTER', 'TWITTER SCRAPE', 'SCRAPE TWEETS'],
     install_requires=[
```

### Comparing `tweety-ns-0.8/src/tweety/bot.py` & `tweety-ns-0.9/src/tweety/bot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import functools
 import re
 from typing import Union
 
 from .types.n_types import Proxy
 from .exceptions_ import *
+from .session import Session
 from .http import Request
 from .types.usertweet import UserTweets
 from .types.search import Search
 from .types.mentions import Mention
-from .types.inbox import Inbox, SendMessage, Conversation
-from .updates import UpdateMethods
+from .types.inbox import Inbox, SendMessage
 from .types.twDataTypes import User, Trends, Tweet
 from .utils import create_conversation_id
 
 
 def AuthRequired(f):
     @functools.wraps(f)
     def wrapper(self, *args, **kwargs):
@@ -21,31 +21,28 @@
             raise AuthenticationRequired(200, "GenericForbidden", None)
 
         return f(self, *args, **kwargs)
 
     return wrapper
 
 
-class Twitter(UpdateMethods):
-    def __init__(self, max_retires: int = 10, proxy: Union[dict, Proxy] = None, cookies: Union[str, dict] = None):
+class BotMethods:
+    def __init__(self, session_name: Union[str, Session], proxy: Union[dict, Proxy] = None):
         """
         Constructor of the Twitter Public class
 
-        :param max_retires: (`int`) Number of retries the script would make , if the guest token wasn't found
+        :param session_name: (`str`, `Session`) This is the name of the session which will be saved and can be loaded later
         :param proxy: (`dict` or `Proxy`) Provide the proxy you want to use while making a request
-        :param cookies: (`str` or `dict`) Cookies which will be used for user authentication
         """
 
-        if not cookies:
-            raise AuthenticationRequired(200, "GenericForbidden", None)
-
-        self.request = Request(max_retries=max_retires, proxy=proxy, cookies=cookies)
-        self.user = self.get_user_info()
-        super().__init__(self.request)
-        self.request.set_user(self.user)
+        self._event_builders = []
+        self.session = Session(session_name) if isinstance(session_name, str) else session_name
+        self.logged_in = False
+        self.request = Request(max_retries=10, proxy=proxy)
+        self.user = None
 
     def get_user_info(self, username: str = None, banner_extensions: bool = False, image_extensions: bool = False):
         """
         Get the User Info of the specified username
 
         :param username: (`str`) username to get information of
         :param banner_extensions: (`boolean`) Get the Banner extension on the user page
@@ -155,15 +152,14 @@
                 if i['item']['content']['trend']['trendMetadata']['metaDescription']:
                     data['tweet_count'] = i['item']['content']['trend']['trendMetadata']['metaDescription']
             except:
                 pass
             trends.append(Trends(data))
         return trends
 
-    @AuthRequired
     def search(self, keyword: str, pages: int = 1, filter_: str = None, wait_time: int = 2, cursor: str = None):
         """
         Search for a keyword or hashtag on Twitter
 
         :param keyword: (`str`) The keyword which is supposed to be searched
         :param pages: (`int`) The number of pages to get
         :param filter_: (
@@ -181,15 +177,14 @@
         search = Search(keyword, self.request, pages, filter_, wait_time, cursor)
 
         # TODO : Find proper way to run the generator
         results = [i for i in search.generator()]
 
         return search
 
-    @AuthRequired
     def iter_search(self, keyword: str, pages: int = 1, filter_: str = None, wait_time: int = 2, cursor: str = None):
         """
         Search for a keyword or hashtag on Twitter
 
         :param keyword: (`str`) The keyword which is supposed to be searched
         :param pages: (`int`) The number of pages to get
         :param filter_: (
```

### Comparing `tweety-ns-0.8/src/tweety/builder.py` & `tweety-ns-0.9/src/tweety/builder.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,30 +18,44 @@
 
 
 class UrlBuilder:
     URL_GUEST_TOKEN = "https://api.twitter.com/1.1/guest/activate.json"
     URL_API_INIT = "https://twitter.com/i/api/1.1/branch/init.json"
     URL_USER_BY_SCREEN_NAME = "https://twitter.com/i/api/graphql/oUZZZ8Oddwxs8Cd3iW3UEA/UserByScreenName"
     URL_USER_TWEETS = "https://twitter.com/i/api/graphql/WzJjibAcDa-oCjCcLOotcg/UserTweets"
-    URL_USER_TWEETS_WITH_REPLIES = "https://twitter.com/i/api/graphql/nrdle2catTyGnTyj1Qa7wA/UserTweetsAndReplies"
+    URL_USER_TWEETS_WITH_REPLIES = "https://twitter.com/i/api/graphql/1-5o8Qhfc2kWlu_2rWNcug/UserTweetsAndReplies"
     URL_TRENDS = "https://twitter.com/i/api/2/guide.json"
     URL_SEARCH = "https://twitter.com/i/api/graphql/nK1dw4oV3k4w5TdtcAdSww/SearchTimeline"
     URL_TWEET_DETAILS = "https://twitter.com/i/api/graphql/3XDB26fBve-MmjHaWTUZxA/TweetDetail"
-    URL_AUSER_INBOX = "https://twitter.com/i/api/1.1/dm/user_updates.json" # noqa
-    URL_AUSER_TRUSTED_INBOX = "https://twitter.com/i/api/1.1/dm/inbox_timeline/trusted.json" # noqa
-    URL_AUSER_NOTIFICATION_MENTIONS = "https://twitter.com/i/api/2/notifications/mentions.json" # noqa
+    URL_AUSER_INBOX = "https://twitter.com/i/api/1.1/dm/user_updates.json"  # noqa
+    URL_AUSER_TRUSTED_INBOX = "https://twitter.com/i/api/1.1/dm/inbox_timeline/trusted.json"  # noqa
+    URL_AUSER_NOTIFICATION_MENTIONS = "https://twitter.com/i/api/2/notifications/mentions.json"  # noqa
     URL_AUSER_SETTINGS = "https://api.twitter.com/1.1/account/settings.json"  # noqa
     URL_AUSER_SEND_MESSAGE = "https://twitter.com/i/api/1.1/dm/new2.json"  # noqa
-    URL_AUSER_CONVERSATION = "https://twitter.com/i/api/1.1/dm/conversation/{}.json" # noqa
+    URL_AUSER_CONVERSATION = "https://twitter.com/i/api/1.1/dm/conversation/{}.json"  # noqa
 
-    def __init__(self, cookies=None):
-        self.cookies = cookies
+    def __init__(self):
+        self.cookies = None
         self.user_id = None
         self.guest_token = None
 
+    def set_cookies(self, cookies):
+        if isinstance(cookies, dict):
+            self.cookies = cookies
+        else:
+            self.cookies = dict()
+            split_cookies = cookies.split(";")
+            for cookie in split_cookies:
+                split_cookie = cookie.split("=")
+
+                if len(split_cookie) == 2:
+                    key = cookie.split("=")[0]
+                    value = cookie.split("=")[1]
+                    self.cookies[key] = value
+
     def _get_headers(self):
         headers = {
             'authority': 'twitter.com',
             'accept': '*/*',
             'accept-language': 'en-PK,en;q=0.9',
             'authorization': 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs%3D1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA',
             'content-type': 'application/x-www-form-urlencoded',
@@ -83,14 +97,18 @@
         return "POST", self.URL_GUEST_TOKEN
 
     @return_with_headers
     def init_api(self):
         return "POST", self.URL_API_INIT
 
     @return_with_headers
+    def build_flow(self, _url):
+        return "POST", _url
+
+    @return_with_headers
     def user_by_screen_name(self, username):
         variables = {"screen_name": str(username), "withSafetyModeUserFields": True}
         features = {"hidden_profile_likes_enabled": False, "responsive_web_graphql_exclude_directive_enabled": True,
                     "verified_phone_label_enabled": False,
                     "subscriptions_verification_info_verified_since_enabled": True,
                     "highlights_tweets_tab_ui_enabled": True, "creator_subscriptions_tweet_preview_api_enabled": True,
                     "responsive_web_graphql_skip_user_profile_image_extensions_enabled": False,
@@ -98,43 +116,65 @@
 
         params = {'variables': str(json.dumps(variables)), 'features': str(json.dumps(features))}
 
         return "GET", self._build(self.URL_USER_BY_SCREEN_NAME, urlencode(params))
 
     @return_with_headers
     def user_tweets(self, user_id, replies=False, cursor=None):
-        variables = {"userId": str(user_id), "count": 20, "includePromotedContent": True,
-                     "withQuickPromoteEligibilityTweetFields": True, "withVoice": True, "withV2Timeline": True}
-        features = {"rweb_lists_timeline_redesign_enabled": False, "blue_business_profile_image_shape_enabled": True,
-                    "responsive_web_graphql_exclude_directive_enabled": True, "verified_phone_label_enabled": False,
-                    "creator_subscriptions_tweet_preview_api_enabled": False,
-                    "responsive_web_graphql_timeline_navigation_enabled": True,
-                    "responsive_web_graphql_skip_user_profile_image_extensions_enabled": False,
-                    "tweetypie_unmention_optimization_enabled": True, "vibe_api_enabled": True,
-                    "responsive_web_edit_tweet_api_enabled": True,
-                    "graphql_is_translatable_rweb_tweet_is_translatable_enabled": True,
-                    "view_counts_everywhere_api_enabled": True, "longform_notetweets_consumption_enabled": True,
-                    "tweet_awards_web_tipping_enabled": False, "freedom_of_speech_not_reach_fetch_enabled": True,
-                    "standardized_nudges_misinfo": True,
-                    "tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled": False,
-                    "interactive_text_enabled": True, "responsive_web_text_conversations_enabled": False,
-                    "longform_notetweets_rich_text_read_enabled": True,
-                    "longform_notetweets_inline_media_enabled": False, "responsive_web_enhance_cards_enabled": False}
-        fieldToggles = {"withArticleRichContentState": False}
+        if not replies:
+            variables = {"userId": str(user_id), "count": 20, "includePromotedContent": True,
+                         "withQuickPromoteEligibilityTweetFields": True, "withVoice": True, "withV2Timeline": True}
+            features = {"rweb_lists_timeline_redesign_enabled": True,
+                        "blue_business_profile_image_shape_enabled": True,
+                        "responsive_web_graphql_exclude_directive_enabled": True, "verified_phone_label_enabled": False,
+                        "creator_subscriptions_tweet_preview_api_enabled": False,
+                        "responsive_web_graphql_timeline_navigation_enabled": True,
+                        "responsive_web_graphql_skip_user_profile_image_extensions_enabled": False,
+                        "tweetypie_unmention_optimization_enabled": True, "vibe_api_enabled": True,
+                        "responsive_web_edit_tweet_api_enabled": True,
+                        "graphql_is_translatable_rweb_tweet_is_translatable_enabled": True,
+                        "view_counts_everywhere_api_enabled": True, "longform_notetweets_consumption_enabled": True,
+                        "tweet_awards_web_tipping_enabled": False, "freedom_of_speech_not_reach_fetch_enabled": True,
+                        "standardized_nudges_misinfo": True,
+                        "tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled": False,
+                        "interactive_text_enabled": True, "responsive_web_text_conversations_enabled": False,
+                        "longform_notetweets_rich_text_read_enabled": True,
+                        "longform_notetweets_inline_media_enabled": False,
+                        "responsive_web_enhance_cards_enabled": False}
+            fieldToggles = {"withArticleRichContentState": False}
+            url = self.URL_USER_TWEETS
+        else:
+            variables = {"userId": str(user_id), "count": 20, "includePromotedContent": True, "withCommunity": True,
+                         "withVoice": True, "withV2Timeline": True}
+            features = {"rweb_lists_timeline_redesign_enabled": True,
+                        "responsive_web_graphql_exclude_directive_enabled": True, "verified_phone_label_enabled": False,
+                        "creator_subscriptions_tweet_preview_api_enabled": True,
+                        "responsive_web_graphql_timeline_navigation_enabled": True,
+                        "responsive_web_graphql_skip_user_profile_image_extensions_enabled": False,
+                        "tweetypie_unmention_optimization_enabled": True, "responsive_web_edit_tweet_api_enabled": True,
+                        "graphql_is_translatable_rweb_tweet_is_translatable_enabled": True,
+                        "view_counts_everywhere_api_enabled": True, "longform_notetweets_consumption_enabled": True,
+                        "responsive_web_twitter_article_tweet_consumption_enabled": False,
+                        "tweet_awards_web_tipping_enabled": False, "freedom_of_speech_not_reach_fetch_enabled": True,
+                        "standardized_nudges_misinfo": True,
+                        "tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled": True,
+                        "longform_notetweets_rich_text_read_enabled": True,
+                        "longform_notetweets_inline_media_enabled": True,
+                        "responsive_web_media_download_video_enabled": False,
+                        "responsive_web_enhance_cards_enabled": False}
+            fieldToggles = {"withAuxiliaryUserLabels": False, "withArticleRichContentState": False}
+            url = self.URL_USER_TWEETS_WITH_REPLIES
 
         if cursor:
             variables['cursor'] = str(cursor)
 
         params = {'variables': str(json.dumps(variables)), 'features': str(json.dumps(features)),
                   'fieldToggles': str(json.dumps(fieldToggles))}
 
-        if replies:
-            return "GET", self._build(self.URL_USER_TWEETS_WITH_REPLIES, urlencode(params))
-
-        return "GET", self._build(self.URL_USER_TWEETS, urlencode(params))
+        return "GET", self._build(url, urlencode(params))
 
     @return_with_headers
     def trends(self):
         params = {
             'include_profile_interstitial_type': '1',
             'include_blocking': '1',
             'include_blocked_by': '1',
@@ -456,18 +496,176 @@
         }
 
         return "POST", self._build(self.URL_AUSER_SEND_MESSAGE, urlencode(params))
 
     @return_with_headers
     def aUser_settings(self):
         params = {
-            'include_mention_filter': 'True',
-            'include_nsfw_user_flag': 'True',
-            'include_nsfw_admin_flag': 'True',
-            'include_ranked_timeline': 'True',
-            'include_alt_text_compose': 'True',
+            'include_mention_filter': True,
+            'include_nsfw_user_flag': True,
+            'include_nsfw_admin_flag': True,
+            'include_ranked_timeline': True,
+            'include_alt_text_compose': True,
             'ext': 'ssoConnections',
-            'include_country_code': 'True',
-            'include_ext_dm_nsfw_media_filter': 'True',
-            'include_ext_sharing_audiospaces_listening_data_with_followers': 'True',
+            'include_country_code': True,
+            'include_ext_dm_nsfw_media_filter': True,
+            'include_ext_sharing_audiospaces_listening_data_with_followers': True,
         }
+
         return "GET", self._build(self.URL_AUSER_SETTINGS, urlencode(params))
+
+
+class FlowData:
+    IGNORE_MEMBERS = ['get']
+
+    def __init__(self, username, password, extra):
+        self._username = username
+        self._password = password
+        self._extra = extra
+        self.initial_state = "startFlow"
+
+    def get(self, called_member, **kwargs):
+        for member in dir(self):
+            if member not in self.IGNORE_MEMBERS and callable(getattr(self, member)):
+                if member == called_member:
+                    return getattr(self, member)(**kwargs)
+
+    @staticmethod
+    def get_flow_token(_json):
+        return _json['flow_token']
+
+    @staticmethod
+    def startFlow(json_, username, password):
+        return {
+            'input_flow_data': {
+                'flow_context': {
+                    'debug_overrides': {},
+                    'start_location': {
+                        'location': 'unknown',
+                    },
+                },
+            },
+            'subtask_versions': {
+                'action_list': 2,
+                'alert_dialog': 1,
+                'app_download_cta': 1,
+                'check_logged_in_account': 1,
+                'choice_selection': 3,
+                'contacts_live_sync_permission_prompt': 0,
+                'cta': 7,
+                'email_verification': 2,
+                'end_flow': 1,
+                'enter_date': 1,
+                'enter_email': 2,
+                'enter_password': 5,
+                'enter_phone': 2,
+                'enter_recaptcha': 1,
+                'enter_text': 5,
+                'enter_username': 2,
+                'generic_urt': 3,
+                'in_app_notification': 1,
+                'interest_picker': 3,
+                'js_instrumentation': 1,
+                'menu_dialog': 1,
+                'notifications_permission_prompt': 2,
+                'open_account': 2,
+                'open_home_timeline': 1,
+                'open_link': 1,
+                'phone_verification': 4,
+                'privacy_options': 1,
+                'security_key': 3,
+                'select_avatar': 4,
+                'select_banner': 2,
+                'settings_list': 7,
+                'show_code': 1,
+                'sign_up': 2,
+                'sign_up_review': 4,
+                'tweet_selection_urt': 1,
+                'update_users': 1,
+                'upload_media': 1,
+                'user_recommendations_list': 4,
+                'user_recommendations_urt': 1,
+                'wait_spinner': 3,
+                'web_modal': 1,
+            },
+        }
+
+    def LoginJsInstrumentationSubtask(self, json_, username, password):
+        return {
+            "flow_token": self.get_flow_token(json_),
+            "subtask_inputs": [
+                {
+                    "subtask_id": "LoginJsInstrumentationSubtask",
+                    'js_instrumentation': {
+                        'response': "{\"rf\":{\"ee9d114bd114827ce8d4cca456f19b3374321d65f0c52660b185810fef13f85e\":-8,\"a1a6293fd3b347788d825c22dc3f5da69e314776cd4e10978f0508c1727c471e\":124,\"ad9f941bbb8b0a8bbc18aeebb8d5b2b3ee363c68fbde149b7f9ee9945abfe522\":-214,\"c32d5d4020fe0180a3afdee9e931d1c38a436cfa58e511be8f0be534934beba1\":203},\"s\":\"WCdLUtsnS3qdTPMQrei9PN3O7Ln86ojKdsZyfMmr5q0jEsdXE6KR7qrF1eOaKlf75eReaup2xTEuBSAXd55oPEDL79NZtoM5tr33sVgNhL2N2YVLPI7X3h-0Ah2NvS6WaQTbLXK0ShEiGS9z48qalQ-oM5smlxhZhLRL7rS-y9IB_euQooEmwC3Dyn-Ka8uXybagc8C6ENaKBk9cBDkw7CFHBKekunjnKElUr0VGCYuuWJtX2PL4AMkZgBtpD_2PVbl_RN8mZkw7cx5Qbr_dGvo8vNKSmHdCwYFwKz6q38TMXXEEgQw_3BnYpqnhC4P-xDwrR_b3W7S2zZ8rSp6wUgAAAYj7_CMQ\"}",
+                        'link': 'next_link',
+                    }
+                }
+            ]
+        }
+
+    def LoginEnterUserIdentifierSSO(self, json_, username, password):
+        return {
+            "flow_token": self.get_flow_token(json_),
+            'subtask_inputs': [
+                {
+                    'subtask_id': 'LoginEnterUserIdentifierSSO',
+                    'settings_list': {
+                        'setting_responses': [
+                            {
+                                'key': 'user_identifier',
+                                'response_data': {
+                                    'text_data': {
+                                        'result': username,
+                                    },
+                                },
+                            },
+                        ],
+                        'link': 'next_link',
+                    },
+                },
+            ]
+        }
+
+    def LoginEnterPassword(self, json_, username, password):
+        return {
+            "flow_token": self.get_flow_token(json_),
+            "subtask_inputs": [
+                {
+                    "subtask_id": "LoginEnterPassword",
+                    "enter_password": {
+                        "password": password,
+                        "link": "next_link"
+                    }
+                }
+            ]
+        }
+
+    def AccountDuplicationCheck(self, json_, username, password):
+        return {
+            "flow_token": self.get_flow_token(json_),
+            "subtask_inputs": [
+                {
+                    "subtask_id": "AccountDuplicationCheck",
+                    "check_logged_in_account": {
+                        "link": "AccountDuplicationCheck_false"
+                    }
+                }
+            ]
+        }
+
+    def LoginEnterAlternateIdentifierSubtask(self, json_, username, password):
+        reason = json_['subtasks'][0]['enter_text']['secondary_text']['text']
+        print(reason)
+        getAlternate = input("> ")
+        return {
+            "flow_token": self.get_flow_token(json_),
+            "subtask_inputs": [
+                {
+                    "subtask_id": "LoginEnterAlternateIdentifierSubtask",
+                    "enter_text": {
+                        "text": getAlternate,
+                        "link": "next_link"
+                    }
+                }
+            ]
+        }
```

### Comparing `tweety-ns-0.8/src/tweety/events/newmessage.py` & `tweety-ns-0.9/src/tweety/events/newmessage.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-0.8/src/tweety/exceptions_.py` & `tweety-ns-0.9/src/tweety/exceptions_.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -136,8 +136,8 @@
     """
 
     def __init__(self, error_code, error_name, response, message="You need to be authenticated to make this request"):
         self.message = message
         self.error_code = error_code
         self.error_name = error_name
         self.response = response
-        super().__init__(self.message)
+        super().__init__(self.message)
```

### Comparing `tweety-ns-0.8/src/tweety/http.py` & `tweety-ns-0.9/src/tweety/http.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,38 @@
+import json
 import os
 import httpx as s
 from tqdm import tqdm
 from .exceptions_ import GuestTokenNotFound, UnknownError, UserNotFound, InvalidCredentials
 from .types.n_types import GenericError
 from .utils import custom_json, create_request_id
 from .builder import UrlBuilder
 
 
 s.Response.json_ = custom_json
 
 
 class Request:
-    def __init__(self, max_retries=10, proxy=None, cookies=None):
+    def __init__(self, max_retries=10, proxy=None):
         self.user = None
         self.username = None
-        self.__is_client = True if cookies else False
-        self.__session = s.Client(proxies=proxy, cookies=self._parse_cookies(cookies), timeout=60)
-        self.__builder = UrlBuilder(self.__session.cookies)
+        self.__session = s.Client(proxies=proxy, timeout=60)
+        self.__builder = UrlBuilder()
         self.__guest_token = self._get_guest_token(max_retries)
+
+    def set_cookies(self, cookies):
+        self.__session.headers['Cookie'] = cookies
+        self.__builder.set_cookies(cookies)
         self._verify_cookies()
-    
+
     def set_user(self, user):
         self.user = user
-    
-    def __get_response__(self, **request_data):
+        self.__builder.set_cookies(self.__session.cookies)
+
+    def __get_response__(self, return_raw=False, **request_data):
         response = self.__session.request(**request_data)
         response_json = response.json_() # noqa
 
         if not response_json:
             raise UnknownError(
                 error_code=500,
                 error_name="Server Error",
@@ -36,62 +41,34 @@
             )
 
         if response_json.get("errors") and not response_json.get("data"):
             error = response_json['errors'][0]
             return GenericError(
                 response, error.get("code"), error.get("message")
             )
+        if return_raw:
+            return response
 
         return response_json
 
-    @staticmethod
-    def _parse_cookies(cookies):
-        if not cookies:
-            return None
-
-        true_cookies = dict()
-        if isinstance(cookies, str):
-            cookie_list = cookies.split(";")
-            for cookie in cookie_list:
-                split_cookie = cookie.strip().split("=")
-
-                if len(split_cookie) >= 2:
-                    cookie_key = split_cookie[0]
-                    cookie_value = split_cookie[1]
-                    true_cookies[cookie_key] = cookie_value
-        elif isinstance(cookies, dict):
-            true_cookies = cookies
-        else:
-            raise TypeError("cookies should be of class 'str' or 'dict' not {}".format(cookies.__class__))
-
-        if not true_cookies.get("ct0"):
-            raise InvalidCredentials(None, None, None, "'ct0' key in cookies isn't available")
-
-        return true_cookies
-
     def _get_guest_token(self, max_retries=10):
-        if self.__is_client:
-            return
-
         for retry in range(max_retries):
             response = self.__get_response__(**self.__builder.get_guest_token())
 
             token = self.__builder.guest_token = response['guest_token'] # noqa
             return token
 
         raise GuestTokenNotFound(None, None, None, f"Guest Token couldn't be found after {max_retries} retires.")
 
     def _init_api(self):
         data = self.__builder.init_api()
         data['json'] = {}
         self.__get_response__(**data)
 
     def _verify_cookies(self):
-        if not self.__is_client:
-            return
 
         data = self.__builder.aUser_settings()
         response = self.__get_response__(**data)
 
         if not response.get("screen_name"):
             raise InvalidCredentials(None, None, None)
 
@@ -108,14 +85,20 @@
         response = self.__get_response__(**self.__builder.user_by_screen_name(username))
 
         if response.get("data"): # noqa
             return response
 
         raise UserNotFound(error_code=50, error_name="GenericUserNotFound", response=response)
 
+    def login(self, _url, _payload):
+        request_data = self.__builder.build_flow(_url)
+        request_data['json'] = _payload
+        response = self.__get_response__(True, **request_data)
+        return response
+
     def get_tweets(self, user_id, replies=False, cursor=None):
         request_data = self.__builder.user_tweets(user_id=user_id, replies=replies, cursor=cursor)
         response = self.__get_response__(**request_data)
         return response
 
     def get_trends(self):
         response = self.__get_response__(**self.__builder.trends())
```

### Comparing `tweety-ns-0.8/src/tweety/types/inbox.py` & `tweety-ns-0.9/src/tweety/types/inbox.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-0.8/src/tweety/types/mentions.py` & `tweety-ns-0.9/src/tweety/types/mentions.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-0.8/src/tweety/types/search.py` & `tweety-ns-0.9/src/tweety/types/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
                     except:
                         pass
                 self['users'] = self.users
             else:
                 tweets = self._get_tweet_content_key(entry)
                 for tweet in tweets:
                     try:
-                        parsed = Tweet(response, tweet, self.http)
+                        parsed = Tweet(tweet, self.http, response)
                         self.tweets.append(parsed)
                         thisObjects.append(parsed)
                     except:
                         pass
 
                 self['tweets'] = self.tweets
```

### Comparing `tweety-ns-0.8/src/tweety/types/twDataTypes.py` & `tweety-ns-0.9/src/tweety/types/twDataTypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -755,14 +755,18 @@
         self.verified = self._get_verified()
         self.can_dm = self._get_key("can_dm")
         # self.verified_type = self._get_key("verified_type")
         self.possibly_sensitive = self._get_key("possibly_sensitive")
         self.pinned_tweets = self._get_key("pinned_tweet_ids_str")
         self.profile_url = "https://twitter.com/{}".format(self.screen_name)
 
+        for k, v in vars(self).items():
+            if not k.startswith("_"):
+                self[k] = v
+
     def __repr__(self):
         return "User(id={}, username={}, name={}, verified={})".format(
             self.id, self.username, self.name, self.verified
         )
 
     def _get_verified(self):
         verified = self._get_key("verified", False)
```

### Comparing `tweety-ns-0.8/src/tweety/types/usertweet.py` & `tweety-ns-0.9/src/tweety/types/usertweet.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-0.8/src/tweety/utils.py` & `tweety-ns-0.9/src/tweety/utils.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-0.8/src/tweety_ns.egg-info/PKG-INFO` & `tweety-ns-0.9/src/tweety_ns.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweety-ns
-Version: 0.8
+Version: 0.9
 Summary: An easy Twitter Scraper
 Home-page: https://github.com/mahrtayyab/tweety
 Author: Tayyab Kharl
 Author-email: tayyabmahr@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mahrtayyab/tweety/issues
 Project-URL: Documentation, https://github.com/mahrtayyab/tweety
@@ -37,22 +37,22 @@
 ```
 
 ## Keep synced with latest fixes
 
 ##### **Pip might not be always updated , so to keep everything synced.**
 
 ```bash
-pip install git+https://github.com/mahrtayyab/tweety.git --upgrade --force-reinstall
+pip install https://github.com/mahrtayyab/tweety/archive/main.zip --upgrade --force-reinstall
 ```
 
 ## A Quick Example:
 ```python
   from tweety.bot import Twitter
   
-  app = Twitter("elonmusk")
+  app = Twitter()
   
-  all_tweets = app.get_tweets()
+  all_tweets = app.get_tweets("elonmusk")
   for tweet in all_tweets:
       print(tweet)
 ```
 
 Full Documentation and Changelogs are [here](https://mahrtayyab.github.io/tweety_docs/)
```

### Comparing `tweety-ns-0.8/src/tweety_ns.egg-info/SOURCES.txt` & `tweety-ns-0.9/src/tweety_ns.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/tweety/__init__.py
+src/tweety/auth.py
 src/tweety/bot.py
 src/tweety/builder.py
 src/tweety/exceptions_.py
 src/tweety/filters.py
 src/tweety/http.py
+src/tweety/session.py
 src/tweety/updates.py
 src/tweety/utils.py
 src/tweety/events/__init__.py
 src/tweety/events/newmessage.py
 src/tweety/types/__init__.py
 src/tweety/types/inbox.py
 src/tweety/types/mentions.py
```

