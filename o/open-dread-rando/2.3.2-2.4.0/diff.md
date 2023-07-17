# Comparing `tmp/open-dread-rando-2.3.2.tar.gz` & `tmp/open-dread-rando-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-dread-rando-2.3.2.tar", last modified: Thu Jun 15 12:14:30 2023, max compression
+gzip compressed data, was "open-dread-rando-2.4.0.tar", last modified: Mon Jul 17 10:10:51 2023, max compression
```

## Comparing `open-dread-rando-2.3.2.tar` & `open-dread-rando-2.4.0.tar`

### file list

```diff
@@ -1,242 +1,222 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.772692 open-dread-rando-2.3.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.748692 open-dread-rando-2.3.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.748692 open-dread-rando-2.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/.github/workflows/patch.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/.github/workflows/python.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.748692 open-dread-rando-2.3.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-15 12:14:30.772692 open-dread-rando-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.752692 open-dread-rando-2.3.2/open_dread_rando/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.752692 open-dread-rando-2.3.2/open_dread_rando/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/__pyinstaller/hook-open_dread_rando.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/cosmetic_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/custom_door_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    21271 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/door_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/dread_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/elevator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/environmental_damage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/environmental_damage_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/exefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.756692 open-dread-rando-2.3.2/open_dread_rando/files/
--rw-r--r--   0 runner    (1001) docker     (123)    15151 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/custom_scenario.lua
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.756692 open-dread-rando-2.3.2/open_dread_rando/files/dread_depackager/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/dread_depackager/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/dread_depackager/main.npdm
--rw-r--r--   0 runner    (1001) docker     (123)   190964 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/dread_depackager/subsdk9
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.756692 open-dread-rando-2.3.2/open_dread_rando/files/exefs_patches/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/exefs_patches/debug_input.s
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.756692 open-dread-rando-2.3.2/open_dread_rando/files/levels/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/levels/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)    67135 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/levels/s010_cave.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    37704 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/levels/s020_magma.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    23300 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/levels/s030_baselab.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    32062 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/levels/s040_aqua.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    25145 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/levels/s050_forest.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/levels/s060_quarantine.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    30569 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/levels/s070_basesanc.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    16577 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/levels/s080_shipyard.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/levels/s090_skybase.lc.lua
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.756692 open-dread-rando-2.3.2/open_dread_rando/files/lua_libraries/
--rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/lua_libraries/bit.lua
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/lua_libraries/data_structures.lua
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/lua_libraries/death_counter.lua
--rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/lua_libraries/guilib.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/lua_libraries/input_handling.lua
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/lua_libraries/room_names.lua
--rw-r--r--   0 runner    (1001) docker     (123)    26346 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/msemenu_mainmenu.lua
--rw-r--r--   0 runner    (1001) docker     (123)    12659 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/randomizer_powerup.lua
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.748692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.744692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.740692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.736692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/item_cube/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.736692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/item_cube/model/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.756692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_camo.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_sonr.bsmat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.736692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/item_cube_broken/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.756692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/
--rw-r--r--   0 runner    (1001) docker     (123)   422936 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_camo.bcmdl
--rw-r--r--   0 runner    (1001) docker     (123)   422936 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_sonr.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.736692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/item_missiletank/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.760692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/item_missiletank/models/
--rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__BK.bcmdl
--rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__BL.bcmdl
--rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__CY.bcmdl
--rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__GN.bcmdl
--rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__GY.bcmdl
--rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__MG.bcmdl
--rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__OR.bcmdl
--rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__PK.bcmdl
--rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__PR.bcmdl
--rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__WH.bcmdl
--rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/item_missiletank/models/item_missile__YL.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.740692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/itemsphere/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.760692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/itemsphere/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.760692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/speedboost_mp_opaque_01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/itemsphere/models/speed_booster.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.740692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_bomb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.760692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.760692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphhologram.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphmaterial.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    19348 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/powerup_morph.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.740692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_doublejump/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.760692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.760692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_magnet01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_white__01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    33012 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/powerup_magnet.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.740692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.760692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.760692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mat0001.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mp_fxhologram_0001.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    13404 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/powerup_powerbomb.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.740692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_supermissile/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.760692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.760692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/powerup_ice__missile_mp_opaque_01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    28948 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/powerup_ice__missile.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.740692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_widebeam/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.760692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.760692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_autoilum.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_bola.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_cangrejo.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    47996 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/powerup_wavebeam.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.748692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.744692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/doorshieldmissile/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.760692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/doorshieldmissile/collisions/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/doorshieldmissile/collisions/shield_bomb_colls.bmscd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.744692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/doorshieldpowerbomb___/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.760692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/doorshieldpowerbomb___/models/
--rw-r--r--   0 runner    (1001) docker     (123)    23292 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/doorshieldpowerbomb___/models/doorshieldpowerbomb___.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.764692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/doorshieldpowerbomb___/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/doorshieldpowerbomb___/models/imats/doorshieldpowerbomb____mp_opaque_01.bsmat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.744692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/shield___diffusion/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.764692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.764692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/shield_diffusion_matfx.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/shield_diffusion_mp_opaque_01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)   140588 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/shield_diffusion.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.744692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/shield_bombs_regular__/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.764692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/shield_bombs_regular__/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.764692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/shield_bombs_regular__/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/shield_bombs_regular__/models/imats/shield_bombs_regular___mp_opaque_01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    23292 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/shield_bombs_regular__/models/shield_bombs_regular__.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.744692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/shield_cross_bomb_____/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.764692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/shield_cross_bomb_____/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.764692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/shield_cross_bomb_____/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/shield_cross_bomb_____/models/imats/shield_cross_bomb______mp_opaque_01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    23292 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/shield_cross_bomb_____/models/shield_cross_bomb_____.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.748692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/shield_icemissile/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.764692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.764692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/imats/shield_icemissile_mp_opaque_01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    22156 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/shield_icemissile.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.748692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/shield_storm_mssl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.764692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/shield_storm_mssl/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.764692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/shield_storm_mssl/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/shield_storm_mssl/models/imats/shield_storm_mssl_mp_opaque_01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    22156 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/props/shield_storm_mssl/models/shield_storm_mssl.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.748692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.748692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.748692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.748692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/itemsphere/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.748692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.764692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)    28804 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_at.bctex
--rw-r--r--   0 runner    (1001) docker     (123)    19894 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_bc.bctex
--rw-r--r--   0 runner    (1001) docker     (123)    42001 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_nm.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.748692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.748692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.764692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)    14467 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphat.bctex
--rw-r--r--   0 runner    (1001) docker     (123)    17196 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphbc.bctex
--rw-r--r--   0 runner    (1001) docker     (123)    34728 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphnm.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.748692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.748692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.764692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)    75887 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/powerup_spi_magnet_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.748692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.748692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.764692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)    71298 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/powerup_ice__missile_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.748692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.748692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.764692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)   155165 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/pup_wavebeam_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.748692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/props/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.748692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.748692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.764692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)    28577 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshield_____bomb_bc.bctex
--rw-r--r--   0 runner    (1001) docker     (123)    31290 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldcrossbomb_bc.bctex
--rw-r--r--   0 runner    (1001) docker     (123)    35688 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldpowerbomb_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.748692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/props/shield_storm_mssl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.748692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/props/shield_storm_mssl/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.764692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/props/shield_storm_mssl/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)    24331 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/props/shield_storm_mssl/models/textures/shield_storm_mssl_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.748692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/system/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.748692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/system/minimap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.764692 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/system/minimap/icons/
--rw-r--r--   0 runner    (1001) docker     (123)   431407 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/system/minimap/icons/icons.bctex
--rw-r--r--   0 runner    (1001) docker     (123)    28273 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/files/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/game_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/lua_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/lua_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14311 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/map_icons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/missile_color_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    27016 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/model_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/objective.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/output_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/patch_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/patcher_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/pickup.py
--rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/static_fixes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.768692 open-dread-rando-2.3.2/open_dread_rando/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/templates/boss_powerup_template.lua
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/templates/cc_to_room_name.lua
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/templates/custom_core_x.lua
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/templates/custom_core_x_superquetzoa.lua
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/templates/custom_init.lua
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/templates/progressive_model_template.lua
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/templates/randomizer_progressive_template.lua
--rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/templates/template_doorshield_energy_bmsad.json
--rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/templates/template_doorshield_hexs_bmsad.json
--rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/templates/template_doorshield_tris_bmsad.json
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/templates/template_powerup_bmsad.json
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/text_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/tilegroup_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/open_dread_rando/validator_with_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-15 12:14:30.000000 open-dread-rando-2.3.2/open_dread_rando/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.752692 open-dread-rando-2.3.2/open_dread_rando.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-15 12:14:30.000000 open-dread-rando-2.3.2/open_dread_rando.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-06-15 12:14:30.000000 open-dread-rando-2.3.2/open_dread_rando.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 12:14:30.000000 open-dread-rando-2.3.2/open_dread_rando.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-15 12:14:30.000000 open-dread-rando-2.3.2/open_dread_rando.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 12:14:21.000000 open-dread-rando-2.3.2/open_dread_rando.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-15 12:14:30.000000 open-dread-rando-2.3.2/open_dread_rando.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 12:14:30.000000 open-dread-rando-2.3.2/open_dread_rando.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-15 12:14:30.772692 open-dread-rando-2.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.768692 open-dread-rando-2.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/tests/test_dread_patcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:14:30.768692 open-dread-rando-2.3.2/tests/test_files/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/tests/test_files/randomizer_progressive_expected.lua
--rw-r--r--   0 runner    (1001) docker     (123)   153802 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/tests/test_files/starter_preset_patcher.json
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/tests/test_lua_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-15 12:14:04.000000 open-dread-rando-2.3.2/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.080011 open-dread-rando-2.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.064011 open-dread-rando-2.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.064011 open-dread-rando-2.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/.github/workflows/patch.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/.github/workflows/python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.064011 open-dread-rando-2.4.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-17 10:10:51.080011 open-dread-rando-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 10:10:51.080011 open-dread-rando-2.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.052011 open-dread-rando-2.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.068011 open-dread-rando-2.4.0/src/open_dread_rando/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.068011 open-dread-rando-2.4.0/src/open_dread_rando/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/__pyinstaller/hook-open_dread_rando.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/cosmetic_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18393 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/custom_door_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21213 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/door_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/dread_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/elevator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/environmental_damage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/environmental_damage_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/exefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.068011 open-dread-rando-2.4.0/src/open_dread_rando/files/
+-rw-r--r--   0 runner    (1001) docker     (123)    15151 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/custom_scenario.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.068011 open-dread-rando-2.4.0/src/open_dread_rando/files/dread_depackager/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/dread_depackager/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/dread_depackager/main.npdm
+-rw-r--r--   0 runner    (1001) docker     (123)   190964 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/dread_depackager/subsdk9
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.068011 open-dread-rando-2.4.0/src/open_dread_rando/files/exefs_patches/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/exefs_patches/debug_input.s
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.068011 open-dread-rando-2.4.0/src/open_dread_rando/files/levels/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/levels/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    67135 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s010_cave.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    37704 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s020_magma.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    23300 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s030_baselab.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    32062 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s040_aqua.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    25145 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s050_forest.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s060_quarantine.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    30569 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s070_basesanc.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    16577 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s080_shipyard.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s090_skybase.lc.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.072011 open-dread-rando-2.4.0/src/open_dread_rando/files/lua_libraries/
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/lua_libraries/bit.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/lua_libraries/data_structures.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/lua_libraries/death_counter.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/lua_libraries/guilib.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/lua_libraries/input_handling.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/lua_libraries/room_names.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    26346 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/msemenu_mainmenu.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/randomizer_powerup.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.056011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.056011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.056011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.056011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/item_cube/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.056011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/item_cube/model/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.072011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_camo.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_sonr.bsmat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.056011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/item_cube_broken/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.072011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/
+-rw-r--r--   0 runner    (1001) docker     (123)   422936 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_camo.bcmdl
+-rw-r--r--   0 runner    (1001) docker     (123)   422936 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_sonr.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.056011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/itemsphere/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.072011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/itemsphere/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.072011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/speedboost_mp_opaque_01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/itemsphere/models/speed_booster.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.056011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.072011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.072011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphhologram.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphmaterial.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)    19348 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/powerup_morph.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.056011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.072011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.072011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_magnet01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_white__01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)    33012 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/powerup_magnet.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.056011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.072011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.072011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mat0001.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mp_fxhologram_0001.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)    13404 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/powerup_powerbomb.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.056011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.072011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.072011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/powerup_ice__missile_mp_opaque_01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)    28948 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/powerup_ice__missile.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.056011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.072011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.072011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_autoilum.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_bola.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_cangrejo.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)    47996 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/powerup_wavebeam.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.056011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/props/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.056011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/props/doorshieldmissile/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.076011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/props/doorshieldmissile/collisions/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/props/doorshieldmissile/collisions/shield_bomb_colls.bmscd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.056011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.056011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.076011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    28804 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_at.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    19894 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_bc.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    42001 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_nm.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.076011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    14467 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphat.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    17196 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphbc.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    34728 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphnm.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.076011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    75887 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/powerup_spi_magnet_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.076011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    71298 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/powerup_ice__missile_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.076011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)   155165 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/pup_wavebeam_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.076011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    27131 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/models/textures/doorshieldbomb_alt_bc.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    28577 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/models/textures/doorshieldbomb_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldcrossbomb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldcrossbomb/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.076011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldcrossbomb/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    37130 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldcrossbomb/models/textures/doorshieldcrossbomb_alt_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldicemissile/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldicemissile/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.076011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldicemissile/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    49869 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldicemissile/models/textures/doorshieldicemissile_alt_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.076011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)   128743 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/models/textures/shield_no_attribs_at.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)   102269 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/models/textures/shield_no_normals_nm.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.076011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    35688 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldpowerbomb_alt_bc.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    31290 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldpowerbomb_rdv_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.076011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    45613 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/models/textures/doorshieldstormmissile_alt_bc.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    24331 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/models/textures/doorshieldstormmissile_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/shield_diffusion/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/shield_diffusion/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.076011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/shield_diffusion/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    39003 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/shield_diffusion/models/textures/shield_diffusion_alt_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/system/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/system/minimap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.076011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/system/minimap/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)   431407 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/system/minimap/icons/icons.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    29925 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/game_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/lua_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/lua_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14293 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/map_icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/material_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/missile_color_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27001 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/model_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/model_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/output_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/patch_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/patcher_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/pickup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13491 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/static_fixes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.080011 open-dread-rando-2.4.0/src/open_dread_rando/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/templates/boss_powerup_template.lua
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/templates/cc_to_room_name.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/templates/custom_core_x.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/templates/custom_core_x_superquetzoa.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/templates/custom_init.lua
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/templates/progressive_model_template.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/templates/randomizer_progressive_template.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/templates/template_doorshield_energy_bmsad.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/templates/template_doorshield_hexs_bmsad.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/templates/template_doorshield_tris_bmsad.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/templates/template_powerup_bmsad.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/text_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/tilegroup_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/validator_with_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-17 10:10:50.000000 open-dread-rando-2.4.0/src/open_dread_rando/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.068011 open-dread-rando-2.4.0/src/open_dread_rando.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-17 10:10:50.000000 open-dread-rando-2.4.0/src/open_dread_rando.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8381 2023-07-17 10:10:51.000000 open-dread-rando-2.4.0/src/open_dread_rando.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 10:10:50.000000 open-dread-rando-2.4.0/src/open_dread_rando.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-17 10:10:50.000000 open-dread-rando-2.4.0/src/open_dread_rando.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-17 10:10:50.000000 open-dread-rando-2.4.0/src/open_dread_rando.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-17 10:10:50.000000 open-dread-rando-2.4.0/src/open_dread_rando.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.080011 open-dread-rando-2.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/tests/test_dread_patcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.080011 open-dread-rando-2.4.0/tests/test_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/tests/test_files/randomizer_progressive_expected.lua
+-rw-r--r--   0 runner    (1001) docker     (123)   154075 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/tests/test_files/starter_preset_patcher.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/tests/test_lua_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/tests/test_schema.py
```

### Comparing `open-dread-rando-2.3.2/.github/dependabot.yml` & `open-dread-rando-2.4.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/.github/workflows/patch.yml` & `open-dread-rando-2.4.0/.github/workflows/patch.yml`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/.github/workflows/python.yml` & `open-dread-rando-2.4.0/.github/workflows/python.yml`

 * *Files 14% similar despite different names*

```diff
@@ -24,19 +24,16 @@
         uses: actions/setup-python@v4
         with:
           python-version: "3.9"
      
       - name: Install Python packages
         run: python -m pip install --upgrade pip setuptools build
 
-      - name: build wheel
-        run: python -m build --wheel
-
-      - name: build sdist
-        run: python -m build --sdist
+      - name: build
+        run: PYTHONWARNINGS=error python -m build
       
       - name: Store the packages
         uses: actions/upload-artifact@v3
         with:
           name: python-package-distributions
           path: dist
 
@@ -118,27 +115,7 @@
           body: "New release"
 
       - name: Publish 📦 to PyPI
         if: ${{ startsWith(github.ref, 'refs/tags/') }}
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.pypi_password }}
-
-  ruff:
-    runs-on: 'ubuntu-latest'
-
-    steps:
-    - name: Checkout
-      uses: actions/checkout@v3
-      with:
-        fetch-depth: 0
-
-    - name: Set up Python
-      uses: actions/setup-python@v4
-      with:
-        python-version: "3.9"
-
-    - name: Install Python packages
-      run: python -m pip install ruff==0.0.252
-
-    - name: Run ruff
-      run: ruff check .
```

### Comparing `open-dread-rando-2.3.2/.gitignore` & `open-dread-rando-2.4.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -128,8 +128,8 @@
 # Pyre type checker
 .pyre/
 
 # PyCharm
 .idea/
 
 # Project
-open_dread_rando/version.py
+src/open_dread_rando/version.py
```

### Comparing `open-dread-rando-2.3.2/LICENSE` & `open-dread-rando-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/PKG-INFO` & `open-dread-rando-2.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: open-dread-rando
-Version: 2.3.2
+Version: 2.4.0
 Summary: An open source randomizer patcher for Metroid Dread.
-Home-page: https://github.com/randovania/open-dread-rando
-Author: Henrique Gemignani
+Project-URL: Homepage, https://github.com/randovania/open-dread-rando
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `open-dread-rando-2.3.2/README.md` & `open-dread-rando-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/cli.py` & `open-dread-rando-2.4.0/src/open_dread_rando/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,8 +61,8 @@
     start = time.time()
     dread_patcher.patch_extracted(
         args.input_path,
         args.output_path,
         configuration,
     )
     end = time.time()
-    print("Patcher took {:.03f} seconds".format(end - start))
+    print(f"Patcher took {end - start:.03f} seconds")
```

### Comparing `open-dread-rando-2.3.2/open_dread_rando/cosmetic_patches.py` & `open-dread-rando-2.4.0/src/open_dread_rando/cosmetic_patches.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/door_patcher.py` & `open-dread-rando-2.4.0/src/open_dread_rando/door_patcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import copy
 from bisect import insort
+from collections.abc import Sequence
 from enum import Enum
 from pathlib import Path
-from typing import Sequence
 
 from construct import Container, ListContainer
+from mercury_engine_data_structures.formats import Bmscc
 
 from open_dread_rando.constants import ALL_SCENARIOS
 from open_dread_rando.patcher_editor import PatcherEditor
 
-from mercury_engine_data_structures.formats import Bmscc
-
 # copied from existing entity, so we don't have to make a whole shield
 _EXAMPLE_SHIELD = {"scenario": "s010_cave", "layer": "default", "actor": "Door003_missileShield"}
 
 
 class MinimapIconData(Enum):
     """
     Enum representing minimap data. Also contains functions that return mapDoor and mapBlockage Containers.
@@ -68,15 +67,15 @@
         return cont
 
     def create_map_blockage(self, pos: Sequence[float], dir: str) -> Container:
         """Creates a mapBlockage for a shield in a given direction"""
         cont = Container()
         cont["vPos"] = ListContainer([pos[0], pos[1]])
 
-        # get delta, which depends on shield dir. 
+        # get delta, which depends on shield dir.
         # shield L needs no adjustments so delta is zero.
         # shield R needs to be moved oBoxMin[0] + oBoxMax[0] to the right.
         delta = 0 if dir == "L" else -(self.oBox_min[0] + self.oBox_max[0])
 
         cont["oBox"] = Container(
             Min=ListContainer([pos[0] + self.oBox_min[0] + delta, pos[1] + self.oBox_min[1]]),
             Max=ListContainer([pos[0] + self.oBox_max[0] + delta, pos[1] + self.oBox_max[1]]))
@@ -98,22 +97,22 @@
     DOOR_POWER = (["doorpowerpower", "doorpowerclosed", "doorclosedpower"], MinimapIconData.DOOR_POWER)
     DOOR_CHARGE = (["doorchargecharge", "doorchargeclosed", "doorclosedcharge"], MinimapIconData.DOOR_CHARGE)
     DOOR_GRAPPLE = (["doorgrapplegrapple", "doorgrappleclosed", "doorclosedgrapple"], MinimapIconData.DOOR_GRAPPLE)
     DOOR_PRESENCE = (["doorpresencepresence", "doorframepresence", "doorpresenceframe"], MinimapIconData.DOOR_PRESENCE)
     SHIELD_WIDE_BEAM = (["doorwidebeam"], MinimapIconData.SHIELD_WIDE_BEAM)
     SHIELD_PLASMA_BEAM = (["door_shield_plasma"], MinimapIconData.SHIELD_PLASMA_BEAM)
     SHIELD_WAVE_BEAM = (["doorwavebeam"], MinimapIconData.SHIELD_WAVE_BEAM)
-    SHIELD_DIFFUSION_BEAM = (["shield___diffusion"], MinimapIconData.SHIELD_DIFFUSION)
+    SHIELD_DIFFUSION_BEAM = (["shield_diffusion"], MinimapIconData.SHIELD_DIFFUSION)
     SHIELD_MISSILE = (["doorshieldmissile"], MinimapIconData.SHIELD_MISSILE)
     SHIELD_SUPER_MISSILE = (["doorshieldsupermissile"], MinimapIconData.SHIELD_SUPER_MISSILE)
-    SHIELD_ICE_MISSILE = (["shield_icemissile"], MinimapIconData.SHIELD_ICE_MISSILE)
-    SHIELD_STORM_MISSILE = (["shield_storm_mssl"], MinimapIconData.SHIELD_STORM_MISSILE)
-    SHIELD_BOMB = (["shield_bombs_regular__"], MinimapIconData.SHIELD_BOMB)
-    SHIELD_CROSS_BOMB = (["shield_cross_bomb_____"], MinimapIconData.SHIELD_CROSS_BOMB)
-    SHIELD_POWER_BOMB = (["doorshieldpowerbomb___"], MinimapIconData.SHIELD_POWER_BOMB)
+    SHIELD_ICE_MISSILE = (["doorshieldicemissile"], MinimapIconData.SHIELD_ICE_MISSILE)
+    SHIELD_STORM_MISSILE = (["doorshieldstormmissile"], MinimapIconData.SHIELD_STORM_MISSILE)
+    SHIELD_BOMB = (["doorshieldbomb"], MinimapIconData.SHIELD_BOMB)
+    SHIELD_CROSS_BOMB = (["doorshieldcrossbomb"], MinimapIconData.SHIELD_CROSS_BOMB)
+    SHIELD_POWER_BOMB = (["doorshieldpowerbomb"], MinimapIconData.SHIELD_POWER_BOMB)
 
     def __init__(self, actordef: list[str], minimap: MinimapIconData):
         # generate actordefs
         self.actordefs = [f"actors/props/{v}/charclasses/{v}.bmsad" for v in actordef]
         self.minimapData = minimap
 
 
@@ -125,41 +124,41 @@
     door: the door's ActorData
     need_shield: whether the actor needs a shield
     shield: the shield's ActorData
     """
     FRAME = ("frame", ActorData.DOOR_FRAME)
     POWER = ("power_beam", ActorData.DOOR_POWER)
     CHARGE = ("charge_beam", ActorData.DOOR_CHARGE)
-    DIFFUSION = ("diffusion_beam", ActorData.DOOR_POWER, True, ActorData.SHIELD_DIFFUSION_BEAM, True, True, 
+    DIFFUSION = ("diffusion_beam", ActorData.DOOR_POWER, True, ActorData.SHIELD_DIFFUSION_BEAM, True, True,
                  ["actors/props/door_shield_plasma"])
-    WIDE_BEAM = ("wide_beam", ActorData.DOOR_POWER, True, ActorData.SHIELD_WIDE_BEAM, True, True, 
+    WIDE_BEAM = ("wide_beam", ActorData.DOOR_POWER, True, ActorData.SHIELD_WIDE_BEAM, True, True,
                  ["actors/props/doorshieldmissile"])
     PLASMA_BEAM = ("plasma_beam", ActorData.DOOR_POWER, True, ActorData.SHIELD_PLASMA_BEAM)
     WAVE_BEAM = ("wave_beam", ActorData.DOOR_POWER, True, ActorData.SHIELD_WAVE_BEAM)
     MISSILE = ("missile", ActorData.DOOR_POWER, True, ActorData.SHIELD_MISSILE)
     SUPER_MISSILE = ("super_missile", ActorData.DOOR_POWER, True, ActorData.SHIELD_SUPER_MISSILE)
-    SUPER_CHARGE_MISSILE = ("super_charge_missile", ActorData.DOOR_CHARGE, True, 
+    SUPER_CHARGE_MISSILE = ("super_charge_missile", ActorData.DOOR_CHARGE, True,
                             ActorData.SHIELD_SUPER_MISSILE, True, False)
-    ICE_MISSILE = ("ice_missile", ActorData.DOOR_POWER, True, ActorData.SHIELD_ICE_MISSILE, True, True, 
+    ICE_MISSILE = ("ice_missile", ActorData.DOOR_POWER, True, ActorData.SHIELD_ICE_MISSILE, True, True,
                    ["actors/props/doorshieldmissile"])
     STORM_MISSILE = ("storm_missile", ActorData.DOOR_POWER, True, ActorData.SHIELD_STORM_MISSILE, True, True,
                      ["actors/props/doorshieldmissile"])
     BOMB = ("bomb", ActorData.DOOR_POWER, True, ActorData.SHIELD_BOMB, True, True,
-                    ["actors/props/doorshieldmissile", "actors/props/doorshieldsupermissile"])
-    CROSS_BOMB = ("cross_bomb", ActorData.DOOR_POWER, True, ActorData.SHIELD_CROSS_BOMB, True, True, 
+            ["actors/props/doorshieldmissile", "actors/props/doorshieldsupermissile"])
+    CROSS_BOMB = ("cross_bomb", ActorData.DOOR_POWER, True, ActorData.SHIELD_CROSS_BOMB, True, True,
                   ["actors/props/doorshieldmissile"])
     POWER_BOMB = ("power_bomb", ActorData.DOOR_POWER, True, ActorData.SHIELD_POWER_BOMB, True, True,
                   ["actors/props/door_shield_plasma"])
-    GRAPPLE = ("grapple_beam", ActorData.DOOR_GRAPPLE, False, None, True, True, 
+    GRAPPLE = ("grapple_beam", ActorData.DOOR_GRAPPLE, False, None, True, True,
                ["actors/props/door"])
-    PRESENCE = ("phantom_cloak", ActorData.DOOR_PRESENCE, False, None, True, False, 
+    PRESENCE = ("phantom_cloak", ActorData.DOOR_PRESENCE, False, None, True, False,
                 ["actors/props/door"])
 
     def __init__(self, rdv_door_type: str, door_data: ActorData, need_shield: bool = False,
-                 shield_data: ActorData = None, can_be_removed: bool = True, can_be_added: bool = True, 
+                 shield_data: ActorData = None, can_be_removed: bool = True, can_be_added: bool = True,
                  additional_asset_folders: list[str] = None):
         self.type = rdv_door_type
         self.need_shield = need_shield
         self.door = door_data
         self.shield = shield_data
         self.can_be_removed = can_be_removed
         self.can_be_added = can_be_added
@@ -238,16 +237,16 @@
         if len(possible_enum_values) == 1:
             return possible_enum_values[0]
         else:
             raise ValueError(f"Door {door.sName} in scenario {scenario} is not a patchable door!")
 
     def patch_door(self, door_ref: dict, door_type: str):
         """
-        Patches a door given a reference. 
-        
+        Patches a door given a reference.
+
         @param door: A dictionary representing a requested door patch.
         """
 
         scenario = door_ref["scenario"]
         door_actor = self.editor.resolve_actor_reference(door_ref)
 
         # get the type of door we are patching to
@@ -255,16 +254,17 @@
         if door_type.can_be_added is False:
             raise ValueError(f"Door type {door_type} cannot be patched in!")
 
         # get the type of door we are patching
         door_in_scenario_type = self.door_actor_to_type(door_actor, scenario)
         if door_in_scenario_type.can_be_removed is False:
             raise ValueError(
-                f"Base game door {door_in_scenario_type.type} cannot be patched!" + \
-                    f"Requested door: {door_ref['actor']} in {scenario}")
+                f"Base game door {door_in_scenario_type.type} cannot be patched! "
+                f"Requested door: {door_ref['actor']} in {scenario}"
+            )
 
         self.door_to_basic(door_actor, door_in_scenario_type, scenario)
         self.power_to_door_type(door_actor, door_type, scenario)
 
     def door_to_basic(self, door: Container, door_type: DoorType, scenario: str):
         """
         Reverts a door to a basic (power) door based on its door_type
@@ -278,16 +278,16 @@
         # only needs patching if door isn't power
         if door_type.door is not ActorData.DOOR_POWER:
             self.any_door_to_power(door, scenario)
 
     # removes any shields if the door has them
     def remove_shields(self, door: Container, scenario: str):
         """
-        Removes a door's shields. Assumes that the door has shields. 
-        
+        Removes a door's shields. Assumes that the door has shields.
+
         param door: a door actor
         param scenario: the scenario string
         """
         life_comp = door.pComponents.LIFE
         for link_name in ["wpLeftDoorShieldEntity", "wpRightDoorShieldEntity"]:
             link = life_comp[link_name]
             if link == '{EMPTY}':
@@ -312,15 +312,15 @@
         if door_type.need_shield:
             life_comp = door.pComponents["LIFE"]
 
             shield_l = self.create_shield(scenario, door, door_type.shield, "L")
             shield_r = self.create_shield(scenario, door, door_type.shield, "R")
             life_comp["wpLeftDoorShieldEntity"] = self.editor.build_link(shield_l.sName)
             life_comp["wpRightDoorShieldEntity"] = self.editor.build_link(shield_r.sName)
-        
+
         # ensure assets are present
         for folder in door_type.required_asset_folders:
             for asset in self.editor.get_asset_names_in_folder(folder):
                 self.editor.ensure_present_in_scenario(scenario, asset)
 
     def set_door_type(self, door: Container, door_type: DoorType, scenario: str):
         # set actor def to two-sided actordef
@@ -358,22 +358,22 @@
         for scenario in ALL_SCENARIOS:
             bmmap = self.editor.get_scenario_map(scenario)
             bmmap.raw.Root.mapBlockages = Container()
 
     def rename_all_shields(self):
         for scenario in ALL_SCENARIOS:
             brfld = self.editor.get_scenario(scenario)
-            
-            # we have to cache doors that have shields here and rename them outside the loop, 
-            # as otherwise it will rename actors in the actor list and confuse the program. 
+
+            # we have to cache doors that have shields here and rename them outside the loop,
+            # as otherwise it will rename actors in the actor list and confuse the program.
             shielded_doors = []
             for layer_name, actor_name, actor in list(brfld.all_actors()):
 
-                # this is the door added to the Artaria CU. 
-                # For some reason is_door crashes on this so we add a check here. 
+                # this is the door added to the Artaria CU.
+                # For some reason is_door crashes on this so we add a check here.
                 if actor_name == "DreadRando_CUDoor":
                     continue
 
                 if not is_door(actor):
                     continue
 
                 if actor.oActorDefLink[9:] not in ActorData.DOOR_POWER.actordefs:
@@ -391,15 +391,15 @@
             if link == "{EMPTY}":
                 continue
 
             # get shield actor and cache its sName
             shieldActor = self.editor.resolve_actor_reference(self.editor.reference_for_link(link, scenario))
             old_sName = shieldActor.sName
 
-            # skip hdoors (doors where the environment covers one side of the door) 
+            # skip hdoors (doors where the environment covers one side of the door)
             # as they have terrain attached to the ShieldEntity links
             if "db_hdoor" in old_sName:
                 continue
 
             # reclaim old shield id if this is a RandoShield
             self.reclaim_old_shield_id(shieldActor.sName, scenario)
 
@@ -414,30 +414,30 @@
             self.editor.copy_actor_groups(scenario, old_sName, new_id)
             brfld.actors_for_layer('default').pop(old_sName)
 
             # update the minimap entry as well
             mapBlockages = self.editor.get_scenario_map(scenario).raw.Root.mapBlockages
             mapBlockages[new_id] = copy.deepcopy(mapBlockages[old_sName])
 
-            # flip the icon on rightfacing shields in order to optimize the icons file, 
+            # flip the icon on rightfacing shields in order to optimize the icons file,
             # allowing room for new assets in custom_door_types.py
             if link_name.startswith("wpRight"):
                 mapBlockages[new_id]["bFlipX"] = True
             mapBlockages.pop(old_sName)
 
     def get_shield_id(self, scenario: str):
         # since the available shield ids is auto sorted, just pop the first value
         return f"RandoShield_{self.available_shield_ids[scenario].pop(0)}"
 
     def reclaim_old_shield_id(self, sName: str, scenario: str):
         # if it's a RandoShield, reclaim the old id after the underscore
         shieldId = int(sName.split("_")[1]) if "RandoShield" in sName else None
         if shieldId is not None:
             insort(self.available_shield_ids[scenario], shieldId)
-    
+
     def patch_doorpresence_collision(self):
         # extends the door collider in doorpresence actor to 300x300 to maintain the size of normal doors
         # this looks a bit bad, but it'll do until we figure out how to edit navmeshes
         # (or whatever is storing the intended hitboxes for doors)
         doorpresence = self.editor.get_file("actors/props/doorpresence/collisions/doorpresence.bmscd", Bmscc)
         door_collider = doorpresence.raw.layers[0].entries[0]
-        door_collider.data.max = ListContainer([300.0,320.0])
+        door_collider.data.max = ListContainer([300.0, 320.0])
```

### Comparing `open-dread-rando-2.3.2/open_dread_rando/dread_patcher.py` & `open-dread-rando-2.4.0/src/open_dread_rando/dread_patcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import json
 import shutil
 import typing
 from pathlib import Path
 
-
 from construct import ListContainer
 from mercury_engine_data_structures.file_tree_editor import OutputFormat
 
-from open_dread_rando import elevator, lua_util, game_patches
-from open_dread_rando.cosmetic_patches import apply_cosmetic_patches
+from open_dread_rando import elevator, game_patches, lua_util
 from open_dread_rando.constants import FadeTimes
+from open_dread_rando.cosmetic_patches import apply_cosmetic_patches
 from open_dread_rando.custom_door_types import create_all_shield_assets
 from open_dread_rando.door_patcher import DoorPatcher
 from open_dread_rando.environmental_damage import apply_constant_damage
 from open_dread_rando.exefs import include_depackager, patch_exefs
 from open_dread_rando.logger import LOG
 from open_dread_rando.lua_editor import LuaEditor
 from open_dread_rando.missile_color_patcher import generate_missile_colors
@@ -123,17 +122,17 @@
         LOG.debug("Writing pickup %d: %s", i, pickup["resources"][0][0]["item_id"])
         try:
             pickup_object_for(lua_scripts, pickup, i, configuration).patch(editor)
         except NotImplementedError as e:
             LOG.warning(e)
 
 
-def patch_doors(editor: PatcherEditor, doors_config: list[dict]):
+def patch_doors(editor: PatcherEditor, doors_config: list[dict], shield_model_config: dict[str, str]):
     editor.map_icon_editor.add_all_new_door_icons()
-    create_all_shield_assets(editor)
+    create_all_shield_assets(editor, shield_model_config)
 
     door_patcher = DoorPatcher(editor)
     for door in doors_config:
         door_patcher.patch_door(door["actor"], door["door_type"])
 
 
 def patch_spawn_points(editor: PatcherEditor, spawn_config: list[dict]):
@@ -214,15 +213,15 @@
     patch_pickups(editor, lua_scripts, configuration["pickups"], configuration)
 
     # Hints
     if "hints" in configuration:
         patch_hints(editor, configuration["hints"])
 
     # Doors
-    patch_doors(editor, configuration["door_patches"])
+    patch_doors(editor, configuration["door_patches"], configuration["cosmetic_patches"]["shield_versions"])
 
     # custom spawn points
     patch_spawn_points(editor, configuration["new_spawn_points"])
 
     for tile_group in configuration["tile_group_patches"]:
         patch_tilegroup(editor, tile_group)
```

### Comparing `open-dread-rando-2.3.2/open_dread_rando/elevator.py` & `open-dread-rando-2.4.0/src/open_dread_rando/elevator.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/environmental_damage.py` & `open-dread-rando-2.4.0/src/open_dread_rando/environmental_damage.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/environmental_damage_sources.py` & `open-dread-rando-2.4.0/src/open_dread_rando/environmental_damage_sources.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/exefs.py` & `open-dread-rando-2.4.0/src/open_dread_rando/exefs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import shutil
 from pathlib import Path
-from typing import NamedTuple, Tuple
+from typing import NamedTuple
 
 import ips
 import keystone
 
 VERSIONS = {
     "1.0.0": "49161D9CCBC15DF944D0B6278A3C446C006B0BE8",
     "2.1.0": "646761F643AFEBB379EDD5E6A5151AF2CEF93DC1",
@@ -44,15 +44,15 @@
     def _asm(self, version: str) -> bytes:
         return self.asm_template.format_map(self.versions[version].replacements).encode('ascii')
 
     def _data(self, version: str) -> bytes:
         encoding, count = self.assembler.asm(self._asm(version), self.versions[version].offset, True)
         return encoding
 
-    def patch(self, version: str) -> Tuple[int, bytes]:
+    def patch(self, version: str) -> tuple[int, bytes]:
         if version not in self.versions:
             raise RuntimeError(f"Unsupported version: {version}")
         return self.versions[version].offset, self._data(version)
 
 
 def _patch_corpius(patch: ips.Patch, version: str, configuration: dict):
     # patches corpius to not give the phantom cloak, and not to display the
@@ -103,16 +103,16 @@
     offset, data = debug_input.patch(version)
     if offset is not None:
         patch.add_record(offset, data)
 
 def _patch_door_lock_buffer(patch: ips.Patch, version: str):
     """ Update capacities in unknown allocator to avoid doorlock crash
     changes size of buffer inside data field initializer (I think)
-    size of linked-list buffer increased from 500 to 1000. 
-    if 0x33250c in 1.0.0 is crashing, it's likely that this is still too small. 
+    size of linked-list buffer increased from 500 to 1000.
+    if 0x33250c in 1.0.0 is crashing, it's likely that this is still too small.
     original instruction: MOV w2,#0x1f4
     patched instruction: MOV w2,#0x3e8
     """
     buffer_size = {
         "1.0.0": (0x00ae6f70, bytes.fromhex('027D8052')),
         "2.1.0": (0x00ae9d70, bytes.fromhex('027D8052')),
     }
```

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/custom_scenario.lua` & `open-dread-rando-2.4.0/src/open_dread_rando/files/custom_scenario.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/dread_depackager/main.npdm` & `open-dread-rando-2.4.0/src/open_dread_rando/files/dread_depackager/main.npdm`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/dread_depackager/subsdk9` & `open-dread-rando-2.4.0/src/open_dread_rando/files/dread_depackager/subsdk9`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/exefs_patches/debug_input.s` & `open-dread-rando-2.4.0/src/open_dread_rando/files/exefs_patches/debug_input.s`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/levels/s010_cave.lc.lua` & `open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s010_cave.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/levels/s020_magma.lc.lua` & `open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s020_magma.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/levels/s030_baselab.lc.lua` & `open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s030_baselab.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/levels/s040_aqua.lc.lua` & `open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s040_aqua.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/levels/s050_forest.lc.lua` & `open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s050_forest.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/levels/s060_quarantine.lc.lua` & `open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s060_quarantine.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/levels/s070_basesanc.lc.lua` & `open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s070_basesanc.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/levels/s080_shipyard.lc.lua` & `open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s080_shipyard.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/levels/s090_skybase.lc.lua` & `open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s090_skybase.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/lua_libraries/bit.lua` & `open-dread-rando-2.4.0/src/open_dread_rando/files/lua_libraries/bit.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/lua_libraries/data_structures.lua` & `open-dread-rando-2.4.0/src/open_dread_rando/files/lua_libraries/data_structures.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/lua_libraries/death_counter.lua` & `open-dread-rando-2.4.0/src/open_dread_rando/files/lua_libraries/death_counter.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/lua_libraries/guilib.lua` & `open-dread-rando-2.4.0/src/open_dread_rando/files/lua_libraries/guilib.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/lua_libraries/input_handling.lua` & `open-dread-rando-2.4.0/src/open_dread_rando/files/lua_libraries/input_handling.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/lua_libraries/room_names.lua` & `open-dread-rando-2.4.0/src/open_dread_rando/files/lua_libraries/room_names.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/msemenu_mainmenu.lua` & `open-dread-rando-2.4.0/src/open_dread_rando/files/msemenu_mainmenu.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/randomizer_powerup.lua` & `open-dread-rando-2.4.0/src/open_dread_rando/files/randomizer_powerup.lua`

 * *Files 3% similar despite different names*

```diff
@@ -177,20 +177,25 @@
 
     -- Not etank or epart, quit
     if item_id ~= "ITEM_ENERGY_TANKS" and item_id ~= "ITEM_LIFE_SHARDS" then return end
 
     local energy = Init.fEnergyPerTank
 
     if item_id == "ITEM_LIFE_SHARDS" then
+        local shards_amount = RandomizerPowerup.GetItemAmount(item_id)
         if Init.bImmediateEnergyParts then
             energy = Init.fEnergyPerPart
-        elseif (RandomizerPowerup.GetItemAmount(item_id) % 4) ~= 0 then
-            -- only change energy every 4 parts if not immediate!
+        elseif (shards_amount % 4) ~= 0 then
+            -- only change energy every 4 parts if not immediate but change internal amount
+            Game.GetPlayer().LIFE.fLifeShards = shards_amount
             return
         end
+        -- remove all life shards as energy will be increased by following code
+        RandomizerPowerup.SetItemAmount("ITEM_LIFE_SHARDS", 0)
+        Game.GetPlayer().LIFE.fLifeShards = 0
     end
 
     Game.LogWarn(0, "Increasing player energy.")
 
     local new_max = RandomizerPowerup.GetItemAmount("ITEM_MAX_LIFE") + energy
     new_max = math.min(new_max, MAX_ENERGY)
 
@@ -345,14 +350,15 @@
     )
 end
 
 RandomizerEnergyPart = {}
 setmetatable(RandomizerEnergyPart, {__index = RandomizerPowerup})
 function RandomizerEnergyPart.OnPickedUp(actor, progression)
     Game.LogWarn(0, "RandomizerEnergyPart " .. type(progression))
-    progression = progression or {{{ item_id = "ITEM_LIFE_SHARDS", quantity = 1 }}}
-    if Init.bImmediateEnergyParts or not actor then
-        for _, resource in ipairs(progression[1]) do
-            RandomizerPowerup.IncreaseEnergy(resource)
-        end
+    if not Init.bImmediateEnergyParts and actor then
+        name = actor.sName
+        RandomizerPowerup.MarkLocationCollected(string.format("%s_%s", Scenario.CurrentScenarioID, name))
+    else
+        progression = progression or {{{ item_id = "ITEM_LIFE_SHARDS", quantity = 1 }}}
+        RandomizerPowerup.OnPickedUp(actor, progression)
     end
 end
```

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_camo.bsmat` & `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_camo.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_sonr.bsmat` & `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_sonr.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_camo.bcmdl` & `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_camo.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_sonr.bcmdl` & `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_sonr.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/speedboost_mp_opaque_01.bsmat` & `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/speedboost_mp_opaque_01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/itemsphere/models/speed_booster.bcmdl` & `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/itemsphere/models/speed_booster.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphhologram.bsmat` & `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphhologram.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphmaterial.bsmat` & `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphmaterial.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/powerup_morph.bcmdl` & `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/powerup_morph.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_magnet01.bsmat` & `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_magnet01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_white__01.bsmat` & `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_white__01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/powerup_magnet.bcmdl` & `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/powerup_magnet.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mp_fxhologram_0001.bsmat` & `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mp_fxhologram_0001.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/powerup_powerbomb.bcmdl` & `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/powerup_powerbomb.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/powerup_ice__missile_mp_opaque_01.bsmat` & `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/powerup_ice__missile_mp_opaque_01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/powerup_ice__missile.bcmdl` & `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/powerup_ice__missile.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_cangrejo.bsmat` & `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_cangrejo.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/powerup_wavebeam.bcmdl` & `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/powerup_wavebeam.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_at.bctex` & `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_at.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_bc.bctex` & `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_nm.bctex` & `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_nm.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphat.bctex` & `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphat.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphbc.bctex` & `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphbc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphnm.bctex` & `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphnm.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/powerup_spi_magnet_bc.bctex` & `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/powerup_spi_magnet_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/powerup_ice__missile_bc.bctex` & `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/powerup_ice__missile_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/pup_wavebeam_bc.bctex` & `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/pup_wavebeam_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshield_____bomb_bc.bctex` & `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/models/textures/doorshieldbomb_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldcrossbomb_bc.bctex` & `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldpowerbomb_rdv_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldpowerbomb_bc.bctex` & `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldpowerbomb_alt_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/actors/props/shield_storm_mssl/models/textures/shield_storm_mssl_bc.bctex` & `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/models/textures/doorshieldstormmissile_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/romfs/textures/system/minimap/icons/icons.bctex` & `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/system/minimap/icons/icons.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/files/schema.json` & `open-dread-rando-2.4.0/src/open_dread_rando/files/schema.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998412698412699%*

 * *Differences: {"'properties'": "{'cosmetic_patches': {'properties': {'shield_versions': OrderedDict([('type', "*

 * *                 "'object'), ('description', 'Contains a list of all shields and whether they are "*

 * *                 "default or alternate cosmetic'), ('properties', OrderedDict([('ice_missile', "*

 * *                 "OrderedDict([('type', 'string'), ('enum', ['DEFAULT', 'ALTERNATE']), ('default', "*

 * *                 "'DEFAULT')])), ('diffusion_beam', OrderedDict([('type', 'string'), ('enum', "*

 * *                 "[' […]*

```diff
@@ -260,19 +260,74 @@
                                     "type": "string"
                                 }
                             },
                             "type": "object"
                         }
                     },
                     "type": "object"
+                },
+                "shield_versions": {
+                    "description": "Contains a list of all shields and whether they are default or alternate cosmetic",
+                    "properties": {
+                        "bomb": {
+                            "default": "DEFAULT",
+                            "enum": [
+                                "DEFAULT",
+                                "ALTERNATE"
+                            ],
+                            "type": "string"
+                        },
+                        "cross_bomb": {
+                            "default": "DEFAULT",
+                            "enum": [
+                                "DEFAULT",
+                                "ALTERNATE"
+                            ],
+                            "type": "string"
+                        },
+                        "diffusion_beam": {
+                            "default": "DEFAULT",
+                            "enum": [
+                                "DEFAULT",
+                                "ALTERNATE"
+                            ],
+                            "type": "string"
+                        },
+                        "ice_missile": {
+                            "default": "DEFAULT",
+                            "enum": [
+                                "DEFAULT",
+                                "ALTERNATE"
+                            ],
+                            "type": "string"
+                        },
+                        "power_bomb": {
+                            "default": "DEFAULT",
+                            "enum": [
+                                "DEFAULT",
+                                "ALTERNATE"
+                            ],
+                            "type": "string"
+                        },
+                        "storm_missile": {
+                            "default": "DEFAULT",
+                            "enum": [
+                                "DEFAULT",
+                                "ALTERNATE"
+                            ],
+                            "type": "string"
+                        }
+                    },
+                    "type": "object"
                 }
             },
             "required": [
                 "config",
-                "lua"
+                "lua",
+                "shield_versions"
             ],
             "type": "object"
         },
         "debug_export_modified_files": {
             "default": false,
             "description": "Saves all modified files to a _debug sub-directory.",
             "type": "boolean"
```

### Comparing `open-dread-rando-2.3.2/open_dread_rando/game_patches.py` & `open-dread-rando-2.4.0/src/open_dread_rando/game_patches.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/lua_editor.py` & `open-dread-rando-2.4.0/src/open_dread_rando/lua_editor.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/lua_util.py` & `open-dread-rando-2.4.0/src/open_dread_rando/lua_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,20 +29,20 @@
 
     return code
 
 
 def lua_convert(data, wrap_strings: bool = False) -> str:
     if isinstance(data, list):
         return "{\n" + "\n".join(
-            "{},".format(lua_convert(item, wrap_strings))
+            f"{lua_convert(item, wrap_strings)},"
             for item in data
         ) + "\n}"
     if isinstance(data, dict):
         return "{\n" + "\n".join(
-            "{} = {},".format(key, lua_convert(value, wrap_strings))
+            f"{key} = {lua_convert(value, wrap_strings)},"
             for key, value in data.items()
         ) + "\n}"
     if isinstance(data, bool):
         return "true" if data else "false"
     if data is None:
         return "nil"
     if wrap_strings and isinstance(data, str):
```

### Comparing `open-dread-rando-2.3.2/open_dread_rando/map_icons.py` & `open-dread-rando-2.4.0/src/open_dread_rando/map_icons.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from __future__ import annotations
 
 import dataclasses
-from typing import Tuple, Union, TYPE_CHECKING
+from typing import TYPE_CHECKING
 
 from mercury_engine_data_structures.formats import Bmmdef
 
 from open_dread_rando.constants import ALL_SCENARIOS
 from open_dread_rando.text_patches import patch_text
+
 if TYPE_CHECKING:
     from open_dread_rando.patcher_editor import PatcherEditor
 
 
 @dataclasses.dataclass(frozen=True)
 class MapIcon:
     icon_id: str
-    coords: Tuple[int, int]
+    coords: tuple[int, int]
     label: str
     disabled_id: str = 'ItemAdquired'
-    offset: Tuple[int, int] = (0, 0)
+    offset: tuple[int, int] = (0, 0)
     auto_scale: bool = True
     is_global: bool = True
     full_zoom_scale: bool = True
 
     def __post_init__(self):
         object.__setattr__(self, "string_key", f"MAP_ICON_{self.icon_id}")
 
@@ -36,15 +37,15 @@
             self.offset,
             self.auto_scale,
             bIsGlobal=self.is_global,
             bFullZoomScale=self.full_zoom_scale
         )
 
 
-ALL_ICONS: dict[str, Union[MapIcon, str]] = {
+ALL_ICONS: dict[str, MapIcon | str] = {
     "powerup_speedbooster": MapIcon(
         icon_id="ItemSpeedBooster",
         coords=(3, 7),
         label="SPEED BOOSTER"
     ),
     "powerup_widebeam": MapIcon(
         icon_id="ItemWideBeam",
@@ -455,8 +456,8 @@
                 if actor["sIconId"] in blockages_to_fix:
                     actor["bFlipX"] = True
 
     def add_all_new_door_icons(self):
         for icon in ["BlockageIceL", "BlockageIceR", "BlockageDiffusionL", "BlockageDiffusionR",
                      "BlockageStormL", "BlockageStormR", "BlockageBombL", "BlockageBombR",
                      "BlockageCrossBombL", "BlockageCrossBombR", "BlockagePowerBombL", "BlockagePowerBombR"]:
-            self.add_icon(ALL_ICONS[icon])
+            self.add_icon(ALL_ICONS[icon])
```

### Comparing `open-dread-rando-2.3.2/open_dread_rando/missile_color_patcher.py` & `open-dread-rando-2.4.0/src/open_dread_rando/missile_color_patcher.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,57 @@
 import dataclasses
-from copy import deepcopy
 
+from open_dread_rando.material_patcher import MaterialData, create_custom_material
+from open_dread_rando.model_patcher import ModelData, create_custom_model
 from open_dread_rando.patcher_editor import PatcherEditor
 
-from mercury_engine_data_structures.formats.bsmat import Bsmat
 
 # model names for pride missiles
 @dataclasses.dataclass()
 class MissileVariant:
     mat_name: str
+    model_path: str
     shader_path: str
     rgba: tuple[float, float, float, float]
 
     def __init__(self, name: str, color: tuple[float, float, float, float]):
         self.mat_name = f"{name}_mp_fxhologram_01"
+        self.model_path = f"actors/items/item_missiletank/models/{name}.bcmdl"
         self.shader_path = f"actors/items/item_missiletank/models/imats/{self.mat_name}.bsmat"
 
         self.rgba = color
-    
+
 ALL_VARIANTS: dict[str, MissileVariant] = {
-    
+
     "ORANGE": MissileVariant(
-        name="item_missile__OR", 
+        name="item_missile__OR",
         color=[75.0, 10.0, 0.0, 1.0]
     ),
     "YELLOW": MissileVariant(
-        name="item_missile__YL", 
+        name="item_missile__YL",
         color=[30.0, 30.0, 0.0, 1.0]
     ),
     "GREEN": MissileVariant(
-        name="item_missile__GN", 
+        name="item_missile__GN",
         color=[0.0, 30.0, 0.0, 1.0]
     ),
     "BLUE": MissileVariant(
-        name="item_missile__BL", 
+        name="item_missile__BL",
         color=[0.05, 0.5, 75.0, 1.0]
     ),
     "CYAN": MissileVariant(
-        name="item_missile__CY", 
+        name="item_missile__CY",
         color=[0.05, 10.0, 10.0, 1.0]
     ),
     "PURPLE": MissileVariant(
-        name="item_missile__PR", 
+        name="item_missile__PR",
         color=[15.0, 0.5, 70.0, 1.0]
     ),
     "PINK": MissileVariant(
-        name="item_missile__PK", 
+        name="item_missile__PK",
         color=[70.0, 0.5, 7.0, 1.0]
     ),
     "MAGENTA": MissileVariant(
         name="item_missile__MG",
         color=[70.0, 0.5, 70.0, 1.0]
     ),
     "WHITE": MissileVariant(
@@ -63,19 +65,25 @@
     "GRAY": MissileVariant(
         name="item_missile__GY",
         color=[0.2, 0.2, 0.2, 1.0]
     ),
 }
 
 def generate_missile_colors(editor: PatcherEditor):
-    mat = editor.get_file("actors/items/item_missiletank/models/imats/item_missiletank_mp_fxhologram_01.bsmat", Bsmat)
-
     for _, variant in ALL_VARIANTS.items():
-        # copy missile material
-        new_mat = deepcopy(mat)
-        
-        # replace texture name and vTex0EmissiveColor
-        new_mat.raw.name = variant.mat_name
-        tex0_emissive = new_mat.raw.shader_stages[0].uniform_params[5]
-        tex0_emissive.value = variant.rgba
+        mat_dat = MaterialData(
+            base_mat="actors/items/item_missiletank/models/imats/item_missiletank_mp_fxhologram_01.bsmat",
+            new_mat_name=variant.mat_name,
+            new_path=variant.shader_path,
+            uniform_params={
+                "vTex0EmissiveColor": variant.rgba
+            }
+        )
+
+        model_dat = ModelData(
+            base_model="actors/items/item_missiletank/models/item_missiletank.bcmdl",
+            new_path=variant.model_path,
+            materials={"mp_fxhologram_01": variant.shader_path}
+        )
 
-        editor.add_new_asset(variant.shader_path, new_mat, [])
+        create_custom_material(editor, mat_dat)
+        create_custom_model(editor, model_dat)
```

### Comparing `open-dread-rando-2.3.2/open_dread_rando/model_data.py` & `open-dread-rando-2.4.0/src/open_dread_rando/model_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import dataclasses
-from typing import Optional, Tuple
+from typing import Optional
 
 
 @dataclasses.dataclass(frozen=True)
 class Transform:
-    position: Tuple[float, float, float] = (0.0, 0.0, 0.0)
-    angle: Tuple[float, float, float] = (0.0, 0.0, 0.0)
-    scale: Tuple[float, float, float] = (1.0, 1.0, 1.0)
+    position: tuple[float, float, float] = (0.0, 0.0, 0.0)
+    angle: tuple[float, float, float] = (0.0, 0.0, 0.0)
+    scale: tuple[float, float, float] = (1.0, 1.0, 1.0)
 
 
 @dataclasses.dataclass(frozen=True)
 class ModelData:
     bcmdl_path: str
     bmsas: str
     dependencies: tuple[str, ...]
@@ -399,25 +399,25 @@
         bmsas="actors/items/item_missiletank/charclasses/item_missiletank.bmsas",
         dependencies=(
             "actors/items/item_missiletank/models/item_missile__BK.bcmdl",
             "actors/items/item_missiletank/models/imats/item_missiletank_mat01.bsmat",
             "actors/items/item_missiletank/models/imats/item_missile__BK_mp_fxhologram_01.bsmat",
         ),
     ),
-    
+
     "item_missiletank_white": ModelData(
         bcmdl_path="actors/items/item_missiletank/models/item_missile__WH.bcmdl",
         bmsas="actors/items/item_missiletank/charclasses/item_missiletank.bmsas",
         dependencies=(
             "actors/items/item_missiletank/models/item_missile__WH.bcmdl",
             "actors/items/item_missiletank/models/imats/item_missiletank_mat01.bsmat",
             "actors/items/item_missiletank/models/imats/item_missile__WH_mp_fxhologram_01.bsmat",
         ),
     ),
-    
+
     "item_missiletank_gray": ModelData(
         bcmdl_path="actors/items/item_missiletank/models/item_missile__GY.bcmdl",
         bmsas="actors/items/item_missiletank/charclasses/item_missiletank.bmsas",
         dependencies=(
             "actors/items/item_missiletank/models/item_missile__GY.bcmdl",
             "actors/items/item_missiletank/models/imats/item_missiletank_mat01.bsmat",
             "actors/items/item_missiletank/models/imats/item_missile__GY_mp_fxhologram_01.bsmat",
```

### Comparing `open-dread-rando-2.3.2/open_dread_rando/objective.py` & `open-dread-rando-2.4.0/src/open_dread_rando/objective.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/output_config.py` & `open-dread-rando-2.4.0/src/open_dread_rando/output_config.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/patch_util.py` & `open-dread-rando-2.4.0/src/open_dread_rando/patch_util.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/patcher_editor.py` & `open-dread-rando-2.4.0/src/open_dread_rando/patcher_editor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 import copy
 import shutil
 import typing
 from pathlib import Path
 
 from construct import Container
 from mercury_engine_data_structures.file_tree_editor import FileTreeEditor
-from mercury_engine_data_structures.formats import BaseResource, Brfld, Brsa, ALL_FORMATS, Bmmap
+from mercury_engine_data_structures.formats import ALL_FORMATS, BaseResource, Bmmap, Brfld, Brsa
 from mercury_engine_data_structures.game_check import Game
+
 from open_dread_rando.map_icons import MapIconEditor
 
 T = typing.TypeVar("T")
 
 
 def path_for_level(level_name: str) -> str:
     return f"maps/levels/c10_samus/{level_name}/{level_name}"
 
 
-def extension_for_type(type_hint: typing.Type[T]) -> str:
+def extension_for_type(type_hint: type[T]) -> str:
     return next(ext for ext, t in ALL_FORMATS.items() if t == type_hint).lower()
 
 
 class PatcherEditor(FileTreeEditor):
     memory_files: dict[str, BaseResource]
     map_icon_editor: MapIconEditor
 
     def __init__(self, root: Path):
         super().__init__(root, target_game=Game.DREAD)
         self.memory_files = {}
         self.map_icon_editor = MapIconEditor(self)
 
-    def get_file(self, path: str, type_hint: typing.Type[T] = BaseResource) -> T:
+    def get_file(self, path: str, type_hint: type[T] = BaseResource) -> T:
         if path not in self.memory_files:
             self.memory_files[path] = self.get_parsed_asset(path, type_hint=type_hint)
         return self.memory_files[path]
 
-    def get_scenario_file(self, name: str, type_hint: typing.Type[T]) -> T:
+    def get_scenario_file(self, name: str, type_hint: type[T]) -> T:
         path = f"{path_for_level(name)}.{extension_for_type(type_hint)}"
         return self.get_file(path, type_hint)
 
     def get_scenario(self, name: str) -> Brfld:
         return self.get_scenario_file(name, Brfld)
 
     def get_subarea_manager(self, name: str) -> Brsa:
@@ -88,16 +89,16 @@
 
         scenario.actors_for_layer(layer).pop(actor_name)
         if map_category is not None:
             self.get_scenario_map(reference["scenario"]).raw.Root[map_category].pop(actor_name)
 
     def copy_actor_groups(self, scenario_name: str, base_actor_name: str, new_actor_name: str):
         """
-        Copies a base actor's groups to a new actor's groups. Both actors must be in the same scenario. 
-        
+        Copies a base actor's groups to a new actor's groups. Both actors must be in the same scenario.
+
         param baseRef: the actor that you are copying groups from
         param newRef: the actor that will have the same actor groups as baseRef
         """
         scenario = self.get_scenario(scenario_name)
         for group_name in scenario.all_actor_groups():
             if (scenario.is_actor_in_group(group_name, base_actor_name)):
                 scenario.add_actor_to_group(group_name, new_actor_name)
@@ -123,15 +124,15 @@
         newActor.vPos = [float(c) + offset for c, offset in zip(coords, offset)]
 
         return newActor
 
     def find_type_of_actor(self, scenarioStr: str, actordef: str, layer: str = "default"):
         """
         Returns a list of actors with given actordef in the scenario
-        
+
         param scenario: the scenario string
         param layer: an optional layer to filter, standard layer is default
         param actordef: the actor definition (bmsad) to filter for
         returns: a list of all actors that match the criteria
         """
         scenario = self.get_scenario(scenarioStr)
         actors_on_layer = scenario.actors_for_layer(layer)
@@ -141,15 +142,15 @@
             if a.oActorDefLink.split(':')[1] == actordef:
                 filtered.append(actor)
         return filtered
 
     def reference_for_link(self, link: str, scenario: str) -> dict:
         """
         Changes a link string (wp data type) into a reference dict
-        
+
         param link: a reference string consisting of 7 components separated by colons
         param scenario: the scenario this actor is in
         returns: a reference dict
         """
         split_link = link.split(":")
         if len(split_link) != 7:
             raise ValueError(f"Expected 7 components in {link}, got {len(split_link)}")
```

### Comparing `open-dread-rando-2.3.2/open_dread_rando/pickup.py` & `open-dread-rando-2.4.0/src/open_dread_rando/pickup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import copy
 import functools
 import json
 from enum import Enum
 from pathlib import Path
-from typing import Type
 
 from construct import Container
-from mercury_engine_data_structures.formats import Bmsad, Bmmap
+from mercury_engine_data_structures.formats import Bmmap, Bmsad
 
 from open_dread_rando import model_data
 from open_dread_rando.lua_editor import LuaEditor
 from open_dread_rando.patcher_editor import PatcherEditor
 from open_dread_rando.text_patches import patch_text
 
 EXPANSION_ITEM_IDS = {
@@ -305,15 +304,15 @@
             editor,
             self.pickup,
             self.pickup["pickup_lua_callback"],
             'GUI.ShowMessage({}, true, "")'.format(repr(self.pickup["caption"]))
         )
 
 
-_PICKUP_TYPE_TO_CLASS: dict[PickupType, Type[BasePickup]] = {
+_PICKUP_TYPE_TO_CLASS: dict[PickupType, type[BasePickup]] = {
     PickupType.ACTOR: ActorPickup,
     PickupType.EMMI: EmmiPickup,
     PickupType.COREX: CoreXPickup,
     PickupType.CORPIUS: CorpiusPickup,
     PickupType.CUTSCENE: CutscenePickup,
 }
```

### Comparing `open-dread-rando-2.3.2/open_dread_rando/static_fixes.py` & `open-dread-rando-2.4.0/src/open_dread_rando/static_fixes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import copy
 from typing import Optional
 
 import construct
+from mercury_engine_data_structures.formats import Brfld
 from mercury_engine_data_structures.formats.gui_files import Bmscp
 
 from open_dread_rando import door_patcher
 from open_dread_rando.constants import ALL_SCENARIOS
 from open_dread_rando.logger import LOG
 from open_dread_rando.map_icons import MapIconEditor
 from open_dread_rando.patcher_editor import PatcherEditor
@@ -15,69 +16,73 @@
     if icon_id.endswith("R"):
         return icon_id[:-1] + "L"
     elif icon_id.endswith("L"):
         return icon_id[:-1] + "R"
     raise ValueError(f"Unable to flip icon {icon_id}")
 
 
-def apply_one_sided_door_fixes(editor: PatcherEditor):
+def _apply_one_sided_door_fix(scenario: Brfld, map_blockages: construct.Container,
+                              layer_name: str, actor_name: str, actor: construct.Container):
+    # Continue if this isn't a door
+    if not door_patcher.is_door(actor):
+        return
+
+    if actor.oActorDefLink != "actordef:actors/props/doorpowerpower/charclasses/doorpowerpower.bmsad":
+        return
+
+    life_comp = actor.pComponents.LIFE
+    left = scenario.follow_link(life_comp.wpLeftDoorShieldEntity)
+    right = scenario.follow_link(life_comp.wpRightDoorShieldEntity)
+
+    if left is None and right is None:
+        return
+
+    elif left is None:
+        other = right
+        direction = "wpLeftDoorShieldEntity"
+
+    elif right is None:
+        other = left
+        direction = "wpRightDoorShieldEntity"
+    else:
+        return
+
+    if "db_hdoor" in other.oActorDefLink:
+        return
+
+    LOG.debug("%s/%s: copy %s into %s", layer_name, actor_name, other.sName, direction)
+    mirrored = copy.deepcopy(other)
+    mirrored.sName += "_mirrored"
+    mirrored.vAng = [other.vAng[0], -other.vAng[1], other.vAng[2]]
+    scenario.actors_for_layer(layer_name)[mirrored.sName] = mirrored
+
+    mirrored_map = copy.deepcopy(map_blockages[other.sName])
+    mirrored_map["sIconId"] = flip_icon_id(mirrored_map["sIconId"])
+    delta = 450 if mirrored_map["sIconId"].endswith("R") else -450
+    mirrored_map["oBox"]["Min"][0] += delta
+    mirrored_map["oBox"]["Max"][0] += delta
+    map_blockages[mirrored.sName] = mirrored_map
+
+    # Add a reference to the other shield to the main actor
+    life_comp[direction] = f"Root:pScenario:rEntitiesLayer:dctSublayers:{layer_name}:dctActors:{mirrored.sName}"
+
+    for group_name in scenario.all_actor_groups():
+        if any(scenario.is_actor_in_group(group_name, x, layer_name) for x in [actor_name, other.sName]):
+            for name in [actor_name, mirrored.sName, other.sName]:
+                scenario.add_actor_to_group(group_name, name, layer_name)
+
 
+def apply_one_sided_door_fixes(editor: PatcherEditor):
     for scenario_name in ALL_SCENARIOS:
         scenario = editor.get_scenario(scenario_name)
         bmmap = editor.get_scenario_map(scenario_name)
         map_blockages = bmmap.raw.Root.mapBlockages
 
         for layer_name, actor_name, actor in list(scenario.all_actors()):
-            # Continue if this isn't a door
-            if not door_patcher.is_door(actor):
-                continue
-
-            if actor.oActorDefLink != "actordef:actors/props/doorpowerpower/charclasses/doorpowerpower.bmsad":
-                continue
-
-            life_comp = actor.pComponents.LIFE
-            left = scenario.follow_link(life_comp.wpLeftDoorShieldEntity)
-            right = scenario.follow_link(life_comp.wpRightDoorShieldEntity)
-
-            if left is None and right is None:
-                continue
-
-            elif left is None:
-                other = right
-                direction = "wpLeftDoorShieldEntity"
-
-            elif right is None:
-                other = left
-                direction = "wpRightDoorShieldEntity"
-            else:
-                continue
-
-            if "db_hdoor" in other.oActorDefLink:
-                continue
-
-            LOG.debug("%s/%s/%s: copy %s into %s", scenario_name, layer_name, actor_name, other.sName, direction)
-            mirrored = copy.deepcopy(other)
-            mirrored.sName += "_mirrored"
-            mirrored.vAng = [other.vAng[0], -other.vAng[1], other.vAng[2]]
-            scenario.actors_for_layer(layer_name)[mirrored.sName] = mirrored
-
-            mirrored_map = copy.deepcopy(map_blockages[other.sName])
-            mirrored_map["sIconId"] = flip_icon_id(mirrored_map["sIconId"])
-            delta = 450 if mirrored_map["sIconId"].endswith("R") else -450
-            mirrored_map["oBox"]["Min"][0] += delta
-            mirrored_map["oBox"]["Max"][0] += delta
-            map_blockages[mirrored.sName] = mirrored_map
-
-            # Add a reference to the other shield to the main actor
-            life_comp[direction] = f"Root:pScenario:rEntitiesLayer:dctSublayers:{layer_name}:dctActors:{mirrored.sName}"
-
-            for group_name in scenario.all_actor_groups():
-                if any(scenario.is_actor_in_group(group_name, x, layer_name) for x in [actor_name, other.sName]):
-                    for name in [actor_name, mirrored.sName, other.sName]:
-                        scenario.add_actor_to_group(group_name, name, layer_name)
+            _apply_one_sided_door_fix(scenario, map_blockages, layer_name, actor_name, actor)
 
 
 PROBLEM_LAYERS = {
     "PostXRelease": {
         "s010_cave": [
             "collision_camera_026",  # Chain reaction
             "collision_camera_020",  # Corpius arena
@@ -144,14 +149,15 @@
 def apply_corpius_fixes(editor: PatcherEditor):
     _apply_boss_cutscene_fixes(editor, {
         "scenario": "s010_cave",
         "layer": "Cutscenes",
         "actor": "cutsceneplayer_57"
     }, "CurrentScenario.OnCorpiusDeath_CUSTOM", 0)
 
+
 def apply_kraid_fixes(editor: PatcherEditor):
     _apply_boss_cutscene_fixes(editor, {
         "scenario": "s020_magma",
         "layer": "cutscenes",
         "actor": "cutsceneplayer_61"
     }, "CurrentScenario.OnKraidDeath_CUSTOM", -1)
 
@@ -348,18 +354,20 @@
     cutscene_player = editor.resolve_actor_reference({
         "scenario": "s080_shipyard",
         "layer": "cutscenes",
         "actor": "cutsceneplayer_12",
     })
     cutscene_player.bEnabled = False
 
+
 def fix_map_icons(map_editor: MapIconEditor):
     map_editor.mirror_bmmdef_icons()
     map_editor.mirror_bmmap_icons()
 
+
 def apply_static_fixes(editor: PatcherEditor):
     remove_problematic_x_layers(editor)
     activate_emmi_zones(editor)
     apply_one_sided_door_fixes(editor)
     apply_kraid_fixes(editor)
     apply_corpius_fixes(editor)
     fix_backdoor_white_cu(editor)
```

### Comparing `open-dread-rando-2.3.2/open_dread_rando/templates/custom_core_x.lua` & `open-dread-rando-2.4.0/src/open_dread_rando/templates/custom_core_x.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/templates/custom_core_x_superquetzoa.lua` & `open-dread-rando-2.4.0/src/open_dread_rando/templates/custom_core_x_superquetzoa.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/templates/custom_init.lua` & `open-dread-rando-2.4.0/src/open_dread_rando/templates/custom_init.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/templates/template_doorshield_energy_bmsad.json` & `open-dread-rando-2.4.0/src/open_dread_rando/templates/template_doorshield_energy_bmsad.json`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/templates/template_doorshield_hexs_bmsad.json` & `open-dread-rando-2.4.0/src/open_dread_rando/templates/template_doorshield_hexs_bmsad.json`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/templates/template_doorshield_tris_bmsad.json` & `open-dread-rando-2.4.0/src/open_dread_rando/templates/template_doorshield_tris_bmsad.json`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/templates/template_powerup_bmsad.json` & `open-dread-rando-2.4.0/src/open_dread_rando/templates/template_powerup_bmsad.json`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/text_patches.py` & `open-dread-rando-2.4.0/src/open_dread_rando/text_patches.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.3.2/open_dread_rando/tilegroup_patcher.py` & `open-dread-rando-2.4.0/src/open_dread_rando/tilegroup_patcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def is_tilegroup(actor):
     return "TILEGROUP" in actor.pComponents and actor.pComponents.TILEGROUP["@type"] == "CBreakableTileGroupComponent"
 
 
 def patch_tilegroup(editor: PatcherEditor, group: dict):
     """
     Patches a tilegroup from its original tile type into a new tile type
-    
+
     :param editor: the PatcherEditor
     :param group: a dictionary containing the actor reference stored in 'actor' key and a tile type
     stored in 'tiletype' key
     """
     actor = editor.resolve_actor_reference(group["actor"])
 
     if not is_tilegroup(actor):
```

### Comparing `open-dread-rando-2.3.2/open_dread_rando/validator_with_default.py` & `open-dread-rando-2.4.0/src/open_dread_rando/validator_with_default.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,18 +5,17 @@
     validate_properties = validator_class.VALIDATORS["properties"]
 
     def set_defaults(validator, properties, instance, schema):
         for property, subschema in properties.items():
             if "default" in subschema:
                 instance.setdefault(property, subschema["default"])
 
-        for error in validate_properties(
+        yield from validate_properties(
                 validator, properties, instance, schema,
-        ):
-            yield error
+        )
 
     return validators.extend(
         validator_class, {"properties": set_defaults},
     )
 
 
 DefaultValidatingDraft7Validator = extend_with_default(Draft7Validator)
```

### Comparing `open-dread-rando-2.3.2/open_dread_rando.egg-info/PKG-INFO` & `open-dread-rando-2.4.0/src/open_dread_rando.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: open-dread-rando
-Version: 2.3.2
+Version: 2.4.0
 Summary: An open source randomizer patcher for Metroid Dread.
-Home-page: https://github.com/randovania/open-dread-rando
-Author: Henrique Gemignani
+Project-URL: Homepage, https://github.com/randovania/open-dread-rando
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `open-dread-rando-2.3.2/tests/test_dread_patcher.py` & `open-dread-rando-2.4.0/tests/test_dread_patcher.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,14 +22,22 @@
             "lua": {
                 "custom_init": {
                     "enable_death_counter": False,
                     "enable_room_name_display": "NEVER"
                 },
                 "camera_names_dict": {
                 }
+            },
+            "shield_versions": {
+                "ice_missile": "ALTERNATE",
+                "diffusion_beam": "ALTERNATE",
+                "storm_missile": "ALTERNATE",
+                "bomb": "ALTERNATE",
+                "cross_bomb": "ALTERNATE",
+                "power_bomb": "DEFAULT"
             }
         },
         "energy_per_tank": 75,
         "immediate_energy_parts": True,
         "constant_environment_damage": {
             "heat": 20,
             "cold": 20,
@@ -53,8 +61,8 @@
     result = dread_patcher.create_custom_init(editor, configuration)
 
     # Assert
     lua_runtime.execute("Init = {}")
     lua_runtime.execute(result)
 
     assert lua_runtime.eval("Init.fEnergyPerTank") == 75
-    assert lua_runtime.eval("Init.sLayoutUUID") == layoutUUID
+    assert lua_runtime.eval("Init.sLayoutUUID") == layoutUUID
```

### Comparing `open-dread-rando-2.3.2/tests/test_files/starter_preset_patcher.json` & `open-dread-rando-2.4.0/tests/test_files/starter_preset_patcher.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9916666666666668%*

 * *Differences: {"'cosmetic_patches'": "{'shield_versions': OrderedDict([('ice_missile', 'ALTERNATE'), "*

 * *                       "('diffusion_beam', 'ALTERNATE'), ('storm_missile', 'ALTERNATE'), ('bomb', "*

 * *                       "'ALTERNATE'), ('cross_bomb', 'ALTERNATE'), ('power_bomb', 'DEFAULT')])}"}*

```diff
@@ -365,14 +365,22 @@
                     "collision_camera_004": "Raven Beak Arena"
                 }
             },
             "custom_init": {
                 "enable_death_counter": true,
                 "enable_room_name_display": "NEVER"
             }
+        },
+        "shield_versions": {
+            "bomb": "ALTERNATE",
+            "cross_bomb": "ALTERNATE",
+            "diffusion_beam": "ALTERNATE",
+            "ice_missile": "ALTERNATE",
+            "power_bomb": "DEFAULT",
+            "storm_missile": "ALTERNATE"
         }
     },
     "door_patches": [
         {
             "actor": {
                 "actor": "doorpowerpower_005",
                 "layer": "default",
```

### Comparing `open-dread-rando-2.3.2/tests/test_lua_util.py` & `open-dread-rando-2.4.0/tests/test_lua_util.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -26,8 +26,8 @@
     })
 
     test_files: Path = Path(__file__).parent.joinpath("test_files")
 
     with test_files.joinpath("randomizer_progressive_expected.lua").open() as f:
         expected_code = f.read()
 
-        assert generated_code == expected_code
+        assert generated_code == expected_code
```

