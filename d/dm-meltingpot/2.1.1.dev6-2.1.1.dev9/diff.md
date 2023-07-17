# Comparing `tmp/dm-meltingpot-2.1.1.dev6.tar.gz` & `tmp/dm-meltingpot-2.1.1.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dm-meltingpot-2.1.1.dev6.tar", last modified: Thu Jun 29 07:28:56 2023, max compression
+gzip compressed data, was "dm-meltingpot-2.1.1.dev9.tar", last modified: Fri Jul 14 16:06:57 2023, max compression
```

## Comparing `dm-meltingpot-2.1.1.dev6.tar` & `dm-meltingpot-2.1.1.dev9.tar`

### file list

```diff
@@ -1,101 +1,274 @@
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:28:56.796981 dm-meltingpot-2.1.1.dev6/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    11358 2022-06-29 10:08:59.000000 dm-meltingpot-2.1.1.dev6/LICENSE
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     8547 2023-06-29 07:28:56.796804 dm-meltingpot-2.1.1.dev6/PKG-INFO
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     7567 2023-06-28 09:22:13.000000 dm-meltingpot-2.1.1.dev6/README.md
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:28:56.787854 dm-meltingpot-2.1.1.dev6/dm_meltingpot.egg-info/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     8547 2023-06-29 07:28:56.000000 dm-meltingpot-2.1.1.dev6/dm_meltingpot.egg-info/PKG-INFO
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     3183 2023-06-29 07:28:56.000000 dm-meltingpot-2.1.1.dev6/dm_meltingpot.egg-info/SOURCES.txt
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)        1 2023-06-29 07:28:56.000000 dm-meltingpot-2.1.1.dev6/dm_meltingpot.egg-info/dependency_links.txt
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)      294 2023-06-29 07:28:56.000000 dm-meltingpot-2.1.1.dev6/dm_meltingpot.egg-info/requires.txt
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)       11 2023-06-29 07:28:56.000000 dm-meltingpot-2.1.1.dev6/dm_meltingpot.egg-info/top_level.txt
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:28:56.787984 dm-meltingpot-2.1.1.dev6/meltingpot/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)      595 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/__init__.py
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:28:56.786381 dm-meltingpot-2.1.1.dev6/meltingpot/lua/
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:28:56.786283 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:28:56.788292 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/allelopathic_harvest/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    32772 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/allelopathic_harvest/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1414 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/allelopathic_harvest/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:28:56.788578 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/boat_race/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    30236 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/boat_race/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     2292 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/boat_race/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:28:56.788875 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/clean_up/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    17922 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/clean_up/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1402 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/clean_up/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:28:56.789135 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/coins/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    11909 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/coins/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1399 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/coins/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:28:56.789421 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/collaborative_cooking/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    18568 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/collaborative_cooking/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1411 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/collaborative_cooking/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:28:56.789693 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/commons_harvest/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     8393 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/commons_harvest/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1405 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/commons_harvest/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:28:56.789980 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/coop_mining/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     9293 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/coop_mining/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1401 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/coop_mining/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:28:56.790266 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/daycare/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    24162 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/daycare/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1387 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/daycare/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:28:56.790531 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/externality_mushrooms/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    13306 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/externality_mushrooms/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1390 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/externality_mushrooms/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:28:56.790818 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/factory_of_the_commons/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    27587 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/factory_of_the_commons/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     2753 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/factory_of_the_commons/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:28:56.791099 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/gift_refinements/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    13877 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/gift_refinements/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1406 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/gift_refinements/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:28:56.791383 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/grid_land/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    28617 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/grid_land/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1503 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/grid_land/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:28:56.791688 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/hidden_agenda/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    58910 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/hidden_agenda/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1129 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/hidden_agenda/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:28:56.791831 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/paintball/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    15261 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/paintball/shared_components.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:28:56.792111 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/paintball__capture_the_flag/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    12969 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/paintball__capture_the_flag/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1729 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/paintball__capture_the_flag/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:28:56.792389 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/paintball__king_of_the_hill/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    11357 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/paintball__king_of_the_hill/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1729 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/paintball__king_of_the_hill/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:28:56.792669 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/predator_prey/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    28175 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/predator_prey/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     2214 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/predator_prey/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:28:56.792806 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/stamina/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    15208 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/stamina/shared_components.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:28:56.793066 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/territory/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    14438 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/territory/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1704 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/territory/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:28:56.793360 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/the_matrix/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    43847 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/the_matrix/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1396 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/the_matrix/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:28:56.793649 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/trade/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    34427 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/trade/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1749 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/trade/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:28:56.796612 dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     3528 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/api_factory.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     6450 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/avatar_grappling.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     9559 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/avatar_grasp.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    46382 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/avatar_library.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     2765 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/avatar_library_test.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    22521 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/base_simulation.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     4761 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/base_simulation_test.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     4388 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/colors.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     3536 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/component.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    42148 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/component_library.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     2627 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/component_library_test.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1721 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/component_registry.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1904 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/component_registry_test.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     5483 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/error_handling.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     2421 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/error_handling_test.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    21610 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/game_object.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    12410 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/game_object_test.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     2585 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/piece_movement_test.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     6260 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/prefab_utils.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     6046 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/prefab_utils_test.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    11744 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/updater_registry.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    12308 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/updater_registry_test.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)      214 2023-06-28 09:22:13.000000 dm-meltingpot-2.1.1.dev6/pyproject.toml
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)       38 2023-06-29 07:28:56.797028 dm-meltingpot-2.1.1.dev6/setup.cfg
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     4748 2023-06-29 07:28:41.000000 dm-meltingpot-2.1.1.dev6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.128118 dm-meltingpot-2.1.1.dev9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-14 16:06:57.128118 dm-meltingpot-2.1.1.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.084118 dm-meltingpot-2.1.1.dev9/dm_meltingpot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-14 16:06:57.000000 dm-meltingpot-2.1.1.dev9/dm_meltingpot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12402 2023-07-14 16:06:57.000000 dm-meltingpot-2.1.1.dev9/dm_meltingpot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:06:57.000000 dm-meltingpot-2.1.1.dev9/dm_meltingpot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-14 16:06:57.000000 dm-meltingpot-2.1.1.dev9/dm_meltingpot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-14 16:06:57.000000 dm-meltingpot-2.1.1.dev9/dm_meltingpot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.080118 dm-meltingpot-2.1.1.dev9/meltingpot/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.080118 dm-meltingpot-2.1.1.dev9/meltingpot/lua/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.080118 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.084118 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/allelopathic_harvest/
+-rw-r--r--   0 runner    (1001) docker     (123)    32772 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/allelopathic_harvest/components.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/allelopathic_harvest/init.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.084118 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/boat_race/
+-rw-r--r--   0 runner    (1001) docker     (123)    30236 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/boat_race/components.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/boat_race/init.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.084118 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/clean_up/
+-rw-r--r--   0 runner    (1001) docker     (123)    17922 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/clean_up/components.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/clean_up/init.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.084118 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/coins/
+-rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/coins/components.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/coins/init.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.084118 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/collaborative_cooking/
+-rw-r--r--   0 runner    (1001) docker     (123)    18568 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/collaborative_cooking/components.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/collaborative_cooking/init.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.084118 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/commons_harvest/
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/commons_harvest/components.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/commons_harvest/init.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.084118 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/coop_mining/
+-rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/coop_mining/components.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/coop_mining/init.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.088118 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/daycare/
+-rw-r--r--   0 runner    (1001) docker     (123)    24162 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/daycare/components.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/daycare/init.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.088118 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/externality_mushrooms/
+-rw-r--r--   0 runner    (1001) docker     (123)    13306 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/externality_mushrooms/components.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/externality_mushrooms/init.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.088118 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/factory_of_the_commons/
+-rw-r--r--   0 runner    (1001) docker     (123)    27587 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/factory_of_the_commons/components.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/factory_of_the_commons/init.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.088118 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/gift_refinements/
+-rw-r--r--   0 runner    (1001) docker     (123)    13877 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/gift_refinements/components.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/gift_refinements/init.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.088118 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/grid_land/
+-rw-r--r--   0 runner    (1001) docker     (123)    28617 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/grid_land/components.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/grid_land/init.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.088118 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/hidden_agenda/
+-rw-r--r--   0 runner    (1001) docker     (123)    58910 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/hidden_agenda/components.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/hidden_agenda/init.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.088118 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/paintball/
+-rw-r--r--   0 runner    (1001) docker     (123)    15261 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/paintball/shared_components.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.088118 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/paintball__capture_the_flag/
+-rw-r--r--   0 runner    (1001) docker     (123)    12969 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/paintball__capture_the_flag/components.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/paintball__capture_the_flag/init.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.088118 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/paintball__king_of_the_hill/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/paintball__king_of_the_hill/components.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/paintball__king_of_the_hill/init.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.092118 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/predator_prey/
+-rw-r--r--   0 runner    (1001) docker     (123)    28175 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/predator_prey/components.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/predator_prey/init.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.092118 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/stamina/
+-rw-r--r--   0 runner    (1001) docker     (123)    15208 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/stamina/shared_components.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.092118 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/territory/
+-rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/territory/components.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/territory/init.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.092118 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/the_matrix/
+-rw-r--r--   0 runner    (1001) docker     (123)    43847 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/the_matrix/components.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/the_matrix/init.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.092118 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/trade/
+-rw-r--r--   0 runner    (1001) docker     (123)    34427 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/trade/components.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/trade/init.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.096118 dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/api_factory.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/avatar_grappling.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     9559 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/avatar_grasp.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    46382 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/avatar_library.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/avatar_library_test.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    22521 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/base_simulation.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/base_simulation_test.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/colors.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/component.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    42148 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/component_library.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/component_library_test.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/component_registry.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/component_registry_test.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/error_handling.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/error_handling_test.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    21610 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/game_object.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    12410 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/game_object_test.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/piece_movement_test.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/prefab_utils.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/prefab_utils_test.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    11744 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/updater_registry.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    12308 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/updater_registry_test.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.096118 dm-meltingpot-2.1.1.dev9/meltingpot/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/bot_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.096118 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.100118 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)   135960 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/bots/bot_configs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.100118 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (123)   161988 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/scenarios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/scenarios/scenario_configs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.112118 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35017 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/allelopathic_harvest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/allelopathic_harvest__open.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18564 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/bach_or_stravinsky_in_the_matrix__arena.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18521 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/bach_or_stravinsky_in_the_matrix__repeated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28622 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/boat_race.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/boat_race__eight_races.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/chemistry__three_metabolic_cycles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17185 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/chemistry__three_metabolic_cycles_with_plentiful_distractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14017 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/chemistry__two_metabolic_cycles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/chemistry__two_metabolic_cycles_with_distractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18910 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/chicken_in_the_matrix__arena.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20558 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/chicken_in_the_matrix__repeated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26851 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/clean_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16931 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/coins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26329 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/collaborative_cooking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/collaborative_cooking__asymmetric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/collaborative_cooking__circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/collaborative_cooking__cramped.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/collaborative_cooking__crowded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/collaborative_cooking__figure_eight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/collaborative_cooking__forced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/collaborative_cooking__ring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17547 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/commons_harvest__closed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18780 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/commons_harvest__open.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/commons_harvest__partnership.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14508 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/coop_mining.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29111 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/daycare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36385 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/externality_mushrooms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/externality_mushrooms__dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76885 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/factory_commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/factory_commons__either_or.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42413 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/fruit_market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/fruit_market__concentric_rivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16195 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/gift_refinements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50815 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/hidden_agenda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27689 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/paintball__capture_the_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25977 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/paintball__king_of_the_hill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52934 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/predator_prey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/predator_prey__alley_hunt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/predator_prey__open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/predator_prey__orchard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/predator_prey__random_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18574 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/prisoners_dilemma_in_the_matrix__arena.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20458 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/prisoners_dilemma_in_the_matrix__repeated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20555 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/pure_coordination_in_the_matrix__arena.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20614 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/pure_coordination_in_the_matrix__repeated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20678 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/rationalizable_coordination_in_the_matrix__arena.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20591 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/rationalizable_coordination_in_the_matrix__repeated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19927 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/reaction_graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19369 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/running_with_scissors_in_the_matrix__arena.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22192 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/running_with_scissors_in_the_matrix__one_shot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22588 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/running_with_scissors_in_the_matrix__repeated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18912 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/stag_hunt_in_the_matrix__arena.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20380 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/stag_hunt_in_the_matrix__repeated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27209 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/territory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/territory__inside_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/territory__open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/territory__rooms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/substrates/the_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.116118 dm-meltingpot-2.1.1.dev9/meltingpot/python/human_players/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/human_players/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14328 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/human_players/level_playing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/human_players/play_allelopathic_harvest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/human_players/play_anything_in_the_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/human_players/play_boat_race.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/human_players/play_chemistry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/human_players/play_clean_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/human_players/play_coins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/human_players/play_collaborative_cooking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/human_players/play_commons_harvest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/human_players/play_coop_mining.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/human_players/play_daycare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/human_players/play_externality_mushrooms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/human_players/play_factory_commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/human_players/play_fruit_market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/human_players/play_gift_refinements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/human_players/play_hidden_agenda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/human_players/play_level_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/human_players/play_paintball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/human_players/play_predator_and_prey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/human_players/play_territory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/scenario_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/substrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/substrate_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.116118 dm-meltingpot-2.1.1.dev9/meltingpot/python/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/testing/bots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/testing/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/testing/mocks_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/testing/substrates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.116118 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.116118 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/evaluation/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/evaluation/evaluation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.120118 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/policies/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/policies/fixed_action_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/policies/permissive_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/policies/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/policies/policy_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/policies/puppet_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/policies/saved_model_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.124118 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/puppeteers/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/puppeteers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/puppeteers/alternator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/puppeteers/alternator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/puppeteers/clean_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/puppeteers/clean_up_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/puppeteers/coins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/puppeteers/coins_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/puppeteers/coordination_in_the_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/puppeteers/coordination_in_the_matrix_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/puppeteers/fixed_goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/puppeteers/fixed_goal_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/puppeteers/gift_refinements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/puppeteers/gift_refinements_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/puppeteers/in_the_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18705 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/puppeteers/in_the_matrix_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/puppeteers/puppeteer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/puppeteers/running_with_scissors_in_the_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/puppeteers/running_with_scissors_in_the_matrix_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/puppeteers/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.124118 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/scenarios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/scenarios/population.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11427 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/scenarios/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/scenarios/scenario_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/scenarios/scenario_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.124118 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/substrates/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/substrates/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/substrates/builder_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/substrates/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/substrates/game_object_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/substrates/game_object_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/substrates/map_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20231 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/substrates/reaction_graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71300 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/substrates/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/substrates/shapes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/substrates/specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/substrates/substrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/substrates/substrate_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/substrates/substrate_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:57.128118 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/substrates/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/substrates/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/substrates/wrappers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/substrates/wrappers/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/substrates/wrappers/collective_reward_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/substrates/wrappers/collective_reward_wrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/substrates/wrappers/discrete_action_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/substrates/wrappers/discrete_action_wrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/substrates/wrappers/multiplayer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/substrates/wrappers/multiplayer_wrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/substrates/wrappers/observables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/substrates/wrappers/observables_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/substrates/wrappers/observables_wrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/meltingpot/python/utils/substrates/wrappers/reset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:06:57.128118 dm-meltingpot-2.1.1.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-07-14 16:06:32.000000 dm-meltingpot-2.1.1.dev9/setup.py
```

### Comparing `dm-meltingpot-2.1.1.dev6/LICENSE` & `dm-meltingpot-2.1.1.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/PKG-INFO` & `dm-meltingpot-2.1.1.dev9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,13 @@
-Metadata-Version: 2.1
-Name: dm-meltingpot
-Version: 2.1.1.dev6
-Summary: A suite of test scenarios for multi-agent reinforcement learning.
-Home-page: https://github.com/deepmind/meltingpot
-Download-URL: https://github.com/deepmind/meltingpot
-Author: DeepMind
-Author-email: noreply@google.com
-License: Apache 2.0
-Keywords: multi-agent reinforcement-learning python machine-learning
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: rllib
-Provides-Extra: pettingzoo
-License-File: LICENSE
-
 # Melting Pot
 
 *A suite of test scenarios for multi-agent reinforcement learning.*
 
 
-[![meltingpot-tests](../../actions/workflows/ci.yml/badge.svg)](../../actions/workflows/ci.yml)
+[![Tests](../../actions/workflows/ci.yml/badge.svg)](../../actions/workflows/ci.yml)
 
 <div align="center">
   <img src="docs/images/meltingpot_montage.gif"
        alt="Melting Pot substrates"
        height="250" width="250" />
 </div>
 
@@ -64,33 +39,14 @@
 [Extending Melting Pot](docs/extending.md) documentation.
 
 ## Installation
 
 Melting Pot is built on top of
 [DeepMind Lab2D](https://github.com/deepmind/lab2d).
 
-### Devcontainer (x86 only)
-
-*NOTE: This Devcontainer only works for x86 platforms. For arm64 (newer M1 Macs) users will have to follow the manual installation steps.*
-
-This project includes a pre-configured development environment ([devcontainer](https://containers.dev)).
-
-You can launch a working development environment with one click, using e.g. [Github
-Codespaces](https://github.com/features/codespaces) or the [VSCode
-Containers](https://code.visualstudio.com/docs/remote/containers-tutorial)
-extension.
-
-#### CUDA support
-
-To enable CUDA support (required for GPU training), make sure you have the
-[nvidia-container-toolkit](https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/install-guide.html)
-package installed, and then run Docker with the `---gpus all` flag enabled. Note
-that for GitHub Codespaces this isn't necessary, as it's done for you
-automatically.
-
 ### Manual install
 
 The installation steps are as follows:
 
 1.  (Optional) Activate a virtual environment, e.g.:
 
     ```shell
@@ -143,39 +99,82 @@
     [`install-extras.sh`](https://github.com/deepmind/meltingpot/blob/main/install-meltingpot.sh)
     for an example installation script):
 
     ```shell
     pip install .[rllib,pettingzoo]
     ```
 
+### Devcontainer (x86 only)
+
+*NOTE: This Devcontainer only works for x86 platforms. For arm64 (newer M1 Macs)
+users will have to follow the manual installation steps.*
+
+This project includes a pre-configured development environment
+([devcontainer](https://containers.dev)).
+
+You can launch a working development environment with one click, using e.g.
+[Github Codespaces](https://github.com/features/codespaces) or the
+[VSCode Containers](https://code.visualstudio.com/docs/remote/containers-tutorial)
+extension.
+
+#### CUDA support
+
+To enable CUDA support (required for GPU training), make sure you have the
+[nvidia-container-toolkit](https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/install-guide.html)
+package installed, and then run Docker with the `---gpus all` flag enabled. Note
+that for GitHub Codespaces this isn't necessary, as it's done for you
+automatically.
+
 ## Example usage
 
+### Evaluation
+
+The [evaluation](meltingpot/python/evaluation/evaluation.py) library can be used
+to evaluate [SavedModel](https://www.tensorflow.org/guide/saved_model)s
+trained on Melting Pot substrates.
+
+Evaluation results from the [Melting Pot 2.0 Tech Report](https://arxiv.org/abs/2211.13746)
+can be viewed in the [Evaluation Notebook](notebooks/evaluation_results.ipynb).
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/deepmind/meltingpot/blob/main/notebooks/evaluation_results.ipynb)
+
+### Interacting with the substrates
+
 You can try out the substrates interactively with the
-[human_players](meltingpot/python/human_players) scripts. For example, to play the
-`clean_up` substrate, you can run:
+[human_players](meltingpot/python/human_players) scripts. For example, to play
+the `clean_up` substrate, you can run:
 
 ```shell
 python3 meltingpot/python/human_players/play_clean_up.py
 ```
 
 You can move around with the `W`, `A`, `S`, `D` keys, Turn with `Q`, and `E`,
 fire the zapper with `1`, and fire the cleaning beam with `2`. You can switch
 between players with `TAB`. There are other substrates available in the
-[human_players](meltingpot/python/human_players) directory. Some have multiple variants,
-which you select with the `--level_name` flag.
+[human_players](meltingpot/python/human_players) directory. Some have multiple
+variants, which you select with the `--level_name` flag.
 
 NOTE: If you get a `ModuleNotFoundError: No module named 'meltingpot.python'`
       error, you can solve it by exporting the meltingpot home directory as
       `PYTHONPATH` (e.g. by calling `export PYTHONPATH=$(pwd)`).
 
 ### Training agents
-We provide two example scripts using RLlib and [PettingZoo](https://github.com/Farama-Foundation/PettingZoo) with [Stable-Baselines3](https://github.com/DLR-RM/stable-baselines3) (SB3) respectively. Note that Melting Pot is agnostic to how you train your agents, and as such, these scripts are not meant to be a suggestion on how to achieve good scores in the task suite.
+
+We provide two example scripts: one using
+[RLlib](https://github.com/ray-project/ray), and another using
+[PettingZoo](https://github.com/Farama-Foundation/PettingZoo) with
+[Stable-Baselines3](https://github.com/DLR-RM/stable-baselines3) (SB3). Note
+that Melting Pot is agnostic to how you train your agents, and as such, these
+scripts are not meant to be a suggestion on how to achieve good scores in the
+task suite.
 
 #### RLlib
-This example uses [RLLib](https://github.com/ray-project/ray) to train agents in self-play on a Melting Pot substrate.
+
+This example uses RLlib to train agents in
+self-play on a Melting Pot substrate.
 
 First you will need to install the dependencies needed by the RLlib example:
 
 ```shell
 cd <meltingpot_root>
 pip3 install -e .[rllib]
 ```
@@ -184,36 +183,32 @@
 
 ```shell
 cd <meltingpot_root>/examples/rllib
 python3 self_play_train.py
 ```
 
 #### PettingZoo and Stable-Baselines3
-This example uses a PettingZoo wrapper with a fully parameter shared PPO agent from SB3.
+
+This example uses a PettingZoo wrapper with a fully parameter shared PPO agent
+from SB3.
 
 The PettingZoo wrapper can be used separately from SB3 and
 can be found [here](examples/pettingzoo/utils.py).
 
 ```shell
 cd <meltingpot_root>
 pip3 install -e .[pettingzoo]
 ```
 
 ```shell
 cd <meltingpot_root>/examples/pettingzoo
 python3 sb3_train.py
 ```
 
-### Evaluation
-
-Evaluation results from the [Melting Pot 2.0 Tech Report](https://arxiv.org/abs/2211.13746)
-can be viewed in the [Evaluation Notebook](notebooks/evaluation_results.ipynb).
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/deepmind/meltingpot/blob/main/notebooks/evaluation_results.ipynb)
-
-### Documentation
+## Documentation
 
 Full documentation is available [here](docs/index.md).
 
 ## Citing Melting Pot
 
 If you use Melting Pot in your work, please cite the accompanying article:
 
@@ -223,14 +218,16 @@
            Melting Pot},
     author={Joel Z. Leibo AND Edgar Du\'e\~nez-Guzm\'an AND Alexander Sasha
             Vezhnevets AND John P. Agapiou AND Peter Sunehag AND Raphael Koster
             AND Jayd Matyas AND Charles Beattie AND Igor Mordatch AND Thore
             Graepel},
     year={2021},
     journal={International conference on machine learning},
-    organization={PMLR}
+    organization={PMLR},
+    url={https://doi.org/10.48550/arXiv.2107.06857},
+    doi={10.48550/arXiv.2107.06857}
 }
 ```
 
 ## Disclaimer
 
 This is not an officially supported Google product.
```

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/__init__.py` & `dm-meltingpot-2.1.1.dev9/meltingpot/python/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/allelopathic_harvest/components.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/allelopathic_harvest/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/allelopathic_harvest/init.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/allelopathic_harvest/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/boat_race/components.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/boat_race/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/boat_race/init.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/boat_race/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/clean_up/components.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/clean_up/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/clean_up/init.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/clean_up/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/coins/components.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/coins/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/coins/init.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/coins/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/collaborative_cooking/components.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/collaborative_cooking/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/collaborative_cooking/init.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/collaborative_cooking/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/commons_harvest/components.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/commons_harvest/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/commons_harvest/init.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/commons_harvest/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/coop_mining/components.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/coop_mining/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/coop_mining/init.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/coop_mining/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/daycare/components.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/daycare/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/daycare/init.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/daycare/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/externality_mushrooms/components.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/externality_mushrooms/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/externality_mushrooms/init.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/externality_mushrooms/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/factory_of_the_commons/components.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/factory_of_the_commons/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/factory_of_the_commons/init.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/factory_of_the_commons/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/gift_refinements/components.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/gift_refinements/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/gift_refinements/init.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/gift_refinements/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/grid_land/components.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/grid_land/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/grid_land/init.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/grid_land/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/hidden_agenda/components.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/hidden_agenda/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/hidden_agenda/init.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/hidden_agenda/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/paintball/shared_components.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/paintball/shared_components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/paintball__capture_the_flag/components.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/paintball__capture_the_flag/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/paintball__capture_the_flag/init.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/paintball__capture_the_flag/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/paintball__king_of_the_hill/components.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/paintball__king_of_the_hill/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/paintball__king_of_the_hill/init.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/paintball__king_of_the_hill/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/predator_prey/components.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/predator_prey/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/predator_prey/init.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/predator_prey/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/stamina/shared_components.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/stamina/shared_components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/territory/components.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/territory/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/territory/init.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/territory/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/the_matrix/components.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/the_matrix/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/the_matrix/init.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/the_matrix/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/trade/components.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/trade/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/levels/trade/init.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/levels/trade/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/api_factory.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/api_factory.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/avatar_grappling.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/avatar_grappling.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/avatar_grasp.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/avatar_grasp.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/avatar_library.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/avatar_library.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/avatar_library_test.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/avatar_library_test.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/base_simulation.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/base_simulation.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/base_simulation_test.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/base_simulation_test.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/colors.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/colors.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/component.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/component.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/component_library.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/component_library.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/component_library_test.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/component_library_test.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/component_registry.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/component_registry.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/component_registry_test.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/component_registry_test.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/error_handling.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/error_handling.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/error_handling_test.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/error_handling_test.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/game_object.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/game_object.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/game_object_test.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/game_object_test.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/piece_movement_test.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/piece_movement_test.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/prefab_utils.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/prefab_utils.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/prefab_utils_test.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/prefab_utils_test.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/updater_registry.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/updater_registry.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/meltingpot/lua/modules/updater_registry_test.lua` & `dm-meltingpot-2.1.1.dev9/meltingpot/lua/modules/updater_registry_test.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev6/setup.py` & `dm-meltingpot-2.1.1.dev9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import shutil
 import tarfile
 import urllib.request
 
 import setuptools
 from setuptools.command import build_py
 
-VERSION = '2.1.1-dev.6'
+VERSION = '2.1.1-dev.9'
 ASSETS_VERSION = '2.1.0'
 
 ASSETS_URL = f'http://storage.googleapis.com/dm-meltingpot/meltingpot-assets-{ASSETS_VERSION}.tar.gz'
 
 IS_M1_MAC = platform.system() == 'Darwin' and platform.machine() == 'arm64'
 
 
@@ -47,24 +47,27 @@
       print(f'found cached assets {tar_file_path}', flush=True)
     else:
       os.makedirs(os.path.dirname(tar_file_path), exist_ok=True)
       print('downloading assets...', flush=True)
       urllib.request.urlretrieve(ASSETS_URL, filename=tar_file_path)
       print(f'downloaded {tar_file_path}', flush=True)
 
-    root = self.get_package_dir('meltingpot')
+    root = os.path.join(self.get_package_dir(''), 'meltingpot')
+    os.makedirs(root, exist_ok=True)
     if os.path.exists(f'{root}/assets'):
       shutil.rmtree(f'{root}/assets')
       print('deleted existing assets', flush=True)
     with tarfile.open(tar_file_path, mode='r|*') as tarball:
       tarball.extractall(root)
     print(f'extracted assets from {tar_file_path} to {root}/assets', flush=True)
 
   def build_assets(self):
-    package_root = self.get_package_dir('meltingpot')
+    """Copies assets from package to build lib."""
+    package_root = os.path.join(self.get_package_dir(''), 'meltingpot')
+    os.makedirs(package_root, exist_ok=True)
     build_root = os.path.join(self.build_lib, 'meltingpot')
     if os.path.exists(f'{build_root}/assets'):
       shutil.rmtree(f'{build_root}/assets')
       print('deleted existing assets', flush=True)
     shutil.copytree(f'{package_root}/assets', f'{build_root}/assets')
     print(f'copied assets from {package_root}/assets to {build_root}/assets',
           flush=True)
@@ -72,68 +75,68 @@
 
 setuptools.setup(
     name='dm-meltingpot',
     version=VERSION,
     license='Apache 2.0',
     license_files=['LICENSE'],
     url='https://github.com/deepmind/meltingpot',
-    download_url='https://github.com/deepmind/meltingpot',
+    download_url='https://github.com/deepmind/meltingpot/releases',
     author='DeepMind',
     author_email='noreply@google.com',
     description=(
         'A suite of test scenarios for multi-agent reinforcement learning.'),
-    long_description=open('README.md').read(),
-    long_description_content_type='text/markdown',
     keywords='multi-agent reinforcement-learning python machine-learning',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Intended Audience :: Education',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: POSIX :: Linux',
         'Operating System :: MacOS :: MacOS X',
         'Programming Language :: Python :: 3 :: Only',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
     ],
     cmdclass={'build_py': BuildPy},
-    packages=['meltingpot'],
+    package_dir={
+        'meltingpot': 'meltingpot/python',
+        'meltingpot.lua': 'meltingpot/lua',
+    },
     package_data={
-        'meltingpot': [
-            'lua/modules/*',
-            'lua/levels/**/*',
-        ],
+        'meltingpot.lua': ['**'],
     },
     python_requires='>=3.9',
     install_requires=[
         'absl-py',
         'chex',
         'dm_env',
-        'dmlab2d==1.0.0.dev7',
+        'dmlab2d',
+        'dm-tree',
         'immutabledict',
         'ml-collections',
         'networkx',
         'numpy',
         'opencv-python',
         'pandas',
         'pygame',
         'reactivex',
         'tensorflow-macos' if IS_M1_MAC else 'tensorflow',
     ],
     extras_require={
         # Dependencies required for rllib example.
         'rllib': [
-            'dm-tree',
             'gym',
             'ray[rllib,default]==2.0.0',
             'numpy<1.23',  # Needed by Ray because it uses `np.bool`.
         ],
         # Dependencies required for pettingzoo example.
         'pettingzoo': [
-            'dm-tree',
             'gym',
             'matplotlib',
             'pettingzoo>=1.22.3',
             'stable-baselines3',
             'supersuit>=3.7.2',
             'torch',
         ],
```

