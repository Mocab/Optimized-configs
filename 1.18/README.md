# Optimized Purpur Configuration Files
This repository contains all the optimized configuration files for a 1.18.2 [Purpur](https://purpurmc.org) server:
+ [bukkit.yml](https://raw.githubusercontent.com/Mocab/Optimized-Minecraft-server-configurations/b531d1b99ce5f703a0aa12211bbfa468aa6d1581/1.18/bukkit.yml)
+ [spigot.yml](https://raw.githubusercontent.com/Mocab/Optimized-Minecraft-server-configurations/b531d1b99ce5f703a0aa12211bbfa468aa6d1581/1.18/spigot.yml)
+ [paper.yml](https://raw.githubusercontent.com/Mocab/Optimized-Minecraft-server-configurations/b531d1b99ce5f703a0aa12211bbfa468aa6d1581/1.18/paper.yml)
+ [purpur.yml](https://raw.githubusercontent.com/Mocab/Optimized-Minecraft-server-configurations/b531d1b99ce5f703a0aa12211bbfa468aa6d1581/1.18/purpur.yml)
+ [pufferfish.yml](https://raw.githubusercontent.com/Mocab/Optimized-Minecraft-server-configurations/b531d1b99ce5f703a0aa12211bbfa468aa6d1581/1.18/pufferfish.yml)
+ [server.properties](https://raw.githubusercontent.com/Mocab/Optimized-Minecraft-server-configurations/b531d1b99ce5f703a0aa12211bbfa468aa6d1581/1.18/server.properties)


## Usage:
Prerequisites:
+ An already set up Purpur server

Simply download the configuration files included above and upload them to your server's root/container. Alternatively you can copy the file's contents then paste them into your server's configuration files.

## Changes:
These configs slightly change certain aspects of the game, however these are usually insignificant or are not noticeable. They may still break plugins and/or farms (unlikely), so we recommend that you go through the changes made below and make any changes needed:

---------------------------------------------------------------

### [Bukkit.yml](https://github.com/Mocab/Optimized-Minecraft-server-configurations/blob/main/1.18/bukkit.yml)

**spawn-limits**

```diff
-  monsters: 70
-  animals: 10
-  water-animals: 5
-  water-ambient: 20
-  water-underground-creature: 5
-  axolotls: 5
-  ambient: 15
+  monsters: 35
+  animals: 5
+  water-animals: 3
+  water-ambient: 7
+  water-underground-creature: 3
+  axolotls: 3
+  ambient: 3
```

**ticks-per**

```diff
   animal-spawns: 400
-  monster-spawns: 1
-  water-spawns: 1
-  water-ambient-spawns: 1
-  water-underground-creature-spawns: 1
-  axolotl-spawns: 1
-  ambient-spawns: 1
+  monster-spawns: 10
+  water-spawns: 400
+  water-ambient-spawns: 400
+  water-underground-creature-spawns: 400
+  axolotl-spawns: 400
+  ambient-spawns: 400
```
---------------------------------------------------------------

### [Spigot.yml](https://github.com/Mocab/Optimized-Minecraft-server-configurations/blob/main/1.18/spigot.yml)

**save-user-cache-on-stop-only**

```diff
-  save-user-cache-on-stop-only: false
+  save-user-cache-on-stop-only: true
```

**moved-wrongly-threshold**

```diff
-  moved-wrongly-threshold: 0.0625
+  moved-wrongly-threshold: 1.0625
```

**moved-too-quickly-multiplier**

```diff
-  moved-too-quickly-multiplier: 10.0
+  moved-too-quickly-multiplier: 20.0
```

**merge-radius**

```diff
-      item: 2.5
-      exp: 3.0
+      item: 3.5
+      exp: 4.0
```

**mob-spawn-range**

```diff
-    mob-spawn-range: 8
+    mob-spawn-range: 6
```

**entity-activation-range**

```diff
-      animals: 32
-      monsters: 32
-      raiders: 48
-      misc: 16
-      water: 16
-      villagers: 32
-      flying-monsters: 32
+      animals: 28
+      monsters: 32
+      raiders: 48
+      misc: 12
+      water: 16
+      villagers: 24
+      flying-monsters: 32
```

**tick-inactive-villagers**

```diff
-      tick-inactive-villagers: true
+      tick-inactive-villagers: false
```

**max-tick-time**

```diff
-      tile: 50
-      entity: 50
+      tile: 1000
+      entity: 1000
```

-----------------------------------------------

### [Paper.yml](https://github.com/Mocab/Optimized-Minecraft-server-configurations/blob/main/1.18/paper.yml)

**keep-spawn-loaded**

```diff
-    keep-spawn-loaded: true
+    keep-spawn-loaded: false
```

**fix-climbing-bypassing-cramming-rule**

```diff
-    fix-climbing-bypassing-cramming-rule: false
+    fix-climbing-bypassing-cramming-rule: true
```

**grass-spread-tick-rate**

```diff
-    grass-spread-tick-rate: 1
+    grass-spread-tick-rate: 4
```

**use-faster-eigencraft-redstone**

```diff
-    use-faster-eigencraft-redstone: false
+    use-faster-eigencraft-redstone: true
```

**remove-corrupt-tile-entities**

```diff
-    remove-corrupt-tile-entities: false
+    remove-corrupt-tile-entities: true
```

**non-player-arrow-despawn-rate**

```diff
-    non-player-arrow-despawn-rate: -1
+    non-player-arrow-despawn-rate: 100
```

**max-auto-save-chunks-per-tick**

```diff
-    max-auto-save-chunks-per-tick: 24
+    max-auto-save-chunks-per-tick: 12
```

**optimize-explosions**

```diff
-    optimize-explosions: false
+    optimize-explosions: true
```

**prevent-moving-into-unloaded-chunks**

```diff
-    prevent-moving-into-unloaded-chunks: false
+    prevent-moving-into-unloaded-chunks: true
```

**despawn-ranges**

```diff
       monster:
         soft: 32
-        hard: 128
+        hard: 98
       creature:
         soft: 32
-        hard: 128
+        hard: 98
       ambient:
         soft: 32
-        hard: 128
+        hard: 82
       axolotls:
         soft: 32
-        hard: 128
+        hard: 98
       underground_water_creature:
         soft: 32
-        hard: 128
+        hard: 82
       water_creature:
         soft: 32
-        hard: 128
+        hard: 98
       water_ambient:
-        soft: 32
-        hard: 64
       misc:
         soft: 32
-        hard: 128
+        hard: 98
```

**update-pathfinding-on-block-update**

```diff
-    update-pathfinding-on-block-update: true
+    update-pathfinding-on-block-update: false
```

**entity-per-chunk-save-limit**

```diff
-      experience_orb: -1
-      snowball: -1
-      ender_pearl: -1
-      arrow: -1
-      fireball: -1
-      small_fireball: -1
+      experience_orb: 10
+      snowball: 5
+      ender_pearl: 5
+      arrow: 5
+      fireball: 5
+      small_fireball: 5
```

**alt-item-despawn-rate**

```diff
-      enabled: false
+      enabled: true
       items:
-        COBBLESTONE: 300
+        KELP: 600
+        BAMBOO: 600
+        CACTUS: 600
+        WHEAT_SEEDS: 600
```

----------------------------------------------------------

### [Purpur.yml](https://github.com/Mocab/Optimized-Minecraft-server-configurations/blob/main/1.18/purpur.yml)

**use-alternate-keepalive**

```diff
-  use-alternate-keepalive: false
+  use-alternate-keepalive: true
```

**can-move-in-water-over-fence**

```diff
-        can-move-in-water-over-fence: true
+        can-move-in-water-over-fence: false
```

------------------------------------------

### [Pufferfish.yml](https://github.com/Mocab/Optimized-Minecraft-server-configurations/blob/main/1.18/pufferfish.yml)

No changes have been made.

-----------------------------------------------

### [Server.properties](https://github.com/Mocab/Optimized-Minecraft-server-configurations/blob/main/1.18/server.properties)

**view-distance**

```diff
- view-distance=10
+ view-distance=8
```

**simulation-distance**

```diff
- simulation-distance=10
+ simulation-distance=6
```

----------------------------------------------------------------------

#### This guide was made based on [Paper Chan’s Little Guide to Minecraft Server Optimization!](https://eternity.community/index.php/paper-optimization/) and [Minecraft server optimization guide](https://github.com/YouHaveTrouble/minecraft-optimization), I would highly recommend going through them, they contain a lot of information which could help you.

> Do not forget to set `server-port=25565` (server.properties) to your server's port.
