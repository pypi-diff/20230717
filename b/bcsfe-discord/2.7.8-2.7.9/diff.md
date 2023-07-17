# Comparing `tmp/bcsfe-discord-2.7.8.tar.gz` & `tmp/bcsfe-discord-2.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcsfe-discord-2.7.8.tar", last modified: Thu Feb 23 05:33:39 2023, max compression
+gzip compressed data, was "bcsfe-discord-2.7.9.tar", last modified: Thu Feb 23 05:56:25 2023, max compression
```

## Comparing `bcsfe-discord-2.7.8.tar` & `bcsfe-discord-2.7.9.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-02-23 05:33:39.784082 bcsfe-discord-2.7.8/
--rw-r--r--   0 hayun      (502) staff       (20)      242 2023-02-23 05:33:39.783318 bcsfe-discord-2.7.8/PKG-INFO
--rw-r--r--   0 hayun      (502) staff       (20)       38 2023-02-23 05:33:39.784278 bcsfe-discord-2.7.8/setup.cfg
--rw-r--r--   0 hayun      (502) staff       (20)      737 2023-02-23 05:33:25.000000 bcsfe-discord-2.7.8/setup.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-02-23 05:33:39.722786 bcsfe-discord-2.7.8/src/
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-02-23 05:33:39.734946 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/
--rw-r--r--   0 hayun      (502) staff       (20)      322 2023-02-19 11:04:21.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/__init__.py
--rw-r--r--   0 hayun      (502) staff       (20)     9533 2023-02-19 11:04:26.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/__main__.py
--rw-r--r--   0 hayun      (502) staff       (20)    10263 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/adb_handler.py
--rw-r--r--   0 hayun      (502) staff       (20)    11632 2023-02-09 06:30:56.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/config_manager.py
--rw-r--r--   0 hayun      (502) staff       (20)     1554 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/csv_handler.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-02-23 05:33:39.735539 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/
--rw-r--r--   0 hayun      (502) staff       (20)       67 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/__init__.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-02-23 05:33:39.738470 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/basic/
--rw-r--r--   0 hayun      (502) staff       (20)       59 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/basic/__init__.py
--rw-r--r--   0 hayun      (502) staff       (20)    10203 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/basic/basic_items.py
--rw-r--r--   0 hayun      (502) staff       (20)     1550 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/basic/catfruit.py
--rw-r--r--   0 hayun      (502) staff       (20)     2008 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/basic/catseyes.py
--rw-r--r--   0 hayun      (502) staff       (20)     3452 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/basic/talent_orbs.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-02-23 05:33:39.745155 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/cats/
--rw-r--r--   0 hayun      (502) staff       (20)      190 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/cats/__init__.py
--rw-r--r--   0 hayun      (502) staff       (20)     9336 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/cats/cat_helper.py
--rw-r--r--   0 hayun      (502) staff       (20)    11487 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/cats/cat_id_selector.py
--rw-r--r--   0 hayun      (502) staff       (20)     3352 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/cats/chara_drop.py
--rw-r--r--   0 hayun      (502) staff       (20)     1106 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/cats/clear_cat_guide.py
--rw-r--r--   0 hayun      (502) staff       (20)     2941 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/cats/evolve_cats.py
--rw-r--r--   0 hayun      (502) staff       (20)     1185 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/cats/get_remove_cats.py
--rw-r--r--   0 hayun      (502) staff       (20)     8177 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/cats/talents.py
--rw-r--r--   0 hayun      (502) staff       (20)     1964 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/cats/upgrade_blue.py
--rw-r--r--   0 hayun      (502) staff       (20)     3614 2023-02-13 01:59:43.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/cats/upgrade_cats.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-02-23 05:33:39.750884 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/gamototo/
--rw-r--r--   0 hayun      (502) staff       (20)       66 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/gamototo/__init__.py
--rw-r--r--   0 hayun      (502) staff       (20)      319 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/gamototo/fix_gamatoto.py
--rw-r--r--   0 hayun      (502) staff       (20)     2922 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/gamototo/gamatoto_xp.py
--rw-r--r--   0 hayun      (502) staff       (20)     3515 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/gamototo/helpers.py
--rw-r--r--   0 hayun      (502) staff       (20)     4305 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/gamototo/ototo_cat_cannon.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-02-23 05:33:39.764022 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/
--rw-r--r--   0 hayun      (502) staff       (20)      331 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/__init__.py
--rw-r--r--   0 hayun      (502) staff       (20)     1056 2023-02-17 05:55:02.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/aku.py
--rw-r--r--   0 hayun      (502) staff       (20)      506 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/allow_filibuster_clearing.py
--rw-r--r--   0 hayun      (502) staff       (20)      812 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/behemoth_culling.py
--rw-r--r--   0 hayun      (502) staff       (20)      666 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/clear_tutorial.py
--rw-r--r--   0 hayun      (502) staff       (20)     1162 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/enigma_stages.py
--rw-r--r--   0 hayun      (502) staff       (20)     6108 2023-02-17 04:34:02.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/event_stages.py
--rw-r--r--   0 hayun      (502) staff       (20)     1921 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/gauntlet.py
--rw-r--r--   0 hayun      (502) staff       (20)      989 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/itf_timed_scores.py
--rw-r--r--   0 hayun      (502) staff       (20)     1502 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/legend_quest.py
--rw-r--r--   0 hayun      (502) staff       (20)     4517 2023-02-15 07:15:34.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/main_story.py
--rw-r--r--   0 hayun      (502) staff       (20)     2424 2023-02-17 04:11:19.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/outbreaks.py
--rw-r--r--   0 hayun      (502) staff       (20)     2922 2023-02-15 05:57:15.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/story_level_id_selector.py
--rw-r--r--   0 hayun      (502) staff       (20)     1205 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/towers.py
--rw-r--r--   0 hayun      (502) staff       (20)     9165 2023-02-20 02:43:04.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/treasures.py
--rw-r--r--   0 hayun      (502) staff       (20)      899 2023-02-17 04:37:58.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/uncanny.py
--rw-r--r--   0 hayun      (502) staff       (20)      812 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/unlock_aku_realm.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-02-23 05:33:39.776832 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/other/
--rw-r--r--   0 hayun      (502) staff       (20)      291 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/other/__init__.py
--rw-r--r--   0 hayun      (502) staff       (20)     5681 2023-02-20 04:20:27.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/other/cat_shrine.py
--rw-r--r--   0 hayun      (502) staff       (20)     1135 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/other/claim_user_rank_rewards.py
--rw-r--r--   0 hayun      (502) staff       (20)     1091 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/other/create_new_account.py
--rw-r--r--   0 hayun      (502) staff       (20)     2238 2023-02-19 10:58:32.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/other/fix_elsewhere.py
--rw-r--r--   0 hayun      (502) staff       (20)      685 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/other/fix_time_issues.py
--rw-r--r--   0 hayun      (502) staff       (20)     3306 2023-02-02 15:00:48.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/other/get_gold_pass.py
--rw-r--r--   0 hayun      (502) staff       (20)     7329 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/other/meow_medals.py
--rw-r--r--   0 hayun      (502) staff       (20)     4449 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/other/missions.py
--rw-r--r--   0 hayun      (502) staff       (20)      997 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/other/play_time.py
--rw-r--r--   0 hayun      (502) staff       (20)     4723 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/other/scheme_item.py
--rw-r--r--   0 hayun      (502) staff       (20)     1751 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/other/trade_progress.py
--rw-r--r--   0 hayun      (502) staff       (20)      947 2023-02-20 04:13:23.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/other/unlock_enemy_guide.py
--rw-r--r--   0 hayun      (502) staff       (20)      338 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/other/unlock_equip_menu.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-02-23 05:33:39.779823 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/save_management/
--rw-r--r--   0 hayun      (502) staff       (20)       46 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/save_management/__init__.py
--rw-r--r--   0 hayun      (502) staff       (20)     2645 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/save_management/load.py
--rw-r--r--   0 hayun      (502) staff       (20)      725 2023-02-23 05:31:49.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/save_management/other.py
--rw-r--r--   0 hayun      (502) staff       (20)     2111 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/save_management/save.py
--rw-r--r--   0 hayun      (502) staff       (20)     1958 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/save_management/server_upload.py
--rw-r--r--   0 hayun      (502) staff       (20)    12716 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/feature_handler.py
--rw-r--r--   0 hayun      (502) staff       (20)     4500 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/game_data_getter.py
--rw-r--r--   0 hayun      (502) staff       (20)    23323 2023-02-23 05:30:46.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/helper.py
--rw-r--r--   0 hayun      (502) staff       (20)     8953 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/item.py
--rw-r--r--   0 hayun      (502) staff       (20)     1317 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/managed_item.py
--rw-r--r--   0 hayun      (502) staff       (20)    67598 2023-02-18 14:04:15.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/parse_save.py
--rw-r--r--   0 hayun      (502) staff       (20)     1354 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/patcher.py
--rw-r--r--   0 hayun      (502) staff       (20)     2510 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/root_handler.py
--rw-r--r--   0 hayun      (502) staff       (20)    53471 2023-02-18 14:40:27.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/serialise_save.py
--rw-r--r--   0 hayun      (502) staff       (20)    19801 2023-01-30 23:32:18.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/server_handler.py
--rw-r--r--   0 hayun      (502) staff       (20)     3432 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/tracker.py
--rw-r--r--   0 hayun      (502) staff       (20)     3588 2023-02-18 09:22:48.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/updater.py
--rw-r--r--   0 hayun      (502) staff       (20)     7034 2023-02-20 02:44:31.000000 bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/user_input_handler.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-02-23 05:33:39.782645 bcsfe-discord-2.7.8/src/bcsfe_discord.egg-info/
--rw-r--r--   0 hayun      (502) staff       (20)      242 2023-02-23 05:33:39.000000 bcsfe-discord-2.7.8/src/bcsfe_discord.egg-info/PKG-INFO
--rw-r--r--   0 hayun      (502) staff       (20)     3983 2023-02-23 05:33:39.000000 bcsfe-discord-2.7.8/src/bcsfe_discord.egg-info/SOURCES.txt
--rw-r--r--   0 hayun      (502) staff       (20)        1 2023-02-23 05:33:39.000000 bcsfe-discord-2.7.8/src/bcsfe_discord.egg-info/dependency_links.txt
--rw-r--r--   0 hayun      (502) staff       (20)       72 2023-02-23 05:33:39.000000 bcsfe-discord-2.7.8/src/bcsfe_discord.egg-info/requires.txt
--rw-r--r--   0 hayun      (502) staff       (20)       21 2023-02-23 05:33:39.000000 bcsfe-discord-2.7.8/src/bcsfe_discord.egg-info/top_level.txt
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-02-23 05:56:25.806426 bcsfe-discord-2.7.9/
+-rw-r--r--   0 hayun      (502) staff       (20)      242 2023-02-23 05:56:25.805919 bcsfe-discord-2.7.9/PKG-INFO
+-rw-r--r--   0 hayun      (502) staff       (20)       38 2023-02-23 05:56:25.806652 bcsfe-discord-2.7.9/setup.cfg
+-rw-r--r--   0 hayun      (502) staff       (20)      737 2023-02-23 05:56:09.000000 bcsfe-discord-2.7.9/setup.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-02-23 05:56:25.721721 bcsfe-discord-2.7.9/src/
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-02-23 05:56:25.740952 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/
+-rw-r--r--   0 hayun      (502) staff       (20)      322 2023-02-19 11:04:21.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/__init__.py
+-rw-r--r--   0 hayun      (502) staff       (20)     9533 2023-02-19 11:04:26.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/__main__.py
+-rw-r--r--   0 hayun      (502) staff       (20)    10263 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/adb_handler.py
+-rw-r--r--   0 hayun      (502) staff       (20)    11632 2023-02-09 06:30:56.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/config_manager.py
+-rw-r--r--   0 hayun      (502) staff       (20)     1554 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/csv_handler.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-02-23 05:56:25.741517 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/
+-rw-r--r--   0 hayun      (502) staff       (20)       67 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/__init__.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-02-23 05:56:25.745854 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/basic/
+-rw-r--r--   0 hayun      (502) staff       (20)       59 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/basic/__init__.py
+-rw-r--r--   0 hayun      (502) staff       (20)    10203 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/basic/basic_items.py
+-rw-r--r--   0 hayun      (502) staff       (20)     1550 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/basic/catfruit.py
+-rw-r--r--   0 hayun      (502) staff       (20)     2008 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/basic/catseyes.py
+-rw-r--r--   0 hayun      (502) staff       (20)     3452 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/basic/talent_orbs.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-02-23 05:56:25.754107 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/cats/
+-rw-r--r--   0 hayun      (502) staff       (20)      190 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/cats/__init__.py
+-rw-r--r--   0 hayun      (502) staff       (20)     9336 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/cats/cat_helper.py
+-rw-r--r--   0 hayun      (502) staff       (20)    11487 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/cats/cat_id_selector.py
+-rw-r--r--   0 hayun      (502) staff       (20)     3352 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/cats/chara_drop.py
+-rw-r--r--   0 hayun      (502) staff       (20)     1106 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/cats/clear_cat_guide.py
+-rw-r--r--   0 hayun      (502) staff       (20)     2941 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/cats/evolve_cats.py
+-rw-r--r--   0 hayun      (502) staff       (20)     1185 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/cats/get_remove_cats.py
+-rw-r--r--   0 hayun      (502) staff       (20)     8177 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/cats/talents.py
+-rw-r--r--   0 hayun      (502) staff       (20)     1964 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/cats/upgrade_blue.py
+-rw-r--r--   0 hayun      (502) staff       (20)     3614 2023-02-13 01:59:43.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/cats/upgrade_cats.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-02-23 05:56:25.757090 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/gamototo/
+-rw-r--r--   0 hayun      (502) staff       (20)       66 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/gamototo/__init__.py
+-rw-r--r--   0 hayun      (502) staff       (20)      319 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/gamototo/fix_gamatoto.py
+-rw-r--r--   0 hayun      (502) staff       (20)     2922 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/gamototo/gamatoto_xp.py
+-rw-r--r--   0 hayun      (502) staff       (20)     3515 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/gamototo/helpers.py
+-rw-r--r--   0 hayun      (502) staff       (20)     4305 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/gamototo/ototo_cat_cannon.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-02-23 05:56:25.780162 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/
+-rw-r--r--   0 hayun      (502) staff       (20)      331 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/__init__.py
+-rw-r--r--   0 hayun      (502) staff       (20)     1056 2023-02-17 05:55:02.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/aku.py
+-rw-r--r--   0 hayun      (502) staff       (20)      506 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/allow_filibuster_clearing.py
+-rw-r--r--   0 hayun      (502) staff       (20)      812 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/behemoth_culling.py
+-rw-r--r--   0 hayun      (502) staff       (20)      666 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/clear_tutorial.py
+-rw-r--r--   0 hayun      (502) staff       (20)     1162 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/enigma_stages.py
+-rw-r--r--   0 hayun      (502) staff       (20)     6108 2023-02-17 04:34:02.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/event_stages.py
+-rw-r--r--   0 hayun      (502) staff       (20)     1921 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/gauntlet.py
+-rw-r--r--   0 hayun      (502) staff       (20)      989 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/itf_timed_scores.py
+-rw-r--r--   0 hayun      (502) staff       (20)     1502 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/legend_quest.py
+-rw-r--r--   0 hayun      (502) staff       (20)     4517 2023-02-15 07:15:34.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/main_story.py
+-rw-r--r--   0 hayun      (502) staff       (20)     2424 2023-02-17 04:11:19.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/outbreaks.py
+-rw-r--r--   0 hayun      (502) staff       (20)     2922 2023-02-15 05:57:15.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/story_level_id_selector.py
+-rw-r--r--   0 hayun      (502) staff       (20)     1205 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/towers.py
+-rw-r--r--   0 hayun      (502) staff       (20)     9165 2023-02-20 02:43:04.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/treasures.py
+-rw-r--r--   0 hayun      (502) staff       (20)      899 2023-02-17 04:37:58.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/uncanny.py
+-rw-r--r--   0 hayun      (502) staff       (20)      812 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/unlock_aku_realm.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-02-23 05:56:25.795788 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/other/
+-rw-r--r--   0 hayun      (502) staff       (20)      291 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/other/__init__.py
+-rw-r--r--   0 hayun      (502) staff       (20)     5681 2023-02-20 04:20:27.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/other/cat_shrine.py
+-rw-r--r--   0 hayun      (502) staff       (20)     1135 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/other/claim_user_rank_rewards.py
+-rw-r--r--   0 hayun      (502) staff       (20)     1091 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/other/create_new_account.py
+-rw-r--r--   0 hayun      (502) staff       (20)     2238 2023-02-19 10:58:32.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/other/fix_elsewhere.py
+-rw-r--r--   0 hayun      (502) staff       (20)      685 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/other/fix_time_issues.py
+-rw-r--r--   0 hayun      (502) staff       (20)     3306 2023-02-02 15:00:48.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/other/get_gold_pass.py
+-rw-r--r--   0 hayun      (502) staff       (20)     7329 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/other/meow_medals.py
+-rw-r--r--   0 hayun      (502) staff       (20)     4449 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/other/missions.py
+-rw-r--r--   0 hayun      (502) staff       (20)      997 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/other/play_time.py
+-rw-r--r--   0 hayun      (502) staff       (20)     4723 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/other/scheme_item.py
+-rw-r--r--   0 hayun      (502) staff       (20)     1751 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/other/trade_progress.py
+-rw-r--r--   0 hayun      (502) staff       (20)      947 2023-02-20 04:13:23.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/other/unlock_enemy_guide.py
+-rw-r--r--   0 hayun      (502) staff       (20)      338 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/other/unlock_equip_menu.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-02-23 05:56:25.801049 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/save_management/
+-rw-r--r--   0 hayun      (502) staff       (20)       46 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/save_management/__init__.py
+-rw-r--r--   0 hayun      (502) staff       (20)     2645 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/save_management/load.py
+-rw-r--r--   0 hayun      (502) staff       (20)      681 2023-02-23 05:53:11.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/save_management/other.py
+-rw-r--r--   0 hayun      (502) staff       (20)     2111 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/save_management/save.py
+-rw-r--r--   0 hayun      (502) staff       (20)     1958 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/save_management/server_upload.py
+-rw-r--r--   0 hayun      (502) staff       (20)    12716 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/feature_handler.py
+-rw-r--r--   0 hayun      (502) staff       (20)     4500 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/game_data_getter.py
+-rw-r--r--   0 hayun      (502) staff       (20)    23351 2023-02-23 05:54:48.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/helper.py
+-rw-r--r--   0 hayun      (502) staff       (20)     8953 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/item.py
+-rw-r--r--   0 hayun      (502) staff       (20)     1317 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/managed_item.py
+-rw-r--r--   0 hayun      (502) staff       (20)    67598 2023-02-18 14:04:15.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/parse_save.py
+-rw-r--r--   0 hayun      (502) staff       (20)     1354 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/patcher.py
+-rw-r--r--   0 hayun      (502) staff       (20)     2510 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/root_handler.py
+-rw-r--r--   0 hayun      (502) staff       (20)    53471 2023-02-18 14:40:27.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/serialise_save.py
+-rw-r--r--   0 hayun      (502) staff       (20)    19801 2023-01-30 23:32:18.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/server_handler.py
+-rw-r--r--   0 hayun      (502) staff       (20)     3432 2023-01-09 00:09:35.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/tracker.py
+-rw-r--r--   0 hayun      (502) staff       (20)     3588 2023-02-18 09:22:48.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/updater.py
+-rw-r--r--   0 hayun      (502) staff       (20)     7034 2023-02-20 02:44:31.000000 bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/user_input_handler.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-02-23 05:56:25.804638 bcsfe-discord-2.7.9/src/bcsfe_discord.egg-info/
+-rw-r--r--   0 hayun      (502) staff       (20)      242 2023-02-23 05:56:25.000000 bcsfe-discord-2.7.9/src/bcsfe_discord.egg-info/PKG-INFO
+-rw-r--r--   0 hayun      (502) staff       (20)     3983 2023-02-23 05:56:25.000000 bcsfe-discord-2.7.9/src/bcsfe_discord.egg-info/SOURCES.txt
+-rw-r--r--   0 hayun      (502) staff       (20)        1 2023-02-23 05:56:25.000000 bcsfe-discord-2.7.9/src/bcsfe_discord.egg-info/dependency_links.txt
+-rw-r--r--   0 hayun      (502) staff       (20)       72 2023-02-23 05:56:25.000000 bcsfe-discord-2.7.9/src/bcsfe_discord.egg-info/requires.txt
+-rw-r--r--   0 hayun      (502) staff       (20)       21 2023-02-23 05:56:25.000000 bcsfe-discord-2.7.9/src/bcsfe_discord.egg-info/top_level.txt
```

### Comparing `bcsfe-discord-2.7.8/setup.py` & `bcsfe-discord-2.7.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 import setuptools
 setup(
     name="bcsfe-discord",
-    version='2.7.8',
+    version='2.7.9',
     author="CintagramABP",
     description="BCSFE_Python personal api",
     long_description="BCSFE_Python personal api",
     url="",
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.9",
```

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/__main__.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/__main__.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/adb_handler.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/adb_handler.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/config_manager.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/config_manager.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/csv_handler.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/csv_handler.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/basic/basic_items.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/basic/basic_items.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/basic/catfruit.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/basic/catfruit.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/basic/catseyes.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/basic/catseyes.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/basic/talent_orbs.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/basic/talent_orbs.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/cats/cat_helper.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/cats/cat_helper.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/cats/cat_id_selector.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/cats/cat_id_selector.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/cats/chara_drop.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/cats/chara_drop.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/cats/clear_cat_guide.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/cats/clear_cat_guide.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/cats/evolve_cats.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/cats/evolve_cats.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/cats/get_remove_cats.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/cats/get_remove_cats.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/cats/talents.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/cats/talents.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/cats/upgrade_blue.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/cats/upgrade_blue.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/cats/upgrade_cats.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/cats/upgrade_cats.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/gamototo/gamatoto_xp.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/gamototo/gamatoto_xp.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/gamototo/helpers.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/gamototo/helpers.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/gamototo/ototo_cat_cannon.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/gamototo/ototo_cat_cannon.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/aku.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/aku.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/behemoth_culling.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/behemoth_culling.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/clear_tutorial.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/clear_tutorial.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/enigma_stages.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/enigma_stages.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/event_stages.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/event_stages.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/gauntlet.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/gauntlet.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/itf_timed_scores.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/itf_timed_scores.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/legend_quest.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/legend_quest.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/main_story.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/main_story.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/outbreaks.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/outbreaks.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/story_level_id_selector.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/story_level_id_selector.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/towers.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/towers.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/treasures.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/treasures.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/uncanny.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/uncanny.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/levels/unlock_aku_realm.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/levels/unlock_aku_realm.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/other/cat_shrine.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/other/cat_shrine.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/other/claim_user_rank_rewards.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/other/claim_user_rank_rewards.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/other/create_new_account.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/other/create_new_account.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/other/fix_elsewhere.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/other/fix_elsewhere.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/other/fix_time_issues.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/other/fix_time_issues.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/other/get_gold_pass.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/other/get_gold_pass.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/other/meow_medals.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/other/meow_medals.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/other/missions.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/other/missions.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/other/play_time.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/other/play_time.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/other/scheme_item.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/other/scheme_item.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/other/trade_progress.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/other/trade_progress.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/other/unlock_enemy_guide.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/other/unlock_enemy_guide.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/save_management/load.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/save_management/load.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/save_management/other.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/save_management/other.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,18 +4,16 @@
 
 from ... import adb_handler, helper
 
 
 def export(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Export the save stats to a json file"""
 
-    helper.export_json(save_stats, helper.get_save_path() + ".json")
+    file = helper.export_json(save_stats, helper.get_save_path() + ".json")
 
-    file = helper.get_save_path() + ".json"
-    
     return save_stats, file
 
 
 def clear_data(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Clear data wrapper for the clear_data function"""
 
     confirm = input("Do want to clear your data (y/n)?:").lower()
```

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/save_management/save.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/save_management/save.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/edits/save_management/server_upload.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/edits/save_management/server_upload.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/feature_handler.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/feature_handler.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/game_data_getter.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/game_data_getter.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/helper.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -830,15 +830,15 @@
     """Export the save stats to a json file"""
 
     ordered_data = parse_save.re_order(save_stats)
     if os.path.isdir(path):
         path = os.path.join(path, f"{get_save_path_home()}.json")
     write_file_string(path, json.dumps(ordered_data, indent=4))
     colored_text(f"Successfully wrote json to &{os.path.abspath(path)}&")
-    
+    return os.path.abspath(path)
 
 
 def load_json_handler(json_path: str) -> Union[None, str]:
     """Load a save_data json file and serialise it"""
 
     save_stats = load_json(json_path)
     save_data = serialise_save.start_serialize(save_stats)
```

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/item.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/item.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/managed_item.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/managed_item.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/parse_save.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/parse_save.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/patcher.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/patcher.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/root_handler.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/root_handler.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/serialise_save.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/serialise_save.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/server_handler.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/server_handler.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/tracker.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/tracker.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/updater.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/updater.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/BCSFE_Python_Discord/user_input_handler.py` & `bcsfe-discord-2.7.9/src/BCSFE_Python_Discord/user_input_handler.py`

 * *Files identical despite different names*

### Comparing `bcsfe-discord-2.7.8/src/bcsfe_discord.egg-info/SOURCES.txt` & `bcsfe-discord-2.7.9/src/bcsfe_discord.egg-info/SOURCES.txt`

 * *Files identical despite different names*

