# Comparing `tmp/pythonmc-1.0.4.tar.gz` & `tmp/pythonmc-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonmc-1.0.4.tar", last modified: Fri Jun 23 19:04:45 2023, max compression
+gzip compressed data, was "pythonmc-1.0.5.tar", last modified: Sun Jun 25 17:44:49 2023, max compression
```

## Comparing `pythonmc-1.0.4.tar` & `pythonmc-1.0.5.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.561409 pythonmc-1.0.4/
--rw-rw-rw-   0        0        0     5394 2023-06-23 19:04:45.560395 pythonmc-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4877 2023-06-23 17:56:35.000000 pythonmc-1.0.4/README.md
--rw-rw-rw-   0        0        0      108 2023-06-20 00:42:26.000000 pythonmc-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-23 19:04:45.561409 pythonmc-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      823 2023-06-23 19:04:36.000000 pythonmc-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.493425 pythonmc-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.501926 pythonmc-1.0.4/src/pythonmc/
--rw-rw-rw-   0        0        0     2857 2023-06-23 19:01:34.000000 pythonmc-1.0.4/src/pythonmc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.510245 pythonmc-1.0.4/src/pythonmc/block/
--rw-rw-rw-   0        0        0      120 2023-06-23 19:00:22.000000 pythonmc-1.0.4/src/pythonmc/block/__init__.py
--rw-rw-rw-   0        0        0      187 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/block/block.py
--rw-rw-rw-   0        0        0       90 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/block/block_pos.py
--rw-rw-rw-   0        0        0      110 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/block/block_state.py
--rw-rw-rw-   0        0        0    25267 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/block/blocks.py
-drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.516799 pythonmc-1.0.4/src/pythonmc/entity/
--rw-rw-rw-   0        0        0      251 2023-06-23 19:00:22.000000 pythonmc-1.0.4/src/pythonmc/entity/__init__.py
--rw-rw-rw-   0        0        0       41 2023-06-23 18:41:02.000000 pythonmc-1.0.4/src/pythonmc/entity/arm.py
--rw-rw-rw-   0        0        0      450 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/entity/damage_sources.py
-drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.520954 pythonmc-1.0.4/src/pythonmc/entity/effects/
--rw-rw-rw-   0        0        0       99 2023-06-23 19:00:22.000000 pythonmc-1.0.4/src/pythonmc/entity/effects/__init__.py
--rw-rw-rw-   0        0        0       66 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/entity/effects/status_effect_instance.py
--rw-rw-rw-   0        0        0      680 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/entity/effects/status_effects.py
--rw-rw-rw-   0        0        0     2341 2023-06-23 18:41:02.000000 pythonmc-1.0.4/src/pythonmc/entity/entities.py
--rw-rw-rw-   0        0        0     2388 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/entity/entity.py
--rw-rw-rw-   0        0        0       50 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/entity/hand.py
--rw-rw-rw-   0        0        0     2522 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/entity/living_entity.py
--rw-rw-rw-   0        0        0      142 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/entity/removal_reasons.py
-drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.525417 pythonmc-1.0.4/src/pythonmc/item/
--rw-rw-rw-   0        0        0      179 2023-06-23 19:00:22.000000 pythonmc-1.0.4/src/pythonmc/item/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.529423 pythonmc-1.0.4/src/pythonmc/item/enchantment/
--rw-rw-rw-   0        0        0      126 2023-06-23 18:59:00.000000 pythonmc-1.0.4/src/pythonmc/item/enchantment/__init__.py
--rw-rw-rw-   0        0        0       51 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/item/enchantment/enchantment.py
--rw-rw-rw-   0        0        0       93 2023-06-23 18:41:02.000000 pythonmc-1.0.4/src/pythonmc/item/enchantment/enchantment_rarity.py
--rw-rw-rw-   0        0        0      806 2023-06-23 18:41:02.000000 pythonmc-1.0.4/src/pythonmc/item/enchantment/enchantments.py
--rw-rw-rw-   0        0        0      171 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/item/hide_flags.py
--rw-rw-rw-   0        0        0       57 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/item/item.py
--rw-rw-rw-   0        0        0       81 2023-06-23 18:41:02.000000 pythonmc-1.0.4/src/pythonmc/item/item_rarity.py
--rw-rw-rw-   0        0        0     1365 2023-06-23 18:42:29.000000 pythonmc-1.0.4/src/pythonmc/item/item_stack.py
--rw-rw-rw-   0        0        0    31019 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/item/items.py
-drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.533422 pythonmc-1.0.4/src/pythonmc/player/
--rw-rw-rw-   0        0        0      183 2023-06-23 19:00:22.000000 pythonmc-1.0.4/src/pythonmc/player/__init__.py
--rw-rw-rw-   0        0        0       44 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/player/ender_chest_inventory.py
--rw-rw-rw-   0        0        0       86 2023-06-23 18:41:02.000000 pythonmc-1.0.4/src/pythonmc/player/hunger_manager.py
--rw-rw-rw-   0        0        0     1063 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/player/player_entity.py
--rw-rw-rw-   0        0        0      846 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/player/player_inventory.py
--rw-rw-rw-   0        0        0      873 2023-06-23 18:41:02.000000 pythonmc-1.0.4/src/pythonmc/player/player_manager.py
--rw-rw-rw-   0        0        0        0 2023-06-23 17:56:35.000000 pythonmc-1.0.4/src/pythonmc/py.typed
-drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.540094 pythonmc-1.0.4/src/pythonmc/scoreboard/
--rw-rw-rw-   0        0        0      286 2023-06-23 19:00:22.000000 pythonmc-1.0.4/src/pythonmc/scoreboard/__init__.py
--rw-rw-rw-   0        0        0       53 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/scoreboard/render_types.py
-drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.542598 pythonmc-1.0.4/src/pythonmc/scoreboard/rules/
--rw-rw-rw-   0        0        0       90 2023-06-23 19:00:22.000000 pythonmc-1.0.4/src/pythonmc/scoreboard/rules/__init__.py
--rw-rw-rw-   0        0        0      103 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/scoreboard/rules/collision_rules.py
--rw-rw-rw-   0        0        0      112 2023-06-23 18:41:02.000000 pythonmc-1.0.4/src/pythonmc/scoreboard/rules/visibility_rules.py
--rw-rw-rw-   0        0        0      907 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/scoreboard/scoreboard.py
--rw-rw-rw-   0        0        0     1156 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/scoreboard/scoreboard_criterions.py
--rw-rw-rw-   0        0        0      262 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/scoreboard/scoreboard_objective.py
--rw-rw-rw-   0        0        0      284 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/scoreboard/scoreboard_player_score.py
--rw-rw-rw-   0        0        0      957 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/scoreboard/team.py
-drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.544606 pythonmc-1.0.4/src/pythonmc/server/
--rw-rw-rw-   0        0        0       97 2023-06-23 19:00:22.000000 pythonmc-1.0.4/src/pythonmc/server/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.546606 pythonmc-1.0.4/src/pythonmc/server/difficulty/
--rw-rw-rw-   0        0        0       74 2023-06-23 18:57:40.000000 pythonmc-1.0.4/src/pythonmc/server/difficulty/__init__.py
--rw-rw-rw-   0        0        0       83 2023-06-23 18:41:02.000000 pythonmc-1.0.4/src/pythonmc/server/difficulty/difficulties.py
--rw-rw-rw-   0        0        0       59 2023-06-23 18:41:02.000000 pythonmc-1.0.4/src/pythonmc/server/difficulty/difficulty.py
-drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.548872 pythonmc-1.0.4/src/pythonmc/server/gamemode/
--rw-rw-rw-   0        0        0       66 2023-06-23 18:57:30.000000 pythonmc-1.0.4/src/pythonmc/server/gamemode/__init__.py
--rw-rw-rw-   0        0        0      117 2023-06-23 18:41:02.000000 pythonmc-1.0.4/src/pythonmc/server/gamemode/game_mode.py
--rw-rw-rw-   0        0        0       92 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/server/gamemode/game_modes.py
--rw-rw-rw-   0        0        0      940 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/server/server.py
-drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.550872 pythonmc-1.0.4/src/pythonmc/server/text/
--rw-rw-rw-   0        0        0       58 2023-06-23 19:00:22.000000 pythonmc-1.0.4/src/pythonmc/server/text/__init__.py
--rw-rw-rw-   0        0        0      394 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/server/text/formatting.py
--rw-rw-rw-   0        0        0      108 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/server/text/text.py
-drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.557395 pythonmc-1.0.4/src/pythonmc/world/
--rw-rw-rw-   0        0        0      193 2023-06-23 19:00:22.000000 pythonmc-1.0.4/src/pythonmc/world/__init__.py
--rw-rw-rw-   0        0        0      323 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/world/executor.py
--rw-rw-rw-   0        0        0     1851 2023-06-23 18:40:37.000000 pythonmc-1.0.4/src/pythonmc/world/particles.py
-drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.559397 pythonmc-1.0.4/src/pythonmc/world/position/
--rw-rw-rw-   0        0        0       50 2023-06-23 18:55:59.000000 pythonmc-1.0.4/src/pythonmc/world/position/__init__.py
--rw-rw-rw-   0        0        0       73 2023-06-23 18:41:02.000000 pythonmc-1.0.4/src/pythonmc/world/position/vec2f.py
--rw-rw-rw-   0        0        0       87 2023-06-23 18:41:02.000000 pythonmc-1.0.4/src/pythonmc/world/position/vec3d.py
--rw-rw-rw-   0        0        0       73 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/world/time_.py
--rw-rw-rw-   0        0        0       62 2023-06-23 18:41:02.000000 pythonmc-1.0.4/src/pythonmc/world/weather.py
--rw-rw-rw-   0        0        0      780 2023-06-23 18:41:03.000000 pythonmc-1.0.4/src/pythonmc/world/world.py
--rw-rw-rw-   0        0        0       63 2023-06-23 18:41:02.000000 pythonmc-1.0.4/src/pythonmc/world/worlds.py
-drwxrwxrwx   0        0        0        0 2023-06-23 19:04:45.506236 pythonmc-1.0.4/src/pythonmc.egg-info/
--rw-rw-rw-   0        0        0     5394 2023-06-23 19:04:45.000000 pythonmc-1.0.4/src/pythonmc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2566 2023-06-23 19:04:45.000000 pythonmc-1.0.4/src/pythonmc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 19:04:45.000000 pythonmc-1.0.4/src/pythonmc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-23 19:04:45.000000 pythonmc-1.0.4/src/pythonmc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.919944 pythonmc-1.0.5/
+-rw-rw-rw-   0        0        0     5394 2023-06-25 17:44:49.918936 pythonmc-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4877 2023-06-23 17:56:35.000000 pythonmc-1.0.5/README.md
+-rw-rw-rw-   0        0        0      108 2023-06-23 19:54:25.000000 pythonmc-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-25 17:44:49.920462 pythonmc-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      792 2023-06-25 17:44:37.000000 pythonmc-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.852601 pythonmc-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.863929 pythonmc-1.0.5/src/pythonmc/
+-rw-rw-rw-   0        0        0        0 2023-06-25 17:29:40.000000 pythonmc-1.0.5/src/pythonmc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.872607 pythonmc-1.0.5/src/pythonmc/block/
+-rw-rw-rw-   0        0        0      124 2023-06-25 17:22:49.000000 pythonmc-1.0.5/src/pythonmc/block/__init__.py
+-rw-rw-rw-   0        0        0      214 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/block/block.py
+-rw-rw-rw-   0        0        0      108 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/block/block_pos.py
+-rw-rw-rw-   0        0        0      140 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/block/block_state.py
+-rw-rw-rw-   0        0        0    28276 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/block/blocks.py
+drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.879869 pythonmc-1.0.5/src/pythonmc/entity/
+-rw-rw-rw-   0        0        0      259 2023-06-25 17:23:05.000000 pythonmc-1.0.5/src/pythonmc/entity/__init__.py
+-rw-rw-rw-   0        0        0       47 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/entity/arm.py
+-rw-rw-rw-   0        0        0      519 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/entity/damage_sources.py
+drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.881920 pythonmc-1.0.5/src/pythonmc/entity/effects/
+-rw-rw-rw-   0        0        0      101 2023-06-25 17:24:15.000000 pythonmc-1.0.5/src/pythonmc/entity/effects/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/entity/effects/status_effect_instance.py
+-rw-rw-rw-   0        0        0      779 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/entity/effects/status_effects.py
+-rw-rw-rw-   0        0        0     2713 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/entity/entities.py
+-rw-rw-rw-   0        0        0     2946 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/entity/entity.py
+-rw-rw-rw-   0        0        0       56 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/entity/hand.py
+-rw-rw-rw-   0        0        0     3026 2023-06-25 17:20:49.000000 pythonmc-1.0.5/src/pythonmc/entity/living_entity.py
+-rw-rw-rw-   0        0        0      157 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/entity/removal_reasons.py
+drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.886518 pythonmc-1.0.5/src/pythonmc/item/
+-rw-rw-rw-   0        0        0      185 2023-06-25 17:23:02.000000 pythonmc-1.0.5/src/pythonmc/item/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.890188 pythonmc-1.0.5/src/pythonmc/item/enchantment/
+-rw-rw-rw-   0        0        0      129 2023-06-25 17:24:18.000000 pythonmc-1.0.5/src/pythonmc/item/enchantment/__init__.py
+-rw-rw-rw-   0        0        0       57 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/item/enchantment/enchantment.py
+-rw-rw-rw-   0        0        0      105 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/item/enchantment/enchantment_rarity.py
+-rw-rw-rw-   0        0        0      923 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/item/enchantment/enchantments.py
+-rw-rw-rw-   0        0        0      195 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/item/hide_flags.py
+-rw-rw-rw-   0        0        0       76 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/item/item.py
+-rw-rw-rw-   0        0        0       93 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/item/item_rarity.py
+-rw-rw-rw-   0        0        0     1680 2023-06-25 17:13:02.000000 pythonmc-1.0.5/src/pythonmc/item/item_stack.py
+-rw-rw-rw-   0        0        0    34784 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/item/items.py
+drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.894782 pythonmc-1.0.5/src/pythonmc/player/
+-rw-rw-rw-   0        0        0      187 2023-06-25 17:22:56.000000 pythonmc-1.0.5/src/pythonmc/player/__init__.py
+-rw-rw-rw-   0        0        0       47 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/player/ender_chest_inventory.py
+-rw-rw-rw-   0        0        0       95 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/player/hunger_manager.py
+-rw-rw-rw-   0        0        0     1261 2023-06-25 17:40:06.000000 pythonmc-1.0.5/src/pythonmc/player/player_entity.py
+-rw-rw-rw-   0        0        0     1023 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/player/player_inventory.py
+-rw-rw-rw-   0        0        0     1041 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/player/player_manager.py
+-rw-rw-rw-   0        0        0        0 2023-06-23 17:56:35.000000 pythonmc-1.0.5/src/pythonmc/py.typed
+drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.899953 pythonmc-1.0.5/src/pythonmc/scoreboard/
+-rw-rw-rw-   0        0        0      293 2023-06-25 17:22:44.000000 pythonmc-1.0.5/src/pythonmc/scoreboard/__init__.py
+-rw-rw-rw-   0        0        0       59 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/scoreboard/render_types.py
+drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.902007 pythonmc-1.0.5/src/pythonmc/scoreboard/rules/
+-rw-rw-rw-   0        0        0       92 2023-06-25 17:22:58.000000 pythonmc-1.0.5/src/pythonmc/scoreboard/rules/__init__.py
+-rw-rw-rw-   0        0        0      115 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/scoreboard/rules/collision_rules.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/scoreboard/rules/visibility_rules.py
+-rw-rw-rw-   0        0        0     1078 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/scoreboard/scoreboard.py
+-rw-rw-rw-   0        0        0     1285 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/scoreboard/scoreboard_criterions.py
+-rw-rw-rw-   0        0        0      316 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/scoreboard/scoreboard_objective.py
+-rw-rw-rw-   0        0        0      410 2023-06-25 17:38:22.000000 pythonmc-1.0.5/src/pythonmc/scoreboard/scoreboard_player_score.py
+-rw-rw-rw-   0        0        0     1137 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/scoreboard/team.py
+drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.903034 pythonmc-1.0.5/src/pythonmc/server/
+-rw-rw-rw-   0        0        0      101 2023-06-25 17:22:25.000000 pythonmc-1.0.5/src/pythonmc/server/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.905617 pythonmc-1.0.5/src/pythonmc/server/difficulty/
+-rw-rw-rw-   0        0        0       76 2023-06-25 17:20:46.000000 pythonmc-1.0.5/src/pythonmc/server/difficulty/__init__.py
+-rw-rw-rw-   0        0        0       95 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/server/difficulty/difficulties.py
+-rw-rw-rw-   0        0        0       68 2023-06-25 17:07:52.000000 pythonmc-1.0.5/src/pythonmc/server/difficulty/difficulty.py
+drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.907640 pythonmc-1.0.5/src/pythonmc/server/gamemode/
+-rw-rw-rw-   0        0        0       68 2023-06-25 17:24:06.000000 pythonmc-1.0.5/src/pythonmc/server/gamemode/__init__.py
+-rw-rw-rw-   0        0        0      135 2023-06-25 17:07:52.000000 pythonmc-1.0.5/src/pythonmc/server/gamemode/game_mode.py
+-rw-rw-rw-   0        0        0      104 2023-06-25 17:07:52.000000 pythonmc-1.0.5/src/pythonmc/server/gamemode/game_modes.py
+-rw-rw-rw-   0        0        0     1138 2023-06-25 17:07:52.000000 pythonmc-1.0.5/src/pythonmc/server/server.py
+drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.910199 pythonmc-1.0.5/src/pythonmc/server/text/
+-rw-rw-rw-   0        0        0       60 2023-06-25 17:24:23.000000 pythonmc-1.0.5/src/pythonmc/server/text/__init__.py
+-rw-rw-rw-   0        0        0      460 2023-06-25 17:07:52.000000 pythonmc-1.0.5/src/pythonmc/server/text/formatting.py
+-rw-rw-rw-   0        0        0      140 2023-06-25 17:07:52.000000 pythonmc-1.0.5/src/pythonmc/server/text/text.py
+drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.915836 pythonmc-1.0.5/src/pythonmc/world/
+-rw-rw-rw-   0        0        0      200 2023-06-25 17:22:53.000000 pythonmc-1.0.5/src/pythonmc/world/__init__.py
+-rw-rw-rw-   0        0        0      476 2023-06-25 17:37:56.000000 pythonmc-1.0.5/src/pythonmc/world/executor.py
+-rw-rw-rw-   0        0        0     2109 2023-06-25 17:07:52.000000 pythonmc-1.0.5/src/pythonmc/world/particles.py
+drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.918936 pythonmc-1.0.5/src/pythonmc/world/position/
+-rw-rw-rw-   0        0        0       52 2023-06-25 17:20:37.000000 pythonmc-1.0.5/src/pythonmc/world/position/__init__.py
+-rw-rw-rw-   0        0        0       88 2023-06-25 17:07:52.000000 pythonmc-1.0.5/src/pythonmc/world/position/vec2f.py
+-rw-rw-rw-   0        0        0      105 2023-06-25 17:07:52.000000 pythonmc-1.0.5/src/pythonmc/world/position/vec3d.py
+-rw-rw-rw-   0        0        0       85 2023-06-25 17:07:52.000000 pythonmc-1.0.5/src/pythonmc/world/time_.py
+-rw-rw-rw-   0        0        0       71 2023-06-25 17:07:52.000000 pythonmc-1.0.5/src/pythonmc/world/weather.py
+-rw-rw-rw-   0        0        0     1178 2023-06-25 17:41:28.000000 pythonmc-1.0.5/src/pythonmc/world/world.py
+-rw-rw-rw-   0        0        0       72 2023-06-25 17:07:52.000000 pythonmc-1.0.5/src/pythonmc/world/worlds.py
+drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.868035 pythonmc-1.0.5/src/pythonmc.egg-info/
+-rw-rw-rw-   0        0        0     5394 2023-06-25 17:44:49.000000 pythonmc-1.0.5/src/pythonmc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2566 2023-06-25 17:44:49.000000 pythonmc-1.0.5/src/pythonmc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 17:44:49.000000 pythonmc-1.0.5/src/pythonmc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-25 17:44:49.000000 pythonmc-1.0.5/src/pythonmc.egg-info/top_level.txt
```

### Comparing `pythonmc-1.0.4/PKG-INFO` & `pythonmc-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonmc
-Version: 1.0.4
+Version: 1.0.5
 Summary: The python library for PythonMC
 Home-page: https://github.com/RevolvingMadness/PythonMC
 Author: RevolvingMadness
 Author-email: revolvingmad@gmail.com
 Project-URL: Bug Tracker, https://github.com/RevolvingMadness/PythonMC/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pythonmc Version: 1.0.4 Summary: The python library
+Metadata-Version: 2.1 Name: pythonmc Version: 1.0.5 Summary: The python library
 for PythonMC Home-page: https://github.com/RevolvingMadness/PythonMC Author:
 RevolvingMadness Author-email: revolvingmad@gmail.com Project-URL: Bug Tracker,
 https://github.com/RevolvingMadness/PythonMC/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown  [![Contributors][contributors-shield]]
 [contributors-url] [![Forks][forks-shield]][forks-url] [![Stargazers][stars-
```

### Comparing `pythonmc-1.0.4/README.md` & `pythonmc-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pythonmc-1.0.4/setup.py` & `pythonmc-1.0.5/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pythonmc",
-    version="1.0.4",
+    version="1.0.5",
     author="RevolvingMadness",
     author_email="revolvingmad@gmail.com",
     description="The python library for PythonMC",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/RevolvingMadness/PythonMC",
-    project_urls={
-        "Bug Tracker": "https://github.com/RevolvingMadness/PythonMC/issues"
-    },
+    project_urls={"Bug Tracker": "https://github.com/RevolvingMadness/PythonMC/issues"},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages("src"),
     package_dir={"": "src"},
     python_requires=">=3.9",
-    package_data={
-        "pythonmc": ["py.typed"]
-    }
+    package_data={"pythonmc": ["py.typed"]},
 )
```

### Comparing `pythonmc-1.0.4/src/pythonmc/entity/living_entity.py` & `pythonmc-1.0.5/src/pythonmc/entity/living_entity.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,182 +1,180 @@
-from src.pythonmc.entity.entity import Entity
+from .entity import Entity
 
 
 class LivingEntity(Entity):
-	def addStatusEffect(
-			self, effect, duration, amplifier, visible
-	):
-		...
+    def addStatusEffect(self, effect, duration, amplifier, visible):
+        ...
 
-	def canBreatheInWater(self):
-		...
+    def canBreatheInWater(self):
+        ...
 
-	def canHaveStatusEffect(self, effect):
-		...
+    def canHaveStatusEffect(self, effect):
+        ...
 
-	def canSee(self, entity):
-		...
+    def canSee(self, entity):
+        ...
 
-	def canTakeDamage(self):
-		...
+    def canTakeDamage(self):
+        ...
 
-	def clearStatusEffects(self):
-		...
+    def clearStatusEffects(self):
+        ...
 
-	def damageArmor(self, damageSource, amount):
-		...
+    def damageArmor(self, damageSource, amount):
+        ...
 
-	def damageHelmet(self, damageSource, amount):
-		...
+    def damageHelmet(self, damageSource, amount):
+        ...
 
-	def damageShield(self, amount):
-		...
+    def damageShield(self, amount):
+        ...
 
-	def eatFood(self, stack):
-		...
+    def eatFood(self, stack):
+        ...
 
-	def getAbsorptionAmount(self):
-		...
+    def getAbsorptionAmount(self):
+        ...
 
-	def getActiveHand(self):
-		...
+    def getActiveHand(self):
+        ...
 
-	def getActiveItem(self):
-		...
+    def getActiveItem(self):
+        ...
 
-	def getArmor(self):
-		...
+    def getArmor(self):
+        ...
 
-	def getAttacker(self):
-		...
+    def getAttacker(self):
+        ...
 
-	def getAttacking(self):
-		...
+    def getAttacking(self):
+        ...
 
-	def getMainArm(self):
-		...
+    def getMainArm(self):
+        ...
 
-	def getMainHandStack(self):
-		...
+    def getMainHandStack(self):
+        ...
 
-	def getMaxHealth(self):
-		...
+    def getMaxHealth(self):
+        ...
 
-	def getMovementSpeed(self):
-		...
+    def getMovementSpeed(self):
+        ...
 
-	def getScaleFactor(self):
-		...
+    def getScaleFactor(self):
+        ...
 
-	def getStackInHand(self, hand):
-		...
+    def getStackInHand(self, hand):
+        ...
 
-	def getStatusEffect(self, effect):
-		...
+    def getStatusEffect(self, effect):
+        ...
 
-	def getStatusEffects(self):
-		...
+    def getStatusEffects(self):
+        ...
 
-	def getStuckArrowCount(self):
-		...
+    def getStuckArrowCount(self):
+        ...
 
-	def hasStatusEffect(self, effect):
-		...
+    def hasStatusEffect(self, effect):
+        ...
 
-	def heal(self, amount):
-		...
+    def heal(self, amount):
+        ...
 
-	def getHealth(self):
-		...
+    def getHealth(self):
+        ...
 
-	def isAffectedBySplashPotions(self):
-		...
+    def isAffectedBySplashPotions(self):
+        ...
 
-	def isBaby(self):
-		...
+    def isBaby(self):
+        ...
 
-	def isBlocking(self):
-		...
+    def isBlocking(self):
+        ...
 
-	def isClimbing(self):
-		...
+    def isClimbing(self):
+        ...
 
-	def isDead(self):
-		...
+    def isDead(self):
+        ...
 
-	def isFallFlying(self):
-		...
+    def isFallFlying(self):
+        ...
 
-	def isHolding(self, item):
-		...
+    def isHolding(self, item):
+        ...
 
-	def isHoldingOntoLadder(self):
-		...
+    def isHoldingOntoLadder(self):
+        ...
 
-	def isHurtByWater(self):
-		...
+    def isHurtByWater(self):
+        ...
 
-	def isMobOrPlayer(self):
-		...
+    def isMobOrPlayer(self):
+        ...
 
-	def isSleeping(self):
-		...
+    def isSleeping(self):
+        ...
 
-	def isUndead(self):
-		...
+    def isUndead(self):
+        ...
 
-	def isUsingItem(self):
-		...
+    def isUsingItem(self):
+        ...
 
-	def isUsingRiptide(self):
-		...
+    def isUsingRiptide(self):
+        ...
 
-	def removeStatusEffect(self, effect):
-		...
+    def removeStatusEffect(self, effect):
+        ...
 
-	def setAbsorptionAmount(self, amount):
-		...
+    def setAbsorptionAmount(self, amount):
+        ...
 
-	def setAttacker(self, entity):
-		...
+    def setAttacker(self, entity):
+        ...
 
-	def setAttacking(self, entity):
-		...
+    def setAttacking(self, entity):
+        ...
 
-	def setCurrentHand(self, hand):
-		...
+    def setCurrentHand(self, hand):
+        ...
 
-	def setHealth(self, amount):
-		...
+    def setHealth(self, amount):
+        ...
 
-	def setJumping(self, jumping):
-		...
+    def setJumping(self, jumping):
+        ...
 
-	def setMovementSpeed(self, movementSpeed):
-		...
+    def setMovementSpeed(self, movementSpeed):
+        ...
 
-	def setStackInHand(self, hand, stack):
-		...
+    def setStackInHand(self, hand, stack):
+        ...
 
-	def setStingerCount(self, stingerCount):
-		...
+    def setStingerCount(self, stingerCount):
+        ...
 
-	def setStuckArrowCount(self, stuckArrowCount):
-		...
+    def setStuckArrowCount(self, stuckArrowCount):
+        ...
 
-	def shouldDisplaySoulSpeedEffects(self):
-		...
+    def shouldDisplaySoulSpeedEffects(self):
+        ...
 
-	def shouldDropXp(self):
-		...
+    def shouldDropXp(self):
+        ...
 
-	def swingHand(self, hand):
-		...
+    def swingHand(self, hand):
+        ...
 
-	def takeKnockback(self, strength, x, z):
-		...
+    def takeKnockback(self, strength, x, z):
+        ...
 
-	def teleport(self, position):
-		...
+    def teleport(self, position):
+        ...
 
-	def tiltScreen(self, deltaX, deltaY):
-		...
+    def tiltScreen(self, deltaX, deltaY):
+        ...
```

### Comparing `pythonmc-1.0.4/src/pythonmc/item/items.py` & `pythonmc-1.0.5/src/pythonmc/block/blocks.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,1256 +1,1004 @@
-class Items:
-	AIR = None
-	STONE = None
-	GRANITE = None
-	POLISHED_GRANITE = None
-	DIORITE = None
-	POLISHED_DIORITE = None
-	ANDESITE = None
-	POLISHED_ANDESITE = None
-	DEEPSLATE = None
-	COBBLED_DEEPSLATE = None
-	POLISHED_DEEPSLATE = None
-	CALCITE = None
-	TUFF = None
-	DRIPSTONE_BLOCK = None
-	GRASS_BLOCK = None
-	DIRT = None
-	COARSE_DIRT = None
-	PODZOL = None
-	ROOTED_DIRT = None
-	MUD = None
-	CRIMSON_NYLIUM = None
-	WARPED_NYLIUM = None
-	COBBLESTONE = None
-	OAK_PLANKS = None
-	SPRUCE_PLANKS = None
-	BIRCH_PLANKS = None
-	JUNGLE_PLANKS = None
-	ACACIA_PLANKS = None
-	CHERRY_PLANKS = None
-	DARK_OAK_PLANKS = None
-	MANGROVE_PLANKS = None
-	BAMBOO_PLANKS = None
-	CRIMSON_PLANKS = None
-	WARPED_PLANKS = None
-	BAMBOO_MOSAIC = None
-	OAK_SAPLING = None
-	SPRUCE_SAPLING = None
-	BIRCH_SAPLING = None
-	JUNGLE_SAPLING = None
-	ACACIA_SAPLING = None
-	CHERRY_SAPLING = None
-	DARK_OAK_SAPLING = None
-	MANGROVE_PROPAGULE = None
-	BEDROCK = None
-	SAND = None
-	SUSPICIOUS_SAND = None
-	SUSPICIOUS_GRAVEL = None
-	RED_SAND = None
-	GRAVEL = None
-	COAL_ORE = None
-	DEEPSLATE_COAL_ORE = None
-	IRON_ORE = None
-	DEEPSLATE_IRON_ORE = None
-	COPPER_ORE = None
-	DEEPSLATE_COPPER_ORE = None
-	GOLD_ORE = None
-	DEEPSLATE_GOLD_ORE = None
-	REDSTONE_ORE = None
-	DEEPSLATE_REDSTONE_ORE = None
-	EMERALD_ORE = None
-	DEEPSLATE_EMERALD_ORE = None
-	LAPIS_ORE = None
-	DEEPSLATE_LAPIS_ORE = None
-	DIAMOND_ORE = None
-	DEEPSLATE_DIAMOND_ORE = None
-	NETHER_GOLD_ORE = None
-	NETHER_QUARTZ_ORE = None
-	ANCIENT_DEBRIS = None
-	COAL_BLOCK = None
-	RAW_IRON_BLOCK = None
-	RAW_COPPER_BLOCK = None
-	RAW_GOLD_BLOCK = None
-	AMETHYST_BLOCK = None
-	BUDDING_AMETHYST = None
-	IRON_BLOCK = None
-	COPPER_BLOCK = None
-	GOLD_BLOCK = None
-	DIAMOND_BLOCK = None
-	NETHERITE_BLOCK = None
-	EXPOSED_COPPER = None
-	WEATHERED_COPPER = None
-	OXIDIZED_COPPER = None
-	CUT_COPPER = None
-	EXPOSED_CUT_COPPER = None
-	WEATHERED_CUT_COPPER = None
-	OXIDIZED_CUT_COPPER = None
-	CUT_COPPER_STAIRS = None
-	EXPOSED_CUT_COPPER_STAIRS = None
-	WEATHERED_CUT_COPPER_STAIRS = None
-	OXIDIZED_CUT_COPPER_STAIRS = None
-	CUT_COPPER_SLAB = None
-	EXPOSED_CUT_COPPER_SLAB = None
-	WEATHERED_CUT_COPPER_SLAB = None
-	OXIDIZED_CUT_COPPER_SLAB = None
-	WAXED_COPPER_BLOCK = None
-	WAXED_EXPOSED_COPPER = None
-	WAXED_WEATHERED_COPPER = None
-	WAXED_OXIDIZED_COPPER = None
-	WAXED_CUT_COPPER = None
-	WAXED_EXPOSED_CUT_COPPER = None
-	WAXED_WEATHERED_CUT_COPPER = None
-	WAXED_OXIDIZED_CUT_COPPER = None
-	WAXED_CUT_COPPER_STAIRS = None
-	WAXED_EXPOSED_CUT_COPPER_STAIRS = None
-	WAXED_WEATHERED_CUT_COPPER_STAIRS = None
-	WAXED_OXIDIZED_CUT_COPPER_STAIRS = None
-	WAXED_CUT_COPPER_SLAB = None
-	WAXED_EXPOSED_CUT_COPPER_SLAB = None
-	WAXED_WEATHERED_CUT_COPPER_SLAB = None
-	WAXED_OXIDIZED_CUT_COPPER_SLAB = None
-	OAK_LOG = None
-	SPRUCE_LOG = None
-	BIRCH_LOG = None
-	JUNGLE_LOG = None
-	ACACIA_LOG = None
-	CHERRY_LOG = None
-	DARK_OAK_LOG = None
-	MANGROVE_LOG = None
-	MANGROVE_ROOTS = None
-	MUDDY_MANGROVE_ROOTS = None
-	CRIMSON_STEM = None
-	WARPED_STEM = None
-	BAMBOO_BLOCK = None
-	STRIPPED_OAK_LOG = None
-	STRIPPED_SPRUCE_LOG = None
-	STRIPPED_BIRCH_LOG = None
-	STRIPPED_JUNGLE_LOG = None
-	STRIPPED_ACACIA_LOG = None
-	STRIPPED_CHERRY_LOG = None
-	STRIPPED_DARK_OAK_LOG = None
-	STRIPPED_MANGROVE_LOG = None
-	STRIPPED_CRIMSON_STEM = None
-	STRIPPED_WARPED_STEM = None
-	STRIPPED_OAK_WOOD = None
-	STRIPPED_SPRUCE_WOOD = None
-	STRIPPED_BIRCH_WOOD = None
-	STRIPPED_JUNGLE_WOOD = None
-	STRIPPED_ACACIA_WOOD = None
-	STRIPPED_CHERRY_WOOD = None
-	STRIPPED_DARK_OAK_WOOD = None
-	STRIPPED_MANGROVE_WOOD = None
-	STRIPPED_CRIMSON_HYPHAE = None
-	STRIPPED_WARPED_HYPHAE = None
-	STRIPPED_BAMBOO_BLOCK = None
-	OAK_WOOD = None
-	SPRUCE_WOOD = None
-	BIRCH_WOOD = None
-	JUNGLE_WOOD = None
-	ACACIA_WOOD = None
-	CHERRY_WOOD = None
-	DARK_OAK_WOOD = None
-	MANGROVE_WOOD = None
-	CRIMSON_HYPHAE = None
-	WARPED_HYPHAE = None
-	OAK_LEAVES = None
-	SPRUCE_LEAVES = None
-	BIRCH_LEAVES = None
-	JUNGLE_LEAVES = None
-	ACACIA_LEAVES = None
-	CHERRY_LEAVES = None
-	DARK_OAK_LEAVES = None
-	MANGROVE_LEAVES = None
-	AZALEA_LEAVES = None
-	FLOWERING_AZALEA_LEAVES = None
-	SPONGE = None
-	WET_SPONGE = None
-	GLASS = None
-	TINTED_GLASS = None
-	LAPIS_BLOCK = None
-	SANDSTONE = None
-	CHISELED_SANDSTONE = None
-	CUT_SANDSTONE = None
-	COBWEB = None
-	GRASS = None
-	FERN = None
-	AZALEA = None
-	FLOWERING_AZALEA = None
-	DEAD_BUSH = None
-	SEAGRASS = None
-	SEA_PICKLE = None
-	WHITE_WOOL = None
-	ORANGE_WOOL = None
-	MAGENTA_WOOL = None
-	LIGHT_BLUE_WOOL = None
-	YELLOW_WOOL = None
-	LIME_WOOL = None
-	PINK_WOOL = None
-	GRAY_WOOL = None
-	LIGHT_GRAY_WOOL = None
-	CYAN_WOOL = None
-	PURPLE_WOOL = None
-	BLUE_WOOL = None
-	BROWN_WOOL = None
-	GREEN_WOOL = None
-	RED_WOOL = None
-	BLACK_WOOL = None
-	DANDELION = None
-	POPPY = None
-	BLUE_ORCHID = None
-	ALLIUM = None
-	AZURE_BLUET = None
-	RED_TULIP = None
-	ORANGE_TULIP = None
-	WHITE_TULIP = None
-	PINK_TULIP = None
-	OXEYE_DAISY = None
-	CORNFLOWER = None
-	LILY_OF_THE_VALLEY = None
-	WITHER_ROSE = None
-	TORCHFLOWER = None
-	PITCHER_PLANT = None
-	SPORE_BLOSSOM = None
-	BROWN_MUSHROOM = None
-	RED_MUSHROOM = None
-	CRIMSON_FUNGUS = None
-	WARPED_FUNGUS = None
-	CRIMSON_ROOTS = None
-	WARPED_ROOTS = None
-	NETHER_SPROUTS = None
-	WEEPING_VINES = None
-	TWISTING_VINES = None
-	SUGAR_CANE = None
-	KELP = None
-	MOSS_CARPET = None
-	PINK_PETALS = None
-	MOSS_BLOCK = None
-	HANGING_ROOTS = None
-	BIG_DRIPLEAF = None
-	SMALL_DRIPLEAF = None
-	BAMBOO = None
-	OAK_SLAB = None
-	SPRUCE_SLAB = None
-	BIRCH_SLAB = None
-	JUNGLE_SLAB = None
-	ACACIA_SLAB = None
-	CHERRY_SLAB = None
-	DARK_OAK_SLAB = None
-	MANGROVE_SLAB = None
-	BAMBOO_SLAB = None
-	BAMBOO_MOSAIC_SLAB = None
-	CRIMSON_SLAB = None
-	WARPED_SLAB = None
-	STONE_SLAB = None
-	SMOOTH_STONE_SLAB = None
-	SANDSTONE_SLAB = None
-	CUT_SANDSTONE_SLAB = None
-	PETRIFIED_OAK_SLAB = None
-	COBBLESTONE_SLAB = None
-	BRICK_SLAB = None
-	STONE_BRICK_SLAB = None
-	MUD_BRICK_SLAB = None
-	NETHER_BRICK_SLAB = None
-	QUARTZ_SLAB = None
-	RED_SANDSTONE_SLAB = None
-	CUT_RED_SANDSTONE_SLAB = None
-	PURPUR_SLAB = None
-	PRISMARINE_SLAB = None
-	PRISMARINE_BRICK_SLAB = None
-	DARK_PRISMARINE_SLAB = None
-	SMOOTH_QUARTZ = None
-	SMOOTH_RED_SANDSTONE = None
-	SMOOTH_SANDSTONE = None
-	SMOOTH_STONE = None
-	BRICKS = None
-	BOOKSHELF = None
-	CHISELED_BOOKSHELF = None
-	DECORATED_POT = None
-	MOSSY_COBBLESTONE = None
-	OBSIDIAN = None
-	TORCH = None
-	END_ROD = None
-	CHORUS_PLANT = None
-	CHORUS_FLOWER = None
-	PURPUR_BLOCK = None
-	PURPUR_PILLAR = None
-	PURPUR_STAIRS = None
-	SPAWNER = None
-	CHEST = None
-	CRAFTING_TABLE = None
-	FARMLAND = None
-	FURNACE = None
-	LADDER = None
-	COBBLESTONE_STAIRS = None
-	SNOW = None
-	ICE = None
-	SNOW_BLOCK = None
-	CACTUS = None
-	CLAY = None
-	JUKEBOX = None
-	OAK_FENCE = None
-	SPRUCE_FENCE = None
-	BIRCH_FENCE = None
-	JUNGLE_FENCE = None
-	ACACIA_FENCE = None
-	CHERRY_FENCE = None
-	DARK_OAK_FENCE = None
-	MANGROVE_FENCE = None
-	BAMBOO_FENCE = None
-	CRIMSON_FENCE = None
-	WARPED_FENCE = None
-	PUMPKIN = None
-	CARVED_PUMPKIN = None
-	JACK_O_LANTERN = None
-	NETHERRACK = None
-	SOUL_SAND = None
-	SOUL_SOIL = None
-	BASALT = None
-	POLISHED_BASALT = None
-	SMOOTH_BASALT = None
-	SOUL_TORCH = None
-	GLOWSTONE = None
-	INFESTED_STONE = None
-	INFESTED_COBBLESTONE = None
-	INFESTED_STONE_BRICKS = None
-	INFESTED_MOSSY_STONE_BRICKS = None
-	INFESTED_CRACKED_STONE_BRICKS = None
-	INFESTED_CHISELED_STONE_BRICKS = None
-	INFESTED_DEEPSLATE = None
-	STONE_BRICKS = None
-	MOSSY_STONE_BRICKS = None
-	CRACKED_STONE_BRICKS = None
-	CHISELED_STONE_BRICKS = None
-	PACKED_MUD = None
-	MUD_BRICKS = None
-	DEEPSLATE_BRICKS = None
-	CRACKED_DEEPSLATE_BRICKS = None
-	DEEPSLATE_TILES = None
-	CRACKED_DEEPSLATE_TILES = None
-	CHISELED_DEEPSLATE = None
-	REINFORCED_DEEPSLATE = None
-	BROWN_MUSHROOM_BLOCK = None
-	RED_MUSHROOM_BLOCK = None
-	MUSHROOM_STEM = None
-	IRON_BARS = None
-	CHAIN = None
-	GLASS_PANE = None
-	MELON = None
-	VINE = None
-	GLOW_LICHEN = None
-	BRICK_STAIRS = None
-	STONE_BRICK_STAIRS = None
-	MUD_BRICK_STAIRS = None
-	MYCELIUM = None
-	LILY_PAD = None
-	NETHER_BRICKS = None
-	CRACKED_NETHER_BRICKS = None
-	CHISELED_NETHER_BRICKS = None
-	NETHER_BRICK_FENCE = None
-	NETHER_BRICK_STAIRS = None
-	SCULK = None
-	SCULK_VEIN = None
-	SCULK_CATALYST = None
-	SCULK_SHRIEKER = None
-	ENCHANTING_TABLE = None
-	END_PORTAL_FRAME = None
-	END_STONE = None
-	END_STONE_BRICKS = None
-	DRAGON_EGG = None
-	SANDSTONE_STAIRS = None
-	ENDER_CHEST = None
-	EMERALD_BLOCK = None
-	OAK_STAIRS = None
-	SPRUCE_STAIRS = None
-	BIRCH_STAIRS = None
-	JUNGLE_STAIRS = None
-	ACACIA_STAIRS = None
-	CHERRY_STAIRS = None
-	DARK_OAK_STAIRS = None
-	MANGROVE_STAIRS = None
-	BAMBOO_STAIRS = None
-	BAMBOO_MOSAIC_STAIRS = None
-	CRIMSON_STAIRS = None
-	WARPED_STAIRS = None
-	COMMAND_BLOCK = None
-	BEACON = None
-	COBBLESTONE_WALL = None
-	MOSSY_COBBLESTONE_WALL = None
-	BRICK_WALL = None
-	PRISMARINE_WALL = None
-	RED_SANDSTONE_WALL = None
-	MOSSY_STONE_BRICK_WALL = None
-	GRANITE_WALL = None
-	STONE_BRICK_WALL = None
-	MUD_BRICK_WALL = None
-	NETHER_BRICK_WALL = None
-	ANDESITE_WALL = None
-	RED_NETHER_BRICK_WALL = None
-	SANDSTONE_WALL = None
-	END_STONE_BRICK_WALL = None
-	DIORITE_WALL = None
-	BLACKSTONE_WALL = None
-	POLISHED_BLACKSTONE_WALL = None
-	POLISHED_BLACKSTONE_BRICK_WALL = None
-	COBBLED_DEEPSLATE_WALL = None
-	POLISHED_DEEPSLATE_WALL = None
-	DEEPSLATE_BRICK_WALL = None
-	DEEPSLATE_TILE_WALL = None
-	ANVIL = None
-	CHIPPED_ANVIL = None
-	DAMAGED_ANVIL = None
-	CHISELED_QUARTZ_BLOCK = None
-	QUARTZ_BLOCK = None
-	QUARTZ_BRICKS = None
-	QUARTZ_PILLAR = None
-	QUARTZ_STAIRS = None
-	WHITE_TERRACOTTA = None
-	ORANGE_TERRACOTTA = None
-	MAGENTA_TERRACOTTA = None
-	LIGHT_BLUE_TERRACOTTA = None
-	YELLOW_TERRACOTTA = None
-	LIME_TERRACOTTA = None
-	PINK_TERRACOTTA = None
-	GRAY_TERRACOTTA = None
-	LIGHT_GRAY_TERRACOTTA = None
-	CYAN_TERRACOTTA = None
-	PURPLE_TERRACOTTA = None
-	BLUE_TERRACOTTA = None
-	BROWN_TERRACOTTA = None
-	GREEN_TERRACOTTA = None
-	RED_TERRACOTTA = None
-	BLACK_TERRACOTTA = None
-	BARRIER = None
-	LIGHT = None
-	HAY_BLOCK = None
-	WHITE_CARPET = None
-	ORANGE_CARPET = None
-	MAGENTA_CARPET = None
-	LIGHT_BLUE_CARPET = None
-	YELLOW_CARPET = None
-	LIME_CARPET = None
-	PINK_CARPET = None
-	GRAY_CARPET = None
-	LIGHT_GRAY_CARPET = None
-	CYAN_CARPET = None
-	PURPLE_CARPET = None
-	BLUE_CARPET = None
-	BROWN_CARPET = None
-	GREEN_CARPET = None
-	RED_CARPET = None
-	BLACK_CARPET = None
-	TERRACOTTA = None
-	PACKED_ICE = None
-	DIRT_PATH = None
-	SUNFLOWER = None
-	LILAC = None
-	ROSE_BUSH = None
-	PEONY = None
-	TALL_GRASS = None
-	LARGE_FERN = None
-	WHITE_STAINED_GLASS = None
-	ORANGE_STAINED_GLASS = None
-	MAGENTA_STAINED_GLASS = None
-	LIGHT_BLUE_STAINED_GLASS = None
-	YELLOW_STAINED_GLASS = None
-	LIME_STAINED_GLASS = None
-	PINK_STAINED_GLASS = None
-	GRAY_STAINED_GLASS = None
-	LIGHT_GRAY_STAINED_GLASS = None
-	CYAN_STAINED_GLASS = None
-	PURPLE_STAINED_GLASS = None
-	BLUE_STAINED_GLASS = None
-	BROWN_STAINED_GLASS = None
-	GREEN_STAINED_GLASS = None
-	RED_STAINED_GLASS = None
-	BLACK_STAINED_GLASS = None
-	WHITE_STAINED_GLASS_PANE = None
-	ORANGE_STAINED_GLASS_PANE = None
-	MAGENTA_STAINED_GLASS_PANE = None
-	LIGHT_BLUE_STAINED_GLASS_PANE = None
-	YELLOW_STAINED_GLASS_PANE = None
-	LIME_STAINED_GLASS_PANE = None
-	PINK_STAINED_GLASS_PANE = None
-	GRAY_STAINED_GLASS_PANE = None
-	LIGHT_GRAY_STAINED_GLASS_PANE = None
-	CYAN_STAINED_GLASS_PANE = None
-	PURPLE_STAINED_GLASS_PANE = None
-	BLUE_STAINED_GLASS_PANE = None
-	BROWN_STAINED_GLASS_PANE = None
-	GREEN_STAINED_GLASS_PANE = None
-	RED_STAINED_GLASS_PANE = None
-	BLACK_STAINED_GLASS_PANE = None
-	PRISMARINE = None
-	PRISMARINE_BRICKS = None
-	DARK_PRISMARINE = None
-	PRISMARINE_STAIRS = None
-	PRISMARINE_BRICK_STAIRS = None
-	DARK_PRISMARINE_STAIRS = None
-	SEA_LANTERN = None
-	RED_SANDSTONE = None
-	CHISELED_RED_SANDSTONE = None
-	CUT_RED_SANDSTONE = None
-	RED_SANDSTONE_STAIRS = None
-	REPEATING_COMMAND_BLOCK = None
-	CHAIN_COMMAND_BLOCK = None
-	MAGMA_BLOCK = None
-	NETHER_WART_BLOCK = None
-	WARPED_WART_BLOCK = None
-	RED_NETHER_BRICKS = None
-	BONE_BLOCK = None
-	STRUCTURE_VOID = None
-	SHULKER_BOX = None
-	WHITE_SHULKER_BOX = None
-	ORANGE_SHULKER_BOX = None
-	MAGENTA_SHULKER_BOX = None
-	LIGHT_BLUE_SHULKER_BOX = None
-	YELLOW_SHULKER_BOX = None
-	LIME_SHULKER_BOX = None
-	PINK_SHULKER_BOX = None
-	GRAY_SHULKER_BOX = None
-	LIGHT_GRAY_SHULKER_BOX = None
-	CYAN_SHULKER_BOX = None
-	PURPLE_SHULKER_BOX = None
-	BLUE_SHULKER_BOX = None
-	BROWN_SHULKER_BOX = None
-	GREEN_SHULKER_BOX = None
-	RED_SHULKER_BOX = None
-	BLACK_SHULKER_BOX = None
-	WHITE_GLAZED_TERRACOTTA = None
-	ORANGE_GLAZED_TERRACOTTA = None
-	MAGENTA_GLAZED_TERRACOTTA = None
-	LIGHT_BLUE_GLAZED_TERRACOTTA = None
-	YELLOW_GLAZED_TERRACOTTA = None
-	LIME_GLAZED_TERRACOTTA = None
-	PINK_GLAZED_TERRACOTTA = None
-	GRAY_GLAZED_TERRACOTTA = None
-	LIGHT_GRAY_GLAZED_TERRACOTTA = None
-	CYAN_GLAZED_TERRACOTTA = None
-	PURPLE_GLAZED_TERRACOTTA = None
-	BLUE_GLAZED_TERRACOTTA = None
-	BROWN_GLAZED_TERRACOTTA = None
-	GREEN_GLAZED_TERRACOTTA = None
-	RED_GLAZED_TERRACOTTA = None
-	BLACK_GLAZED_TERRACOTTA = None
-	WHITE_CONCRETE = None
-	ORANGE_CONCRETE = None
-	MAGENTA_CONCRETE = None
-	LIGHT_BLUE_CONCRETE = None
-	YELLOW_CONCRETE = None
-	LIME_CONCRETE = None
-	PINK_CONCRETE = None
-	GRAY_CONCRETE = None
-	LIGHT_GRAY_CONCRETE = None
-	CYAN_CONCRETE = None
-	PURPLE_CONCRETE = None
-	BLUE_CONCRETE = None
-	BROWN_CONCRETE = None
-	GREEN_CONCRETE = None
-	RED_CONCRETE = None
-	BLACK_CONCRETE = None
-	WHITE_CONCRETE_POWDER = None
-	ORANGE_CONCRETE_POWDER = None
-	MAGENTA_CONCRETE_POWDER = None
-	LIGHT_BLUE_CONCRETE_POWDER = None
-	YELLOW_CONCRETE_POWDER = None
-	LIME_CONCRETE_POWDER = None
-	PINK_CONCRETE_POWDER = None
-	GRAY_CONCRETE_POWDER = None
-	LIGHT_GRAY_CONCRETE_POWDER = None
-	CYAN_CONCRETE_POWDER = None
-	PURPLE_CONCRETE_POWDER = None
-	BLUE_CONCRETE_POWDER = None
-	BROWN_CONCRETE_POWDER = None
-	GREEN_CONCRETE_POWDER = None
-	RED_CONCRETE_POWDER = None
-	BLACK_CONCRETE_POWDER = None
-	TURTLE_EGG = None
-	SNIFFER_EGG = None
-	DEAD_TUBE_CORAL_BLOCK = None
-	DEAD_BRAIN_CORAL_BLOCK = None
-	DEAD_BUBBLE_CORAL_BLOCK = None
-	DEAD_FIRE_CORAL_BLOCK = None
-	DEAD_HORN_CORAL_BLOCK = None
-	TUBE_CORAL_BLOCK = None
-	BRAIN_CORAL_BLOCK = None
-	BUBBLE_CORAL_BLOCK = None
-	FIRE_CORAL_BLOCK = None
-	HORN_CORAL_BLOCK = None
-	TUBE_CORAL = None
-	BRAIN_CORAL = None
-	BUBBLE_CORAL = None
-	FIRE_CORAL = None
-	HORN_CORAL = None
-	DEAD_BRAIN_CORAL = None
-	DEAD_BUBBLE_CORAL = None
-	DEAD_FIRE_CORAL = None
-	DEAD_HORN_CORAL = None
-	DEAD_TUBE_CORAL = None
-	TUBE_CORAL_FAN = None
-	BRAIN_CORAL_FAN = None
-	BUBBLE_CORAL_FAN = None
-	FIRE_CORAL_FAN = None
-	HORN_CORAL_FAN = None
-	DEAD_TUBE_CORAL_FAN = None
-	DEAD_BRAIN_CORAL_FAN = None
-	DEAD_BUBBLE_CORAL_FAN = None
-	DEAD_FIRE_CORAL_FAN = None
-	DEAD_HORN_CORAL_FAN = None
-	BLUE_ICE = None
-	CONDUIT = None
-	POLISHED_GRANITE_STAIRS = None
-	SMOOTH_RED_SANDSTONE_STAIRS = None
-	MOSSY_STONE_BRICK_STAIRS = None
-	POLISHED_DIORITE_STAIRS = None
-	MOSSY_COBBLESTONE_STAIRS = None
-	END_STONE_BRICK_STAIRS = None
-	STONE_STAIRS = None
-	SMOOTH_SANDSTONE_STAIRS = None
-	SMOOTH_QUARTZ_STAIRS = None
-	GRANITE_STAIRS = None
-	ANDESITE_STAIRS = None
-	RED_NETHER_BRICK_STAIRS = None
-	POLISHED_ANDESITE_STAIRS = None
-	DIORITE_STAIRS = None
-	COBBLED_DEEPSLATE_STAIRS = None
-	POLISHED_DEEPSLATE_STAIRS = None
-	DEEPSLATE_BRICK_STAIRS = None
-	DEEPSLATE_TILE_STAIRS = None
-	POLISHED_GRANITE_SLAB = None
-	SMOOTH_RED_SANDSTONE_SLAB = None
-	MOSSY_STONE_BRICK_SLAB = None
-	POLISHED_DIORITE_SLAB = None
-	MOSSY_COBBLESTONE_SLAB = None
-	END_STONE_BRICK_SLAB = None
-	SMOOTH_SANDSTONE_SLAB = None
-	SMOOTH_QUARTZ_SLAB = None
-	GRANITE_SLAB = None
-	ANDESITE_SLAB = None
-	RED_NETHER_BRICK_SLAB = None
-	POLISHED_ANDESITE_SLAB = None
-	DIORITE_SLAB = None
-	COBBLED_DEEPSLATE_SLAB = None
-	POLISHED_DEEPSLATE_SLAB = None
-	DEEPSLATE_BRICK_SLAB = None
-	DEEPSLATE_TILE_SLAB = None
-	SCAFFOLDING = None
-	REDSTONE = None
-	REDSTONE_TORCH = None
-	REDSTONE_BLOCK = None
-	REPEATER = None
-	COMPARATOR = None
-	PISTON = None
-	STICKY_PISTON = None
-	SLIME_BLOCK = None
-	HONEY_BLOCK = None
-	OBSERVER = None
-	HOPPER = None
-	DISPENSER = None
-	DROPPER = None
-	LECTERN = None
-	TARGET = None
-	LEVER = None
-	LIGHTNING_ROD = None
-	DAYLIGHT_DETECTOR = None
-	SCULK_SENSOR = None
-	CALIBRATED_SCULK_SENSOR = None
-	TRIPWIRE_HOOK = None
-	TRAPPED_CHEST = None
-	TNT = None
-	REDSTONE_LAMP = None
-	NOTE_BLOCK = None
-	STONE_BUTTON = None
-	POLISHED_BLACKSTONE_BUTTON = None
-	OAK_BUTTON = None
-	SPRUCE_BUTTON = None
-	BIRCH_BUTTON = None
-	JUNGLE_BUTTON = None
-	ACACIA_BUTTON = None
-	CHERRY_BUTTON = None
-	DARK_OAK_BUTTON = None
-	MANGROVE_BUTTON = None
-	BAMBOO_BUTTON = None
-	CRIMSON_BUTTON = None
-	WARPED_BUTTON = None
-	STONE_PRESSURE_PLATE = None
-	POLISHED_BLACKSTONE_PRESSURE_PLATE = None
-	LIGHT_WEIGHTED_PRESSURE_PLATE = None
-	HEAVY_WEIGHTED_PRESSURE_PLATE = None
-	OAK_PRESSURE_PLATE = None
-	SPRUCE_PRESSURE_PLATE = None
-	BIRCH_PRESSURE_PLATE = None
-	JUNGLE_PRESSURE_PLATE = None
-	ACACIA_PRESSURE_PLATE = None
-	CHERRY_PRESSURE_PLATE = None
-	DARK_OAK_PRESSURE_PLATE = None
-	MANGROVE_PRESSURE_PLATE = None
-	BAMBOO_PRESSURE_PLATE = None
-	CRIMSON_PRESSURE_PLATE = None
-	WARPED_PRESSURE_PLATE = None
-	IRON_DOOR = None
-	OAK_DOOR = None
-	SPRUCE_DOOR = None
-	BIRCH_DOOR = None
-	JUNGLE_DOOR = None
-	ACACIA_DOOR = None
-	CHERRY_DOOR = None
-	DARK_OAK_DOOR = None
-	MANGROVE_DOOR = None
-	BAMBOO_DOOR = None
-	CRIMSON_DOOR = None
-	WARPED_DOOR = None
-	IRON_TRAPDOOR = None
-	OAK_TRAPDOOR = None
-	SPRUCE_TRAPDOOR = None
-	BIRCH_TRAPDOOR = None
-	JUNGLE_TRAPDOOR = None
-	ACACIA_TRAPDOOR = None
-	CHERRY_TRAPDOOR = None
-	DARK_OAK_TRAPDOOR = None
-	MANGROVE_TRAPDOOR = None
-	BAMBOO_TRAPDOOR = None
-	CRIMSON_TRAPDOOR = None
-	WARPED_TRAPDOOR = None
-	OAK_FENCE_GATE = None
-	SPRUCE_FENCE_GATE = None
-	BIRCH_FENCE_GATE = None
-	JUNGLE_FENCE_GATE = None
-	ACACIA_FENCE_GATE = None
-	CHERRY_FENCE_GATE = None
-	DARK_OAK_FENCE_GATE = None
-	MANGROVE_FENCE_GATE = None
-	BAMBOO_FENCE_GATE = None
-	CRIMSON_FENCE_GATE = None
-	WARPED_FENCE_GATE = None
-	POWERED_RAIL = None
-	DETECTOR_RAIL = None
-	RAIL = None
-	ACTIVATOR_RAIL = None
-	SADDLE = None
-	MINECART = None
-	CHEST_MINECART = None
-	FURNACE_MINECART = None
-	TNT_MINECART = None
-	HOPPER_MINECART = None
-	CARROT_ON_A_STICK = None
-	WARPED_FUNGUS_ON_A_STICK = None
-	ELYTRA = None
-	OAK_BOAT = None
-	OAK_CHEST_BOAT = None
-	SPRUCE_BOAT = None
-	SPRUCE_CHEST_BOAT = None
-	BIRCH_BOAT = None
-	BIRCH_CHEST_BOAT = None
-	JUNGLE_BOAT = None
-	JUNGLE_CHEST_BOAT = None
-	ACACIA_BOAT = None
-	ACACIA_CHEST_BOAT = None
-	CHERRY_BOAT = None
-	CHERRY_CHEST_BOAT = None
-	DARK_OAK_BOAT = None
-	DARK_OAK_CHEST_BOAT = None
-	MANGROVE_BOAT = None
-	MANGROVE_CHEST_BOAT = None
-	BAMBOO_RAFT = None
-	BAMBOO_CHEST_RAFT = None
-	STRUCTURE_BLOCK = None
-	JIGSAW = None
-	TURTLE_HELMET = None
-	SCUTE = None
-	FLINT_AND_STEEL = None
-	APPLE = None
-	BOW = None
-	ARROW = None
-	COAL = None
-	CHARCOAL = None
-	DIAMOND = None
-	EMERALD = None
-	LAPIS_LAZULI = None
-	QUARTZ = None
-	AMETHYST_SHARD = None
-	RAW_IRON = None
-	IRON_INGOT = None
-	RAW_COPPER = None
-	COPPER_INGOT = None
-	RAW_GOLD = None
-	GOLD_INGOT = None
-	NETHERITE_INGOT = None
-	NETHERITE_SCRAP = None
-	WOODEN_SWORD = None
-	WOODEN_SHOVEL = None
-	WOODEN_PICKAXE = None
-	WOODEN_AXE = None
-	WOODEN_HOE = None
-	STONE_SWORD = None
-	STONE_SHOVEL = None
-	STONE_PICKAXE = None
-	STONE_AXE = None
-	STONE_HOE = None
-	GOLDEN_SWORD = None
-	GOLDEN_SHOVEL = None
-	GOLDEN_PICKAXE = None
-	GOLDEN_AXE = None
-	GOLDEN_HOE = None
-	IRON_SWORD = None
-	IRON_SHOVEL = None
-	IRON_PICKAXE = None
-	IRON_AXE = None
-	IRON_HOE = None
-	DIAMOND_SWORD = None
-	DIAMOND_SHOVEL = None
-	DIAMOND_PICKAXE = None
-	DIAMOND_AXE = None
-	DIAMOND_HOE = None
-	NETHERITE_SWORD = None
-	NETHERITE_SHOVEL = None
-	NETHERITE_PICKAXE = None
-	NETHERITE_AXE = None
-	NETHERITE_HOE = None
-	STICK = None
-	BOWL = None
-	MUSHROOM_STEW = None
-	STRING = None
-	FEATHER = None
-	GUNPOWDER = None
-	WHEAT_SEEDS = None
-	WHEAT = None
-	BREAD = None
-	LEATHER_HELMET = None
-	LEATHER_CHESTPLATE = None
-	LEATHER_LEGGINGS = None
-	LEATHER_BOOTS = None
-	CHAINMAIL_HELMET = None
-	CHAINMAIL_CHESTPLATE = None
-	CHAINMAIL_LEGGINGS = None
-	CHAINMAIL_BOOTS = None
-	IRON_HELMET = None
-	IRON_CHESTPLATE = None
-	IRON_LEGGINGS = None
-	IRON_BOOTS = None
-	DIAMOND_HELMET = None
-	DIAMOND_CHESTPLATE = None
-	DIAMOND_LEGGINGS = None
-	DIAMOND_BOOTS = None
-	GOLDEN_HELMET = None
-	GOLDEN_CHESTPLATE = None
-	GOLDEN_LEGGINGS = None
-	GOLDEN_BOOTS = None
-	NETHERITE_HELMET = None
-	NETHERITE_CHESTPLATE = None
-	NETHERITE_LEGGINGS = None
-	NETHERITE_BOOTS = None
-	FLINT = None
-	PORKCHOP = None
-	COOKED_PORKCHOP = None
-	PAINTING = None
-	GOLDEN_APPLE = None
-	ENCHANTED_GOLDEN_APPLE = None
-	OAK_SIGN = None
-	SPRUCE_SIGN = None
-	BIRCH_SIGN = None
-	JUNGLE_SIGN = None
-	ACACIA_SIGN = None
-	CHERRY_SIGN = None
-	DARK_OAK_SIGN = None
-	MANGROVE_SIGN = None
-	BAMBOO_SIGN = None
-	CRIMSON_SIGN = None
-	WARPED_SIGN = None
-	OAK_HANGING_SIGN = None
-	SPRUCE_HANGING_SIGN = None
-	BIRCH_HANGING_SIGN = None
-	JUNGLE_HANGING_SIGN = None
-	ACACIA_HANGING_SIGN = None
-	CHERRY_HANGING_SIGN = None
-	DARK_OAK_HANGING_SIGN = None
-	MANGROVE_HANGING_SIGN = None
-	BAMBOO_HANGING_SIGN = None
-	CRIMSON_HANGING_SIGN = None
-	WARPED_HANGING_SIGN = None
-	BUCKET = None
-	WATER_BUCKET = None
-	LAVA_BUCKET = None
-	POWDER_SNOW_BUCKET = None
-	SNOWBALL = None
-	LEATHER = None
-	MILK_BUCKET = None
-	PUFFERFISH_BUCKET = None
-	SALMON_BUCKET = None
-	COD_BUCKET = None
-	TROPICAL_FISH_BUCKET = None
-	AXOLOTL_BUCKET = None
-	TADPOLE_BUCKET = None
-	BRICK = None
-	CLAY_BALL = None
-	DRIED_KELP_BLOCK = None
-	PAPER = None
-	BOOK = None
-	SLIME_BALL = None
-	EGG = None
-	COMPASS = None
-	RECOVERY_COMPASS = None
-	BUNDLE = None
-	FISHING_ROD = None
-	CLOCK = None
-	SPYGLASS = None
-	GLOWSTONE_DUST = None
-	COD = None
-	SALMON = None
-	TROPICAL_FISH = None
-	PUFFERFISH = None
-	COOKED_COD = None
-	COOKED_SALMON = None
-	INK_SAC = None
-	GLOW_INK_SAC = None
-	COCOA_BEANS = None
-	WHITE_DYE = None
-	ORANGE_DYE = None
-	MAGENTA_DYE = None
-	LIGHT_BLUE_DYE = None
-	YELLOW_DYE = None
-	LIME_DYE = None
-	PINK_DYE = None
-	GRAY_DYE = None
-	LIGHT_GRAY_DYE = None
-	CYAN_DYE = None
-	PURPLE_DYE = None
-	BLUE_DYE = None
-	BROWN_DYE = None
-	GREEN_DYE = None
-	RED_DYE = None
-	BLACK_DYE = None
-	BONE_MEAL = None
-	BONE = None
-	SUGAR = None
-	CAKE = None
-	WHITE_BED = None
-	ORANGE_BED = None
-	MAGENTA_BED = None
-	LIGHT_BLUE_BED = None
-	YELLOW_BED = None
-	LIME_BED = None
-	PINK_BED = None
-	GRAY_BED = None
-	LIGHT_GRAY_BED = None
-	CYAN_BED = None
-	PURPLE_BED = None
-	BLUE_BED = None
-	BROWN_BED = None
-	GREEN_BED = None
-	RED_BED = None
-	BLACK_BED = None
-	COOKIE = None
-	FILLED_MAP = None
-	SHEARS = None
-	MELON_SLICE = None
-	DRIED_KELP = None
-	PUMPKIN_SEEDS = None
-	MELON_SEEDS = None
-	BEEF = None
-	COOKED_BEEF = None
-	CHICKEN = None
-	COOKED_CHICKEN = None
-	ROTTEN_FLESH = None
-	ENDER_PEARL = None
-	BLAZE_ROD = None
-	GHAST_TEAR = None
-	GOLD_NUGGET = None
-	NETHER_WART = None
-	POTION = None
-	GLASS_BOTTLE = None
-	SPIDER_EYE = None
-	FERMENTED_SPIDER_EYE = None
-	BLAZE_POWDER = None
-	MAGMA_CREAM = None
-	BREWING_STAND = None
-	CAULDRON = None
-	ENDER_EYE = None
-	GLISTERING_MELON_SLICE = None
-	ALLAY_SPAWN_EGG = None
-	AXOLOTL_SPAWN_EGG = None
-	BAT_SPAWN_EGG = None
-	BEE_SPAWN_EGG = None
-	BLAZE_SPAWN_EGG = None
-	CAT_SPAWN_EGG = None
-	CAMEL_SPAWN_EGG = None
-	CAVE_SPIDER_SPAWN_EGG = None
-	CHICKEN_SPAWN_EGG = None
-	COD_SPAWN_EGG = None
-	COW_SPAWN_EGG = None
-	CREEPER_SPAWN_EGG = None
-	DOLPHIN_SPAWN_EGG = None
-	DONKEY_SPAWN_EGG = None
-	DROWNED_SPAWN_EGG = None
-	ELDER_GUARDIAN_SPAWN_EGG = None
-	ENDER_DRAGON_SPAWN_EGG = None
-	ENDERMAN_SPAWN_EGG = None
-	ENDERMITE_SPAWN_EGG = None
-	EVOKER_SPAWN_EGG = None
-	FOX_SPAWN_EGG = None
-	FROG_SPAWN_EGG = None
-	GHAST_SPAWN_EGG = None
-	GLOW_SQUID_SPAWN_EGG = None
-	GOAT_SPAWN_EGG = None
-	GUARDIAN_SPAWN_EGG = None
-	HOGLIN_SPAWN_EGG = None
-	HORSE_SPAWN_EGG = None
-	HUSK_SPAWN_EGG = None
-	IRON_GOLEM_SPAWN_EGG = None
-	LLAMA_SPAWN_EGG = None
-	MAGMA_CUBE_SPAWN_EGG = None
-	MOOSHROOM_SPAWN_EGG = None
-	MULE_SPAWN_EGG = None
-	OCELOT_SPAWN_EGG = None
-	PANDA_SPAWN_EGG = None
-	PARROT_SPAWN_EGG = None
-	PHANTOM_SPAWN_EGG = None
-	PIG_SPAWN_EGG = None
-	PIGLIN_SPAWN_EGG = None
-	PIGLIN_BRUTE_SPAWN_EGG = None
-	PILLAGER_SPAWN_EGG = None
-	POLAR_BEAR_SPAWN_EGG = None
-	PUFFERFISH_SPAWN_EGG = None
-	RABBIT_SPAWN_EGG = None
-	RAVAGER_SPAWN_EGG = None
-	SALMON_SPAWN_EGG = None
-	SHEEP_SPAWN_EGG = None
-	SHULKER_SPAWN_EGG = None
-	SILVERFISH_SPAWN_EGG = None
-	SKELETON_SPAWN_EGG = None
-	SKELETON_HORSE_SPAWN_EGG = None
-	SLIME_SPAWN_EGG = None
-	SNIFFER_SPAWN_EGG = None
-	SNOW_GOLEM_SPAWN_EGG = None
-	SPIDER_SPAWN_EGG = None
-	SQUID_SPAWN_EGG = None
-	STRAY_SPAWN_EGG = None
-	STRIDER_SPAWN_EGG = None
-	TADPOLE_SPAWN_EGG = None
-	TRADER_LLAMA_SPAWN_EGG = None
-	TROPICAL_FISH_SPAWN_EGG = None
-	TURTLE_SPAWN_EGG = None
-	VEX_SPAWN_EGG = None
-	VILLAGER_SPAWN_EGG = None
-	VINDICATOR_SPAWN_EGG = None
-	WANDERING_TRADER_SPAWN_EGG = None
-	WARDEN_SPAWN_EGG = None
-	WITCH_SPAWN_EGG = None
-	WITHER_SPAWN_EGG = None
-	WITHER_SKELETON_SPAWN_EGG = None
-	WOLF_SPAWN_EGG = None
-	ZOGLIN_SPAWN_EGG = None
-	ZOMBIE_SPAWN_EGG = None
-	ZOMBIE_HORSE_SPAWN_EGG = None
-	ZOMBIE_VILLAGER_SPAWN_EGG = None
-	ZOMBIFIED_PIGLIN_SPAWN_EGG = None
-	EXPERIENCE_BOTTLE = None
-	FIRE_CHARGE = None
-	WRITABLE_BOOK = None
-	WRITTEN_BOOK = None
-	ITEM_FRAME = None
-	GLOW_ITEM_FRAME = None
-	FLOWER_POT = None
-	CARROT = None
-	POTATO = None
-	BAKED_POTATO = None
-	POISONOUS_POTATO = None
-	MAP = None
-	GOLDEN_CARROT = None
-	SKELETON_SKULL = None
-	WITHER_SKELETON_SKULL = None
-	PLAYER_HEAD = None
-	ZOMBIE_HEAD = None
-	CREEPER_HEAD = None
-	DRAGON_HEAD = None
-	PIGLIN_HEAD = None
-	NETHER_STAR = None
-	PUMPKIN_PIE = None
-	FIREWORK_ROCKET = None
-	FIREWORK_STAR = None
-	ENCHANTED_BOOK = None
-	NETHER_BRICK = None
-	PRISMARINE_SHARD = None
-	PRISMARINE_CRYSTALS = None
-	RABBIT = None
-	COOKED_RABBIT = None
-	RABBIT_STEW = None
-	RABBIT_FOOT = None
-	RABBIT_HIDE = None
-	ARMOR_STAND = None
-	IRON_HORSE_ARMOR = None
-	GOLDEN_HORSE_ARMOR = None
-	DIAMOND_HORSE_ARMOR = None
-	LEATHER_HORSE_ARMOR = None
-	LEAD = None
-	NAME_TAG = None
-	COMMAND_BLOCK_MINECART = None
-	MUTTON = None
-	COOKED_MUTTON = None
-	WHITE_BANNER = None
-	ORANGE_BANNER = None
-	MAGENTA_BANNER = None
-	LIGHT_BLUE_BANNER = None
-	YELLOW_BANNER = None
-	LIME_BANNER = None
-	PINK_BANNER = None
-	GRAY_BANNER = None
-	LIGHT_GRAY_BANNER = None
-	CYAN_BANNER = None
-	PURPLE_BANNER = None
-	BLUE_BANNER = None
-	BROWN_BANNER = None
-	GREEN_BANNER = None
-	RED_BANNER = None
-	BLACK_BANNER = None
-	END_CRYSTAL = None
-	CHORUS_FRUIT = None
-	POPPED_CHORUS_FRUIT = None
-	TORCHFLOWER_SEEDS = None
-	PITCHER_POD = None
-	BEETROOT = None
-	BEETROOT_SEEDS = None
-	BEETROOT_SOUP = None
-	DRAGON_BREATH = None
-	SPLASH_POTION = None
-	SPECTRAL_ARROW = None
-	TIPPED_ARROW = None
-	LINGERING_POTION = None
-	SHIELD = None
-	TOTEM_OF_UNDYING = None
-	SHULKER_SHELL = None
-	IRON_NUGGET = None
-	KNOWLEDGE_BOOK = None
-	DEBUG_STICK = None
-	MUSIC_DISC_13 = None
-	MUSIC_DISC_CAT = None
-	MUSIC_DISC_BLOCKS = None
-	MUSIC_DISC_CHIRP = None
-	MUSIC_DISC_FAR = None
-	MUSIC_DISC_MALL = None
-	MUSIC_DISC_MELLOHI = None
-	MUSIC_DISC_STAL = None
-	MUSIC_DISC_STRAD = None
-	MUSIC_DISC_WARD = None
-	MUSIC_DISC_11 = None
-	MUSIC_DISC_WAIT = None
-	MUSIC_DISC_OTHERSIDE = None
-	MUSIC_DISC_RELIC = None
-	MUSIC_DISC_5 = None
-	MUSIC_DISC_PIGSTEP = None
-	DISC_FRAGMENT_5 = None
-	TRIDENT = None
-	PHANTOM_MEMBRANE = None
-	NAUTILUS_SHELL = None
-	HEART_OF_THE_SEA = None
-	CROSSBOW = None
-	SUSPICIOUS_STEW = None
-	LOOM = None
-	FLOWER_BANNER_PATTERN = None
-	CREEPER_BANNER_PATTERN = None
-	SKULL_BANNER_PATTERN = None
-	MOJANG_BANNER_PATTERN = None
-	GLOBE_BANNER_PATTERN = None
-	PIGLIN_BANNER_PATTERN = None
-	GOAT_HORN = None
-	COMPOSTER = None
-	BARREL = None
-	SMOKER = None
-	BLAST_FURNACE = None
-	CARTOGRAPHY_TABLE = None
-	FLETCHING_TABLE = None
-	GRINDSTONE = None
-	SMITHING_TABLE = None
-	STONECUTTER = None
-	BELL = None
-	LANTERN = None
-	SOUL_LANTERN = None
-	SWEET_BERRIES = None
-	GLOW_BERRIES = None
-	CAMPFIRE = None
-	SOUL_CAMPFIRE = None
-	SHROOMLIGHT = None
-	HONEYCOMB = None
-	BEE_NEST = None
-	BEEHIVE = None
-	HONEY_BOTTLE = None
-	HONEYCOMB_BLOCK = None
-	LODESTONE = None
-	CRYING_OBSIDIAN = None
-	BLACKSTONE = None
-	BLACKSTONE_SLAB = None
-	BLACKSTONE_STAIRS = None
-	GILDED_BLACKSTONE = None
-	POLISHED_BLACKSTONE = None
-	POLISHED_BLACKSTONE_SLAB = None
-	POLISHED_BLACKSTONE_STAIRS = None
-	CHISELED_POLISHED_BLACKSTONE = None
-	POLISHED_BLACKSTONE_BRICKS = None
-	POLISHED_BLACKSTONE_BRICK_SLAB = None
-	POLISHED_BLACKSTONE_BRICK_STAIRS = None
-	CRACKED_POLISHED_BLACKSTONE_BRICKS = None
-	RESPAWN_ANCHOR = None
-	CANDLE = None
-	WHITE_CANDLE = None
-	ORANGE_CANDLE = None
-	MAGENTA_CANDLE = None
-	LIGHT_BLUE_CANDLE = None
-	YELLOW_CANDLE = None
-	LIME_CANDLE = None
-	PINK_CANDLE = None
-	GRAY_CANDLE = None
-	LIGHT_GRAY_CANDLE = None
-	CYAN_CANDLE = None
-	PURPLE_CANDLE = None
-	BLUE_CANDLE = None
-	BROWN_CANDLE = None
-	GREEN_CANDLE = None
-	RED_CANDLE = None
-	BLACK_CANDLE = None
-	SMALL_AMETHYST_BUD = None
-	MEDIUM_AMETHYST_BUD = None
-	LARGE_AMETHYST_BUD = None
-	AMETHYST_CLUSTER = None
-	POINTED_DRIPSTONE = None
-	OCHRE_FROGLIGHT = None
-	VERDANT_FROGLIGHT = None
-	PEARLESCENT_FROGLIGHT = None
-	FROGSPAWN = None
-	ECHO_SHARD = None
-	BRUSH = None
-	NETHERITE_UPGRADE_SMITHING_TEMPLATE = None
-	SENTRY_ARMOR_TRIM_SMITHING_TEMPLATE = None
-	DUNE_ARMOR_TRIM_SMITHING_TEMPLATE = None
-	COAST_ARMOR_TRIM_SMITHING_TEMPLATE = None
-	WILD_ARMOR_TRIM_SMITHING_TEMPLATE = None
-	WARD_ARMOR_TRIM_SMITHING_TEMPLATE = None
-	EYE_ARMOR_TRIM_SMITHING_TEMPLATE = None
-	VEX_ARMOR_TRIM_SMITHING_TEMPLATE = None
-	TIDE_ARMOR_TRIM_SMITHING_TEMPLATE = None
-	SNOUT_ARMOR_TRIM_SMITHING_TEMPLATE = None
-	RIB_ARMOR_TRIM_SMITHING_TEMPLATE = None
-	SPIRE_ARMOR_TRIM_SMITHING_TEMPLATE = None
-	WAYFINDER_ARMOR_TRIM_SMITHING_TEMPLATE = None
-	SHAPER_ARMOR_TRIM_SMITHING_TEMPLATE = None
-	SILENCE_ARMOR_TRIM_SMITHING_TEMPLATE = None
-	RAISER_ARMOR_TRIM_SMITHING_TEMPLATE = None
-	HOST_ARMOR_TRIM_SMITHING_TEMPLATE = None
-	ANGLER_POTTERY_SHERD = None
-	ARCHER_POTTERY_SHERD = None
-	ARMS_UP_POTTERY_SHERD = None
-	BLADE_POTTERY_SHERD = None
-	BREWER_POTTERY_SHERD = None
-	BURN_POTTERY_SHERD = None
-	DANGER_POTTERY_SHERD = None
-	EXPLORER_POTTERY_SHERD = None
-	FRIEND_POTTERY_SHERD = None
-	HEART_POTTERY_SHERD = None
-	HEARTBREAK_POTTERY_SHERD = None
-	HOWL_POTTERY_SHERD = None
-	MINER_POTTERY_SHERD = None
-	MOURNER_POTTERY_SHERD = None
-	PLENTY_POTTERY_SHERD = None
-	PRIZE_POTTERY_SHERD = None
-	SHEAF_POTTERY_SHERD = None
-	SHELTER_POTTERY_SHERD = None
-	SKULL_POTTERY_SHERD = None
-	SNORT_POTTERY_SHERD = None
+class Blocks:
+    AIR = None
+    STONE = None
+    GRANITE = None
+    POLISHED_GRANITE = None
+    DIORITE = None
+    POLISHED_DIORITE = None
+    ANDESITE = None
+    POLISHED_ANDESITE = None
+    GRASS_BLOCK = None
+    DIRT = None
+    COARSE_DIRT = None
+    PODZOL = None
+    COBBLESTONE = None
+    OAK_PLANKS = None
+    SPRUCE_PLANKS = None
+    BIRCH_PLANKS = None
+    JUNGLE_PLANKS = None
+    ACACIA_PLANKS = None
+    CHERRY_PLANKS = None
+    DARK_OAK_PLANKS = None
+    MANGROVE_PLANKS = None
+    BAMBOO_PLANKS = None
+    BAMBOO_MOSAIC = None
+    OAK_SAPLING = None
+    SPRUCE_SAPLING = None
+    BIRCH_SAPLING = None
+    JUNGLE_SAPLING = None
+    ACACIA_SAPLING = None
+    CHERRY_SAPLING = None
+    DARK_OAK_SAPLING = None
+    MANGROVE_PROPAGULE = None
+    BEDROCK = None
+    WATER = None
+    LAVA = None
+    SAND = None
+    SUSPICIOUS_SAND = None
+    RED_SAND = None
+    GRAVEL = None
+    SUSPICIOUS_GRAVEL = None
+    GOLD_ORE = None
+    DEEPSLATE_GOLD_ORE = None
+    IRON_ORE = None
+    DEEPSLATE_IRON_ORE = None
+    COAL_ORE = None
+    DEEPSLATE_COAL_ORE = None
+    NETHER_GOLD_ORE = None
+    OAK_LOG = None
+    SPRUCE_LOG = None
+    BIRCH_LOG = None
+    JUNGLE_LOG = None
+    ACACIA_LOG = None
+    CHERRY_LOG = None
+    DARK_OAK_LOG = None
+    MANGROVE_LOG = None
+    MANGROVE_ROOTS = None
+    MUDDY_MANGROVE_ROOTS = None
+    BAMBOO_BLOCK = None
+    STRIPPED_SPRUCE_LOG = None
+    STRIPPED_BIRCH_LOG = None
+    STRIPPED_JUNGLE_LOG = None
+    STRIPPED_ACACIA_LOG = None
+    STRIPPED_CHERRY_LOG = None
+    STRIPPED_DARK_OAK_LOG = None
+    STRIPPED_OAK_LOG = None
+    STRIPPED_MANGROVE_LOG = None
+    STRIPPED_BAMBOO_BLOCK = None
+    OAK_WOOD = None
+    SPRUCE_WOOD = None
+    BIRCH_WOOD = None
+    JUNGLE_WOOD = None
+    ACACIA_WOOD = None
+    CHERRY_WOOD = None
+    DARK_OAK_WOOD = None
+    MANGROVE_WOOD = None
+    STRIPPED_OAK_WOOD = None
+    STRIPPED_SPRUCE_WOOD = None
+    STRIPPED_BIRCH_WOOD = None
+    STRIPPED_JUNGLE_WOOD = None
+    STRIPPED_ACACIA_WOOD = None
+    STRIPPED_CHERRY_WOOD = None
+    STRIPPED_DARK_OAK_WOOD = None
+    STRIPPED_MANGROVE_WOOD = None
+    OAK_LEAVES = None
+    SPRUCE_LEAVES = None
+    BIRCH_LEAVES = None
+    JUNGLE_LEAVES = None
+    ACACIA_LEAVES = None
+    CHERRY_LEAVES = None
+    DARK_OAK_LEAVES = None
+    MANGROVE_LEAVES = None
+    AZALEA_LEAVES = None
+    FLOWERING_AZALEA_LEAVES = None
+    SPONGE = None
+    WET_SPONGE = None
+    GLASS = None
+    LAPIS_ORE = None
+    DEEPSLATE_LAPIS_ORE = None
+    LAPIS_BLOCK = None
+    DISPENSER = None
+    SANDSTONE = None
+    CHISELED_SANDSTONE = None
+    CUT_SANDSTONE = None
+    NOTE_BLOCK = None
+    WHITE_BED = None
+    ORANGE_BED = None
+    MAGENTA_BED = None
+    LIGHT_BLUE_BED = None
+    YELLOW_BED = None
+    LIME_BED = None
+    PINK_BED = None
+    GRAY_BED = None
+    LIGHT_GRAY_BED = None
+    CYAN_BED = None
+    PURPLE_BED = None
+    BLUE_BED = None
+    BROWN_BED = None
+    GREEN_BED = None
+    RED_BED = None
+    BLACK_BED = None
+    POWERED_RAIL = None
+    DETECTOR_RAIL = None
+    STICKY_PISTON = None
+    COBWEB = None
+    GRASS = None
+    FERN = None
+    DEAD_BUSH = None
+    SEAGRASS = None
+    TALL_SEAGRASS = None
+    PISTON = None
+    PISTON_HEAD = None
+    WHITE_WOOL = None
+    ORANGE_WOOL = None
+    MAGENTA_WOOL = None
+    LIGHT_BLUE_WOOL = None
+    YELLOW_WOOL = None
+    LIME_WOOL = None
+    PINK_WOOL = None
+    GRAY_WOOL = None
+    LIGHT_GRAY_WOOL = None
+    CYAN_WOOL = None
+    PURPLE_WOOL = None
+    BLUE_WOOL = None
+    BROWN_WOOL = None
+    GREEN_WOOL = None
+    RED_WOOL = None
+    BLACK_WOOL = None
+    MOVING_PISTON = None
+    DANDELION = None
+    TORCHFLOWER = None
+    POPPY = None
+    BLUE_ORCHID = None
+    ALLIUM = None
+    AZURE_BLUET = None
+    RED_TULIP = None
+    ORANGE_TULIP = None
+    WHITE_TULIP = None
+    PINK_TULIP = None
+    OXEYE_DAISY = None
+    CORNFLOWER = None
+    WITHER_ROSE = None
+    LILY_OF_THE_VALLEY = None
+    BROWN_MUSHROOM = None
+    RED_MUSHROOM = None
+    GOLD_BLOCK = None
+    IRON_BLOCK = None
+    BRICKS = None
+    TNT = None
+    BOOKSHELF = None
+    CHISELED_BOOKSHELF = None
+    MOSSY_COBBLESTONE = None
+    OBSIDIAN = None
+    TORCH = None
+    WALL_TORCH = None
+    FIRE = None
+    SOUL_FIRE = None
+    SPAWNER = None
+    OAK_STAIRS = None
+    CHEST = None
+    REDSTONE_WIRE = None
+    DIAMOND_ORE = None
+    DEEPSLATE_DIAMOND_ORE = None
+    DIAMOND_BLOCK = None
+    CRAFTING_TABLE = None
+    WHEAT = None
+    FARMLAND = None
+    FURNACE = None
+    OAK_SIGN = None
+    SPRUCE_SIGN = None
+    BIRCH_SIGN = None
+    ACACIA_SIGN = None
+    CHERRY_SIGN = None
+    JUNGLE_SIGN = None
+    DARK_OAK_SIGN = None
+    MANGROVE_SIGN = None
+    BAMBOO_SIGN = None
+    OAK_DOOR = None
+    LADDER = None
+    RAIL = None
+    COBBLESTONE_STAIRS = None
+    OAK_WALL_SIGN = None
+    SPRUCE_WALL_SIGN = None
+    BIRCH_WALL_SIGN = None
+    ACACIA_WALL_SIGN = None
+    CHERRY_WALL_SIGN = None
+    JUNGLE_WALL_SIGN = None
+    DARK_OAK_WALL_SIGN = None
+    MANGROVE_WALL_SIGN = None
+    BAMBOO_WALL_SIGN = None
+    OAK_HANGING_SIGN = None
+    SPRUCE_HANGING_SIGN = None
+    BIRCH_HANGING_SIGN = None
+    ACACIA_HANGING_SIGN = None
+    CHERRY_HANGING_SIGN = None
+    JUNGLE_HANGING_SIGN = None
+    DARK_OAK_HANGING_SIGN = None
+    CRIMSON_HANGING_SIGN = None
+    WARPED_HANGING_SIGN = None
+    MANGROVE_HANGING_SIGN = None
+    BAMBOO_HANGING_SIGN = None
+    OAK_WALL_HANGING_SIGN = None
+    SPRUCE_WALL_HANGING_SIGN = None
+    BIRCH_WALL_HANGING_SIGN = None
+    ACACIA_WALL_HANGING_SIGN = None
+    CHERRY_WALL_HANGING_SIGN = None
+    JUNGLE_WALL_HANGING_SIGN = None
+    DARK_OAK_WALL_HANGING_SIGN = None
+    MANGROVE_WALL_HANGING_SIGN = None
+    CRIMSON_WALL_HANGING_SIGN = None
+    WARPED_WALL_HANGING_SIGN = None
+    BAMBOO_WALL_HANGING_SIGN = None
+    LEVER = None
+    STONE_PRESSURE_PLATE = None
+    IRON_DOOR = None
+    OAK_PRESSURE_PLATE = None
+    SPRUCE_PRESSURE_PLATE = None
+    BIRCH_PRESSURE_PLATE = None
+    JUNGLE_PRESSURE_PLATE = None
+    ACACIA_PRESSURE_PLATE = None
+    CHERRY_PRESSURE_PLATE = None
+    DARK_OAK_PRESSURE_PLATE = None
+    MANGROVE_PRESSURE_PLATE = None
+    BAMBOO_PRESSURE_PLATE = None
+    REDSTONE_ORE = None
+    DEEPSLATE_REDSTONE_ORE = None
+    REDSTONE_TORCH = None
+    REDSTONE_WALL_TORCH = None
+    STONE_BUTTON = None
+    SNOW = None
+    ICE = None
+    SNOW_BLOCK = None
+    CACTUS = None
+    CLAY = None
+    SUGAR_CANE = None
+    JUKEBOX = None
+    OAK_FENCE = None
+    PUMPKIN = None
+    NETHERRACK = None
+    SOUL_SAND = None
+    SOUL_SOIL = None
+    BASALT = None
+    POLISHED_BASALT = None
+    SOUL_TORCH = None
+    SOUL_WALL_TORCH = None
+    GLOWSTONE = None
+    NETHER_PORTAL = None
+    CARVED_PUMPKIN = None
+    JACK_O_LANTERN = None
+    CAKE = None
+    REPEATER = None
+    WHITE_STAINED_GLASS = None
+    ORANGE_STAINED_GLASS = None
+    MAGENTA_STAINED_GLASS = None
+    LIGHT_BLUE_STAINED_GLASS = None
+    YELLOW_STAINED_GLASS = None
+    LIME_STAINED_GLASS = None
+    PINK_STAINED_GLASS = None
+    GRAY_STAINED_GLASS = None
+    LIGHT_GRAY_STAINED_GLASS = None
+    CYAN_STAINED_GLASS = None
+    PURPLE_STAINED_GLASS = None
+    BLUE_STAINED_GLASS = None
+    BROWN_STAINED_GLASS = None
+    GREEN_STAINED_GLASS = None
+    RED_STAINED_GLASS = None
+    BLACK_STAINED_GLASS = None
+    OAK_TRAPDOOR = None
+    SPRUCE_TRAPDOOR = None
+    BIRCH_TRAPDOOR = None
+    JUNGLE_TRAPDOOR = None
+    ACACIA_TRAPDOOR = None
+    CHERRY_TRAPDOOR = None
+    DARK_OAK_TRAPDOOR = None
+    MANGROVE_TRAPDOOR = None
+    BAMBOO_TRAPDOOR = None
+    STONE_BRICKS = None
+    MOSSY_STONE_BRICKS = None
+    CRACKED_STONE_BRICKS = None
+    CHISELED_STONE_BRICKS = None
+    PACKED_MUD = None
+    MUD_BRICKS = None
+    INFESTED_STONE = None
+    INFESTED_COBBLESTONE = None
+    INFESTED_STONE_BRICKS = None
+    INFESTED_MOSSY_STONE_BRICKS = None
+    INFESTED_CRACKED_STONE_BRICKS = None
+    INFESTED_CHISELED_STONE_BRICKS = None
+    BROWN_MUSHROOM_BLOCK = None
+    RED_MUSHROOM_BLOCK = None
+    MUSHROOM_STEM = None
+    IRON_BARS = None
+    CHAIN = None
+    GLASS_PANE = None
+    MELON = None
+    ATTACHED_PUMPKIN_STEM = None
+    ATTACHED_MELON_STEM = None
+    PUMPKIN_STEM = None
+    MELON_STEM = None
+    VINE = None
+    GLOW_LICHEN = None
+    OAK_FENCE_GATE = None
+    BRICK_STAIRS = None
+    STONE_BRICK_STAIRS = None
+    MUD_BRICK_STAIRS = None
+    MYCELIUM = None
+    LILY_PAD = None
+    NETHER_BRICKS = None
+    NETHER_BRICK_FENCE = None
+    NETHER_BRICK_STAIRS = None
+    NETHER_WART = None
+    ENCHANTING_TABLE = None
+    BREWING_STAND = None
+    CAULDRON = None
+    WATER_CAULDRON = None
+    LAVA_CAULDRON = None
+    POWDER_SNOW_CAULDRON = None
+    END_PORTAL = None
+    END_PORTAL_FRAME = None
+    END_STONE = None
+    DRAGON_EGG = None
+    REDSTONE_LAMP = None
+    COCOA = None
+    SANDSTONE_STAIRS = None
+    EMERALD_ORE = None
+    DEEPSLATE_EMERALD_ORE = None
+    ENDER_CHEST = None
+    TRIPWIRE_HOOK = None
+    TRIPWIRE = None
+    EMERALD_BLOCK = None
+    SPRUCE_STAIRS = None
+    BIRCH_STAIRS = None
+    JUNGLE_STAIRS = None
+    COMMAND_BLOCK = None
+    BEACON = None
+    COBBLESTONE_WALL = None
+    MOSSY_COBBLESTONE_WALL = None
+    FLOWER_POT = None
+    POTTED_TORCHFLOWER = None
+    POTTED_OAK_SAPLING = None
+    POTTED_SPRUCE_SAPLING = None
+    POTTED_BIRCH_SAPLING = None
+    POTTED_JUNGLE_SAPLING = None
+    POTTED_ACACIA_SAPLING = None
+    POTTED_CHERRY_SAPLING = None
+    POTTED_DARK_OAK_SAPLING = None
+    POTTED_MANGROVE_PROPAGULE = None
+    POTTED_FERN = None
+    POTTED_DANDELION = None
+    POTTED_POPPY = None
+    POTTED_BLUE_ORCHID = None
+    POTTED_ALLIUM = None
+    POTTED_AZURE_BLUET = None
+    POTTED_RED_TULIP = None
+    POTTED_ORANGE_TULIP = None
+    POTTED_WHITE_TULIP = None
+    POTTED_PINK_TULIP = None
+    POTTED_OXEYE_DAISY = None
+    POTTED_CORNFLOWER = None
+    POTTED_LILY_OF_THE_VALLEY = None
+    POTTED_WITHER_ROSE = None
+    POTTED_RED_MUSHROOM = None
+    POTTED_BROWN_MUSHROOM = None
+    POTTED_DEAD_BUSH = None
+    POTTED_CACTUS = None
+    CARROTS = None
+    POTATOES = None
+    OAK_BUTTON = None
+    SPRUCE_BUTTON = None
+    BIRCH_BUTTON = None
+    JUNGLE_BUTTON = None
+    ACACIA_BUTTON = None
+    CHERRY_BUTTON = None
+    DARK_OAK_BUTTON = None
+    MANGROVE_BUTTON = None
+    BAMBOO_BUTTON = None
+    SKELETON_SKULL = None
+    SKELETON_WALL_SKULL = None
+    WITHER_SKELETON_SKULL = None
+    WITHER_SKELETON_WALL_SKULL = None
+    ZOMBIE_HEAD = None
+    ZOMBIE_WALL_HEAD = None
+    PLAYER_HEAD = None
+    PLAYER_WALL_HEAD = None
+    CREEPER_HEAD = None
+    CREEPER_WALL_HEAD = None
+    DRAGON_HEAD = None
+    DRAGON_WALL_HEAD = None
+    PIGLIN_HEAD = None
+    PIGLIN_WALL_HEAD = None
+    ANVIL = None
+    CHIPPED_ANVIL = None
+    DAMAGED_ANVIL = None
+    TRAPPED_CHEST = None
+    LIGHT_WEIGHTED_PRESSURE_PLATE = None
+    HEAVY_WEIGHTED_PRESSURE_PLATE = None
+    COMPARATOR = None
+    DAYLIGHT_DETECTOR = None
+    REDSTONE_BLOCK = None
+    NETHER_QUARTZ_ORE = None
+    HOPPER = None
+    QUARTZ_BLOCK = None
+    CHISELED_QUARTZ_BLOCK = None
+    QUARTZ_PILLAR = None
+    QUARTZ_STAIRS = None
+    ACTIVATOR_RAIL = None
+    DROPPER = None
+    WHITE_TERRACOTTA = None
+    ORANGE_TERRACOTTA = None
+    MAGENTA_TERRACOTTA = None
+    LIGHT_BLUE_TERRACOTTA = None
+    YELLOW_TERRACOTTA = None
+    LIME_TERRACOTTA = None
+    PINK_TERRACOTTA = None
+    GRAY_TERRACOTTA = None
+    LIGHT_GRAY_TERRACOTTA = None
+    CYAN_TERRACOTTA = None
+    PURPLE_TERRACOTTA = None
+    BLUE_TERRACOTTA = None
+    BROWN_TERRACOTTA = None
+    GREEN_TERRACOTTA = None
+    RED_TERRACOTTA = None
+    BLACK_TERRACOTTA = None
+    WHITE_STAINED_GLASS_PANE = None
+    ORANGE_STAINED_GLASS_PANE = None
+    MAGENTA_STAINED_GLASS_PANE = None
+    LIGHT_BLUE_STAINED_GLASS_PANE = None
+    YELLOW_STAINED_GLASS_PANE = None
+    LIME_STAINED_GLASS_PANE = None
+    PINK_STAINED_GLASS_PANE = None
+    GRAY_STAINED_GLASS_PANE = None
+    LIGHT_GRAY_STAINED_GLASS_PANE = None
+    CYAN_STAINED_GLASS_PANE = None
+    PURPLE_STAINED_GLASS_PANE = None
+    BLUE_STAINED_GLASS_PANE = None
+    BROWN_STAINED_GLASS_PANE = None
+    GREEN_STAINED_GLASS_PANE = None
+    RED_STAINED_GLASS_PANE = None
+    BLACK_STAINED_GLASS_PANE = None
+    ACACIA_STAIRS = None
+    CHERRY_STAIRS = None
+    DARK_OAK_STAIRS = None
+    MANGROVE_STAIRS = None
+    BAMBOO_STAIRS = None
+    BAMBOO_MOSAIC_STAIRS = None
+    SLIME_BLOCK = None
+    BARRIER = None
+    LIGHT = None
+    IRON_TRAPDOOR = None
+    PRISMARINE = None
+    PRISMARINE_BRICKS = None
+    DARK_PRISMARINE = None
+    PRISMARINE_STAIRS = None
+    PRISMARINE_BRICK_STAIRS = None
+    DARK_PRISMARINE_STAIRS = None
+    PRISMARINE_SLAB = None
+    PRISMARINE_BRICK_SLAB = None
+    DARK_PRISMARINE_SLAB = None
+    SEA_LANTERN = None
+    HAY_BLOCK = None
+    WHITE_CARPET = None
+    ORANGE_CARPET = None
+    MAGENTA_CARPET = None
+    LIGHT_BLUE_CARPET = None
+    YELLOW_CARPET = None
+    LIME_CARPET = None
+    PINK_CARPET = None
+    GRAY_CARPET = None
+    LIGHT_GRAY_CARPET = None
+    CYAN_CARPET = None
+    PURPLE_CARPET = None
+    BLUE_CARPET = None
+    BROWN_CARPET = None
+    GREEN_CARPET = None
+    RED_CARPET = None
+    BLACK_CARPET = None
+    TERRACOTTA = None
+    COAL_BLOCK = None
+    PACKED_ICE = None
+    SUNFLOWER = None
+    LILAC = None
+    ROSE_BUSH = None
+    PEONY = None
+    TALL_GRASS = None
+    LARGE_FERN = None
+    WHITE_BANNER = None
+    ORANGE_BANNER = None
+    MAGENTA_BANNER = None
+    LIGHT_BLUE_BANNER = None
+    YELLOW_BANNER = None
+    LIME_BANNER = None
+    PINK_BANNER = None
+    GRAY_BANNER = None
+    LIGHT_GRAY_BANNER = None
+    CYAN_BANNER = None
+    PURPLE_BANNER = None
+    BLUE_BANNER = None
+    BROWN_BANNER = None
+    GREEN_BANNER = None
+    RED_BANNER = None
+    BLACK_BANNER = None
+    WHITE_WALL_BANNER = None
+    ORANGE_WALL_BANNER = None
+    MAGENTA_WALL_BANNER = None
+    LIGHT_BLUE_WALL_BANNER = None
+    YELLOW_WALL_BANNER = None
+    LIME_WALL_BANNER = None
+    PINK_WALL_BANNER = None
+    GRAY_WALL_BANNER = None
+    LIGHT_GRAY_WALL_BANNER = None
+    CYAN_WALL_BANNER = None
+    PURPLE_WALL_BANNER = None
+    BLUE_WALL_BANNER = None
+    BROWN_WALL_BANNER = None
+    GREEN_WALL_BANNER = None
+    RED_WALL_BANNER = None
+    BLACK_WALL_BANNER = None
+    RED_SANDSTONE = None
+    CHISELED_RED_SANDSTONE = None
+    CUT_RED_SANDSTONE = None
+    RED_SANDSTONE_STAIRS = None
+    OAK_SLAB = None
+    SPRUCE_SLAB = None
+    BIRCH_SLAB = None
+    JUNGLE_SLAB = None
+    ACACIA_SLAB = None
+    CHERRY_SLAB = None
+    DARK_OAK_SLAB = None
+    MANGROVE_SLAB = None
+    BAMBOO_SLAB = None
+    BAMBOO_MOSAIC_SLAB = None
+    STONE_SLAB = None
+    SMOOTH_STONE_SLAB = None
+    SANDSTONE_SLAB = None
+    CUT_SANDSTONE_SLAB = None
+    PETRIFIED_OAK_SLAB = None
+    COBBLESTONE_SLAB = None
+    BRICK_SLAB = None
+    STONE_BRICK_SLAB = None
+    MUD_BRICK_SLAB = None
+    NETHER_BRICK_SLAB = None
+    QUARTZ_SLAB = None
+    RED_SANDSTONE_SLAB = None
+    CUT_RED_SANDSTONE_SLAB = None
+    PURPUR_SLAB = None
+    SMOOTH_STONE = None
+    SMOOTH_SANDSTONE = None
+    SMOOTH_QUARTZ = None
+    SMOOTH_RED_SANDSTONE = None
+    SPRUCE_FENCE_GATE = None
+    BIRCH_FENCE_GATE = None
+    JUNGLE_FENCE_GATE = None
+    ACACIA_FENCE_GATE = None
+    CHERRY_FENCE_GATE = None
+    DARK_OAK_FENCE_GATE = None
+    MANGROVE_FENCE_GATE = None
+    BAMBOO_FENCE_GATE = None
+    SPRUCE_FENCE = None
+    BIRCH_FENCE = None
+    JUNGLE_FENCE = None
+    ACACIA_FENCE = None
+    CHERRY_FENCE = None
+    DARK_OAK_FENCE = None
+    MANGROVE_FENCE = None
+    BAMBOO_FENCE = None
+    SPRUCE_DOOR = None
+    BIRCH_DOOR = None
+    JUNGLE_DOOR = None
+    ACACIA_DOOR = None
+    CHERRY_DOOR = None
+    DARK_OAK_DOOR = None
+    MANGROVE_DOOR = None
+    BAMBOO_DOOR = None
+    END_ROD = None
+    CHORUS_PLANT = None
+    CHORUS_FLOWER = None
+    PURPUR_BLOCK = None
+    PURPUR_PILLAR = None
+    PURPUR_STAIRS = None
+    END_STONE_BRICKS = None
+    TORCHFLOWER_CROP = None
+    PITCHER_CROP = None
+    PITCHER_PLANT = None
+    BEETROOTS = None
+    DIRT_PATH = None
+    END_GATEWAY = None
+    REPEATING_COMMAND_BLOCK = None
+    CHAIN_COMMAND_BLOCK = None
+    FROSTED_ICE = None
+    MAGMA_BLOCK = None
+    NETHER_WART_BLOCK = None
+    RED_NETHER_BRICKS = None
+    BONE_BLOCK = None
+    STRUCTURE_VOID = None
+    OBSERVER = None
+    SHULKER_BOX = None
+    WHITE_SHULKER_BOX = None
+    ORANGE_SHULKER_BOX = None
+    MAGENTA_SHULKER_BOX = None
+    LIGHT_BLUE_SHULKER_BOX = None
+    YELLOW_SHULKER_BOX = None
+    LIME_SHULKER_BOX = None
+    PINK_SHULKER_BOX = None
+    GRAY_SHULKER_BOX = None
+    LIGHT_GRAY_SHULKER_BOX = None
+    CYAN_SHULKER_BOX = None
+    PURPLE_SHULKER_BOX = None
+    BLUE_SHULKER_BOX = None
+    BROWN_SHULKER_BOX = None
+    GREEN_SHULKER_BOX = None
+    RED_SHULKER_BOX = None
+    BLACK_SHULKER_BOX = None
+    WHITE_GLAZED_TERRACOTTA = None
+    ORANGE_GLAZED_TERRACOTTA = None
+    MAGENTA_GLAZED_TERRACOTTA = None
+    LIGHT_BLUE_GLAZED_TERRACOTTA = None
+    YELLOW_GLAZED_TERRACOTTA = None
+    LIME_GLAZED_TERRACOTTA = None
+    PINK_GLAZED_TERRACOTTA = None
+    GRAY_GLAZED_TERRACOTTA = None
+    LIGHT_GRAY_GLAZED_TERRACOTTA = None
+    CYAN_GLAZED_TERRACOTTA = None
+    PURPLE_GLAZED_TERRACOTTA = None
+    BLUE_GLAZED_TERRACOTTA = None
+    BROWN_GLAZED_TERRACOTTA = None
+    GREEN_GLAZED_TERRACOTTA = None
+    RED_GLAZED_TERRACOTTA = None
+    BLACK_GLAZED_TERRACOTTA = None
+    WHITE_CONCRETE = None
+    ORANGE_CONCRETE = None
+    MAGENTA_CONCRETE = None
+    LIGHT_BLUE_CONCRETE = None
+    YELLOW_CONCRETE = None
+    LIME_CONCRETE = None
+    PINK_CONCRETE = None
+    GRAY_CONCRETE = None
+    LIGHT_GRAY_CONCRETE = None
+    CYAN_CONCRETE = None
+    PURPLE_CONCRETE = None
+    BLUE_CONCRETE = None
+    BROWN_CONCRETE = None
+    GREEN_CONCRETE = None
+    RED_CONCRETE = None
+    BLACK_CONCRETE = None
+    WHITE_CONCRETE_POWDER = None
+    ORANGE_CONCRETE_POWDER = None
+    MAGENTA_CONCRETE_POWDER = None
+    LIGHT_BLUE_CONCRETE_POWDER = None
+    YELLOW_CONCRETE_POWDER = None
+    LIME_CONCRETE_POWDER = None
+    PINK_CONCRETE_POWDER = None
+    GRAY_CONCRETE_POWDER = None
+    LIGHT_GRAY_CONCRETE_POWDER = None
+    CYAN_CONCRETE_POWDER = None
+    PURPLE_CONCRETE_POWDER = None
+    BLUE_CONCRETE_POWDER = None
+    BROWN_CONCRETE_POWDER = None
+    GREEN_CONCRETE_POWDER = None
+    RED_CONCRETE_POWDER = None
+    BLACK_CONCRETE_POWDER = None
+    KELP = None
+    KELP_PLANT = None
+    DRIED_KELP_BLOCK = None
+    TURTLE_EGG = None
+    SNIFFER_EGG = None
+    DEAD_TUBE_CORAL_BLOCK = None
+    DEAD_BRAIN_CORAL_BLOCK = None
+    DEAD_BUBBLE_CORAL_BLOCK = None
+    DEAD_FIRE_CORAL_BLOCK = None
+    DEAD_HORN_CORAL_BLOCK = None
+    TUBE_CORAL_BLOCK = None
+    BRAIN_CORAL_BLOCK = None
+    BUBBLE_CORAL_BLOCK = None
+    FIRE_CORAL_BLOCK = None
+    HORN_CORAL_BLOCK = None
+    DEAD_TUBE_CORAL = None
+    DEAD_BRAIN_CORAL = None
+    DEAD_BUBBLE_CORAL = None
+    DEAD_FIRE_CORAL = None
+    DEAD_HORN_CORAL = None
+    TUBE_CORAL = None
+    BRAIN_CORAL = None
+    BUBBLE_CORAL = None
+    FIRE_CORAL = None
+    HORN_CORAL = None
+    DEAD_TUBE_CORAL_FAN = None
+    DEAD_BRAIN_CORAL_FAN = None
+    DEAD_BUBBLE_CORAL_FAN = None
+    DEAD_FIRE_CORAL_FAN = None
+    DEAD_HORN_CORAL_FAN = None
+    TUBE_CORAL_FAN = None
+    BRAIN_CORAL_FAN = None
+    BUBBLE_CORAL_FAN = None
+    FIRE_CORAL_FAN = None
+    HORN_CORAL_FAN = None
+    DEAD_TUBE_CORAL_WALL_FAN = None
+    DEAD_BRAIN_CORAL_WALL_FAN = None
+    DEAD_BUBBLE_CORAL_WALL_FAN = None
+    DEAD_FIRE_CORAL_WALL_FAN = None
+    DEAD_HORN_CORAL_WALL_FAN = None
+    TUBE_CORAL_WALL_FAN = None
+    BRAIN_CORAL_WALL_FAN = None
+    BUBBLE_CORAL_WALL_FAN = None
+    FIRE_CORAL_WALL_FAN = None
+    HORN_CORAL_WALL_FAN = None
+    SEA_PICKLE = None
+    BLUE_ICE = None
+    CONDUIT = None
+    BAMBOO_SAPLING = None
+    BAMBOO = None
+    POTTED_BAMBOO = None
+    VOID_AIR = None
+    CAVE_AIR = None
+    BUBBLE_COLUMN = None
+    POLISHED_GRANITE_STAIRS = None
+    SMOOTH_RED_SANDSTONE_STAIRS = None
+    MOSSY_STONE_BRICK_STAIRS = None
+    POLISHED_DIORITE_STAIRS = None
+    MOSSY_COBBLESTONE_STAIRS = None
+    END_STONE_BRICK_STAIRS = None
+    STONE_STAIRS = None
+    SMOOTH_SANDSTONE_STAIRS = None
+    SMOOTH_QUARTZ_STAIRS = None
+    GRANITE_STAIRS = None
+    ANDESITE_STAIRS = None
+    RED_NETHER_BRICK_STAIRS = None
+    POLISHED_ANDESITE_STAIRS = None
+    DIORITE_STAIRS = None
+    POLISHED_GRANITE_SLAB = None
+    SMOOTH_RED_SANDSTONE_SLAB = None
+    MOSSY_STONE_BRICK_SLAB = None
+    POLISHED_DIORITE_SLAB = None
+    MOSSY_COBBLESTONE_SLAB = None
+    END_STONE_BRICK_SLAB = None
+    SMOOTH_SANDSTONE_SLAB = None
+    SMOOTH_QUARTZ_SLAB = None
+    GRANITE_SLAB = None
+    ANDESITE_SLAB = None
+    RED_NETHER_BRICK_SLAB = None
+    POLISHED_ANDESITE_SLAB = None
+    DIORITE_SLAB = None
+    BRICK_WALL = None
+    PRISMARINE_WALL = None
+    RED_SANDSTONE_WALL = None
+    MOSSY_STONE_BRICK_WALL = None
+    GRANITE_WALL = None
+    STONE_BRICK_WALL = None
+    MUD_BRICK_WALL = None
+    NETHER_BRICK_WALL = None
+    ANDESITE_WALL = None
+    RED_NETHER_BRICK_WALL = None
+    SANDSTONE_WALL = None
+    END_STONE_BRICK_WALL = None
+    DIORITE_WALL = None
+    SCAFFOLDING = None
+    LOOM = None
+    BARREL = None
+    SMOKER = None
+    BLAST_FURNACE = None
+    CARTOGRAPHY_TABLE = None
+    FLETCHING_TABLE = None
+    GRINDSTONE = None
+    LECTERN = None
+    SMITHING_TABLE = None
+    STONECUTTER = None
+    BELL = None
+    LANTERN = None
+    SOUL_LANTERN = None
+    CAMPFIRE = None
+    SOUL_CAMPFIRE = None
+    SWEET_BERRY_BUSH = None
+    WARPED_STEM = None
+    STRIPPED_WARPED_STEM = None
+    WARPED_HYPHAE = None
+    STRIPPED_WARPED_HYPHAE = None
+    WARPED_NYLIUM = None
+    WARPED_FUNGUS = None
+    WARPED_WART_BLOCK = None
+    WARPED_ROOTS = None
+    NETHER_SPROUTS = None
+    CRIMSON_STEM = None
+    STRIPPED_CRIMSON_STEM = None
+    CRIMSON_HYPHAE = None
+    STRIPPED_CRIMSON_HYPHAE = None
+    CRIMSON_NYLIUM = None
+    CRIMSON_FUNGUS = None
+    SHROOMLIGHT = None
+    WEEPING_VINES = None
+    WEEPING_VINES_PLANT = None
+    TWISTING_VINES = None
+    TWISTING_VINES_PLANT = None
+    CRIMSON_ROOTS = None
+    CRIMSON_PLANKS = None
+    WARPED_PLANKS = None
+    CRIMSON_SLAB = None
+    WARPED_SLAB = None
+    CRIMSON_PRESSURE_PLATE = None
+    WARPED_PRESSURE_PLATE = None
+    CRIMSON_FENCE = None
+    WARPED_FENCE = None
+    CRIMSON_TRAPDOOR = None
+    WARPED_TRAPDOOR = None
+    CRIMSON_FENCE_GATE = None
+    WARPED_FENCE_GATE = None
+    CRIMSON_STAIRS = None
+    WARPED_STAIRS = None
+    CRIMSON_BUTTON = None
+    WARPED_BUTTON = None
+    CRIMSON_DOOR = None
+    WARPED_DOOR = None
+    CRIMSON_SIGN = None
+    WARPED_SIGN = None
+    CRIMSON_WALL_SIGN = None
+    WARPED_WALL_SIGN = None
+    STRUCTURE_BLOCK = None
+    JIGSAW = None
+    COMPOSTER = None
+    TARGET = None
+    BEE_NEST = None
+    BEEHIVE = None
+    HONEY_BLOCK = None
+    HONEYCOMB_BLOCK = None
+    NETHERITE_BLOCK = None
+    ANCIENT_DEBRIS = None
+    CRYING_OBSIDIAN = None
+    RESPAWN_ANCHOR = None
+    POTTED_CRIMSON_FUNGUS = None
+    POTTED_WARPED_FUNGUS = None
+    POTTED_CRIMSON_ROOTS = None
+    POTTED_WARPED_ROOTS = None
+    LODESTONE = None
+    BLACKSTONE = None
+    BLACKSTONE_STAIRS = None
+    BLACKSTONE_WALL = None
+    BLACKSTONE_SLAB = None
+    POLISHED_BLACKSTONE = None
+    POLISHED_BLACKSTONE_BRICKS = None
+    CRACKED_POLISHED_BLACKSTONE_BRICKS = None
+    CHISELED_POLISHED_BLACKSTONE = None
+    POLISHED_BLACKSTONE_BRICK_SLAB = None
+    POLISHED_BLACKSTONE_BRICK_STAIRS = None
+    POLISHED_BLACKSTONE_BRICK_WALL = None
+    GILDED_BLACKSTONE = None
+    POLISHED_BLACKSTONE_STAIRS = None
+    POLISHED_BLACKSTONE_SLAB = None
+    POLISHED_BLACKSTONE_PRESSURE_PLATE = None
+    POLISHED_BLACKSTONE_BUTTON = None
+    POLISHED_BLACKSTONE_WALL = None
+    CHISELED_NETHER_BRICKS = None
+    CRACKED_NETHER_BRICKS = None
+    QUARTZ_BRICKS = None
+    CANDLE = None
+    WHITE_CANDLE = None
+    ORANGE_CANDLE = None
+    MAGENTA_CANDLE = None
+    LIGHT_BLUE_CANDLE = None
+    YELLOW_CANDLE = None
+    LIME_CANDLE = None
+    PINK_CANDLE = None
+    GRAY_CANDLE = None
+    LIGHT_GRAY_CANDLE = None
+    CYAN_CANDLE = None
+    PURPLE_CANDLE = None
+    BLUE_CANDLE = None
+    BROWN_CANDLE = None
+    GREEN_CANDLE = None
+    RED_CANDLE = None
+    BLACK_CANDLE = None
+    CANDLE_CAKE = None
+    WHITE_CANDLE_CAKE = None
+    ORANGE_CANDLE_CAKE = None
+    MAGENTA_CANDLE_CAKE = None
+    LIGHT_BLUE_CANDLE_CAKE = None
+    YELLOW_CANDLE_CAKE = None
+    LIME_CANDLE_CAKE = None
+    PINK_CANDLE_CAKE = None
+    GRAY_CANDLE_CAKE = None
+    LIGHT_GRAY_CANDLE_CAKE = None
+    CYAN_CANDLE_CAKE = None
+    PURPLE_CANDLE_CAKE = None
+    BLUE_CANDLE_CAKE = None
+    BROWN_CANDLE_CAKE = None
+    GREEN_CANDLE_CAKE = None
+    RED_CANDLE_CAKE = None
+    BLACK_CANDLE_CAKE = None
+    AMETHYST_BLOCK = None
+    BUDDING_AMETHYST = None
+    AMETHYST_CLUSTER = None
+    LARGE_AMETHYST_BUD = None
+    MEDIUM_AMETHYST_BUD = None
+    SMALL_AMETHYST_BUD = None
+    TUFF = None
+    CALCITE = None
+    TINTED_GLASS = None
+    POWDER_SNOW = None
+    SCULK_SENSOR = None
+    CALIBRATED_SCULK_SENSOR = None
+    SCULK = None
+    SCULK_VEIN = None
+    SCULK_CATALYST = None
+    SCULK_SHRIEKER = None
+    OXIDIZED_COPPER = None
+    WEATHERED_COPPER = None
+    EXPOSED_COPPER = None
+    COPPER_BLOCK = None
+    COPPER_ORE = None
+    DEEPSLATE_COPPER_ORE = None
+    OXIDIZED_CUT_COPPER = None
+    WEATHERED_CUT_COPPER = None
+    EXPOSED_CUT_COPPER = None
+    CUT_COPPER = None
+    OXIDIZED_CUT_COPPER_STAIRS = None
+    WEATHERED_CUT_COPPER_STAIRS = None
+    EXPOSED_CUT_COPPER_STAIRS = None
+    CUT_COPPER_STAIRS = None
+    OXIDIZED_CUT_COPPER_SLAB = None
+    WEATHERED_CUT_COPPER_SLAB = None
+    EXPOSED_CUT_COPPER_SLAB = None
+    CUT_COPPER_SLAB = None
+    WAXED_COPPER_BLOCK = None
+    WAXED_WEATHERED_COPPER = None
+    WAXED_EXPOSED_COPPER = None
+    WAXED_OXIDIZED_COPPER = None
+    WAXED_OXIDIZED_CUT_COPPER = None
+    WAXED_WEATHERED_CUT_COPPER = None
+    WAXED_EXPOSED_CUT_COPPER = None
+    WAXED_CUT_COPPER = None
+    WAXED_OXIDIZED_CUT_COPPER_STAIRS = None
+    WAXED_WEATHERED_CUT_COPPER_STAIRS = None
+    WAXED_EXPOSED_CUT_COPPER_STAIRS = None
+    WAXED_CUT_COPPER_STAIRS = None
+    WAXED_OXIDIZED_CUT_COPPER_SLAB = None
+    WAXED_WEATHERED_CUT_COPPER_SLAB = None
+    WAXED_EXPOSED_CUT_COPPER_SLAB = None
+    WAXED_CUT_COPPER_SLAB = None
+    LIGHTNING_ROD = None
+    POINTED_DRIPSTONE = None
+    DRIPSTONE_BLOCK = None
+    CAVE_VINES = None
+    CAVE_VINES_PLANT = None
+    SPORE_BLOSSOM = None
+    AZALEA = None
+    FLOWERING_AZALEA = None
+    MOSS_CARPET = None
+    PINK_PETALS = None
+    MOSS_BLOCK = None
+    BIG_DRIPLEAF = None
+    BIG_DRIPLEAF_STEM = None
+    SMALL_DRIPLEAF = None
+    HANGING_ROOTS = None
+    ROOTED_DIRT = None
+    MUD = None
+    DEEPSLATE = None
+    COBBLED_DEEPSLATE = None
+    COBBLED_DEEPSLATE_STAIRS = None
+    COBBLED_DEEPSLATE_SLAB = None
+    COBBLED_DEEPSLATE_WALL = None
+    POLISHED_DEEPSLATE = None
+    POLISHED_DEEPSLATE_STAIRS = None
+    POLISHED_DEEPSLATE_SLAB = None
+    POLISHED_DEEPSLATE_WALL = None
+    DEEPSLATE_TILES = None
+    DEEPSLATE_TILE_STAIRS = None
+    DEEPSLATE_TILE_SLAB = None
+    DEEPSLATE_TILE_WALL = None
+    DEEPSLATE_BRICKS = None
+    DEEPSLATE_BRICK_STAIRS = None
+    DEEPSLATE_BRICK_SLAB = None
+    DEEPSLATE_BRICK_WALL = None
+    CHISELED_DEEPSLATE = None
+    CRACKED_DEEPSLATE_BRICKS = None
+    CRACKED_DEEPSLATE_TILES = None
+    INFESTED_DEEPSLATE = None
+    SMOOTH_BASALT = None
+    RAW_IRON_BLOCK = None
+    RAW_COPPER_BLOCK = None
+    RAW_GOLD_BLOCK = None
+    POTTED_AZALEA_BUSH = None
+    POTTED_FLOWERING_AZALEA_BUSH = None
+    OCHRE_FROGLIGHT = None
+    VERDANT_FROGLIGHT = None
+    PEARLESCENT_FROGLIGHT = None
+    FROGSPAWN = None
+    REINFORCED_DEEPSLATE = None
+    DECORATED_POT = None
```

### Comparing `pythonmc-1.0.4/src/pythonmc/player/player_manager.py` & `pythonmc-1.0.5/src/pythonmc/player/player_manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 from typing import overload
 
 
 class PlayerManager:
-	def areCheatsAllowed(self):
-		pass
+    def areCheatsAllowed(self):
+        pass
 
-	@overload
-	def broadcast(self, message):
-		pass
+    @overload
+    def broadcast(self, message):
+        pass
 
-	@overload
-	def broadcast(self, text):
-		pass
+    @overload
+    def broadcast(self, text):
+        pass
 
-	def disconnectAllPlayers(self):
-		pass
+    def disconnectAllPlayers(self):
+        pass
 
-	def getCurrentPlayerCount(self):
-		pass
+    def getCurrentPlayerCount(self):
+        pass
 
-	def getMaxPlayerCount(self):
-		pass
+    def getMaxPlayerCount(self):
+        pass
 
-	def getOpNames(self):
-		pass
+    def getOpNames(self):
+        pass
 
-	def getPlayer(self, name):
-		pass
+    def getPlayer(self, name):
+        pass
 
-	def getPlayerList(self):
-		pass
+    def getPlayerList(self):
+        pass
 
-	def getPlayerNames(self):
-		pass
+    def getPlayerNames(self):
+        pass
 
-	def getViewDistance(self):
-		pass
+    def getViewDistance(self):
+        pass
 
-	def getWhitelistedNames(self):
-		pass
+    def getWhitelistedNames(self):
+        pass
 
-	def isWhitelistEnabled(self):
-		pass
+    def isWhitelistEnabled(self):
+        pass
 
-	def reloadWhitelist(self):
-		pass
+    def reloadWhitelist(self):
+        pass
 
-	def setCheatsAllowed(self, cheatsAllowed):
-		pass
+    def setCheatsAllowed(self, cheatsAllowed):
+        pass
 
-	def setSimulationDistance(self, simulationDistance):
-		pass
+    def setSimulationDistance(self, simulationDistance):
+        pass
 
-	def setViewDistance(self, viewDistance):
-		pass
+    def setViewDistance(self, viewDistance):
+        pass
 
-	def setWhitelistEnabled(self, whitelistEnabled):
-		pass
+    def setWhitelistEnabled(self, whitelistEnabled):
+        pass
```

### Comparing `pythonmc-1.0.4/src/pythonmc/scoreboard/scoreboard_criterions.py` & `pythonmc-1.0.5/src/pythonmc/scoreboard/scoreboard_criterions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 class ScoreboardCriterions:
-	DUMMY = None
-	TRIGGER = None
-	DEATH_COUNT = None
-	PLAYER_KILL_COUNT = None
-	TOTAL_KILL_COUNT = None
-	HEALTH = None
-	FOOD = None
-	AIR = None
-	ARMOR = None
-	XP = None
-	LEVEL = None
-	TEAM_KILL_BLACK = None
-	TEAM_KILL_DARK_BLUE = None
-	TEAM_KILL_DARK_GREEN = None
-	TEAM_KILL_DARK_AQUA = None
-	TEAM_KILL_DARK_RED = None
-	TEAM_KILL_DARK_PURPLE = None
-	TEAM_KILL_GOLD = None
-	TEAM_KILL_GRAY = None
-	TEAM_KILL_DARK_GRAY = None
-	TEAM_KILL_BLUE = None
-	TEAM_KILL_GREEN = None
-	TEAM_KILL_AQUA = None
-	TEAM_KILL_RED = None
-	TEAM_KILL_LIGHT_PURPLE = None
-	TEAM_KILL_YELLOW = None
-	TEAM_KILL_WHITE = None
-	KILLED_BY_TEAM_BLACK = None
-	KILLED_BY_TEAM_DARK_BLUE = None
-	KILLED_BY_TEAM_DARK_GREEN = None
-	KILLED_BY_TEAM_DARK_AQUA = None
-	KILLED_BY_TEAM_DARK_RED = None
-	KILLED_BY_TEAM_DARK_PURPLE = None
-	KILLED_BY_TEAM_GOLD = None
-	KILLED_BY_TEAM_GRAY = None
-	KILLED_BY_TEAM_DARK_GRAY = None
-	KILLED_BY_TEAM_BLUE = None
-	KILLED_BY_TEAM_GREEN = None
-	KILLED_BY_TEAM_AQUA = None
-	KILLED_BY_TEAM_RED = None
-	KILLED_BY_TEAM_LIGHT_PURPLE = None
-	KILLED_BY_TEAM_YELLOW = None
-	KILLED_BY_TEAM_WHITE = None
+    DUMMY = None
+    TRIGGER = None
+    DEATH_COUNT = None
+    PLAYER_KILL_COUNT = None
+    TOTAL_KILL_COUNT = None
+    HEALTH = None
+    FOOD = None
+    AIR = None
+    ARMOR = None
+    XP = None
+    LEVEL = None
+    TEAM_KILL_BLACK = None
+    TEAM_KILL_DARK_BLUE = None
+    TEAM_KILL_DARK_GREEN = None
+    TEAM_KILL_DARK_AQUA = None
+    TEAM_KILL_DARK_RED = None
+    TEAM_KILL_DARK_PURPLE = None
+    TEAM_KILL_GOLD = None
+    TEAM_KILL_GRAY = None
+    TEAM_KILL_DARK_GRAY = None
+    TEAM_KILL_BLUE = None
+    TEAM_KILL_GREEN = None
+    TEAM_KILL_AQUA = None
+    TEAM_KILL_RED = None
+    TEAM_KILL_LIGHT_PURPLE = None
+    TEAM_KILL_YELLOW = None
+    TEAM_KILL_WHITE = None
+    KILLED_BY_TEAM_BLACK = None
+    KILLED_BY_TEAM_DARK_BLUE = None
+    KILLED_BY_TEAM_DARK_GREEN = None
+    KILLED_BY_TEAM_DARK_AQUA = None
+    KILLED_BY_TEAM_DARK_RED = None
+    KILLED_BY_TEAM_DARK_PURPLE = None
+    KILLED_BY_TEAM_GOLD = None
+    KILLED_BY_TEAM_GRAY = None
+    KILLED_BY_TEAM_DARK_GRAY = None
+    KILLED_BY_TEAM_BLUE = None
+    KILLED_BY_TEAM_GREEN = None
+    KILLED_BY_TEAM_AQUA = None
+    KILLED_BY_TEAM_RED = None
+    KILLED_BY_TEAM_LIGHT_PURPLE = None
+    KILLED_BY_TEAM_YELLOW = None
+    KILLED_BY_TEAM_WHITE = None
```

### Comparing `pythonmc-1.0.4/src/pythonmc.egg-info/PKG-INFO` & `pythonmc-1.0.5/src/pythonmc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonmc
-Version: 1.0.4
+Version: 1.0.5
 Summary: The python library for PythonMC
 Home-page: https://github.com/RevolvingMadness/PythonMC
 Author: RevolvingMadness
 Author-email: revolvingmad@gmail.com
 Project-URL: Bug Tracker, https://github.com/RevolvingMadness/PythonMC/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pythonmc Version: 1.0.4 Summary: The python library
+Metadata-Version: 2.1 Name: pythonmc Version: 1.0.5 Summary: The python library
 for PythonMC Home-page: https://github.com/RevolvingMadness/PythonMC Author:
 RevolvingMadness Author-email: revolvingmad@gmail.com Project-URL: Bug Tracker,
 https://github.com/RevolvingMadness/PythonMC/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown  [![Contributors][contributors-shield]]
 [contributors-url] [![Forks][forks-shield]][forks-url] [![Stargazers][stars-
```

### Comparing `pythonmc-1.0.4/src/pythonmc.egg-info/SOURCES.txt` & `pythonmc-1.0.5/src/pythonmc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

