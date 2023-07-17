# Comparing `tmp/typetype-1.2.0.tar.gz` & `tmp/typetype-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typetype-1.2.0.tar", last modified: Wed Jul 12 22:52:27 2023, max compression
+gzip compressed data, was "typetype-1.2.1.tar", last modified: Mon Jul 17 02:45:12 2023, max compression
```

## Comparing `typetype-1.2.0.tar` & `typetype-1.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-12 22:52:27.287408 typetype-1.2.0/
--rw-r--r--   0 gulcinozer   (501) staff       (20)       48 2023-07-10 22:56:41.000000 typetype-1.2.0/MANIFEST.in
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1594 2023-07-12 22:52:27.287287 typetype-1.2.0/PKG-INFO
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1397 2023-07-11 23:50:53.000000 typetype-1.2.0/README.md
--rw-r--r--   0 gulcinozer   (501) staff       (20)       38 2023-07-12 22:52:27.287445 typetype-1.2.0/setup.cfg
--rw-r--r--   0 gulcinozer   (501) staff       (20)      662 2023-07-12 22:51:41.000000 typetype-1.2.0/setup.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-12 22:52:27.281602 typetype-1.2.0/typetype/
--rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 22:56:30.000000 typetype-1.2.0/typetype/__init__.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)    10198 2023-07-12 22:51:11.000000 typetype-1.2.0/typetype/ahmetsgame.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-12 22:52:27.282999 typetype-1.2.0/typetype/functions/
--rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:56:46.000000 typetype-1.2.0/typetype/functions/__init__.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)    10371 2023-07-12 01:36:32.000000 typetype-1.2.0/typetype/functions/game_selection.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)     8879 2023-07-11 18:44:03.000000 typetype-1.2.0/typetype/functions/refresh_update.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)     7960 2023-07-12 00:29:14.000000 typetype-1.2.0/typetype/functions/setup_results.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-12 22:52:27.284977 typetype-1.2.0/typetype/words/
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1047 2023-07-10 04:56:06.000000 typetype-1.2.0/typetype/words/200words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)   213194 2023-07-10 04:56:06.000000 typetype-1.2.0/typetype/words/25000words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)    38997 2023-07-10 04:56:06.000000 typetype-1.2.0/typetype/words/5000words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)       42 2023-07-12 22:51:05.000000 typetype-1.2.0/typetype/words/highscores.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)  1605906 2023-07-10 04:56:06.000000 typetype-1.2.0/typetype/words/text.txt
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-12 22:52:27.282285 typetype-1.2.0/typetype.egg-info/
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1594 2023-07-12 22:52:27.000000 typetype-1.2.0/typetype.egg-info/PKG-INFO
--rw-r--r--   0 gulcinozer   (501) staff       (20)      519 2023-07-12 22:52:27.000000 typetype-1.2.0/typetype.egg-info/SOURCES.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)        1 2023-07-12 22:52:27.000000 typetype-1.2.0/typetype.egg-info/dependency_links.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)       58 2023-07-12 22:52:27.000000 typetype-1.2.0/typetype.egg-info/entry_points.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)        9 2023-07-12 22:52:27.000000 typetype-1.2.0/typetype.egg-info/top_level.txt
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-17 02:45:12.184410 typetype-1.2.1/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       48 2023-07-10 22:56:41.000000 typetype-1.2.1/MANIFEST.in
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1738 2023-07-17 02:45:12.184292 typetype-1.2.1/PKG-INFO
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1541 2023-07-12 23:08:54.000000 typetype-1.2.1/README.md
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       38 2023-07-17 02:45:12.184452 typetype-1.2.1/setup.cfg
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      662 2023-07-17 02:44:31.000000 typetype-1.2.1/setup.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-17 02:45:12.178697 typetype-1.2.1/typetype/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 22:56:30.000000 typetype-1.2.1/typetype/__init__.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)    10198 2023-07-17 02:43:05.000000 typetype-1.2.1/typetype/ahmetsgame.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-17 02:45:12.180243 typetype-1.2.1/typetype/functions/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:56:46.000000 typetype-1.2.1/typetype/functions/__init__.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)    10371 2023-07-12 01:36:32.000000 typetype-1.2.1/typetype/functions/game_selection.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     8855 2023-07-17 02:41:59.000000 typetype-1.2.1/typetype/functions/refresh_update.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     7960 2023-07-12 00:29:14.000000 typetype-1.2.1/typetype/functions/setup_results.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-17 02:45:12.181932 typetype-1.2.1/typetype/words/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1047 2023-07-10 04:56:06.000000 typetype-1.2.1/typetype/words/200words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)   213194 2023-07-10 04:56:06.000000 typetype-1.2.1/typetype/words/25000words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)    38997 2023-07-10 04:56:06.000000 typetype-1.2.1/typetype/words/5000words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       42 2023-07-17 02:42:52.000000 typetype-1.2.1/typetype/words/highscores.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)  1605906 2023-07-10 04:56:06.000000 typetype-1.2.1/typetype/words/text.txt
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-17 02:45:12.179500 typetype-1.2.1/typetype.egg-info/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1738 2023-07-17 02:45:12.000000 typetype-1.2.1/typetype.egg-info/PKG-INFO
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      519 2023-07-17 02:45:12.000000 typetype-1.2.1/typetype.egg-info/SOURCES.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        1 2023-07-17 02:45:12.000000 typetype-1.2.1/typetype.egg-info/dependency_links.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       58 2023-07-17 02:45:12.000000 typetype-1.2.1/typetype.egg-info/entry_points.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        9 2023-07-17 02:45:12.000000 typetype-1.2.1/typetype.egg-info/top_level.txt
```

### Comparing `typetype-1.2.0/PKG-INFO` & `typetype-1.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typetype
-Version: 1.2.0
+Version: 1.2.1
 Summary: A command line typing game
 Home-page: https://github.com/ahmet8zer/typetype
 Author: Ahmet Ozer
 Description-Content-Type: text/markdown
 
 # typetype
 A Command Line Typing Game by Ahmet Ozer
@@ -14,15 +14,19 @@
  `pip install typetype`
 
 
 ## Usage
 To start playing the game, simply run:
 `typetype`
 
-## Cursor Option
+## Options
+`-lighter` option will make the untyped characters lighter (windows default)
+
+`-darker` option will make the untyped characters darker (mac default)
+
 To use the custom '|' cursor that I made, run the game with the `-cursor` option.
 
 ## About
 `typetype` is a minimalistic command line typing game. I made this game becuase I couldn't find any command line typing games that I liked, so I decided to make one myself. I made this game in 1 week and worked on it during my trip to canada. Since it is a minimalistic game, I did not include much text/instructions. In order to see the game's unwritten controls please read the Navigation section before playing the game.
 
 ## Controls
 Please read the following instructions to familiarize yourself with the game's controls before playing:
```

### Comparing `typetype-1.2.0/README.md` & `typetype-1.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,19 @@
  `pip install typetype`
 
 
 ## Usage
 To start playing the game, simply run:
 `typetype`
 
-## Cursor Option
+## Options
+`-lighter` option will make the untyped characters lighter (windows default)
+
+`-darker` option will make the untyped characters darker (mac default)
+
 To use the custom '|' cursor that I made, run the game with the `-cursor` option.
 
 ## About
 `typetype` is a minimalistic command line typing game. I made this game becuase I couldn't find any command line typing games that I liked, so I decided to make one myself. I made this game in 1 week and worked on it during my trip to canada. Since it is a minimalistic game, I did not include much text/instructions. In order to see the game's unwritten controls please read the Navigation section before playing the game.
 
 ## Controls
 Please read the following instructions to familiarize yourself with the game's controls before playing:
```

### Comparing `typetype-1.2.0/setup.py` & `typetype-1.2.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='typetype',
-    version='1.2.0',
+    version='1.2.1',
     author='Ahmet Ozer',
     url="https://github.com/ahmet8zer/typetype",
     description='A command line typing game',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `typetype-1.2.0/typetype/ahmetsgame.py` & `typetype-1.2.1/typetype/ahmetsgame.py`

 * *Files identical despite different names*

### Comparing `typetype-1.2.0/typetype/functions/game_selection.py` & `typetype-1.2.1/typetype/functions/game_selection.py`

 * *Files identical despite different names*

### Comparing `typetype-1.2.0/typetype/functions/refresh_update.py` & `typetype-1.2.1/typetype/functions/refresh_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     else:
         curses.curs_set(1)
     stdscr.clear()
     cursorplaced = False
     #get the first word that we have to start at (we only show 2 or 3 lines at a time)
     firstword = find_start_word(stdscr, status, original_words, playing_game, new_words, extras, onword, start_time, timed, cursor)
     #this is how many lines we're going to display
-    linesleft = 3 if firstword!=-1 else 2
+    linesleft = 3
     
     #adjust variables according to the screen dimensions
     height, width = stdscr.getmaxyx()
     line_start = int(width/6)
     line_width = int(width/6*4)
     start_height = int(height/4)
     #if the game hasn't started, then display a message
```

### Comparing `typetype-1.2.0/typetype/functions/setup_results.py` & `typetype-1.2.1/typetype/functions/setup_results.py`

 * *Files identical despite different names*

### Comparing `typetype-1.2.0/typetype/words/200words.txt` & `typetype-1.2.1/typetype/words/200words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.2.0/typetype/words/25000words.txt` & `typetype-1.2.1/typetype/words/25000words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.2.0/typetype/words/5000words.txt` & `typetype-1.2.1/typetype/words/5000words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.2.0/typetype/words/text.txt` & `typetype-1.2.1/typetype/words/text.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.2.0/typetype.egg-info/PKG-INFO` & `typetype-1.2.1/typetype.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typetype
-Version: 1.2.0
+Version: 1.2.1
 Summary: A command line typing game
 Home-page: https://github.com/ahmet8zer/typetype
 Author: Ahmet Ozer
 Description-Content-Type: text/markdown
 
 # typetype
 A Command Line Typing Game by Ahmet Ozer
@@ -14,15 +14,19 @@
  `pip install typetype`
 
 
 ## Usage
 To start playing the game, simply run:
 `typetype`
 
-## Cursor Option
+## Options
+`-lighter` option will make the untyped characters lighter (windows default)
+
+`-darker` option will make the untyped characters darker (mac default)
+
 To use the custom '|' cursor that I made, run the game with the `-cursor` option.
 
 ## About
 `typetype` is a minimalistic command line typing game. I made this game becuase I couldn't find any command line typing games that I liked, so I decided to make one myself. I made this game in 1 week and worked on it during my trip to canada. Since it is a minimalistic game, I did not include much text/instructions. In order to see the game's unwritten controls please read the Navigation section before playing the game.
 
 ## Controls
 Please read the following instructions to familiarize yourself with the game's controls before playing:
```

### Comparing `typetype-1.2.0/typetype.egg-info/SOURCES.txt` & `typetype-1.2.1/typetype.egg-info/SOURCES.txt`

 * *Files identical despite different names*

