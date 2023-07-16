# Comparing `tmp/crankshaft-0.7.2.tar.gz` & `tmp/crankshaft-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crankshaft-0.7.2.tar", max compression
+gzip compressed data, was "crankshaft-0.8.0.tar", max compression
```

## Comparing `crankshaft-0.7.2.tar` & `crankshaft-0.8.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1067 2023-07-10 19:29:07.007621 crankshaft-0.7.2/LICENSE
--rw-r--r--   0        0        0     1564 2023-07-10 19:29:07.007621 crankshaft-0.7.2/README.md
--rw-r--r--   0        0        0      326 2023-07-10 19:29:52.040194 crankshaft-0.7.2/crankshaft/__init__.py
--rw-r--r--   0        0        0      132 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/api.bolt
--rw-r--r--   0        0        0      216 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/config.bolt
--rw-r--r--   0        0        0      513 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/defer.bolt
--rw-r--r--   0        0        0     3872 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/event_handler.bolt
--rw-r--r--   0        0        0     1605 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_entity_attack_player.bolt
--rw-r--r--   0        0        0      207 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_load.bolt
--rw-r--r--   0        0        0      344 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_player_airborne.bolt
--rw-r--r--   0        0        0      644 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_player_airborne_end.bolt
--rw-r--r--   0        0        0      646 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_player_airborne_start.bolt
--rw-r--r--   0        0        0     1605 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_player_attack_entity.bolt
--rw-r--r--   0        0        0      328 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_player_burn.bolt
--rw-r--r--   0        0        0      629 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_player_burn_end.bolt
--rw-r--r--   0        0        0      632 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_player_burn_start.bolt
--rw-r--r--   0        0        0      589 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_player_charge_bow.bolt
--rw-r--r--   0        0        0      975 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_player_charge_bow_end.bolt
--rw-r--r--   0        0        0      665 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_player_charge_bow_start.bolt
--rw-r--r--   0        0        0      332 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_player_glide.bolt
--rw-r--r--   0        0        0      632 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_player_glide_end.bolt
--rw-r--r--   0        0        0      636 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_player_glide_start.bolt
--rw-r--r--   0        0        0      677 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_player_inventory_change.bolt
--rw-r--r--   0        0        0      501 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_player_join.bolt
--rw-r--r--   0        0        0      495 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_player_jump.bolt
--rw-r--r--   0        0        0      608 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_player_land.bolt
--rw-r--r--   0        0        0      471 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_player_load.bolt
--rw-r--r--   0        0        0      748 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_player_shoot_bow.bolt
--rw-r--r--   0        0        0      335 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_player_sneak.bolt
--rw-r--r--   0        0        0      635 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_player_sneak_end.bolt
--rw-r--r--   0        0        0      638 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_player_sneak_start.bolt
--rw-r--r--   0        0        0      341 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_player_sprint.bolt
--rw-r--r--   0        0        0      642 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_player_sprint_end.bolt
--rw-r--r--   0        0        0      644 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_player_sprint_start.bolt
--rw-r--r--   0        0        0      332 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_player_swim.bolt
--rw-r--r--   0        0        0      632 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_player_swim_end.bolt
--rw-r--r--   0        0        0      635 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_player_swim_start.bolt
--rw-r--r--   0        0        0      263 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_player_tick.bolt
--rw-r--r--   0        0        0      558 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_player_use_coas.bolt
--rw-r--r--   0        0        0      573 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_player_use_wfoas.bolt
--rw-r--r--   0        0        0      207 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events/on_tick.bolt
--rw-r--r--   0        0        0     2118 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/events.bolt
--rw-r--r--   0        0        0     3398 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/flag.bolt
--rw-r--r--   0        0        0      377 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/flags/is_airborne.bolt
--rw-r--r--   0        0        0      402 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/flags/is_baby.bolt
--rw-r--r--   0        0        0      411 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/flags/is_burning.bolt
--rw-r--r--   0        0        0     1258 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/flags/is_charging_bow.bolt
--rw-r--r--   0        0        0      377 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/flags/is_gliding.bolt
--rw-r--r--   0        0        0      379 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/flags/is_in_ground.bolt
--rw-r--r--   0        0        0      379 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/flags/is_on_ground.bolt
--rw-r--r--   0        0        0      158 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/flags/is_player.bolt
--rw-r--r--   0        0        0      414 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/flags/is_sneaking.bolt
--rw-r--r--   0        0        0      417 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/flags/is_sprinting.bolt
--rw-r--r--   0        0        0      414 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/flags/is_swimming.bolt
--rw-r--r--   0        0        0      535 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/flags.bolt
--rw-r--r--   0        0        0      443 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/lib/entity_hit_matching/api.bolt
--rw-r--r--   0        0        0      124 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/lib/entity_hit_matching/credits.txt
--rw-r--r--   0        0        0    58171 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/lib/entity_hit_matching/main.bolt
--rw-r--r--   0        0        0      207 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/modules/utils.bolt
--rw-r--r--   0        0        0        0 2023-07-10 19:29:07.007621 crankshaft-0.7.2/crankshaft/py.typed
--rw-r--r--   0        0        0     1329 2023-07-10 19:29:52.064194 crankshaft-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     2373 1970-01-01 00:00:00.000000 crankshaft-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-16 23:42:31.027788 crankshaft-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1564 2023-07-16 23:42:31.027788 crankshaft-0.8.0/README.md
+-rw-r--r--   0        0        0      326 2023-07-16 23:43:31.042436 crankshaft-0.8.0/crankshaft/__init__.py
+-rw-r--r--   0        0        0      132 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/api.bolt
+-rw-r--r--   0        0        0      216 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/config.bolt
+-rw-r--r--   0        0        0      513 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/defer.bolt
+-rw-r--r--   0        0        0     3872 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/event_handler.bolt
+-rw-r--r--   0        0        0     1605 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_entity_attack_player.bolt
+-rw-r--r--   0        0        0      207 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_load.bolt
+-rw-r--r--   0        0        0      566 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_airborne.bolt
+-rw-r--r--   0        0        0      831 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_airborne_end.bolt
+-rw-r--r--   0        0        0      646 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_airborne_start.bolt
+-rw-r--r--   0        0        0     1605 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_attack_entity.bolt
+-rw-r--r--   0        0        0      328 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_burn.bolt
+-rw-r--r--   0        0        0      629 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_burn_end.bolt
+-rw-r--r--   0        0        0      632 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_burn_start.bolt
+-rw-r--r--   0        0        0      589 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_charge_bow.bolt
+-rw-r--r--   0        0        0      975 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_charge_bow_end.bolt
+-rw-r--r--   0        0        0      665 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_charge_bow_start.bolt
+-rw-r--r--   0        0        0      332 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_glide.bolt
+-rw-r--r--   0        0        0      632 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_glide_end.bolt
+-rw-r--r--   0        0        0      636 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_glide_start.bolt
+-rw-r--r--   0        0        0      677 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_inventory_change.bolt
+-rw-r--r--   0        0        0      501 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_join.bolt
+-rw-r--r--   0        0        0      495 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_jump.bolt
+-rw-r--r--   0        0        0      608 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_land.bolt
+-rw-r--r--   0        0        0      471 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_load.bolt
+-rw-r--r--   0        0        0      748 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_shoot_bow.bolt
+-rw-r--r--   0        0        0      335 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_sneak.bolt
+-rw-r--r--   0        0        0      635 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_sneak_end.bolt
+-rw-r--r--   0        0        0      638 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_sneak_start.bolt
+-rw-r--r--   0        0        0      341 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_sprint.bolt
+-rw-r--r--   0        0        0      642 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_sprint_end.bolt
+-rw-r--r--   0        0        0      644 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_sprint_start.bolt
+-rw-r--r--   0        0        0      332 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_swim.bolt
+-rw-r--r--   0        0        0      632 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_swim_end.bolt
+-rw-r--r--   0        0        0      635 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_swim_start.bolt
+-rw-r--r--   0        0        0      263 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_tick.bolt
+-rw-r--r--   0        0        0      558 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_use_coas.bolt
+-rw-r--r--   0        0        0      573 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_use_wfoas.bolt
+-rw-r--r--   0        0        0      207 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_tick.bolt
+-rw-r--r--   0        0        0     2118 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events.bolt
+-rw-r--r--   0        0        0     3398 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/flag.bolt
+-rw-r--r--   0        0        0      377 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/flags/is_airborne.bolt
+-rw-r--r--   0        0        0      402 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/flags/is_baby.bolt
+-rw-r--r--   0        0        0      411 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/flags/is_burning.bolt
+-rw-r--r--   0        0        0     1258 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/flags/is_charging_bow.bolt
+-rw-r--r--   0        0        0      377 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/flags/is_gliding.bolt
+-rw-r--r--   0        0        0      379 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/flags/is_in_ground.bolt
+-rw-r--r--   0        0        0      379 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/flags/is_on_ground.bolt
+-rw-r--r--   0        0        0      158 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/flags/is_player.bolt
+-rw-r--r--   0        0        0      414 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/flags/is_sneaking.bolt
+-rw-r--r--   0        0        0      417 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/flags/is_sprinting.bolt
+-rw-r--r--   0        0        0      414 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/flags/is_swimming.bolt
+-rw-r--r--   0        0        0      535 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/flags.bolt
+-rw-r--r--   0        0        0      443 2023-07-16 23:42:31.031788 crankshaft-0.8.0/crankshaft/modules/lib/entity_hit_matching/api.bolt
+-rw-r--r--   0        0        0      124 2023-07-16 23:42:31.031788 crankshaft-0.8.0/crankshaft/modules/lib/entity_hit_matching/credits.txt
+-rw-r--r--   0        0        0    58171 2023-07-16 23:42:31.031788 crankshaft-0.8.0/crankshaft/modules/lib/entity_hit_matching/main.bolt
+-rw-r--r--   0        0        0      207 2023-07-16 23:42:31.031788 crankshaft-0.8.0/crankshaft/modules/utils.bolt
+-rw-r--r--   0        0        0        0 2023-07-16 23:42:31.031788 crankshaft-0.8.0/crankshaft/py.typed
+-rw-r--r--   0        0        0     1329 2023-07-16 23:43:31.066437 crankshaft-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2373 1970-01-01 00:00:00.000000 crankshaft-0.8.0/PKG-INFO
```

### Comparing `crankshaft-0.7.2/LICENSE` & `crankshaft-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.2/README.md` & `crankshaft-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.2/crankshaft/modules/defer.bolt` & `crankshaft-0.8.0/crankshaft/modules/defer.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.2/crankshaft/modules/event_handler.bolt` & `crankshaft-0.8.0/crankshaft/modules/event_handler.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.2/crankshaft/modules/events/on_entity_attack_player.bolt` & `crankshaft-0.8.0/crankshaft/modules/events/on_entity_attack_player.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.2/crankshaft/modules/events/on_player_airborne_end.bolt` & `crankshaft-0.8.0/crankshaft/modules/events/on_player_burn_end.bolt`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from lightning_rod:api import tag, untag
 from ../event_handler import BuiltinEvent, Entrypoint
 from ./on_player_tick import on_player_tick
 from ../config import Config
-from ../flags/is_airborne import is_airborne
+from ../flags/is_burning import is_burning
 
 
 def handler(event):
     event_fired_tag = f"{Config.TAG_ROOT}.event.{event.id}"
 
-    if not is_airborne:
+    if not is_burning:
         if entity @s[tag=event_fired_tag] function event.path('nested_0'):
             untag(event_fired_tag)
             event.trigger()
     else:
         tag(event_fired_tag)
 
 
-on_player_airborne_end = BuiltinEvent('on_player_airborne_end')
-on_player_airborne_end.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
+on_player_burn_end = BuiltinEvent('on_player_burn_end')
+on_player_burn_end.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.7.2/crankshaft/modules/events/on_player_airborne_start.bolt` & `crankshaft-0.8.0/crankshaft/modules/events/on_player_airborne_start.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.2/crankshaft/modules/events/on_player_attack_entity.bolt` & `crankshaft-0.8.0/crankshaft/modules/events/on_player_attack_entity.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.2/crankshaft/modules/events/on_player_burn_end.bolt` & `crankshaft-0.8.0/crankshaft/modules/events/on_player_sprint_end.bolt`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from lightning_rod:api import tag, untag
 from ../event_handler import BuiltinEvent, Entrypoint
 from ./on_player_tick import on_player_tick
 from ../config import Config
-from ../flags/is_burning import is_burning
+from ../flags/is_sprinting import is_sprinting 
 
 
 def handler(event):
     event_fired_tag = f"{Config.TAG_ROOT}.event.{event.id}"
 
-    if not is_burning:
+    if not is_sprinting:
         if entity @s[tag=event_fired_tag] function event.path('nested_0'):
             untag(event_fired_tag)
             event.trigger()
     else:
         tag(event_fired_tag)
 
 
-on_player_burn_end = BuiltinEvent('on_player_burn_end')
-on_player_burn_end.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
+on_player_sprint_end = BuiltinEvent('on_player_sprint_end')
+on_player_sprint_end.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.7.2/crankshaft/modules/events/on_player_burn_start.bolt` & `crankshaft-0.8.0/crankshaft/modules/events/on_player_burn_start.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.2/crankshaft/modules/events/on_player_charge_bow.bolt` & `crankshaft-0.8.0/crankshaft/modules/events/on_player_charge_bow.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.2/crankshaft/modules/events/on_player_charge_bow_end.bolt` & `crankshaft-0.8.0/crankshaft/modules/events/on_player_charge_bow_end.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.2/crankshaft/modules/events/on_player_charge_bow_start.bolt` & `crankshaft-0.8.0/crankshaft/modules/events/on_player_charge_bow_start.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.2/crankshaft/modules/events/on_player_glide_end.bolt` & `crankshaft-0.8.0/crankshaft/modules/events/on_player_glide_end.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.2/crankshaft/modules/events/on_player_glide_start.bolt` & `crankshaft-0.8.0/crankshaft/modules/events/on_player_glide_start.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.2/crankshaft/modules/events/on_player_inventory_change.bolt` & `crankshaft-0.8.0/crankshaft/modules/events/on_player_inventory_change.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.2/crankshaft/modules/events/on_player_land.bolt` & `crankshaft-0.8.0/crankshaft/modules/events/on_player_land.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.2/crankshaft/modules/events/on_player_shoot_bow.bolt` & `crankshaft-0.8.0/crankshaft/modules/events/on_player_shoot_bow.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.2/crankshaft/modules/events/on_player_sneak_end.bolt` & `crankshaft-0.8.0/crankshaft/modules/events/on_player_sneak_end.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.2/crankshaft/modules/events/on_player_sneak_start.bolt` & `crankshaft-0.8.0/crankshaft/modules/events/on_player_sneak_start.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.2/crankshaft/modules/events/on_player_sprint_end.bolt` & `crankshaft-0.8.0/crankshaft/modules/events/on_player_swim_start.bolt`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from lightning_rod:api import tag, untag
 from ../event_handler import BuiltinEvent, Entrypoint
 from ./on_player_tick import on_player_tick
 from ../config import Config
-from ../flags/is_sprinting import is_sprinting 
+from ../flags/is_swimming import is_swimming 
 
 
 def handler(event):
     event_fired_tag = f"{Config.TAG_ROOT}.event.{event.id}"
 
-    if not is_sprinting:
-        if entity @s[tag=event_fired_tag] function event.path('nested_0'):
-            untag(event_fired_tag)
+    if is_swimming:
+        if entity @s[tag=!event_fired_tag] function event.path('nested_0'):
+            tag(event_fired_tag)
             event.trigger()
     else:
-        tag(event_fired_tag)
+        untag(event_fired_tag)
 
-
-on_player_sprint_end = BuiltinEvent('on_player_sprint_end')
-on_player_sprint_end.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
+on_player_swim_start = BuiltinEvent('on_player_swim_start')
+on_player_swim_start.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.7.2/crankshaft/modules/events/on_player_sprint_start.bolt` & `crankshaft-0.8.0/crankshaft/modules/events/on_player_sprint_start.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.2/crankshaft/modules/events/on_player_swim_end.bolt` & `crankshaft-0.8.0/crankshaft/modules/events/on_player_swim_end.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.2/crankshaft/modules/events/on_player_use_coas.bolt` & `crankshaft-0.8.0/crankshaft/modules/events/on_player_use_coas.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.2/crankshaft/modules/events/on_player_use_wfoas.bolt` & `crankshaft-0.8.0/crankshaft/modules/events/on_player_use_wfoas.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.2/crankshaft/modules/events.bolt` & `crankshaft-0.8.0/crankshaft/modules/events.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.2/crankshaft/modules/flag.bolt` & `crankshaft-0.8.0/crankshaft/modules/flag.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.2/crankshaft/modules/flags/is_charging_bow.bolt` & `crankshaft-0.8.0/crankshaft/modules/flags/is_charging_bow.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.2/crankshaft/modules/flags.bolt` & `crankshaft-0.8.0/crankshaft/modules/flags.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.2/crankshaft/modules/lib/entity_hit_matching/main.bolt` & `crankshaft-0.8.0/crankshaft/modules/lib/entity_hit_matching/main.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.7.2/pyproject.toml` & `crankshaft-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crankshaft"
-version = "0.7.2"
+version = "0.8.0"
 description = "Bolt datapack flow control library."
 authors = ["ArcticYeti <arcticyeti1@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/reapermc/crankshaft"
 readme = "README.md"
```

### Comparing `crankshaft-0.7.2/PKG-INFO` & `crankshaft-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crankshaft
-Version: 0.7.2
+Version: 0.8.0
 Summary: Bolt datapack flow control library.
 Home-page: https://github.com/reapermc/crankshaft
 License: MIT
 Keywords: beet,mecha,bolt,python,minecraft,datapack,minecraft-commands,mcfunction,crankshaft,library,reapermc,flow-control,event,event-handler
 Author: ArcticYeti
 Author-email: arcticyeti1@gmail.com
 Requires-Python: >=3.10,<4.0
```

