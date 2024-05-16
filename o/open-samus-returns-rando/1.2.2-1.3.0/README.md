# Comparing `tmp/open_samus_returns_rando-1.2.2.tar.gz` & `tmp/open_samus_returns_rando-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_samus_returns_rando-1.2.2.tar", last modified: Tue Apr 30 00:40:27 2024, max compression
+gzip compressed data, was "open_samus_returns_rando-1.3.0.tar", last modified: Wed May 15 21:30:01 2024, max compression
```

## Comparing `open_samus_returns_rando-1.2.2.tar` & `open_samus_returns_rando-1.3.0.tar`

### file list

```diff
@@ -1,140 +1,178 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:40:27.516875 open_samus_returns_rando-1.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:40:27.496875 open_samus_returns_rando-1.2.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:40:27.496875 open_samus_returns_rando-1.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/.github/workflows/python.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-30 00:40:27.516875 open_samus_returns_rando-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 00:40:27.516875 open_samus_returns_rando-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:40:27.492875 open_samus_returns_rando-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:40:27.500875 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:40:27.500875 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/__pyinstaller/hook-open_samus_returns_rando.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:40:27.500875 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:40:27.500875 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/custom/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/custom/doors.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/custom/guilib.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/custom/heatzone.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/custom/room_names.lua
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/custom/savestation.lua
--rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/custom/scenario.lua
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/custom/ship.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/custom/sprites_splashes.lua
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:40:27.504875 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/
--rw-r--r--   0 runner    (1001) docker     (127)    26259 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s000_surface.lua
--rw-r--r--   0 runner    (1001) docker     (127)    31259 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s010_area1.lua
--rw-r--r--   0 runner    (1001) docker     (127)    29548 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s020_area2.lua
--rw-r--r--   0 runner    (1001) docker     (127)    15959 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s025_area2b.lua
--rw-r--r--   0 runner    (1001) docker     (127)    13250 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s028_area2c.lua
--rw-r--r--   0 runner    (1001) docker     (127)    27509 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s030_area3.lua
--rw-r--r--   0 runner    (1001) docker     (127)    40894 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s033_area3b.lua
--rw-r--r--   0 runner    (1001) docker     (127)    23245 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s036_area3c.lua
--rw-r--r--   0 runner    (1001) docker     (127)    30051 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s040_area4.lua
--rw-r--r--   0 runner    (1001) docker     (127)    34925 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s050_area5.lua
--rw-r--r--   0 runner    (1001) docker     (127)    15897 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s060_area6.lua
--rw-r--r--   0 runner    (1001) docker     (127)    18453 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s065_area6b.lua
--rw-r--r--   0 runner    (1001) docker     (127)    18231 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s067_area6c.lua
--rw-r--r--   0 runner    (1001) docker     (127)    41935 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s070_area7.lua
--rw-r--r--   0 runner    (1001) docker     (127)    23599 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s090_area9.lua
--rw-r--r--   0 runner    (1001) docker     (127)    39148 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s100_area10.lua
--rw-r--r--   0 runner    (1001) docker     (127)    26016 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s110_surfaceb.lua
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:40:27.508875 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/pickups/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/pickups/randomizerbabyhatchling.lua
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/pickups/randomizerenergyshield.lua
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/pickups/randomizerenergytank.lua
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/pickups/randomizerenergywave.lua
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/pickups/randomizermissilelauncher.lua
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/pickups/randomizermissiletank.lua
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/pickups/randomizerphasedisplacement.lua
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/pickups/randomizerpowerbomb.lua
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/pickups/randomizerpowerbombtank.lua
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/pickups/randomizerreservetanka.lua
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/pickups/randomizerreservetanke.lua
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/pickups/randomizerreservetankm.lua
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/pickups/randomizerscanningpulse.lua
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/pickups/randomizersuit.lua
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/pickups/randomizersupermissile.lua
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/pickups/randomizersupermissiletank.lua
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:40:27.496875 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/romfs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:40:27.492875 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/romfs/actors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:40:27.492875 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/romfs/actors/items/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:40:27.492875 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:40:27.508875 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/
--rw-r--r--   0 runner    (1001) docker     (127)    13308 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/powerup_missilelauncher.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:40:27.508875 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/textures/
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/textures/missile_e.bctex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:40:27.492875 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/romfs/actors/props/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:40:27.492875 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:40:27.496875 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:40:27.508875 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/
--rw-r--r--   0 runner    (1001) docker     (127)    43927 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/chozodnareceivergold_d.bctex
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/dna_d.bctex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:40:27.496875 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/romfs/gui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:40:27.508875 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/romfs/gui/textures/
--rw-r--r--   0 runner    (1001) docker     (127)   524553 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/romfs/gui/textures/gamelogo.bctex
--rw-r--r--   0 runner    (1001) docker     (127)    22654 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:40:27.508875 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/templates/cc_to_room_name.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/templates/chozoseal_template.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/templates/cosmetics.lua
--rw-r--r--   0 runner    (1001) docker     (127)     5268 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/templates/custom_init.lua
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/templates/elevators.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/templates/metroid_template.lua
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/templates/progressive_model_template.lua
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/templates/randomizer_item_template.lua
--rw-r--r--   0 runner    (1001) docker     (127)     6150 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/templates/randomizerpowerup.lua
--rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/templates/template_powerup_bmsad.json
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    15823 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/lua_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:40:27.512875 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/misc_patches/
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/misc_patches/collision_camera_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/misc_patches/credits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/misc_patches/elevators.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/misc_patches/exefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/misc_patches/lua_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/misc_patches/spawn_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/misc_patches/text_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/patch_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/patcher_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:40:27.512875 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/pickups/
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/pickups/custom_pickups.py
--rw-r--r--   0 runner    (1001) docker     (127)    13953 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/pickups/model_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    16072 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/pickups/pickup.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/samus_returns_patcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:40:27.512875 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/specific_patches/
--rw-r--r--   0 runner    (1001) docker     (127)     7328 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/specific_patches/chozo_seal_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/specific_patches/cosmetic_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)    20266 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/specific_patches/door_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/specific_patches/game_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     9260 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/specific_patches/heat_room_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/specific_patches/hint_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/specific_patches/map_icons.py
--rw-r--r--   0 runner    (1001) docker     (127)    12026 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/specific_patches/metroid_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)    12168 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/specific_patches/static_fixes.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/specific_patches/tunable_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/validator_with_default.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 00:40:27.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:40:27.516875 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-30 00:40:27.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-04-30 00:40:27.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 00:40:27.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-30 00:40:27.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-30 00:40:27.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 00:40:27.000000 open_samus_returns_rando-1.2.2/src/open_samus_returns_rando.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:40:27.512875 open_samus_returns_rando-1.2.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:40:27.512875 open_samus_returns_rando-1.2.2/tests/test_files/
--rw-r--r--   0 runner    (1001) docker     (127)    49806 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/tests/test_files/item_models_test.json
--rw-r--r--   0 runner    (1001) docker     (127)   147194 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/tests/test_files/starter_preset_patcher.json
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-30 00:40:17.000000 open_samus_returns_rando-1.2.2/tests/test_lua_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.084432 open_samus_returns_rando-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.056432 open_samus_returns_rando-1.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.056432 open_samus_returns_rando-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/.github/workflows/python.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-15 21:30:01.084432 open_samus_returns_rando-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 21:30:01.084432 open_samus_returns_rando-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.052432 open_samus_returns_rando-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.060432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.060432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/__pyinstaller/hook-open_samus_returns_rando.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.060432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.064432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/custom/doors.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/custom/guilib.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/custom/heatzone.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/custom/room_names.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/custom/savestation.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/custom/scenario.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/custom/ship.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/custom/sprites_splashes.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/custom/sprites_texturehud.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.068432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/
+-rw-r--r--   0 runner    (1001) docker     (127)    26259 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s000_surface.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    31259 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s010_area1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    29548 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s020_area2.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    15959 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s025_area2b.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    13250 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s028_area2c.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    27509 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s030_area3.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    40894 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s033_area3b.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    23245 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s036_area3c.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    30051 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s040_area4.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    34925 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s050_area5.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    15897 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s060_area6.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    18453 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s065_area6b.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    18231 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s067_area6c.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    41935 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s070_area7.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    23599 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s090_area9.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    39148 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s100_area10.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    26016 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s110_surfaceb.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.072432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/pickups/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/pickups/randomizerbabyhatchling.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/pickups/randomizerenergyshield.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/pickups/randomizerenergytank.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/pickups/randomizerenergywave.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/pickups/randomizermissilelauncher.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/pickups/randomizermissiletank.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/pickups/randomizerphasedisplacement.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/pickups/randomizerpowerbomb.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/pickups/randomizerpowerbombtank.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/pickups/randomizerreservetanka.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/pickups/randomizerreservetanke.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/pickups/randomizerreservetankm.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/pickups/randomizerscanningpulse.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/pickups/randomizersuit.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/pickups/randomizersupermissile.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/pickups/randomizersupermissiletank.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.056432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.052432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.052432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/items/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.052432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/items/item_offworld/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.072432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/items/item_offworld/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    23772 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/items/item_offworld/models/item_offworld.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.052432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_icemissile/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.072432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_icemissile/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    13308 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_icemissile/models/powerup_icemissile.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.072432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_icemissile/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_icemissile/models/textures/missile_d.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.052432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.072432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    13308 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/powerup_missilelauncher.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.072432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/textures/missile_e.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.056432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.052432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.052432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.072432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)    43927 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/chozodnareceivergold_d.bctex
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/dna_d.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.052432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbeamburst/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.072432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbeamburst/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbeamburst/models/doorshieldbeamburst.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.072432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbeamburst/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)    11157 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbeamburst/models/textures/doorshieldbeamburst_d.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.052432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbomb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.072432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbomb/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    14360 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbomb/models/doorshieldbomb.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.072432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbomb/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)    22169 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbomb/models/textures/doorshieldbomb_d.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.052432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldgrapplebeam/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.072432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldgrapplebeam/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldgrapplebeam/models/doorshieldgrapplebeam.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.072432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldgrapplebeam/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldgrapplebeam/models/textures/doorgrapple_d.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.056432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldicebeam/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.072432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldicebeam/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    50240 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldicebeam/models/doorshieldicebeam.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.072432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldicebeam/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)    11151 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldicebeam/models/textures/doorcreature_i.bctex
+-rw-r--r--   0 runner    (1001) docker     (127)    11148 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldicebeam/models/textures/spiderweb_i.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.056432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldlocked/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.076432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldlocked/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    47188 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldlocked/models/doorshieldlocked.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.076432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldlocked/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldlocked/models/textures/doorshieldlocked_d.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.056432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/gui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.076432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/gui/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)   524553 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/gui/textures/gamelogo.bctex
+-rw-r--r--   0 runner    (1001) docker     (127)   524555 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/gui/textures/texturehud.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.056432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/maps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.076432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/maps/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)    11140 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/maps/textures/chozoartifactor_o.bctex
+-rw-r--r--   0 runner    (1001) docker     (127)    22930 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.080432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/templates/cc_to_room_name.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/templates/chozoseal_template.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/templates/cosmetics.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     5268 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/templates/custom_init.lua
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/templates/elevators.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/templates/metroid_template.lua
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/templates/progressive_model_template.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/templates/randomizer_item_template.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     6150 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/templates/randomizerpowerup.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/templates/template_powerup_bmsad.json
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16138 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/lua_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.080432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/misc_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/misc_patches/collision_camera_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/misc_patches/credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/misc_patches/elevators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/misc_patches/lua_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/misc_patches/spawn_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/misc_patches/text_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/patch_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/patcher_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.080432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/pickups/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/pickups/custom_pickups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14546 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/pickups/model_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16174 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/pickups/pickup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/samus_returns_patcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.084432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/specific_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/specific_patches/chozo_seal_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/specific_patches/cosmetic_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25146 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/specific_patches/door_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/specific_patches/game_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/specific_patches/heat_room_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/specific_patches/hint_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/specific_patches/map_icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/specific_patches/metroid_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12343 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/specific_patches/static_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/specific_patches/tunable_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/validator_with_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-15 21:30:00.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.084432 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-15 21:30:01.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7841 2024-05-15 21:30:01.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 21:30:01.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-15 21:30:01.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-15 21:30:01.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-15 21:30:01.000000 open_samus_returns_rando-1.3.0/src/open_samus_returns_rando.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.084432 open_samus_returns_rando-1.3.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:30:01.084432 open_samus_returns_rando-1.3.0/tests/test_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    51547 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/tests/test_files/item_models_test.json
+-rw-r--r--   0 runner    (1001) docker     (127)   147194 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/tests/test_files/starter_preset_patcher.json
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-15 21:29:52.000000 open_samus_returns_rando-1.3.0/tests/test_lua_util.py
```

### Comparing `open_samus_returns_rando-1.2.2/.github/dependabot.yml` & `open_samus_returns_rando-1.3.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/.github/workflows/python.yml` & `open_samus_returns_rando-1.3.0/.github/workflows/python.yml`

 * *Files 20% similar despite different names*

```diff
@@ -99,14 +99,54 @@
       - name: Install
         run: venv/bin/python -m pip install -e .
 
       - name: Export
         run:
           venv/bin/python -m open_samus_returns_rando --input-path "$SAMUS_RETURNS_PATH" --output-path export/ --input-json tests/test_files/starter_preset_patcher.json
 
+  mypy:
+    runs-on: 'ubuntu-latest'
+
+    steps:
+      - name: Checkout
+        uses: actions/checkout@v4
+        with:
+          fetch-depth: 0
+
+      - name: Workaround for worktree config
+        run: git config --unset-all extensions.worktreeConfig || true
+
+      - name: Set up Python
+        uses: actions/setup-python@v5
+        with:
+          python-version: "3.12"
+          cache: "pip"
+
+      - name: Install Python packages
+        run: python -m pip install .[typing]
+
+      - name: Mypy on modified files
+        uses: tsuyoshicho/action-mypy@v4
+        with:
+          github_token: ${{ secrets.github_token }}
+          # Change reviewdog reporter if you need [github-pr-check,github-check,github-pr-review].
+          reporter: github-check
+          setup_method: install
+          fail_on_error: false
+
+      - name: Mypy on required files
+        uses: tsuyoshicho/action-mypy@v4
+        with:
+          github_token: ${{ secrets.github_token }}
+          # Change reviewdog reporter if you need [github-pr-check,github-check,github-pr-review].
+          reporter: github-check
+          setup_method: install
+          target: --config-file=pyproject.toml
+          fail_on_error: true
+
 
   pypi:
     runs-on: 'ubuntu-latest'
     needs:
       - test
       - starter_preset_patcher
```

### Comparing `open_samus_returns_rando-1.2.2/.gitignore` & `open_samus_returns_rando-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/LICENSE` & `open_samus_returns_rando-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/PKG-INFO` & `open_samus_returns_rando-1.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 Metadata-Version: 2.1
 Name: open_samus_returns_rando
-Version: 1.2.2
+Version: 1.3.0
 Summary: An open source randomizer patcher for Metroid: Samus Returns.
 Project-URL: Homepage, https://github.com/randovania/open-samus-returns-rando
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mercury-engine-data-structures>=0.27.0
 Requires-Dist: jsonschema>=4.0.0
 Requires-Dist: ips.py>=0.1.2
+Provides-Extra: typing
+Requires-Dist: types-jsonschema; extra == "typing"
+Requires-Dist: construct-typing; extra == "typing"
+Requires-Dist: types-pyinstaller; extra == "typing"
+Requires-Dist: mypy; extra == "typing"
 
 # Open Samus Returns Rando
 Open Source randomizer patcher for Metroid: Samus Returns. Intended for use in [Randovania](https://github.com/randovania).
 Currently supports patching the following:
-- Starting items
-- Starting location
-- Pickups
+- Starting Items
+- Starting Location
+- Pickups (Vanilla and Custom)
 - Items on Metroids
-- Shuffled DNA/Baby Metroid
+- Shuffled DNA
+- Shuffled Baby Metroid
+- Elevator Destinations
+- Door Types
 
 ## Installation and Usage
 `pip install open-samus-returns-rando`
 
 You will need to provide JSON data matching the [JSON schema](https://github.com/randovania/open-samus-returns-rando/blob/main/src/open_samus_returns_rando/files/schema.json) in order to successfully patch the game.
 
 The patcher expects a path to an extracted romfs directory of Metroid: Samus Returns as well as the desired output directory. Output files are in a format compatible with either Luma3DS or Citra.
```

### Comparing `open_samus_returns_rando-1.2.2/README.md` & `open_samus_returns_rando-1.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # Open Samus Returns Rando
 Open Source randomizer patcher for Metroid: Samus Returns. Intended for use in [Randovania](https://github.com/randovania).
 Currently supports patching the following:
-- Starting items
-- Starting location
-- Pickups
+- Starting Items
+- Starting Location
+- Pickups (Vanilla and Custom)
 - Items on Metroids
-- Shuffled DNA/Baby Metroid
+- Shuffled DNA
+- Shuffled Baby Metroid
+- Elevator Destinations
+- Door Types
 
 ## Installation and Usage
 `pip install open-samus-returns-rando`
 
 You will need to provide JSON data matching the [JSON schema](https://github.com/randovania/open-samus-returns-rando/blob/main/src/open_samus_returns_rando/files/schema.json) in order to successfully patch the game.
 
 The patcher expects a path to an extracted romfs directory of Metroid: Samus Returns as well as the desired output directory. Output files are in a format compatible with either Luma3DS or Citra.
```

### Comparing `open_samus_returns_rando-1.2.2/pyproject.toml` & `open_samus_returns_rando-1.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -61,7 +61,23 @@
 # Version to target for generated code.
 target-version = "py39"
 
 [tool.ruff.lint.mccabe]
 # Flag errors (`C901`) whenever the complexity level exceeds 25.
 # Defaults to 10, but we're being very flexible right now
 max-complexity = 25
+
+[project.optional-dependencies]
+typing = [
+    "types-jsonschema",
+    "construct-typing",
+    "types-pyinstaller",
+    "mypy"
+]
+
+[tool.mypy]
+files = [
+    "src/"
+]
+follow_imports = "silent"
+disallow_untyped_defs = true
+local_partial_types = true
```

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/cli.py` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 import logging
 import logging.config
 from pathlib import Path
 
 from open_samus_returns_rando import samus_returns_patcher
 
 
-def create_parser():
+def create_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser()
     parser.add_argument("--input-path", required=True, type=Path,
                         help="Path to where the extracted Metroid: Samus Returns romfs to randomize can be found.")
     parser.add_argument("--output-path", required=True, type=Path,
                         help="Path to where the modified files will be written to.")
     parser.add_argument("--input-json", type=Path,
                         help="Path to the configuration json. If missing, it's read from standard input")
     return parser
 
 
-def setup_logging():
+def setup_logging() -> None:
     handlers = {
         'default': {
             'level': 'DEBUG',
             'formatter': 'default',
             'class': 'logging.StreamHandler',
             'stream': 'ext://sys.stdout',  # Default is stderr
         },
@@ -45,15 +45,15 @@
             'level': 'DEBUG',
             'handlers': list(handlers.keys()),
         },
     })
     logging.info("Hello world.")
 
 
-def main():
+def main() -> None:
     setup_logging()
     parser = create_parser()
     args = parser.parse_args()
     print(args)
 
     with args.input_json.open() as f:
         configuration = json.load(f)
```

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/constants.py` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     "s067_area6c",
     "s070_area7",
     "s090_area9",
     "s100_area10",
     "s110_surfaceb",
 ]
 
-def get_package_name(package_name: str, file_name: str):
+def get_package_name(package_name: str, file_name: str) -> str:
     without = ["bcmdl", "bcwav", "bctex", "bcskla", "bcptl"]
     for ending in without:
         if file_name.endswith(ending):
             return package_name.replace("_discardables", "")
     return package_name
 
-def lua_pkgs(pkgs: list[str]):
+def lua_pkgs(pkgs: list[str]) -> list[str]:
     return [get_package_name(level_pkg, "lc") for level_pkg in pkgs]
```

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/debug.py` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/debug.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from open_samus_returns_rando.patcher_editor import PatcherEditor
 
 
-def unpack_new_actor(new_actor: dict):
+def unpack_new_actor(new_actor: dict) -> tuple[str, str, str, list[float]]:
     scenario_name = new_actor["new_actor"]["scenario"]
     new_actor_name = new_actor["new_actor"]["actor"]
     collision_camera_name = new_actor["collision_camera_name"]
-    new_pos = (new_actor["location"]["x"], new_actor["location"]["y"], new_actor["location"]["z"])
+    new_pos = [new_actor["location"]["x"], new_actor["location"]["y"], new_actor["location"]["z"]]
     return scenario_name,new_actor_name,collision_camera_name,new_pos
 
 
-def debug_spawn_points(editor: PatcherEditor, spawn_config: list[dict]):
+def debug_spawn_points(editor: PatcherEditor, spawn_config: list[dict]) -> None:
     # create custom spawn point
     _EXAMPLE_SP = {"scenario": "s010_area1", "layer": "5", "actor": "StartPoint0"}
     base_actor = editor.resolve_actor_reference(_EXAMPLE_SP)
     for new_spawn in spawn_config:
         scenario_name, new_actor_name, collision_camera_name, new_spawn_pos = unpack_new_actor(new_spawn)
         scenario = editor.get_scenario(scenario_name)
         editor.copy_actor(scenario_name, new_spawn_pos, base_actor, new_actor_name, 5)
         scenario.add_actor_to_entity_groups(collision_camera_name, new_actor_name)
 
 
-def debug_custom_pickups(editor: PatcherEditor, pickup_config: list[dict]):
+def debug_custom_pickups(editor: PatcherEditor, pickup_config: list[dict]) -> None:
     # create custom pickup
     _EXAMPLE_PICKUP = {"scenario": "s000_surface", "layer": "9", "actor": "LE_PowerUP_Morphball"}
     base_actor = editor.resolve_actor_reference(_EXAMPLE_PICKUP)
     for new_pickup in pickup_config:
         scenario_name, new_actor_name, collision_camera_name, new_pos = unpack_new_actor(new_pickup)
         scenario = editor.get_scenario(scenario_name)
         editor.copy_actor(scenario_name, new_pos, base_actor, new_actor_name, 9)
```

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/custom/doors.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/custom/doors.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/custom/guilib.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/custom/guilib.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/custom/heatzone.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/custom/heatzone.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/custom/room_names.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/custom/room_names.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/custom/savestation.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/custom/savestation.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/custom/scenario.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/custom/scenario.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/custom/ship.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/custom/ship.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/custom/sprites_splashes.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/custom/sprites_splashes.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s000_surface.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s000_surface.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s010_area1.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s010_area1.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s020_area2.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s020_area2.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s025_area2b.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s025_area2b.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s028_area2c.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s028_area2c.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s030_area3.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s030_area3.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s033_area3b.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s033_area3b.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s036_area3c.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s036_area3c.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s040_area4.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s040_area4.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s050_area5.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s050_area5.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s060_area6.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s060_area6.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s065_area6b.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s065_area6b.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s067_area6c.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s067_area6c.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s070_area7.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s070_area7.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s090_area9.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s090_area9.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s100_area10.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s100_area10.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/levels/s110_surfaceb.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/levels/s110_surfaceb.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/pickups/randomizerenergytank.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/pickups/randomizerenergytank.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/pickups/randomizermissilelauncher.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/pickups/randomizermissilelauncher.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/pickups/randomizermissiletank.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/pickups/randomizermissiletank.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/pickups/randomizerpowerbomb.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/pickups/randomizerpowerbomb.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/pickups/randomizerpowerbombtank.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/pickups/randomizerpowerbombtank.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/pickups/randomizerreservetanka.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/pickups/randomizerreservetanka.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/pickups/randomizerreservetanke.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/pickups/randomizerreservetanke.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/pickups/randomizersuit.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/pickups/randomizersuit.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/pickups/randomizersupermissile.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/pickups/randomizersupermissile.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/pickups/randomizersupermissiletank.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/pickups/randomizersupermissiletank.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/powerup_missilelauncher.bcmdl` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/powerup_missilelauncher.bcmdl`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/textures/missile_e.bctex` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/textures/missile_e.bctex`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/chozodnareceivergold_d.bctex` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/chozodnareceivergold_d.bctex`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/dna_d.bctex` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/dna_d.bctex`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/romfs/gui/textures/gamelogo.bctex` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/romfs/gui/textures/gamelogo.bctex`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/schema.json` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/schema.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999543313419117%*

 * *Differences: {"'$defs'": "{'item_id': {'enum': {insert: [(78, 'ITEM_OFFWORLD'), (79, "*

 * *            "'ITEM_WEAPON_ICE_MISSILE')]}}}",*

 * * "'properties'": "{'door_patches': {'items': {'properties': {'door_type': {'enum': {insert: [(9, "*

 * *                 "'ice_beam'), (10, 'grapple_beam'), (11, 'bomb'), (12, 'beam_burst'), (13, "*

 * *                 "'locked')]}}}}}}"}*

```diff
@@ -119,15 +119,17 @@
                 "ITEM_RANDO_DNA_35",
                 "ITEM_RANDO_DNA_36",
                 "ITEM_RANDO_DNA_37",
                 "ITEM_RANDO_DNA_38",
                 "ITEM_RANDO_DNA_39",
                 "ITEM_RESERVE_TANK_LIFE",
                 "ITEM_RESERVE_TANK_MISSILE",
-                "ITEM_RESERVE_TANK_SPECIAL_ENERGY"
+                "ITEM_RESERVE_TANK_SPECIAL_ENERGY",
+                "ITEM_OFFWORLD",
+                "ITEM_WEAPON_ICE_MISSILE"
             ],
             "type": "string"
         },
         "metroid_callback": {
             "properties": {
                 "scenario": {
                     "$ref": "#/$defs/scenario_name"
@@ -350,15 +352,20 @@
                             "power_beam",
                             "charge_beam",
                             "spazer_beam",
                             "plasma_beam",
                             "wave_beam",
                             "missile",
                             "super_missile",
-                            "power_bomb"
+                            "power_bomb",
+                            "ice_beam",
+                            "grapple_beam",
+                            "bomb",
+                            "beam_burst",
+                            "locked"
                         ],
                         "type": "string"
                     }
                 },
                 "required": [
                     "actor",
                     "door_type"
```

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/templates/chozoseal_template.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/templates/chozoseal_template.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/templates/cosmetics.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/templates/cosmetics.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/templates/custom_init.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/templates/custom_init.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/templates/metroid_template.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/templates/metroid_template.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/templates/randomizer_item_template.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/templates/randomizer_item_template.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/templates/randomizerpowerup.lua` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/templates/randomizerpowerup.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/files/templates/template_powerup_bmsad.json` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/files/templates/template_powerup_bmsad.json`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/lua_editor.py` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/lua_editor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import itertools
+from collections.abc import Iterable
 
 from construct import Container
 from mercury_engine_data_structures.formats.lua import Lua
 
 from open_samus_returns_rando.constants import ALL_SCENARIOS
 from open_samus_returns_rando.files import files_path
 from open_samus_returns_rando.misc_patches import lua_util
@@ -101,30 +102,30 @@
         parent_file_name = self.get_lua_parent_file_name()
         if not editor.does_asset_exists(parent_file_name):
             parent_content = files_path().joinpath("pickups", f"{self.lua_parent.lower()}.lua").read_text()
             editor.add_new_asset(parent_file_name, Lua(Container(lua_text=parent_content), editor.target_game), [])
 
 
 class LuaEditor:
-    def __init__(self):
-        self._item_classes = {}
-        self._metroid_dict = {}
-        self._dna_count_dict = {}
-        self._hint_dict = {}
+    def __init__(self) -> None:
+        self._item_classes: dict[str, ScriptClass] = {}
+        self._metroid_dict: dict[str, dict[str, str]] = {}
+        self._dna_count_dict: dict[str, int] = {}
+        self._hint_dict: dict[str, dict[str, list[str]]] = {}
         self._progressive_models = ""
         self._custom_level_scripts: dict[str, dict] = self._read_levels()
-        self._metroid_imports = []
+        self._metroid_imports: list[str] = []
 
     def _read_levels(self) -> dict[str, dict]:
         return {
             scenario: {"script": _read_level_lua(scenario), "edited": False}
             for scenario in ALL_SCENARIOS
         }
 
-    def get_parent_for(self, item_id) -> str:
+    def get_parent_for(self, item_id: str) -> str:
         return SPECIFIC_CLASSES.get(item_id, "RandomizerPowerup")
 
     def create_script_class(self, pickup: dict, actordef_id: str = "") -> ScriptClass:
         pickup_resources = pickup["resources"]
         first_item_id = pickup_resources[0][0]["item_id"]
         parent = self.get_parent_for(first_item_id)
         model_array = pickup.get("model", None)
@@ -170,15 +171,15 @@
 
         lua_content = lua_util.replace_lua_template("randomizer_item_template.lua", replacement)
         new_script_class = ScriptClass(class_name, actordef_id, lua_content, parent)
         self._item_classes[hashable_progression] = new_script_class
 
         return new_script_class
 
-    def add_progressive_models(self, pickup: dict, actordef_name: str):
+    def add_progressive_models(self, pickup: dict, actordef_name: str) -> None:
         progressive_models = [
             {
                 "item": lua_util.wrap_string(resource["item_id"]),
                 "alias": lua_util.wrap_string(model_name),
             }
             for resource, model_name in itertools.chain(
                 zip([r[0] for r in pickup["resources"]], pickup["model"][0:])
@@ -229,15 +230,15 @@
             "ITEM_METROID_COUNT": 0,
             "ITEM_METROID_TOTAL_COUNT": 40,
             "ITEM_MISSILE_CHECK": max(1, inventory.get("ITEM_WEAPON_MISSILE_MAX", 0)),
         }
         final_inventory.update(inventory)
 
         # Use itertools batched when upgrading to python 3.12
-        def chunks(array: list[str], n: int):
+        def chunks(array: list[str], n: int) -> Iterable[list[str]]:
             for i in range(0, len(array), n):
                 yield array[i:i + n]
 
         textboxes = 0
         boxes = chunks(starting_text, 3)
         for box in boxes:
             textboxes += 1
@@ -256,15 +257,15 @@
             "textbox_count": textboxes,
             "configuration_identifier": lua_util.wrap_string(configuration_identifier),
             "enable_room_ids": False if cosmetic_options["enable_room_name_display"] == "NEVER" else True,
         }
 
         return lua_util.replace_lua_template("custom_init.lua", replacement)
 
-    def _add_replacement_files(self, editor: PatcherEditor, configuration: dict):
+    def _add_replacement_files(self, editor: PatcherEditor, configuration: dict) -> None:
         # Update init.lc
         lua_util.create_script_copy(editor, "system/scripts/init")
 
         init_script = self._create_custom_init(editor, configuration)
         editor.replace_asset(
             "system/scripts/init.lc",
             Lua(Container(lua_text=init_script), editor.target_game)
@@ -275,16 +276,17 @@
         scenario_lua_content += "\n" + self._progressive_models
         lua_util.replace_script_with_content(editor, "system/scripts/scenario", scenario_lua_content)
 
         lua_util.replace_script(editor, "actors/props/samusship/scripts/samusship", "custom/ship.lua")
         lua_util.replace_script(editor, "actors/props/savestation/scripts/savestation", "custom/savestation.lua")
         lua_util.replace_script(editor, "actors/props/heatzone/scripts/heatzone", "custom/heatzone.lua")
         lua_util.replace_script(editor, "gui/scripts/sprites_splashes", "custom/sprites_splashes.lua")
+        lua_util.replace_script(editor, "gui/scripts/sprites_texturehud", "custom/sprites_texturehud.lua")
 
-    def save_modifications(self, editor: PatcherEditor, configuration: dict):
+    def save_modifications(self, editor: PatcherEditor, configuration: dict) -> None:
         self._add_replacement_files(editor, configuration)
 
         # add new system scripts
         editor.add_new_asset(
             "system/scripts/guilib.lc",
             Lua(Container(lua_text=files_path().joinpath("custom", "guilib.lua").read_text()), editor.target_game),
             []
```

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/misc_patches/collision_camera_table.py` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/misc_patches/collision_camera_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from construct import Container
 from mercury_engine_data_structures.formats.lua import Lua
 from open_samus_returns_rando.misc_patches import lua_util
 from open_samus_returns_rando.patcher_editor import PatcherEditor
 
 
-def create_collision_camera_table(editor: PatcherEditor, configuration: dict):
+def create_collision_camera_table(editor: PatcherEditor, configuration: dict) -> None:
     py_dict: dict = configuration["cosmetic_patches"]["camera_names_dict"]
 
     # Surface
     py_dict["s000_surface"]["collision_camera_017"] = "Transport to Area 8"
     py_dict["s110_surfaceb"]["collision_camera_018"] = "Surface Stash"
     py_dict["s110_surfaceb"]["collision_camera_019"] = "Surface Crumble Block Challenge"
     py_dict["s110_surfaceb"]["collision_camera_021"] = "Landing Site"
```

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/misc_patches/credits.py` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/misc_patches/credits.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         "Haxaplax",
     ],
     "     ": [
         "With contributions from many others.",
     ]
 }
 
-def _create_randomizer_credits(spoiler_log: dict[str, str]):
+def _create_randomizer_credits(spoiler_log: dict[str, str])  -> tuple[list[tuple[str, str]], int, int, int]:
     rando_credits: list[tuple[str, str]] = [
         ("Randomizer Credits", "CREDIT_TITLE"),
     ]
 
     for group, group_members in _PROJECT_MEMBERS.items():
         rando_credits.append((group, "CREDIT_SUBTITLE"))
         for member in group_members:
@@ -42,15 +42,15 @@
 
     rando_credits.append(("     ", "CREDIT_SUBTITLE"))
 
     amount_title = 0
     amount_subtitle = 0
     amount_credit = 0
 
-    def new_sort(prefix: str, item) -> tuple[str, str]:
+    def new_sort(prefix: str, item: str) -> tuple[str, str]:
         nonlocal amount_title
         nonlocal amount_subtitle
         nonlocal amount_credit
         if prefix.startswith("CREDIT_TITLE"):
             amount_title = amount_title + 1
             return (f"{prefix}{amount_title}", item)
         elif prefix.startswith("CREDIT_SUBTITLE"):
@@ -63,15 +63,15 @@
     rando_credits = [
         new_sort(prefix, item)
         for item, prefix in rando_credits
     ]
     return rando_credits, amount_title, amount_subtitle, amount_credit
 
 
-def patch_credits(editor: PatcherEditor, spoiler_log: dict[str, str]):
+def patch_credits(editor: PatcherEditor, spoiler_log: dict[str, str]) -> None:
     english_files = [
         "system/localization/mse_english.txt",
     ]
 
     rando_credits, amount_title, amount_subtitle, amount_credit  = _create_randomizer_credits(spoiler_log)
 
     for file in english_files:
```

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/misc_patches/elevators.py` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/misc_patches/elevators.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from construct import Container
 from mercury_engine_data_structures.formats.lua import Lua
 from open_samus_returns_rando.misc_patches import lua_util
 from open_samus_returns_rando.patcher_editor import PatcherEditor
 
 
-def create_elevator_table(editor: PatcherEditor, configuration: dict):
+def create_elevator_table(editor: PatcherEditor, configuration: dict) -> None:
     py_dict: dict = configuration["elevators"]
 
     file = lua_util.replace_lua_template("elevators.lua", {"elevator_dict": py_dict}, True)
     editor.add_new_asset(
         "system/scripts/elevators.lc",
         Lua(Container(lua_text=file), editor.target_game),
         []
     )
 
 
-def update_elevators(editor: PatcherEditor, configuration: dict):
+def update_elevators(editor: PatcherEditor, configuration: dict) -> None:
     for scenario_name, elevators in configuration["elevators"].items():
         scenario = editor.get_scenario(scenario_name)
         for elevator in elevators:
             platform = scenario.raw.actors[10][elevator]["components"][0]
             platform["arguments"][1]["value"] = "Scenario.RandoOnElevatorUse"
 
 
-def patch_elevators(editor: PatcherEditor, configuration: dict):
+def patch_elevators(editor: PatcherEditor, configuration: dict) -> None:
     create_elevator_table(editor, configuration)
     update_elevators(editor, configuration)
```

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/misc_patches/lua_util.py` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/misc_patches/lua_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import re
+import typing
 
 from construct import Container
 from mercury_engine_data_structures.file_tree_editor import FileTreeEditor
 from mercury_engine_data_structures.formats.lua import Lua
 from open_samus_returns_rando.files import files_path, templates_path
 
 
-def replace_lua_template(file: str, replacement: dict[str, str], wrap_strings: bool = False) -> str:
+def replace_lua_template(file: str, replacement: dict[str, typing.Any], wrap_strings: bool = False) -> str:
     code = templates_path().joinpath(file).read_text()
     for key, content in replacement.items():
         # Replace `TEMPLATE("key")`-style replacements
         code = code.replace(f'TEMPLATE("{key}")', lua_convert(content, wrap_strings))
         # Replace `T__key__T`-style replacements
         code = code.replace(f'T__{key}__T', lua_convert(content, wrap_strings))
 
@@ -19,15 +20,15 @@
 
     if unknown_templates:
         raise ValueError("The following templates were left unfulfilled: " + str(unknown_templates))
 
     return code
 
 
-def lua_convert(data, wrap_strings: bool = False) -> str:
+def lua_convert(data: typing.Any, wrap_strings: bool = False) -> str:
     if isinstance(data, list):
         return "{\n" + "\n".join(
             f"{lua_convert(item, wrap_strings)},"
             for item in data
         ) + "\n}"
     if isinstance(data, dict):
         return "{\n" + "\n".join(
@@ -42,29 +43,29 @@
         return wrap_string(data)
     return str(data)
 
 def wrap_string(data: str) -> str:
     return f'"{data}"'
 
 
-def create_script_copy(editor: FileTreeEditor, path: str):
+def create_script_copy(editor: FileTreeEditor, path: str) -> None:
     original = path + "_original.lc"
     if not editor.does_asset_exists(original):
         original_lc = editor.get_raw_asset(path + ".lc")
         editor.add_new_asset(
             original,
             original_lc,
             editor.find_pkgs(path + ".lc")
         )
 
 
-def replace_script(editor: FileTreeEditor, path: str, replacement_path: str):
+def replace_script(editor: FileTreeEditor, path: str, replacement_path: str) -> None:
     create_script_copy(editor, path)
     lua_content = files_path().joinpath(replacement_path).read_text()
     lua_resource = Lua(Container(lua_text=lua_content), editor.target_game)
     editor.replace_asset(path + ".lc", lua_resource)
 
-def replace_script_with_content(editor: FileTreeEditor, path: str, lua_content: str):
+def replace_script_with_content(editor: FileTreeEditor, path: str, lua_content: str) -> None:
     create_script_copy(editor, path)
     lua_resource = Lua(Container(lua_text=lua_content), editor.target_game)
     editor.replace_asset(path + ".lc", lua_resource)
```

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/misc_patches/spawn_points.py` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/misc_patches/spawn_points.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,24 +20,24 @@
     ),
     NewSpawnPoint(
         "s110_surfaceb", "ST_SurfaceB_Connector", [-23179.0, 4500.0, 0.0], -90, ["collision_camera_017"]
     ),
 ]
 
 
-def add_spawnpoints(editor: PatcherEditor, new_spawnpoint: NewSpawnPoint):
+def add_spawnpoints(editor: PatcherEditor, new_spawnpoint: NewSpawnPoint) -> None:
     template_sp = editor.get_scenario("s000_surface").raw.actors[5]["ST_SG_Alpha_001"]
 
     scenario_name = new_spawnpoint.scenario
     scenario_file = editor.get_scenario(scenario_name)
 
     editor.copy_actor(scenario_name, new_spawnpoint.position, template_sp, new_spawnpoint.name, 5)
 
     scenario_file.raw.actors[5][new_spawnpoint.name]["rotation"][1] = new_spawnpoint.rotation
 
     for entity_group in new_spawnpoint.entity_groups:
         scenario_file.add_actor_to_entity_groups(entity_group, new_spawnpoint.name, True)
 
 
-def patch_custom_spawn_points(editor: PatcherEditor):
+def patch_custom_spawn_points(editor: PatcherEditor) -> None:
     for new_spawnpoint in new_spawnpoints:
         add_spawnpoints(editor, new_spawnpoint)
```

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/misc_patches/text_patches.py` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/misc_patches/text_patches.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,31 +19,31 @@
     "mse_english.txt",
     "us_english.txt",
     "us_french.txt",
     "us_spanish.txt"
 }
 
 
-def patch_text(editor: PatcherEditor, key: str, value: str):
+def patch_text(editor: PatcherEditor, key: str, value: str) -> None:
     for text_file in ALL_TEXT_FILES:
         text = editor.get_file(f"system/localization/{text_file}", Txt)
         text.strings[key] = value
 
 
 def get_text(editor: PatcherEditor, key: str, text_file: str = "us_english.txt") -> str:
     text = editor.get_file(f"system/localization/{text_file}", Txt)
     return text.strings[key]
 
 
-def apply_text_patches(editor: PatcherEditor, patches: dict[str, str]):
+def apply_text_patches(editor: PatcherEditor, patches: dict[str, str]) -> None:
     for k, v in patches.items():
         patch_text(editor, k, v)
 
 
-def add_spiderboost_status(editor: PatcherEditor):
+def add_spiderboost_status(editor: PatcherEditor) -> None:
     status = "GUI_STATUS_POWERBOMB"
     original = get_text(editor, status)
     new = original.replace(
         "one.",
         "one.|The Spider Boost can be used while in Spider Ball form. It will "
         "launch you forward, damaging enemies you make contact with.|It can also be used to reach certain items.",
     )
```

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/patch_util.py` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/patch_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import typing
 from pathlib import Path
 
 from open_samus_returns_rando.logger import LOG
 
 
 def patch_with_status_update(input_path: Path, output_path: Path, configuration: dict,
-                             status_update: typing.Callable[[float, str], None]):
+                             status_update: typing.Callable[[float, str], None]) -> None:
     from open_samus_returns_rando.samus_returns_patcher import patch_extracted
     # messages depends on the layout but it is a good approximation
     total_logs = 410
 
     class StatusUpdateHandler(logging.Handler):
         count = 0
```

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/patcher_editor.py` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/patcher_editor.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,58 +19,58 @@
 class PatcherEditor(FileTreeEditor):
     memory_files: dict[str, BaseResource]
 
     def __init__(self, root: Path):
         super().__init__(root, Game.SAMUS_RETURNS)
         self.memory_files = {}
 
-    def get_file(self, path: str, type_hint: type[T] = BaseResource) -> T:
+    def get_file(self, path: str, type_hint: type[T] = BaseResource) -> T: # type: ignore
         if path not in self.memory_files:
-            self.memory_files[path] = self.get_parsed_asset(path, type_hint=type_hint)
-        return self.memory_files[path]
+            self.memory_files[path] = self.get_parsed_asset(path, type_hint=type_hint) # type: ignore
+        return self.memory_files[path] # type: ignore
 
     def get_level_pkgs(self, name: str) -> set[str]:
         return set(self.find_pkgs(path_for_level(name) + ".bmsld"))
 
     def get_all_level_pkgs(self) -> list[str]:
-        def get_nested_list():
+        def get_nested_list() -> typing.Iterable[set[str]]:
             for scenario in ALL_SCENARIOS:
                 yield self.get_level_pkgs(scenario)
         return [pkg for all_level_pkgs in get_nested_list() for pkg in all_level_pkgs]
 
-    def ensure_present_in_scenario(self, scenario: str, asset):
+    def ensure_present_in_scenario(self, scenario: str, asset: str) -> None:
         for pkg in self.get_level_pkgs(scenario):
             self.ensure_present(get_package_name(pkg, asset), asset)
 
     def get_scenario(self, name: str) -> Bmsld:
         return self.get_file(path_for_level(name) + ".bmsld", Bmsld)
 
     def resolve_actor_reference(self, ref: dict) -> Container:
         scenario = self.get_scenario(ref["scenario"])
         # FIXME: There is no "default" as layer in SR
         layer = int(ref.get("layer", "default"))
         return scenario.raw.actors[layer][ref["actor"]]
 
-    def flush_modified_assets(self):
+    def flush_modified_assets(self) -> None:
         for name, resource in self.memory_files.items():
             self.replace_asset(name, resource)
         self.memory_files = {}
 
-    def copy_actor(self, scenario: str, coords, template_actor: Container, new_name: str,
-                   layer_index: int, offset: tuple = (0, 0, 0)):
+    def copy_actor(self, scenario: str, coords: list[float], template_actor: Container, new_name: str,
+                   layer_index: int, offset: tuple = (0, 0, 0)) -> Container:
         new_actor = copy.deepcopy(template_actor)
         current_scenario = self.get_scenario(scenario)
         current_scenario.raw.actors[layer_index][new_name] = new_actor
         new_actor["position"][0] = coords[0] + offset[0]
         new_actor["position"][1] = coords[1] + offset[1]
         new_actor["position"][2] = coords[2] + offset[2]
 
         return new_actor
 
-    def remove_entity(self, reference: dict):
+    def remove_entity(self, reference: dict)-> None:
         scenario = self.get_scenario(reference["scenario"])
         layer = reference["layer"]
         actor_name = reference["actor"]
 
         scenario.raw.actors[layer].pop(actor_name)
         scenario.remove_actor_from_all_groups(actor_name)
```

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/pickups/model_data.py` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/pickups/model_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -287,12 +287,26 @@
     "powerup_missilelauncher": ModelData(
         bcmdl_path="actors/items/powerup_missilelauncher/models/powerup_missilelauncher.bcmdl",
         dependencies=(
             "actors/items/powerup_missilelauncher/models/powerup_missilelauncher.bcmdl",
             "actors/items/powerup_missilelauncher/models/textures/missile_e.bctex",
         ),
     ),
+    "item_offworld": ModelData(
+        bcmdl_path="actors/items/item_offworld/models/item_offworld.bcmdl",
+        dependencies=(
+            "actors/items/item_offworld/models/item_offworld.bcmdl",
+            "maps/textures/chozoartifactor_o.bctex",
+        ),
+    ),
+    "powerup_icemissile": ModelData(
+        bcmdl_path="actors/items/powerup_icemissile/models/powerup_icemissile.bcmdl",
+        dependencies=(
+            "actors/items/powerup_icemissile/models/powerup_icemissile.bcmdl",
+            "actors/items/powerup_icemissile/models/textures/missile_d.bctex",
+        ),
+    ),
 }
 
 
 def get_data(name: str) -> ModelData:
     return ALL_MODEL_DATA.get(name, ALL_MODEL_DATA["itemsphere"])
```

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/pickups/pickup.py` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/pickups/pickup.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,33 +66,33 @@
             0.0,
             0.0,
         ])
     })
 })
 
 @functools.cache
-def _read_template_powerup():
+def _read_template_powerup() -> dict:
     with templates_path().joinpath("template_powerup_bmsad.json").open() as f:
         return json.load(f)
 
 class PickupType(Enum):
     ACTOR = "actor"
     METROID = "metroid"
 
 class BasePickup:
     def __init__(self, lua_editor: LuaEditor, pickup: dict, pickup_id: int, configuration: dict):
         self.lua_editor = lua_editor
         self.pickup = pickup
         self.pickup_id = pickup_id
         self.configuration = configuration
 
-    def patch(self, editor: PatcherEditor):
+    def patch(self, editor: PatcherEditor) -> None:
         raise NotImplementedError
 
-    def get_scenario(self):
+    def get_scenario(self) -> str:
         raise NotImplementedError
 
 class ActorPickup(BasePickup):
     _bmsad_dict: dict[str, tuple[str, ScriptClass]] = {}
 
     def patch_item_pickup(self, bmsad: dict) -> tuple[dict, ScriptClass]:
         pickable: dict = bmsad["components"]["PICKABLE"]
@@ -124,15 +124,15 @@
         # this actually wants an #GUI identifier but it works
         pickable["functions"][0]["params"]["Param7"]["value"] = self.pickup["caption"]
 
         # Update given item
         new_template, script_class = self.patch_item_pickup(new_template)
 
         new_path = script_class.get_bmsad_path()
-        editor.add_new_asset(new_path, Bmsad(new_template, editor.target_game), in_pkgs=pkgs_for_level)
+        editor.add_new_asset(new_path, Bmsad(new_template, editor.target_game), in_pkgs=pkgs_for_level) # type: ignore
         return script_class
 
 
     def patch_model(self, model_names: list[str], bmsad: dict) -> None:
         MODELUPDATER = bmsad["components"]["MODELUPDATER"]
         item_id: str = self.pickup["resources"][0][0]["item_id"]
         model_name = model_names[0]
@@ -244,15 +244,15 @@
         # offset for single and multimodels
         if model_name not in TANK_MODELS:
             MODELUPDATER["fields"] = OFFSET
             MODELUPDATER["fields"]["vInitPosWorldOffset"]["value"][1] = y_offset
             MODELUPDATER["fields"]["vInitAngWorldOffset"]["value"][0] = 0.0
 
 
-    def patch(self, editor: PatcherEditor):
+    def patch(self, editor: PatcherEditor) -> None:
         actor_reference = self.pickup["pickup_actor"]
         actor_name = actor_reference["actor"]
         model_names: list[str] = self.pickup["model"]
         scenario_name: str = actor_reference['scenario']
 
         pkgs_for_level = set(editor.find_pkgs(path_for_level(self.pickup["pickup_actor"]["scenario"]) + ".bmsld"))
         scenario = editor.get_scenario(scenario_name)
@@ -294,25 +294,25 @@
         # Dependencies
         for level_pkg in pkgs_for_level:
             for model_name in model_names:
                 model_data = get_data(model_name)
                 for dep in model_data.dependencies:
                     editor.ensure_present(get_package_name(level_pkg, dep), dep)
 
-    def get_scenario(self):
+    def get_scenario(self) -> str:
         return self.pickup["pickup_actor"]["scenario"]
 
 
 class MetroidPickup(BasePickup):
-    def patch(self, editor: PatcherEditor):
+    def patch(self, editor: PatcherEditor) -> None:
         script_class = self.lua_editor.create_script_class(self.pickup, f"metroid_{self.pickup_id}")
         script_class.ensure_files(editor)
         self.lua_editor.add_metroid_pickup(self.pickup["metroid_callback"], script_class)
 
-    def get_scenario(self):
+    def get_scenario(self) -> str:
         return self.pickup["metroid_callback"]["scenario"]
 
 
 def ensure_base_models(editor: PatcherEditor) -> None:
     for level_pkg in editor.get_all_level_pkgs():
         # ensure base stuff
         editor.ensure_present(get_package_name(level_pkg, "bmsat"), "system/animtrees/base.bmsat")
@@ -326,21 +326,23 @@
 
         # ensure energytank stuff (base for all tanks)
         editor.ensure_present(get_package_name(level_pkg, "bcskla"), "actors/items/itemtank/animations/relax.bcskla")
         model_data = get_data("item_energytank")
         for dep in model_data.dependencies:
             editor.ensure_present(get_package_name(level_pkg, dep), dep)
 
-def count_dna(lua_scripts: LuaEditor, pickup_object: BasePickup):
+def count_dna(lua_scripts: LuaEditor, pickup_object: BasePickup) -> None:
     item_id = pickup_object.pickup["resources"][0][0]["item_id"]
     if item_id.startswith("ITEM_RANDO_DNA"):
         scenario: str = pickup_object.get_scenario()
         lua_scripts.add_dna(scenario)
 
-def patch_pickups(editor: PatcherEditor, lua_scripts: LuaEditor, pickups_config: list[dict], configuration: dict):
+def patch_pickups(
+        editor: PatcherEditor, lua_scripts: LuaEditor, pickups_config: list[dict], configuration: dict
+        ) -> None:
     ActorPickup._bmsad_dict = {}
     editor.add_new_asset(
         "actors/items/randomizerpowerup/scripts/randomizerpowerup.lc",
         Lua(Container(lua_text=templates_path().joinpath("randomizerpowerup.lua").read_text()), editor.target_game),
         []
     )
     editor.add_new_asset("actors/scripts/metroid.lc", b'', [])
```

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/samus_returns_patcher.py` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/samus_returns_patcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from open_samus_returns_rando.debug import debug_custom_pickups, debug_spawn_points
 from open_samus_returns_rando.files import files_path
 from open_samus_returns_rando.logger import LOG
 from open_samus_returns_rando.lua_editor import LuaEditor
 from open_samus_returns_rando.misc_patches.collision_camera_table import create_collision_camera_table
 from open_samus_returns_rando.misc_patches.credits import patch_credits
 from open_samus_returns_rando.misc_patches.elevators import patch_elevators
-from open_samus_returns_rando.misc_patches.exefs import DSPatch
 from open_samus_returns_rando.misc_patches.spawn_points import patch_custom_spawn_points
 from open_samus_returns_rando.misc_patches.text_patches import add_spiderboost_status, apply_text_patches
 from open_samus_returns_rando.patcher_editor import PatcherEditor
 from open_samus_returns_rando.pickups.custom_pickups import patch_custom_pickups
 from open_samus_returns_rando.pickups.pickup import patch_pickups
 from open_samus_returns_rando.specific_patches import cosmetic_patches, game_patches, tunable_patches
 from open_samus_returns_rando.specific_patches.chozo_seal_patches import patch_chozo_seals
@@ -26,43 +25,37 @@
 from open_samus_returns_rando.specific_patches.map_icons import patch_tiles
 from open_samus_returns_rando.specific_patches.metroid_patches import patch_metroids
 from open_samus_returns_rando.specific_patches.static_fixes import apply_static_fixes
 from open_samus_returns_rando.validator_with_default import DefaultValidatingDraft7Validator
 
 T = typing.TypeVar("T")
 
-def _read_schema():
+def _read_schema() -> dict:
     with Path(__file__).parent.joinpath("files", "schema.json").open() as f:
         return json.load(f)
 
-def add_custom_files(editor: PatcherEditor):
+def add_custom_files(editor: PatcherEditor) -> None:
     custom_romfs = files_path().joinpath("romfs")
     for child in custom_romfs.rglob("*"):
         if not child.is_file():
             continue
         relative = child.relative_to(custom_romfs).as_posix()
         LOG.info("Adding custom asset %s", relative)
         asset_name = str(relative)
         raw_bytes = child.read_bytes()
         try:
             editor.add_new_asset(asset_name, raw_bytes, [])
         except ValueError:
             editor.replace_asset(asset_name, raw_bytes)
 
 
-def patch_exefs(exefs_patches: Path):
-    exefs_patches.mkdir(parents=True, exist_ok=True)
-    patch = DSPatch()
-    # file needs to be named code.ips for Citra
-    exefs_patches.joinpath("code.ips").write_bytes(bytes(patch))
-
-def validate(configuration: dict):
+def validate(configuration: dict) -> None:
     DefaultValidatingDraft7Validator(_read_schema()).validate(configuration)
 
-def patch_extracted(input_path: Path, output_path: Path, configuration: dict):
+def patch_extracted(input_path: Path, output_path: Path, configuration: dict) -> None:
     LOG.info("Will patch files from %s", input_path)
 
     validate(configuration)
 
     editor = PatcherEditor(input_path)
     lua_scripts = LuaEditor()
 
@@ -121,18 +114,14 @@
     patch_elevators(editor, configuration)
 
     out_romfs = output_path.joinpath("romfs")
     out_exefs = output_path.joinpath("exefs")
     shutil.rmtree(out_romfs, ignore_errors=True)
     shutil.rmtree(out_exefs, ignore_errors=True)
 
-    # Create Exefs patches (currently there are none)
-    LOG.info("Creating exefs patches")
-    patch_exefs(out_exefs)
-
     LOG.info("Saving modified lua scripts")
     lua_scripts.save_modifications(editor, configuration)
 
     LOG.info("Flush modified assets")
     editor.flush_modified_assets()
 
     LOG.info("Saving modified pkgs to %s", out_romfs)
```

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/specific_patches/chozo_seal_patches.py` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/specific_patches/chozo_seal_patches.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         }),
     ]),
     "fields": Container(),
     "dependencies": None,
 })
 
 
-def patch_seals(editor: PatcherEditor):
+def patch_seals(editor: PatcherEditor) -> None:
     systemmechdna_name = "actors/props/systemmechdna/charclasses/systemmechdna.bmsad"
     save_station_name = "actors/props/savestation/charclasses/savestation.bmsad"
     chozoseal_name = "actors/props/chozoseal/charclasses/chozoseal.bmsad"
     chozoseal_model_name = "actors/props/chozoseal/models/chozoseal.bcmdl"
 
     # metroid seals
     systemmechdna = editor.get_file(systemmechdna_name, Bmsad)
@@ -106,15 +106,15 @@
         ["collision_camera_022", "collision_camera_024"]
     ),
     NewChozoSeal(
         "s110_surfaceb", [-28150.0, 300.0, 0.0], [-28150.0, 300.0, 0.0], 145, ["collision_camera_017"]
     ),
 ]
 
-def add_chozo_seals(editor: PatcherEditor, new_seal: NewChozoSeal):
+def add_chozo_seals(editor: PatcherEditor, new_seal: NewChozoSeal) -> None:
     template_ap = editor.get_scenario("s000_surface").raw.actors[16]["LE_ChozoUnlockAreaDNA"]
     template_platform = editor.get_scenario("s000_surface").raw.actors[10]["LE_Platform_ChozoUnlockAreaDNA"]
 
     CHOZO_SEAL_ICON = Container({
         "actor_name": new_seal.ap_name,
         "clear_condition": "",
         "icon": "systemmechdna",
@@ -142,15 +142,15 @@
 
     # Dependencies
     editor.ensure_present_in_scenario(scenario_name, "maps/textures/dnaemptyfx_d.bctex")
     for asset in editor.get_asset_names_in_folder("actors/props/systemmechdna"):
         editor.ensure_present_in_scenario(scenario_name, asset)
 
 
-def update_item_seals(editor:PatcherEditor):
+def update_item_seals(editor:PatcherEditor) -> None:
     CHOZO_SEALS = {
         "s000_surface": ["LE_ChozoUnlockAreaDNA"],
         "s010_area1": ["LE_ChozoUnlockAreaDNA"],
         "s028_area2c": ["LE_ChozoUnlockAreaDNA"],
         "s030_area3": ["LE_ChozoUnlockAreaDNA"],
         "s040_area4": ["LE_ChozoUnlockAreaDNA_001", "LE_ChozoUnlockAreaDNA_002"],
         "s060_area6": ["LE_ChozoUnlockAreaDNA"],
@@ -164,12 +164,12 @@
             scenario.raw.actors[16][seal]["type"] = "chozoseal"
 
         # Dependencies
         for asset in editor.get_asset_names_in_folder("actors/props/chozoseal"):
             editor.ensure_present_in_scenario(scenario_name, asset)
 
 
-def patch_chozo_seals(editor: PatcherEditor):
+def patch_chozo_seals(editor: PatcherEditor) -> None:
     patch_seals(editor)
     for new_seal in new_seals:
         add_chozo_seals(editor, new_seal)
     update_item_seals(editor)
```

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/specific_patches/cosmetic_patches.py` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/specific_patches/cosmetic_patches.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from mercury_engine_data_structures.formats.bmtun import Bmtun
 from open_samus_returns_rando.misc_patches import lua_util
 from open_samus_returns_rando.patcher_editor import PatcherEditor
 
 
-def patch_cosmetics(editor: PatcherEditor, configuration: dict):
+def patch_cosmetics(editor: PatcherEditor, configuration: dict) -> None:
     tunables = editor.get_file("system/tunables/tunables.bmtun", Bmtun)
     tunable_cosmetics(tunables, configuration)
 
 
-def tunable_cosmetics(tunables: Bmtun, configuration: dict):
+def tunable_cosmetics(tunables: Bmtun, configuration: dict) -> None:
     aim = tunables.raw["classes"]["CTunableAim"]["tunables"]
     aim["vLaserLockedColor0"]["value"] = configuration["laser_locked_color"]
     aim["vLaserUnlockedColor0"]["value"] = configuration["laser_unlocked_color"]
     aim["vGrappleLaserLockedColor0"]["value"] = configuration["grapple_laser_locked_color"]
     aim["vGrappleLaserUnlockedColor0"]["value"] = configuration["grapple_laser_unlocked_color"]
```

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/specific_patches/door_patches.py` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/specific_patches/door_patches.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-
 import copy
 import re
+import typing
 from enum import Enum
 
 from construct import Container, ListContainer
 from mercury_engine_data_structures.formats import Bmsad, Bmsld, Bmsmsd, Lua
 from mercury_engine_data_structures.formats.bmsmsd import IconPriority
 from open_samus_returns_rando.files import files_path
 from open_samus_returns_rando.patcher_editor import PatcherEditor
@@ -35,23 +35,23 @@
 })
 
 ON_DEAD_CB = Container({
     "unk1": 22,
     "unk2": 1,
     "unk3": 0,
     "args": Container({
-        601445949: Container({
+        601445949: Container({ # type: ignore
             "type": "s",
             "value": "RemoveDoors",
         }),
     }),
 })
 
 
-def _patch_missile_covers(editor: PatcherEditor):
+def _patch_missile_covers(editor: PatcherEditor) -> None:
     ALL_MISSILE_SHIELDS = {
         "s000_surface": ["LE_MissileShield_Door_002", "LE_MissileShield_Door_006"],
         "s010_area1": ["LE_DoorShieldMissile", "LE_DoorShieldMissile001"],
         "s020_area2": ["LE_MissileShield_Door004", "LE_Shield_Door012"],
         "s025_area2b": ["LE_MissileShield_Door006", "LE_MissileShield_Door009",
                         "LE_MissileShield_Door013", "LE_PowerBombShield_Door015"],
         "s030_area3": ["LE_MissileShield_Door003"],
@@ -68,15 +68,15 @@
     for scenario_name, shield in ALL_MISSILE_SHIELDS.items():
         scenario = editor.get_scenario(scenario_name)
         for door in shield:
             actor = scenario.raw.actors[9][door]
             actor["rotation"][1] = 90
 
 
-def _patch_beam_bmsads(editor: PatcherEditor):
+def _patch_beam_bmsads(editor: PatcherEditor) -> None:
     creature_bmsad_files = [
         "actors/props/doorspazerbeam/charclasses/doorspazerbeam.bmsad",
         "actors/props/doorcreature/charclasses/doorcreature.bmsad",
         "actors/props/doorwave/charclasses/doorwave.bmsad",
     ]
     for i, creature_bmsad_file in enumerate(creature_bmsad_files):
         cr_bmsad = editor.get_file(creature_bmsad_file, Bmsad)
@@ -88,27 +88,27 @@
         action_set_anim["events0"].append(ON_DEAD_CB)
         # wave cb didn't work and it has animation id 21.it's maybe a bitmask? because it works
         # with 29 and also with 30 (which the other two are using) and both are setting 2^3 bit
         action_set_anim["animation_id"] = 30
         # modify doorwave collision
         if i == 2:
             # Param6 and Param7 seems to be a position
-            cr_bmsad.components["COLLISION"].functions[1].params["Param7"].value = 148.0
+            cr_bmsad.components["COLLISION"].functions[1].params["Param7"].value = 148.0 # type: ignore
             # Param9 and Param10 are a rectangular
-            cr_bmsad.components["COLLISION"].functions[1].params["Param9"].value = 370.0
-            cr_bmsad.components["COLLISION"].functions[1].params["Param10"].value = 300.0
+            cr_bmsad.components["COLLISION"].functions[1].params["Param9"].value = 370.0 # type: ignore
+            cr_bmsad.components["COLLISION"].functions[1].params["Param10"].value = 300.0 # type: ignore
 
     editor.add_new_asset(
         "actors/props/doors/scripts/doors.lc",
         Lua(Container(lua_text=files_path().joinpath("custom", "doors.lua").read_text()), editor.target_game),
         []
     )
 
 
-def _patch_beam_covers(editor: PatcherEditor):
+def _patch_beam_covers(editor: PatcherEditor) -> None:
     ALL_BEAM_COVERS = {
         "s000_surface": ["LE_PlasmaShield_Door_008"],
         "s010_area1": ["LE_DoorShieldWave008", "LE_SpazerShield_Door007"],
         "s020_area2": ["LE_WaveShield_Door010"],
         "s025_area2b": ["LE_PlasmaShield_Door017", "LE_WaveShield_Door008",
                         "LE_WaveShield_Door016", "LE_WaveShield_Door019"],
         "s033_area3b": ["LE_SpazerShield_Door_010", "LE_WaveShield_Door_007"],
@@ -123,15 +123,15 @@
 
     for scenario_name, beam_covers in ALL_BEAM_COVERS.items():
         scenario = editor.get_scenario(scenario_name)
         for cover_name in beam_covers:
             actor = scenario.raw.actors[9][cover_name]
             new_actor_name = f"{cover_name}_o"
             new_actor = editor.copy_actor(
-                scenario_name, (actor["position"][0], actor["position"][1], actor["position"][2]),
+                scenario_name, [actor["position"][0], actor["position"][1], actor["position"][2]],
                 actor, new_actor_name, 9
             )
             new_actor["rotation"][0] = 0
             new_actor["rotation"][2] = 0
             current_rotation = new_actor["rotation"][1]
             new_actor["rotation"][1] = 180 if current_rotation == 0.0 else 0.0
 
@@ -145,15 +145,15 @@
 
             entity_groups = [group for group_name, group in scenario.all_actor_groups()
                     if group_name in list(scenario.all_actor_group_names_for_actor(cover_name))]
             for group in entity_groups:
                 scenario.insert_into_entity_group(group, new_actor_name)
 
 
-def _patch_charge_doors(editor: PatcherEditor):
+def _patch_charge_doors(editor: PatcherEditor) -> None:
     CHARGE_DOORS = {
         "s000_surface": ["Door004", "Door011"],
         "s010_area1": ["Door002"],
         "s028_area2c": ["Door001", "Door007"],
         "s030_area3": ["Door002", "Door008"],
         "s040_area4": ["Door006", "Door014"],
         "s060_area6": ["Door001"],
@@ -162,15 +162,15 @@
 
     for scenario_name, doors in CHARGE_DOORS.items():
         scenario = editor.get_scenario(scenario_name)
         for door in doors:
             scenario.raw.actors[15][door].type = "doorpowerpower"
 
 
-def _patch_one_way_doors(editor: PatcherEditor):
+def _patch_one_way_doors(editor: PatcherEditor) -> None:
     ONE_WAY_DOORS = {
         # Bombs, Right Exterior Door -> Interior, Exterior Alpha
         "s010_area1": ["Door004", "Door012", "Door016"],
         # Below Wave Beam
         "s025_area2b": ["Door008"],
         # Below Chozo Seal
         "s030_area3": ["Door005", "Door006"],
@@ -186,28 +186,41 @@
         scenario = editor.get_scenario(scenario_name)
         for door in doors:
             properties = scenario.raw.actors[15][door]
             properties.type = "doorpowerpower"
             properties.components[0]["arguments"][2]["value"] = False
 
 
+def _static_door_patches(editor: PatcherEditor) -> None:
+    _patch_one_way_doors(editor)
+    _patch_missile_covers(editor)
+    _patch_beam_bmsads(editor)
+    _patch_beam_covers(editor)
+    _patch_charge_doors(editor)
+
+
 class ActorData(Enum):
     """
     Enum containing data on actors
 
     actordef: the actordef for the actor
     """
     DOOR_POWER = (["doorpowerpower", "doorpowerclosed", "doorclosedpower"])
     DOOR_CHARGE = (["doorchargecharge", "doorchargeclosed", "doorclosedcharge"])
     SHIELD_WAVE_BEAM = (["doorwave"])
     SHIELD_SPAZER_BEAM = (["doorspazerbeam"])
     SHIELD_PLASMA_BEAM = (["doorcreature"])
     SHIELD_MISSILE = (["doorshieldmissile"])
     SHIELD_SUPER_MISSILE = (["doorshieldsupermissile"])
     SHIELD_POWER_BOMB = (["doorshieldpowerbomb"])
+    SHIELD_ICE_BEAM = (["doorshieldicebeam"])
+    SHIELD_GRAPPLE_BEAM = (["doorshieldgrapplebeam"])
+    SHIELD_BEAM_BURST = (["doorshieldbeamburst"])
+    SHIELD_BOMB = (["doorshieldbomb"])
+    SHIELD_LOCKED = (["doorshieldlocked"])
 
 class DoorType(Enum):
     """
     Enum containing info on each door type
 
     type: the name Randovania calls the door
     door: the door's ActorData
@@ -235,80 +248,103 @@
         "actors/props/doorshield", "actors/props/doorshieldsupermissile",
         "sounds/props/doorchargecharge/smissiledoor_hum.bcwav"
     ])
     POWER_BOMB = ("power_bomb", ActorData.DOOR_POWER, "doorpowerbomb", True, ActorData.SHIELD_POWER_BOMB, [
         "actors/props/doorshield", "actors/props/doorshieldpowerbomb",
         "sounds/props/doorchargecharge/powerbombdoor_hum.bcwav"
     ])
+    ICE_BEAM = ("ice_beam", ActorData.DOOR_POWER, "doorice", True, ActorData.SHIELD_ICE_BEAM, [
+        "actors/props/doorshield", "actors/props/doorshieldicebeam","sounds/props/creaturedoor",
+        "system/fx/textures/blood_gray.bctex",
+    ])
+    GRAPPLE_BEAM = ("grapple_beam", ActorData.DOOR_POWER, "doorgrapple", True, ActorData.SHIELD_GRAPPLE_BEAM, [
+        "actors/props/doorshield", "actors/props/doorshieldgrapplebeam",
+        "sounds/props/doorchargecharge/missiledoor_hum.bcwav"
+    ])
+    BOMB = ("bomb", ActorData.DOOR_POWER, "doorbomb", True, ActorData.SHIELD_BOMB, [
+        "actors/props/doorshield", "actors/props/doorshieldsupermissile", "actors/props/doorshieldbomb",
+        "sounds/props/doorchargecharge/smissiledoor_hum.bcwav"
+    ])
+    BEAM_BURST = ("beam_burst", ActorData.DOOR_POWER, "doorbeamburst", True, ActorData.SHIELD_BEAM_BURST, [
+        "actors/props/doorshield", "actors/props/doorshieldpowerbomb", "actors/props/doorshieldbeamburst",
+        "sounds/props/doorchargecharge/powerbombdoor_hum.bcwav"
+    ])
+    LOCKED = ("locked", ActorData.DOOR_POWER, "doorlocked", True, ActorData.SHIELD_LOCKED, [
+        "actors/props/doorshield", "actors/props/doorshieldlocked", "actors/props/doorspazerbeam",
+        "sounds/props/spazerdoor"
+    ])
 
     def __init__(self, rdv_door_type: str, door_data: ActorData, minimap_name: str,
                  need_shield: bool = False, shield_data: ActorData | None = None,
                  additional_asset_folders: list[str] | None = None, rotation: float = 0):
         self.type = rdv_door_type
         self.need_shield = need_shield
         self.door = door_data
         self.shield = shield_data
         self.required_asset_folders = [] if additional_asset_folders is None else additional_asset_folders
         self.minimap_name = minimap_name
         self.rotation = rotation
 
     @classmethod
-    def get_type(cls, type: str):
+    def get_type(cls, type: str) -> typing.Self:
         for e in cls:
             if e.type == type:
                 return e
 
         raise ValueError(f"{type} is not a patchable door!")
 
 class DoorPatcher:
     def __init__(self, editor: PatcherEditor):
         self.editor = editor
         self._example_shield = editor.get_scenario("s000_surface").raw.actors[9]["LE_PlasmaShield_Door_008"]
-        self._index_per_scenario = {}
+        self._index_per_scenario: dict[str, int] = {}
 
-    def _patch_to_power(self, door_actor: Container, scenario: Bmsld):
+    def _patch_to_power(self, door_actor: Container, scenario: Bmsld) -> None:
         for life_component in door_actor.components:
             shield = life_component["arguments"][3]["value"]
             if shield != "":
                 scenario.remove_actor_from_all_groups(shield)
                 scenario.raw.actors[9].pop(shield)
         # pop a life component from our static door patches
         if len(door_actor.components) > 1:
             door_actor.components.pop()
         door_actor.components[0]["arguments"][2]["value"] = False
         door_actor.components[0]["arguments"][3]["value"] = ""
-        door_actor.type = ActorData.DOOR_POWER.value[0]
+        door_actor["type"] = ActorData.DOOR_POWER.value[0]
 
     def _create_shield(
             self, scenario_name: str, position: tuple[float, float, float], shield_name: str, new_type: str
         ) -> Container:
         new_actor = self.editor.copy_actor(
-                scenario_name, (position[0], position[1], position[2]),
+                scenario_name, [position[0], position[1], position[2]],
                 self._example_shield, shield_name, 9
             )
 
         new_actor["type"] = new_type
         return new_actor
 
-    def patch_door(self, editor: PatcherEditor, actor_ref: dict, door_type_str: str):
+    def patch_door(self, editor: PatcherEditor, actor_ref: dict, door_type_str: str) -> None:
         scenario_name = actor_ref["scenario"]
         actor_name = actor_ref["actor"]
         scenario = self.editor.get_scenario(scenario_name)
         door_actor = scenario.raw.actors[15].get(actor_name, None)
         index = self._index_per_scenario.get(scenario_name, 0)
         left_shield_name = f"Shield_{index}"
         right_shield_name = f"Shield_{index}_o"
         new_door: DoorType = DoorType.get_type(door_type_str)
 
         self.patch_actor(
             new_door, scenario_name, actor_name, scenario, door_actor, index, left_shield_name, right_shield_name
         )
         self.patch_minimap(editor, scenario_name, actor_name, left_shield_name, right_shield_name, new_door)
 
-    def patch_minimap(self, editor, scenario_name, actor_name, left_shield_name, right_shield_name, new_door):
+    def patch_minimap(
+            self, editor: PatcherEditor, scenario_name:str, actor_name:str,
+            left_shield_name:str, right_shield_name:str, new_door: DoorType
+            ) -> None:
         scenario_minimap = editor.get_file(f"gui/minimaps/c10_samus/{scenario_name}.bmsmsd", Bmsmsd)
         tiles = scenario_minimap.raw["tiles"]
 
         # find left and right tile
         tiles_for_door = [
             x
             for x in tiles
@@ -372,26 +408,27 @@
 
         # bad special case to force DoorManicMinerBot to doorclosed...
         if actor_name == "DoorManicMinerBot":
             left_tile_icon.icon = 'doorclosedleft'
 
     def patch_actor(
             self, new_door: DoorType, scenario_name: str, actor_name: str, scenario: Bmsld,
-            door_actor, index: int, left_shield_name: str, right_shield_name: str
-        ):
+            door_actor: Container, index: int, left_shield_name: str, right_shield_name: str
+        ) -> None:
         if door_actor is None:
             raise ValueError(f"Actor {actor_name} not found in scenario {scenario_name}")
 
         self._patch_to_power(door_actor, scenario)
 
         # patch to desired type
         if not new_door.need_shield:
-            door_actor.type = new_door.door.value[0]
+            door_actor["type"] = new_door.door.value[0]
         # all other use shields
         else:
+            assert new_door.shield is not None
             shield_position = (door_actor["position"][0], door_actor["position"][1],  door_actor["position"][2])
             new_actor_l = self._create_shield(
                 scenario_name, shield_position, left_shield_name, new_door.shield.value[0]
             )
             new_actor_r = self._create_shield(
                 scenario_name, shield_position, right_shield_name, new_door.shield.value[0]
             )
@@ -409,34 +446,89 @@
             for group in entity_groups:
                 scenario.insert_into_entity_group(group,  left_shield_name)
                 scenario.insert_into_entity_group(group,  right_shield_name)
             self._index_per_scenario[scenario_name] = index + 1
 
         # bad special case to force DoorManicMinerBot to doorclosed...
         if actor_name == "DoorManicMinerBot":
-            door_actor.type = re.sub("(doorpower|doorcharge)", "doorclosed", door_actor.type)
+            door_actor["type"] = re.sub("(doorpower|doorcharge)", "doorclosed", door_actor.type)
 
         # ensure required files
         for folder in new_door.required_asset_folders:
             for asset in self.editor.get_asset_names_in_folder(folder):
                 self.editor.ensure_present_in_scenario(scenario_name, asset)
 
 
-def _static_door_patches(editor: PatcherEditor):
-    _patch_one_way_doors(editor)
-    _patch_missile_covers(editor)
-    _patch_beam_bmsads(editor)
-    _patch_beam_covers(editor)
-    _patch_charge_doors(editor)
+class NewShield(typing.NamedTuple):
+    shield_name: str
+    weakness: str
+    base_shield: str
+
+
+new_shields = [
+    NewShield("beamburst", "WEAPON_BOOST", "doorshieldpowerbomb"),
+    NewShield("bomb", "BOMB", "doorshieldsupermissile"),
+    NewShield("grapplebeam", "GRAPPLE_BEAM", "doorshield"),
+    NewShield("icebeam", "ICE_BEAM", "doorcreature"),
+    NewShield("locked", "", "doorspazerbeam"),
+]
+
+
+def add_custom_shields(editor: PatcherEditor, new_shield: NewShield) -> None:
+    # Missile shields are split across doorshield and doorshieldmissile
+    if new_shield.base_shield == "doorshield":
+        template_bmsad = "actors/props/doorshieldmissile/charclasses/doorshieldmissile.bmsad"
+    else:
+        template_bmsad = f"actors/props/{new_shield.base_shield}/charclasses/{new_shield.base_shield}.bmsad"
+
+    new_model = f"actors/props/doorshield{new_shield.shield_name}/models/doorshield{new_shield.shield_name}.bcmdl"
+    new_bmsad = f"actors/props/doorshield{new_shield.shield_name}/charclasses/doorshield{new_shield.shield_name}.bmsad"
+
+    # Create a copy of the bmsad
+    template_shield = editor.get_file(template_bmsad, Bmsad)
+    editor.add_new_asset(new_bmsad, template_shield, [])
+
+    # Modify the new bmsad
+    custom_shield = editor.get_file(new_bmsad, Bmsad)
+    custom_shield.name = f"doorshield{new_shield.shield_name}"
+    custom_shield.raw["header"]["model_name"] = new_model
+    custom_shield.components["MODELUPDATER"].functions[0].params["Param1"]["value"] = new_model
+
+    # Update the life component
+    life_component = custom_shield.raw["components"]["LIFE"]["functions"]
+    if new_shield.base_shield == "doorshield":
+        # Remove the Super Missile weakness
+        life_component[1]["params"]["Param1"]["value"] = new_shield.weakness
+    elif new_shield.base_shield == "doorspazerbeam":
+        # Remove all weaknesses
+        for i in range(4):
+            life_component[i]["params"]["Param1"]["value"] = new_shield.weakness
+    elif new_shield.base_shield == "doorcreature":
+        # Remove the Power Bomb weakness
+        life_component[1]["params"]["Param1"]["value"] = new_shield.weakness
+        # Set shield health to 1
+        life_component[2]["params"]["Param2"]["value"] = 1.0
+        life_component[3]["params"]["Param2"]["value"] = 1.0
+        # Remove the drops from breaking the shield
+        custom_shield.raw["components"].pop("DROP")
+        # Remove the particle animation that occurs after the shield breaks (color mismatch)
+        custom_shield.raw["action_sets"][0]["animations"][0]["events0"][1]["args"][729149823]["value"] = 0
+    elif new_shield.base_shield in {"doorshieldsupermissile", "doorshieldpowerbomb"}:
+        # Some shaders do not use dissolve fx, so force fx to be used
+        custom_shield.raw["components"]["LIFE"]["fields"]["bDisolveByMaterial"]["value"] = False
+        custom_shield.raw["components"]["LIFE"]["fields"]["fTimeToStartDisolve"]["value"] = 0.2
 
-def patch_doors(editor: PatcherEditor, door_patches: list[dict]):
-    _static_door_patches(editor)
 
+def patch_doors(editor: PatcherEditor, door_patches: list[dict]) -> None:
+    _static_door_patches(editor)
+    for new_shield in new_shields:
+        add_custom_shields(editor, new_shield)
     door_patcher = DoorPatcher(editor)
 
     # small hack to eliminate duplicates (randovania exports everything duplicated)
     import json
+
     set_of_jsons = {json.dumps(d, sort_keys=True) for d in door_patches}
     door_patches_set = [json.loads(t) for t in set_of_jsons]
 
     for door in door_patches_set:
         door_patcher.patch_door(editor, door["actor"], door["door_type"])
```

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/specific_patches/game_patches.py` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/specific_patches/game_patches.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from construct import Container
 from mercury_engine_data_structures.formats import Bmsad, Bmsbk
 from open_samus_returns_rando.patcher_editor import PatcherEditor
 
 
-def apply_game_patches(editor: PatcherEditor, configuration: dict):
+def apply_game_patches(editor: PatcherEditor, configuration: dict) -> None:
     # Weapon patches
     _remove_pb_weaknesses(editor, configuration)
 
     if configuration["nerf_super_missiles"]:
         _remove_super_missile_weakness(editor)
 
     # Area patches
     _remove_grapple_blocks(editor, configuration)
     _patch_crumble_blocks(editor, configuration)
     _patch_reverse_area8(editor, configuration)
 
 
-def _remove_pb_weaknesses(editor: PatcherEditor, configuration: dict):
+def _remove_pb_weaknesses(editor: PatcherEditor, configuration: dict) -> None:
     # Charge Door
     if configuration["charge_door_buff"]:
         for door in ["doorchargecharge", "doorclosedcharge"]:
             charge_door = editor.get_file(
                 f"actors/props/{door}/charclasses/{door}.bmsad", Bmsad
             )
             func = charge_door.raw.components.LIFE.functions[0]
@@ -54,15 +54,15 @@
         for plants in PLANT_FILES:
             plant = editor.get_file(plants, Bmsad)
             plant.raw["components"]["LIFE"]["fields"][
                 "bShouldDieWithPowerBomb"
             ] = Container({"type": "bool", "value": False})
 
 
-def _remove_grapple_blocks(editor: PatcherEditor, configuration: dict):
+def _remove_grapple_blocks(editor: PatcherEditor, configuration: dict) -> None:
     ELEVATOR_GRAPPLE_BLOCKS = {
         # Area 4 West to Area 4 East
         "s040_area4": ["LE_GrappleMov_001"],
         # Area 6 to Area 7
         "s070_area7": ["LE_GrappleMov_001"],
         # Area 7 to Area 8
         "s090_area9": ["LE_GrappleMov_001"],
@@ -80,24 +80,24 @@
 
     if configuration["remove_grapple_block_area3_interior_shortcut"]:
         editor.remove_entity(
             {"scenario": "s036_area3c", "layer": 9, "actor": "LE_GrappleDest_004"}
         )
 
 
-def _remove_super_missile_weakness(editor: PatcherEditor):
+def _remove_super_missile_weakness(editor: PatcherEditor) -> None:
     missile_door = editor.get_file(
         "actors/props/doorshieldmissile/charclasses/doorshieldmissile.bmsad", Bmsad
     )
     func = missile_door.raw.components.LIFE.functions[1]
     if func.params.Param1.value:
         func.params.Param1.value = "MISSILE"
 
 
-def _patch_crumble_blocks(editor: PatcherEditor, configuration: dict):
+def _patch_crumble_blocks(editor: PatcherEditor, configuration: dict) -> None:
     # Crumble blocks after Scan Pulse
     if configuration["patch_surface_crumbles"]:
         surface = editor.get_file(
             "maps/levels/c10_samus/s000_surface/s000_surface.bmsbk", Bmsbk
         )
         post_scan_pulse_crumbles = surface.raw["block_groups"][37]
         post_scan_pulse_crumbles["types"][0]["block_type"] = "power_beam"
@@ -115,12 +115,12 @@
         area1_chozo_seal_crumbles["types"][0]["blocks"][0]["respawn_time"] = 0.0
         area1_chozo_seal_crumbles["types"][0]["blocks"][1]["respawn_time"] = 0.0
         area1_chozo_seal_crumbles["types"][0]["blocks"][2]["respawn_time"] = 0.0
         area1_chozo_seal_crumbles["types"][0]["blocks"][3]["respawn_time"] = 0.0
         area1_chozo_seal_crumbles["types"][0]["blocks"][4]["respawn_time"] = 0.0
 
 
-def _patch_reverse_area8(editor: PatcherEditor, configuration: dict):
+def _patch_reverse_area8(editor: PatcherEditor, configuration: dict) -> None:
     if configuration["reverse_area8"]:
         editor.remove_entity(
             {"scenario": "s100_area10", "layer": 9, "actor": "LE_ValveQueen"}
         )
```

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/specific_patches/map_icons.py` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/specific_patches/map_icons.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from mercury_engine_data_structures.formats import Bmsmsd
 from mercury_engine_data_structures.formats.bmsmsd import TileType
 from open_samus_returns_rando.constants import ALL_SCENARIOS
 from open_samus_returns_rando.patcher_editor import PatcherEditor
 
 
-def patch_tiles(editor: PatcherEditor):
+def patch_tiles(editor: PatcherEditor) -> None:
     SCENARIO_TO_DOORS = {
         "s000_surface": ["Door004", "Door011"],
         "s010_area1": ["Door002", "Door004", "Door012", "Door016"],
         "s025_area2b": ["Door008"],
         "s028_area2c": ["Door001", "Door007"],
         "s030_area3": ["Door002", "Door005", "Door006", "Door008"],
         "s040_area4": ["Door001", "Door006", "Door014"],
```

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/specific_patches/static_fixes.py` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/specific_patches/static_fixes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import copy
+import typing
 
 from construct import Container, ListContainer
 from mercury_engine_data_structures.formats import Bmsad, Bmsbk, Bmtun
 from open_samus_returns_rando.patcher_editor import PatcherEditor
 
 MULTI_ROOM_GAMMAS = [
     {"scenario": "s030_area3", "layer": 0, "actor": "TG_Gamma_005_A"},
@@ -41,15 +42,15 @@
     {"scenario": "s050_area5", "layer": 0, "actor": "TG_Gamma_002_C"},
     {"scenario": "s050_area5", "layer": 3, "actor": "SG_Gamma_002_C"},
     {"scenario": "s050_area5", "layer": 4, "actor": "Gamma_002_C"},
     {"scenario": "s050_area5", "layer": 4, "actor": "Gamma_002_Intro_C"},
 ]
 
 
-def patch_multi_room_gammas(editor: PatcherEditor):
+def patch_multi_room_gammas(editor: PatcherEditor) -> None:
     for reference in MULTI_ROOM_GAMMAS:
         editor.remove_entity(reference)
 
     gamma_actors = [
         ("s030_area3", "SG_Gamma_005_C", "SP_Gamma_005_C", "TG_Gamma_005_C"),
         ("s033_area3b", "SG_Gamma_004_B", "Gamma_004_Intro_B", "TG_Gamma_004_B"),
         ("s036_area3c", "SG_Gamma_007_A", "SP_Gamma_007_Intro_A", "TG_Gamma_007_A"),
@@ -66,27 +67,27 @@
         # make the trigger active
         scenario.raw["actors"][0][trigger]["components"][0]["arguments"][0]["value"] = True
         # move Gamma_002_A so it doesn't just poof into existence when it spawns
         if scenario_name == "s050_area5":
             scenario.raw["actors"][4]["Gamma_002_A"]["position"][0] = 17100.0
 
 
-def patch_pickup_rotation(editor: PatcherEditor):
+def patch_pickup_rotation(editor: PatcherEditor) -> None:
     PICKUPS = {
         "s030_area3": ["LE_PowerUp_GrappleBeam"],
         "s050_area5": ["LE_PowerUp_SpaceJump"],
     }
     for scenario_name, pickups in PICKUPS.items():
         scenario = editor.get_scenario(scenario_name)
         for pickup in pickups:
             actor = scenario.raw.actors[9][pickup]
             actor["rotation"][1] = 0.0
 
 
-def patch_pickup_position(editor: PatcherEditor):
+def patch_pickup_position(editor: PatcherEditor) -> None:
     PICKUPS = {
         "s000_surface": ["LE_SpecialAbility_ScanningPulse"],
         "s010_area1": ["LE_PowerUp_SpiderBall"],
         "s028_area2c": ["LE_SpecialAbility_EnergyShield"],
         "s030_area3": ["LE_SpecialAbility_EnergyWave"],
         "s060_area6": ["LE_SpecialAbility_PhaseDisplacement"],
     }
@@ -96,35 +97,35 @@
             actor = scenario.raw.actors[9][pickup]
             if pickup != "LE_PowerUp_SpiderBall":
                 actor["position"][1] -= 55.0
             else:
                 actor["position"][1] -= 49.0
 
 
-def remove_area7_grapple_block(editor: PatcherEditor):
+def remove_area7_grapple_block(editor: PatcherEditor) -> None:
     editor.remove_entity(
         {"scenario": "s090_area9", "layer": 9, "actor": "LE_GrappleDest_007"}
     )
 
 
-def patch_a7_save_screw_blocks(editor: PatcherEditor):
+def patch_a7_save_screw_blocks(editor: PatcherEditor) -> None:
     area7 = editor.get_file(
         "maps/levels/c10_samus/s090_area9/s090_area9.bmsbk", Bmsbk
     )
     area7.raw["block_groups"][56]["types"][0]["block_type"] = "power_beam"
 
 
-def shoot_supers_without_missiles(editor: PatcherEditor):
+def shoot_supers_without_missiles(editor: PatcherEditor) -> None:
     samus_bmsad = editor.get_file(
         "actors/characters/samus/charclasses/samus.bmsad", Bmsad
     )
     samus_bmsad.raw["components"]["GUN"]["functions"][20]["params"]["Param5"]["value"] = "ITEM_MISSILE_CHECK"
 
 
-def nerf_ridley_fight(editor: PatcherEditor):
+def nerf_ridley_fight(editor: PatcherEditor) -> None:
     '''
     All beams (except Ice) will use the same factor as Plasma which is 0.12
     Power Beam: 25 -> 3
     Ice: 10
     Wave: 50 -> 6
     Spazer: 210 -> 25.2
     Plasma: 36 (default from ridley tunable)
@@ -140,15 +141,15 @@
     ridley_tunables["fPlasmaBeamWeaponBoostPhaseDisplacement"]["value"] = 1.1
     ridley_tunables["fGrabPlasmaBeam"]["value"] = 1.0
     ridley_tunables["fGrabPlasmaBeamCharge"]["value"] = 1.0
     ridley_tunables["fGrabPlasmaBeamWeaponBoost"]["value"] = 1.1
     ridley_tunables["fGrabPlasmaBeamWeaponBoostPhaseDisplacement"]["value"] = 1.1
 
 
-def increase_pb_drop_chance(editor: PatcherEditor):
+def increase_pb_drop_chance(editor: PatcherEditor) -> None:
     ACTOR_FILES = [
         "alpha",
         "alphaevolved",
         "alphanewborn",
         "autoad",
         "autoadblack",
         "autrack",
@@ -198,15 +199,15 @@
         elif drop["fPowerBombProbability"]["value"] == 0.0:
             drop["fPowerBombProbability"]["value"] = 0.1
         # All other enemies excluding Blobthrower
         else:
             drop["fPowerBombProbability"]["value"] *= 2
 
 
-def fix_wrong_cc_actor_deletions(editor: PatcherEditor):
+def fix_wrong_cc_actor_deletions(editor: PatcherEditor) -> None:
     # Prevents hidden item actors from being deleted when its block is broken from an adjacent cc
     CUSTOM_BLOCK = Container({
         "pos": ListContainer([
             -10350.0,
             -1850.0,
             0.0,
         ]),
@@ -269,23 +270,24 @@
             if scenario_name == "s000_surface":
                 new_group = copy.deepcopy(BEAM_GROUP)
                 # Add the missing collision_camera entry
                 bmsbk.raw.collision_cameras.append(BMSBK_GROUP)
             else:
                 new_group = copy.deepcopy(BOMB_GROUP)
             new_block = copy.deepcopy(CUSTOM_BLOCK)
-            new_block.pos = pos
-            new_block.name1 = sg_casca
-            new_group.types[0].blocks.append(new_block)
+            new_block["pos"] = pos
+            new_block["name1"] = sg_casca
+            types: ListContainer = typing.cast(ListContainer, new_group["types"])
+            types[0]["blocks"].append(new_block)
             bmsbk.raw.block_groups.append(new_group)
             bmsbk_cc_obj = next(cc_obj for cc_obj in bmsbk.raw.collision_cameras if cc_name in cc_obj.name)
             bmsbk_cc_obj.entries.append(len(bmsbk.raw.block_groups) - 1)
 
 
-def apply_static_fixes(editor: PatcherEditor):
+def apply_static_fixes(editor: PatcherEditor) -> None:
     patch_multi_room_gammas(editor)
     patch_pickup_rotation(editor)
     patch_pickup_position(editor)
     remove_area7_grapple_block(editor)
     patch_a7_save_screw_blocks(editor)
     shoot_supers_without_missiles(editor)
     nerf_ridley_fight(editor)
```

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando/specific_patches/tunable_patches.py` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando/specific_patches/tunable_patches.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from mercury_engine_data_structures.formats.bmtun import Bmtun
 from open_samus_returns_rando.patcher_editor import PatcherEditor
 
 
-def patch_tunables(editor: PatcherEditor, configuration: dict):
+def patch_tunables(editor: PatcherEditor, configuration: dict) -> None:
     tunables = editor.get_file("system/tunables/tunables.bmtun", Bmtun)
     _patch_scan_pulse(tunables)
     _reserves_per_tank(tunables, configuration)
 
 
-def _patch_scan_pulse(tunables: Bmtun):
+def _patch_scan_pulse(tunables: Bmtun) -> None:
     tunables.raw["classes"]["CTunableAbilityScanningPulse"]["tunables"][
         "fConsumptionOnActivation"
     ]["value"] = 0.0
 
 
-def _reserves_per_tank(tunables: Bmtun, configuration: dict):
+def _reserves_per_tank(tunables: Bmtun, configuration: dict) -> None:
     amiibo = tunables.raw["classes"]["Amiibo|CTunableReserveTanks"]["tunables"]
     amiibo["fLifeTankSize"]["value"] = configuration["life_tank_size"]
     amiibo["fSETankSize"]["value"] = configuration["aeion_tank_size"]
     amiibo["fMissileTankSize"]["value"] = configuration["missile_tank_size"]
     amiibo["fSuperMissileTankSize"]["value"] = configuration["super_missile_tank_size"]
```

### Comparing `open_samus_returns_rando-1.2.2/src/open_samus_returns_rando.egg-info/PKG-INFO` & `open_samus_returns_rando-1.3.0/src/open_samus_returns_rando.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 Metadata-Version: 2.1
 Name: open_samus_returns_rando
-Version: 1.2.2
+Version: 1.3.0
 Summary: An open source randomizer patcher for Metroid: Samus Returns.
 Project-URL: Homepage, https://github.com/randovania/open-samus-returns-rando
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mercury-engine-data-structures>=0.27.0
 Requires-Dist: jsonschema>=4.0.0
 Requires-Dist: ips.py>=0.1.2
+Provides-Extra: typing
+Requires-Dist: types-jsonschema; extra == "typing"
+Requires-Dist: construct-typing; extra == "typing"
+Requires-Dist: types-pyinstaller; extra == "typing"
+Requires-Dist: mypy; extra == "typing"
 
 # Open Samus Returns Rando
 Open Source randomizer patcher for Metroid: Samus Returns. Intended for use in [Randovania](https://github.com/randovania).
 Currently supports patching the following:
-- Starting items
-- Starting location
-- Pickups
+- Starting Items
+- Starting Location
+- Pickups (Vanilla and Custom)
 - Items on Metroids
-- Shuffled DNA/Baby Metroid
+- Shuffled DNA
+- Shuffled Baby Metroid
+- Elevator Destinations
+- Door Types
 
 ## Installation and Usage
 `pip install open-samus-returns-rando`
 
 You will need to provide JSON data matching the [JSON schema](https://github.com/randovania/open-samus-returns-rando/blob/main/src/open_samus_returns_rando/files/schema.json) in order to successfully patch the game.
 
 The patcher expects a path to an extracted romfs directory of Metroid: Samus Returns as well as the desired output directory. Output files are in a format compatible with either Luma3DS or Citra.
```

### Comparing `open_samus_returns_rando-1.2.2/tests/test_files/item_models_test.json` & `open_samus_returns_rando-1.3.0/tests/test_files/item_models_test.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9952380952380953%*

 * *Differences: {"'debug_custom_pickups'": "{insert: [(33, OrderedDict([('new_actor', OrderedDict([('actor', "*

 * *                           "'another_pickup34'), ('scenario', 's000_surface')])), ('location', "*

 * *                           "OrderedDict([('x', -7000.0), ('y', 2100.0), ('z', 0.0)])), "*

 * *                           "('collision_camera_name', 'collision_camera_000')])), (34, "*

 * *                           "OrderedDict([('new_actor', OrderedDict([('actor', 'another_pickup35'), "*

 * *                           "('scenario',  […]*

```diff
@@ -713,14 +713,38 @@
                 "y": 2100.0,
                 "z": 0.0
             },
             "new_actor": {
                 "actor": "another_pickup33",
                 "scenario": "s000_surface"
             }
+        },
+        {
+            "collision_camera_name": "collision_camera_000",
+            "location": {
+                "x": -7000.0,
+                "y": 2100.0,
+                "z": 0.0
+            },
+            "new_actor": {
+                "actor": "another_pickup34",
+                "scenario": "s000_surface"
+            }
+        },
+        {
+            "collision_camera_name": "collision_camera_000",
+            "location": {
+                "x": -6900.0,
+                "y": 2100.0,
+                "z": 0.0
+            },
+            "new_actor": {
+                "actor": "another_pickup35",
+                "scenario": "s000_surface"
+            }
         }
     ],
     "energy_per_tank": 100,
     "game_patches": {},
     "hints": [],
     "new_spawn_points": [
         {
@@ -1389,14 +1413,52 @@
                     },
                     {
                         "item_id": "ITEM_MISSILE_TANKS",
                         "quantity": 3
                     }
                 ]
             ]
+        },
+        {
+            "caption": "Sent Ice Missile to Metroid Dread.",
+            "model": [
+                "powerup_icemissile"
+            ],
+            "pickup_actor": {
+                "actor": "another_pickup34",
+                "scenario": "s000_surface"
+            },
+            "pickup_type": "actor",
+            "resources": [
+                [
+                    {
+                        "item_id": "ITEM_WEAPON_ICE_MISSILE",
+                        "quantity": 1
+                    }
+                ]
+            ]
+        },
+        {
+            "caption": "Sent [Item] to [Player].",
+            "model": [
+                "item_offworld"
+            ],
+            "pickup_actor": {
+                "actor": "another_pickup35",
+                "scenario": "s000_surface"
+            },
+            "pickup_type": "actor",
+            "resources": [
+                [
+                    {
+                        "item_id": "ITEM_OFFWORLD",
+                        "quantity": 1
+                    }
+                ]
+            ]
         }
     ],
     "reveal_map_on_start": false,
     "starting_items": {
         "ITEM_MAX_LIFE": 99,
         "ITEM_MAX_SPECIAL_ENERGY": 1000,
         "ITEM_METROID_COUNT": 0,
```

### Comparing `open_samus_returns_rando-1.2.2/tests/test_files/starter_preset_patcher.json` & `open_samus_returns_rando-1.3.0/tests/test_files/starter_preset_patcher.json`

 * *Files identical despite different names*

