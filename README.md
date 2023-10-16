# Optimized Minecraft Server Configuration Files
This folder/branch contains all the optimized configuration files for a <ins>**1.20.2**</ins> Minecraft server:
+ [bukkit.yml](https://raw.githubusercontent.com/Mocab/Optimized-configs/1.20/bukkit.yml)
+ [spigot.yml](https://raw.githubusercontent.com/Mocab/Optimized-configs/1.20/server.properties)
+ [paper-global.yml](https://raw.githubusercontent.com/Mocab/Optimized-configs/1.20/config/paper-global.yml)
+ [paper-world-defaults.yml](https://raw.githubusercontent.com/Mocab/Optimized-configs/1.20/config/paper-world-defaults.yml)
+ [purpur.yml](https://raw.githubusercontent.com/Mocab/Optimized-configs/1.20/purpur.yml)
+ [pufferfish.yml](https://raw.githubusercontent.com/Mocab/Optimized-configs/1.20/pufferfish.yml)
+ [server.properties](https://raw.githubusercontent.com/Mocab/Optimized-configs/1.20/server.properties)


## Usage:
**Prerequisites:**
+ An already set up Purpur server

> These configurations should work in any server using [Paper](https://papermc.io) or any of its forks ([Purpur](https://purpurmc.org), [Pufferfish](https://github.com/pufferfish-gg/Pufferfish), etc). However you may need to remove some of the configuration files. As an example, Paper does not need `purpur.yml` or `pufferfish.yml`.

**Installation:**

Simply download the configuration files/folders included above (Including the "config" folder) and upload them to your server's root/container.
Alternatively, you can copy the file's contents then paste them into your server's configuration file.

## Changes:
These configs slightly change certain aspects of the game, however these are usually insignificant or are not noticeable. They may still break plugins and/or farms (unlikely), so we recommend that you go through the changes and make any adjustments as seen fit:

---------------------------------------------------------------

<details>
<summary><h3>Bukkit.yml<h3></summary>
<br>

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
+  animals: 10
+  water-animals: 5
+  water-ambient: 10
+  water-underground-creature: 3
+  axolotls: 5
+  ambient: 3
```

**ticks-per**

```diff
-  animal-spawns: 400
-  monster-spawns: 1
-  water-spawns: 1
-  water-ambient-spawns: 1
-  water-underground-creature-spawns: 1
-  axolotl-spawns: 1
-  ambient-spawns: 1
+  animal-spawns: 400
+  monster-spawns: 10
+  water-spawns: 400
+  water-ambient-spawns: 400
+  water-underground-creature-spawns: 400
+  axolotl-spawns: 400
+  ambient-spawns: 400
```

</details>

---------------------------------------------------------------

<details>
<summary><h3>Spigot.yml<h3></summary>
<br>

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

</details>

-----------------------------------------------

<details>
<summary><h3>Paper-global.yml<h3></summary>
<br>

No changes have been made

</details>

-----------------------------------------------

<details>
<summary><h3>Paper-world-defaults.yml<h3></summary>
<br>

**prevent-moving-into-unloaded-chunks**

```diff
-    prevent-moving-into-unloaded-chunks: false
+    prevent-moving-into-unloaded-chunks: true
```

**entity-per-chunk-save-limit**

```diff
-    arrow: -1
-    ender_pearl: -1
-    experience_orb: -1
-    fireball: -1
-    small_fireball: -1
-    snowball: -1
+    area_effect_cloud: 8
+    arrow: 10
+    dragon_fireball: 3
+    egg: 10
+    ender_pearl: 5
+    experience_bottle: 3
+    experience_orb: 16
+    eye_of_ender: 5
+    fireball: 5
+    firework_rocket: 5
+    llama_spit: 3
+    potion: 8
+    shulker_bullet: 5
+    small_fireball: 5
+    snowball: 5
+    spectral_arrow: 10
+    trident: 10
+    wither_skull: 3
```

**max-auto-save-chunks-per-tick**

```diff
-    max-auto-save-chunks-per-tick: 24
+    max-auto-save-chunks-per-tick: 15
```

**max-entity-collisions**

```diff
-  max-entity-collisions: 8
+  max-entity-collisions: 6
```

**fix-climbing-bypassing-cramming-rule**

```diff
-    fix-climbing-bypassing-cramming-rule: false
+    fix-climbing-bypassing-cramming-rule: true
```

**armor-stands**

```diff
-    do-collision-entity-lookups: true
+    do-collision-entity-lookups: false
```

**alt-item-despawn-rate**

```diff
-      enabled: false
-      items:
-        cobblestone: 300
+      enabled: true
+      items:
+        netherrack: 600
+        sand: 600
+        red_sand: 600
+        gravel: 600
+        dirt: 600
+        grass: 600
+        pumpkin: 600
+        melon_slice: 600
+        kelp: 300
+        bamboo: 300
+        sugar_cane: 600
+        twisting_vines: 600
+        weeping_vines: 600
+        oak_leaves: 600
+        spruce_leaves: 600
+        birch_leaves: 600
+        jungle_leaves: 600
+        acacia_leaves: 600
+        dark_oak_leaves: 600
+        mangrove_leaves: 600
+        diorite: 600
+        granite: 600
+        andesite: 600
+        scaffolding: 900
+        wheat_seeds: 300
+        melon_seeds: 300
+        pumpkin_seeds: 300
+        beetroot_seeds: 300
```

**non-player-arrow-despawn-rate**

```diff
-    creative-arrow-despawn-rate: default
+    creative-arrow-despawn-rate: 60
```

**despawn-ranges**

```diff
-      ambient:
-        hard: 128
-        soft: 32
-      axolotls:
-        hard: 128
-        soft: 32
-      creature:
-        hard: 128
-        soft: 32
-      misc:
-        hard: 128
-        soft: 32
-      monster:
-        hard: 128
-        soft: 32
-      underground_water_creature:
-        hard: 128
-        soft: 32
-      water_ambient:
-        hard: 64
-        soft: 32
-      water_creature:
-        hard: 128
-        soft: 32
+      ambient:
+        hard: 82
+        soft: 32
+      axolotls:
+        hard: 98
+        soft: 32
+      creature:
+        hard: 98
+        soft: 32
+      misc:
+        hard: 98
+        soft: 32
+      monster:
+        hard: 98
+        soft: 32
+      underground_water_creature:
+        hard: 82
+        soft: 32
+      water_ambient:
+        hard: 64
+        soft: 32
+      water_creature:
+        hard: 98
+        soft: 32
```

**optimize-explosions**

```diff
-    optimize-explosions: false
+    optimize-explosions: true
```

**redstone-implementation**

```diff
-  redstone-implementation: VANILLA
+  redstone-implementation: ALTERNATE_CURRENT
```

**update-pathfinding-on-block-update**

```diff
-    update-pathfinding-on-block-update: true
+    update-pathfinding-on-block-update: false
```

**keep-spawn-loaded**

```diff
-    keep-spawn-loaded: true
+    keep-spawn-loaded: false
```

**grass-spread**

```diff
-  grass-spread: 1
+  grass-spread: 4
```

**mob-spawner**

```diff
-  mob-spawner: 1
+  mob-spawner: 2
```

**villager**

```diff
-      secondarypoisensor: 40
+      secondarypoisensor: 80
```

</details>

----------------------------------------------------------

<details>
<summary><h3>Purpur.yml<h3></summary>
<br>

**use-alternate-keepalive**

```diff
-  use-alternate-keepalive: false
+  use-alternate-keepalive: true
```

</details>

------------------------------------------

<details>
<summary><h3>Pufferfish.yml<h3></summary>
<br>

**max-loads-per-projectile**

```diff
-  max-loads-per-projectile: 10
+  max-loads-per-projectile: 8
```


</details>

-----------------------------------------------

<details>
<summary><h3>Server.properties<h3></summary>
<br>

**simulation-distance**

```diff
- simulation-distance=10
+ simulation-distance=6
```

</details>

----------------------------------------------------------------------

##### This guide was made based on [Paper Chan’s Little Guide to Minecraft Server Optimization!](https://eternity.community/index.php/paper-optimization/) and [Minecraft server optimization guide](https://github.com/YouHaveTrouble/minecraft-optimization). I would highly recommend going through them, as they contain a lot of useful information that is explained in detail.

> Do not forget to set `server-port=25565` (server.properties) to your server's port.
