# Comparing `tmp/chai-guanaco-1.0.5.tar.gz` & `tmp/chai-guanaco-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chai-guanaco-1.0.5.tar", last modified: Sun Jul 16 03:02:49 2023, max compression
+gzip compressed data, was "dist/chai-guanaco-1.0.6.tar", last modified: Mon Jul 17 01:53:51 2023, max compression
```

## Comparing `chai-guanaco-1.0.5.tar` & `chai-guanaco-1.0.6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/
--rw-rw-r--   0 tom       (1002) tom       (1002)       47 2023-07-13 18:06:47.000000 chai-guanaco-1.0.5/MANIFEST.in
--rw-rw-r--   0 tom       (1002) tom       (1002)    11015 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/PKG-INFO
--rw-rw-r--   0 tom       (1002) tom       (1002)     9305 2023-07-16 03:02:29.000000 chai-guanaco-1.0.5/README.md
--rw-rw-r--   0 tom       (1002) tom       (1002)       46 2023-07-15 23:09:11.000000 chai-guanaco-1.0.5/requirements.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)       38 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/setup.cfg
--rw-rw-r--   0 tom       (1002) tom       (1002)      988 2023-07-16 03:02:45.000000 chai-guanaco-1.0.5/setup.py
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/src/
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/src/chai_guanaco/
--rw-rw-r--   0 tom       (1002) tom       (1002)      270 2023-07-15 23:09:11.000000 chai-guanaco-1.0.5/src/chai_guanaco/__init__.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     4841 2023-07-13 18:06:47.000000 chai-guanaco-1.0.5/src/chai_guanaco/chat.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     3259 2023-07-16 03:02:29.000000 chai-guanaco-1.0.5/src/chai_guanaco/feedback.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     1756 2023-07-13 18:06:47.000000 chai-guanaco-1.0.5/src/chai_guanaco/formatters.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     1966 2023-07-13 18:06:47.000000 chai-guanaco-1.0.5/src/chai_guanaco/login_cli.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     5249 2023-07-16 03:02:29.000000 chai-guanaco-1.0.5/src/chai_guanaco/metrics.py
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/src/chai_guanaco/resources/
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/
--rw-rw-r--   0 tom       (1002) tom       (1002)     1332 2023-07-15 21:49:57.000000 chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/blade.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1529 2023-07-15 21:49:57.000000 chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/captain_wyatt.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     2031 2023-07-13 18:06:47.000000 chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/coffee_shop_girl.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1305 2023-07-13 18:06:47.000000 chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/filbert.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1050 2023-07-15 21:49:57.000000 chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/leo.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1053 2023-07-13 18:06:47.000000 chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/levi.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1821 2023-07-13 18:06:47.000000 chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/mr_wilson.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1094 2023-07-13 18:06:47.000000 chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/nerd_girl.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     2205 2023-07-13 18:06:47.000000 chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/scaramouche.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1386 2023-07-13 18:06:47.000000 chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/story_teller.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     2510 2023-07-13 18:06:47.000000 chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/vampire_queen.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     2246 2023-07-13 18:06:47.000000 chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/wednesday_addams.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     5426 2023-07-15 23:09:11.000000 chai-guanaco-1.0.5/src/chai_guanaco/submit.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     1894 2023-07-16 03:02:29.000000 chai-guanaco-1.0.5/src/chai_guanaco/utils.py
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/src/chai_guanaco.egg-info/
--rw-rw-r--   0 tom       (1002) tom       (1002)    11015 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/src/chai_guanaco.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1002) tom       (1002)     1430 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/src/chai_guanaco.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)        1 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/src/chai_guanaco.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)       61 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/src/chai_guanaco.egg-info/entry_points.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)        1 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/src/chai_guanaco.egg-info/not-zip-safe
--rw-rw-r--   0 tom       (1002) tom       (1002)       46 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/src/chai_guanaco.egg-info/requires.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)       13 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/src/chai_guanaco.egg-info/top_level.txt
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/tests/
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-16 03:02:49.000000 chai-guanaco-1.0.5/tests/resources/
--rw-rw-r--   0 tom       (1002) tom       (1002) 10541478 2023-07-15 23:09:11.000000 chai-guanaco-1.0.5/tests/resources/test_get_leaderboard.yaml
--rw-rw-r--   0 tom       (1002) tom       (1002)  9300316 2023-07-15 23:09:11.000000 chai-guanaco-1.0.5/tests/resources/test_get_submission_metrics.yaml
--rw-rw-r--   0 tom       (1002) tom       (1002)     3537 2023-07-13 18:06:47.000000 chai-guanaco-1.0.5/tests/test_chat.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     3454 2023-06-27 20:36:12.000000 chai-guanaco-1.0.5/tests/test_feedback.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     1629 2023-07-16 03:02:29.000000 chai-guanaco-1.0.5/tests/test_guanaco_python_utils.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     2842 2023-07-13 18:06:47.000000 chai-guanaco-1.0.5/tests/test_login.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     3716 2023-07-16 02:17:04.000000 chai-guanaco-1.0.5/tests/test_metrics.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     5607 2023-07-16 02:17:04.000000 chai-guanaco-1.0.5/tests/test_submit.py
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-17 01:53:51.000000 chai-guanaco-1.0.6/
+-rw-rw-r--   0 tom       (1002) tom       (1002)       47 2023-07-13 18:06:47.000000 chai-guanaco-1.0.6/MANIFEST.in
+-rw-rw-r--   0 tom       (1002) tom       (1002)    11015 2023-07-17 01:53:51.000000 chai-guanaco-1.0.6/PKG-INFO
+-rw-rw-r--   0 tom       (1002) tom       (1002)     9305 2023-07-16 03:02:29.000000 chai-guanaco-1.0.6/README.md
+-rw-rw-r--   0 tom       (1002) tom       (1002)       46 2023-07-15 23:09:11.000000 chai-guanaco-1.0.6/requirements.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)       38 2023-07-17 01:53:51.000000 chai-guanaco-1.0.6/setup.cfg
+-rw-rw-r--   0 tom       (1002) tom       (1002)      988 2023-07-17 01:53:46.000000 chai-guanaco-1.0.6/setup.py
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-17 01:53:51.000000 chai-guanaco-1.0.6/src/
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-17 01:53:51.000000 chai-guanaco-1.0.6/src/chai_guanaco/
+-rw-rw-r--   0 tom       (1002) tom       (1002)      270 2023-07-15 23:09:11.000000 chai-guanaco-1.0.6/src/chai_guanaco/__init__.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     4841 2023-07-17 01:52:36.000000 chai-guanaco-1.0.6/src/chai_guanaco/chat.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     3259 2023-07-16 03:02:29.000000 chai-guanaco-1.0.6/src/chai_guanaco/feedback.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1756 2023-07-13 18:06:47.000000 chai-guanaco-1.0.6/src/chai_guanaco/formatters.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1966 2023-07-13 18:06:47.000000 chai-guanaco-1.0.6/src/chai_guanaco/login_cli.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     6109 2023-07-17 01:52:36.000000 chai-guanaco-1.0.6/src/chai_guanaco/metrics.py
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-17 01:53:51.000000 chai-guanaco-1.0.6/src/chai_guanaco/resources/
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-17 01:53:51.000000 chai-guanaco-1.0.6/src/chai_guanaco/resources/bot_config/
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1332 2023-07-15 21:49:57.000000 chai-guanaco-1.0.6/src/chai_guanaco/resources/bot_config/blade.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1529 2023-07-15 21:49:57.000000 chai-guanaco-1.0.6/src/chai_guanaco/resources/bot_config/captain_wyatt.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     2031 2023-07-13 18:06:47.000000 chai-guanaco-1.0.6/src/chai_guanaco/resources/bot_config/coffee_shop_girl.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1305 2023-07-13 18:06:47.000000 chai-guanaco-1.0.6/src/chai_guanaco/resources/bot_config/filbert.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1050 2023-07-15 21:49:57.000000 chai-guanaco-1.0.6/src/chai_guanaco/resources/bot_config/leo.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1053 2023-07-13 18:06:47.000000 chai-guanaco-1.0.6/src/chai_guanaco/resources/bot_config/levi.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1821 2023-07-13 18:06:47.000000 chai-guanaco-1.0.6/src/chai_guanaco/resources/bot_config/mr_wilson.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1094 2023-07-13 18:06:47.000000 chai-guanaco-1.0.6/src/chai_guanaco/resources/bot_config/nerd_girl.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     2205 2023-07-13 18:06:47.000000 chai-guanaco-1.0.6/src/chai_guanaco/resources/bot_config/scaramouche.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1386 2023-07-13 18:06:47.000000 chai-guanaco-1.0.6/src/chai_guanaco/resources/bot_config/story_teller.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     2510 2023-07-13 18:06:47.000000 chai-guanaco-1.0.6/src/chai_guanaco/resources/bot_config/vampire_queen.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     2246 2023-07-13 18:06:47.000000 chai-guanaco-1.0.6/src/chai_guanaco/resources/bot_config/wednesday_addams.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     5426 2023-07-15 23:09:11.000000 chai-guanaco-1.0.6/src/chai_guanaco/submit.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1894 2023-07-16 03:02:29.000000 chai-guanaco-1.0.6/src/chai_guanaco/utils.py
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-17 01:53:51.000000 chai-guanaco-1.0.6/src/chai_guanaco.egg-info/
+-rw-rw-r--   0 tom       (1002) tom       (1002)    11015 2023-07-17 01:53:51.000000 chai-guanaco-1.0.6/src/chai_guanaco.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1430 2023-07-17 01:53:51.000000 chai-guanaco-1.0.6/src/chai_guanaco.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)        1 2023-07-17 01:53:51.000000 chai-guanaco-1.0.6/src/chai_guanaco.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)       61 2023-07-17 01:53:51.000000 chai-guanaco-1.0.6/src/chai_guanaco.egg-info/entry_points.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)        1 2023-07-17 01:53:51.000000 chai-guanaco-1.0.6/src/chai_guanaco.egg-info/not-zip-safe
+-rw-rw-r--   0 tom       (1002) tom       (1002)       46 2023-07-17 01:53:51.000000 chai-guanaco-1.0.6/src/chai_guanaco.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)       13 2023-07-17 01:53:51.000000 chai-guanaco-1.0.6/src/chai_guanaco.egg-info/top_level.txt
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-17 01:53:51.000000 chai-guanaco-1.0.6/tests/
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-17 01:53:51.000000 chai-guanaco-1.0.6/tests/resources/
+-rw-rw-r--   0 tom       (1002) tom       (1002) 10541478 2023-07-15 23:09:11.000000 chai-guanaco-1.0.6/tests/resources/test_get_leaderboard.yaml
+-rw-rw-r--   0 tom       (1002) tom       (1002)  9300316 2023-07-15 23:09:11.000000 chai-guanaco-1.0.6/tests/resources/test_get_submission_metrics.yaml
+-rw-rw-r--   0 tom       (1002) tom       (1002)     3537 2023-07-13 18:06:47.000000 chai-guanaco-1.0.6/tests/test_chat.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     3454 2023-06-27 20:36:12.000000 chai-guanaco-1.0.6/tests/test_feedback.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1629 2023-07-16 03:02:29.000000 chai-guanaco-1.0.6/tests/test_guanaco_python_utils.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     2842 2023-07-13 18:06:47.000000 chai-guanaco-1.0.6/tests/test_login.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     3884 2023-07-17 01:52:36.000000 chai-guanaco-1.0.6/tests/test_metrics.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     5607 2023-07-16 02:17:04.000000 chai-guanaco-1.0.6/tests/test_submit.py
```

### Comparing `chai-guanaco-1.0.5/PKG-INFO` & `chai-guanaco-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chai-guanaco
-Version: 1.0.5
+Version: 1.0.6
 Summary: Chai Guanaco
 Home-page: https://www.chai-research.com
 Author: Chai Research Corp.
 Author-email: hello@chai-research.com
 License: MIT
 Description: [![Guanaco Banner](https://imgur.com/wJHIeAU.png)](https://www.chai-research.com/competition.html)
```

### Comparing `chai-guanaco-1.0.5/README.md` & `chai-guanaco-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.5/setup.py` & `chai-guanaco-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 if os.environ.get('CI_COMMIT_TAG', None):
     version = os.environ['CI_COMMIT_TAG']
 else:
-    version = "1.0.5"
+    version = "1.0.6"
 
 setup(
     name='chai-guanaco',
     version=version,
     description='Chai Guanaco',
     author='Chai Research Corp.',
     author_email='hello@chai-research.com',
```

### Comparing `chai-guanaco-1.0.5/src/chai_guanaco/chat.py` & `chai-guanaco-1.0.6/src/chai_guanaco/chat.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     developer_key : str
 
     Methods
     --------------
     chat(bot_config_file_name, show_model_input=False)
     Launch a chat session with the bot profile specified in bot_config_file_name
 
-    show_avaliable_bots()
+    show_available_bots()
     Displays the list of bots that are available for chat that can be passed into chat()
 
     Example usage:
     --------------
     chatbot = ChatWithSubmission(submission_id)
     chatbot.chat('vampire_queen')
     """
@@ -53,16 +53,16 @@
         user_input = input("You: ")
         while user_input != 'exit':
             response = bot.response(user_input)
             self._print_bot_response(bot_config, response, show_model_input)
             user_input = input("You: ")
 
     @staticmethod
-    def show_avaliable_bots():
-        avaliable_bots = get_avaliable_bots()
+    def show_available_bots():
+        avaliable_bots = get_available_bots()
         print_color('Avaliable Bots:', 'yellow')
         print(avaliable_bots)
 
     @staticmethod
     def _get_bot_config(config_file_name):
         bot_config_path = os.path.join(RESOURCE_DIR, f'{config_file_name}.json')
         return BotConfig.from_json(bot_config_path)
@@ -135,11 +135,11 @@
         message = {"sender": sender, "message": message}
         self._chat_history.append(message)
 
     def _init_chat_history(self):
         return [{"sender": self.bot_config.bot_label, "message": self.bot_config.first_message}]
 
 
-def get_avaliable_bots():
+def get_available_bots():
     bots = os.listdir(RESOURCE_DIR)
     avaliable_bots = '\n'.join([bot.replace('.json', '') for bot in bots if bot.endswith('.json')])
     return avaliable_bots
```

### Comparing `chai-guanaco-1.0.5/src/chai_guanaco/feedback.py` & `chai-guanaco-1.0.6/src/chai_guanaco/feedback.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.5/src/chai_guanaco/formatters.py` & `chai-guanaco-1.0.6/src/chai_guanaco/formatters.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.5/src/chai_guanaco/login_cli.py` & `chai-guanaco-1.0.6/src/chai_guanaco/login_cli.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.5/src/chai_guanaco/metrics.py` & `chai-guanaco-1.0.6/src/chai_guanaco/metrics.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from chai_guanaco.submit import get_url
 from chai_guanaco.utils import print_color, cache
 
 
 LEADERBOARD_ENDPOINT = "/leaderboard"
 FEEDBACK_CUTOFF_DAYS = 7
 MINIMUM_FEEDBACK_NUMBER_TO_DISPLAY = 50
+SUBMISSION_CUTOFF = datetime(2023, 7, 15)
 
 
 @auto_authenticate
 def display_leaderboard(developer_key=None):
     df = get_leaderboard(developer_key)
     _print_formatted_leaderboard(df)
     return df
@@ -101,24 +102,48 @@
     url = get_url(LEADERBOARD_ENDPOINT)
     resp = requests.get(url, headers=headers)
     assert resp.status_code == 200, resp.json()
     return resp.json().keys()
 
 
 def _print_formatted_leaderboard(df):
+    df = _filter_old_submissions(df)
+    df = _filter_duplicated_submissions(df)
     df = _get_filtered_leaderboard(df)
     df['engagement_score'] = _get_engagement_score(df.mcl, df.user_response_length)
     df['overall_rank'] = _get_overall_rank(df.engagement_score, df.thumbs_up_ratio)
     df = df.sort_values('overall_rank').reset_index(drop=True)
     _print_grand_prize(df)
     _print_engagement_prize(df)
     _print_thumbs_up_prize(df)
     return df
 
 
+def _filter_old_submissions(df):
+    timestamps = df.submission_id.apply(lambda x: x.split('_')[-1])
+    return df[timestamps.apply(_is_after_submission_start_time)]
+
+
+def _filter_duplicated_submissions(df):
+    df = df.sort_values(['total_feedback_count'], ascending=False)
+    df['model_name'] = df.submission_id.apply(lambda x: '_'.join(x.split('_')[:-1]))
+    df = df.drop_duplicates('model_name', keep='first')
+    df.drop('model_name', axis=1, inplace=True)
+    return df
+
+
+def _is_after_submission_start_time(timestamp):
+    try:
+        timestamp = datetime.fromtimestamp(int(timestamp))
+        is_after_cutoff = timestamp >= SUBMISSION_CUTOFF
+    except ValueError:
+        is_after_cutoff = False
+    return is_after_cutoff
+
+
 def _get_engagement_score(mcl, user_response_length):
     return mcl * user_response_length
 
 
 def _get_filtered_leaderboard(df):
     filtered_df = df[df.total_feedback_count > MINIMUM_FEEDBACK_NUMBER_TO_DISPLAY]
     filtered_df = filtered_df.drop(['total_feedback_count'], axis=1)
```

### Comparing `chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/blade.json` & `chai-guanaco-1.0.6/src/chai_guanaco/resources/bot_config/blade.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/captain_wyatt.json` & `chai-guanaco-1.0.6/src/chai_guanaco/resources/bot_config/captain_wyatt.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/coffee_shop_girl.json` & `chai-guanaco-1.0.6/src/chai_guanaco/resources/bot_config/coffee_shop_girl.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/filbert.json` & `chai-guanaco-1.0.6/src/chai_guanaco/resources/bot_config/filbert.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/leo.json` & `chai-guanaco-1.0.6/src/chai_guanaco/resources/bot_config/leo.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/levi.json` & `chai-guanaco-1.0.6/src/chai_guanaco/resources/bot_config/levi.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/mr_wilson.json` & `chai-guanaco-1.0.6/src/chai_guanaco/resources/bot_config/mr_wilson.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/nerd_girl.json` & `chai-guanaco-1.0.6/src/chai_guanaco/resources/bot_config/nerd_girl.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/scaramouche.json` & `chai-guanaco-1.0.6/src/chai_guanaco/resources/bot_config/scaramouche.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/story_teller.json` & `chai-guanaco-1.0.6/src/chai_guanaco/resources/bot_config/story_teller.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/vampire_queen.json` & `chai-guanaco-1.0.6/src/chai_guanaco/resources/bot_config/vampire_queen.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.5/src/chai_guanaco/resources/bot_config/wednesday_addams.json` & `chai-guanaco-1.0.6/src/chai_guanaco/resources/bot_config/wednesday_addams.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.5/src/chai_guanaco/submit.py` & `chai-guanaco-1.0.6/src/chai_guanaco/submit.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.5/src/chai_guanaco/utils.py` & `chai-guanaco-1.0.6/src/chai_guanaco/utils.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.5/src/chai_guanaco.egg-info/PKG-INFO` & `chai-guanaco-1.0.6/src/chai_guanaco.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chai-guanaco
-Version: 1.0.5
+Version: 1.0.6
 Summary: Chai Guanaco
 Home-page: https://www.chai-research.com
 Author: Chai Research Corp.
 Author-email: hello@chai-research.com
 License: MIT
 Description: [![Guanaco Banner](https://imgur.com/wJHIeAU.png)](https://www.chai-research.com/competition.html)
```

### Comparing `chai-guanaco-1.0.5/src/chai_guanaco.egg-info/SOURCES.txt` & `chai-guanaco-1.0.6/src/chai_guanaco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.5/tests/resources/test_get_leaderboard.yaml` & `chai-guanaco-1.0.6/tests/resources/test_get_leaderboard.yaml`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.5/tests/resources/test_get_submission_metrics.yaml` & `chai-guanaco-1.0.6/tests/resources/test_get_submission_metrics.yaml`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.5/tests/test_chat.py` & `chai-guanaco-1.0.6/tests/test_chat.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.5/tests/test_feedback.py` & `chai-guanaco-1.0.6/tests/test_feedback.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.5/tests/test_guanaco_python_utils.py` & `chai-guanaco-1.0.6/tests/test_guanaco_python_utils.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.5/tests/test_login.py` & `chai-guanaco-1.0.6/tests/test_login.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.5/tests/test_metrics.py` & `chai-guanaco-1.0.6/tests/test_metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,21 +85,25 @@
     convo_metrics = metrics.ConversationMetrics(messages)
     assert convo_metrics.mcl == 5
     assert convo_metrics.user_response_length == 4.5
 
 
 def test_print_formatted_leaderboard():
     data = {
-        'total_feedback_count': [10, 60, 100],
-        'mcl': [1.0, 2.0, 3.0],
-        'user_response_length': [500, 600, 700],
-        'thumbs_up_ratio': [0.1, 0.5, 0.8],
+        'submission_id': ['tom_1689542168', 'tom_1689404889', 'val_1689051887', 'zl_1689542168'],
+        'total_feedback_count': [10, 60, 100, 51],
+        'mcl': [1.0, 2.0, 3.0, 4.0],
+        'user_response_length': [500, 600, 700, 800],
+        'thumbs_up_ratio': [0.1, 0.5, 0.8, 0.2],
     }
     all_metrics_df = pd.DataFrame(data)
 
     df = metrics._print_formatted_leaderboard(all_metrics_df)
 
     assert len(df) == 2
-    expected_columns = ['mcl', 'user_response_length', 'thumbs_up_ratio', 'engagement_score', 'overall_rank']
+    expected_columns = [
+            'submission_id', 'mcl', 'user_response_length',
+            'thumbs_up_ratio', 'engagement_score', 'overall_rank'
+        ]
     assert list(df.columns) == expected_columns
     assert pd.api.types.is_integer_dtype(df['overall_rank'])
     pd.testing.assert_frame_equal(all_metrics_df, pd.DataFrame(data))
```

### Comparing `chai-guanaco-1.0.5/tests/test_submit.py` & `chai-guanaco-1.0.6/tests/test_submit.py`

 * *Files identical despite different names*

