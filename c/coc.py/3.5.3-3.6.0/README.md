# Comparing `tmp/coc_py-3.5.3.tar.gz` & `tmp/coc_py-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coc_py-3.5.3.tar", last modified: Tue May 14 18:24:18 2024, max compression
+gzip compressed data, was "coc_py-3.6.0.tar", last modified: Fri May 17 16:52:29 2024, max compression
```

## Comparing `coc_py-3.5.3.tar` & `coc_py-3.6.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:24:18.676546 coc_py-3.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-14 18:24:14.000000 coc_py-3.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-14 18:24:14.000000 coc_py-3.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-05-14 18:24:18.676546 coc_py-3.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-05-14 18:24:14.000000 coc_py-3.5.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:24:18.660546 coc_py-3.5.3/coc/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15861 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/abc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/clans.py
--rw-r--r--   0 runner    (1001) docker     (127)    83549 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9189 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/entry_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    41186 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    12992 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/events.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:24:18.656546 coc_py-3.5.3/coc/ext/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:24:18.664546 coc_py-3.5.3/coc/ext/discordlinks/
--rw-r--r--   0 runner    (1001) docker     (127)     9498 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/ext/discordlinks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:24:18.664546 coc_py-3.5.3/coc/ext/fullwarapi/
--rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/ext/fullwarapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:24:18.664546 coc_py-3.5.3/coc/ext/triggers/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/ext/triggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/ext/triggers/cron.py
--rw-r--r--   0 runner    (1001) docker     (127)    21909 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/ext/triggers/triggers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/hero.py
--rw-r--r--   0 runner    (1001) docker     (127)    24212 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/iterators.py
--rw-r--r--   0 runner    (1001) docker     (127)    21699 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/miscmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/player_clan.py
--rw-r--r--   0 runner    (1001) docker     (127)    30024 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/players.py
--rw-r--r--   0 runner    (1001) docker     (127)    19577 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/raid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/spell.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:24:18.672546 coc_py-3.5.3/coc/static/
--rw-r--r--   0 runner    (1001) docker     (127)  1291668 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/static/buildings.json
--rw-r--r--   0 runner    (1001) docker     (127)  1965460 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/static/characters.json
--rw-r--r--   0 runner    (1001) docker     (127)   220960 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/static/equipment.json
--rw-r--r--   0 runner    (1001) docker     (127)   648975 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/static/heroes.json
--rw-r--r--   0 runner    (1001) docker     (127)   255626 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/static/pets.json
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/static/spell_ids.json
--rw-r--r--   0 runner    (1001) docker     (127)   566845 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/static/spells.json
--rw-r--r--   0 runner    (1001) docker     (127)     8699 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/static/supers.json
--rw-r--r--   0 runner    (1001) docker     (127)  1025147 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/static/texts_EN.json
--rw-r--r--   0 runner    (1001) docker     (127)    92590 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/static/townhall_levels.json
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/static/troop_ids.json
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/static/update_static.py
--rw-r--r--   0 runner    (1001) docker     (127)     8451 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/troop.py
--rw-r--r--   0 runner    (1001) docker     (127)    19780 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4595 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/war_attack.py
--rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/war_clans.py
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/war_members.py
--rw-r--r--   0 runner    (1001) docker     (127)    19658 2024-05-14 18:24:14.000000 coc_py-3.5.3/coc/wars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:24:18.676546 coc_py-3.5.3/coc.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-05-14 18:24:18.000000 coc_py-3.5.3/coc.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-14 18:24:18.000000 coc_py-3.5.3/coc.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 18:24:18.000000 coc_py-3.5.3/coc.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-14 18:24:18.000000 coc_py-3.5.3/coc.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-14 18:24:18.000000 coc_py-3.5.3/coc.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-14 18:24:14.000000 coc_py-3.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 18:24:14.000000 coc_py-3.5.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 18:24:18.676546 coc_py-3.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-14 18:24:14.000000 coc_py-3.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:24:18.676546 coc_py-3.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-05-14 18:24:14.000000 coc_py-3.5.3/tests/test_capitalraidseasons.py
--rw-r--r--   0 runner    (1001) docker     (127)    12050 2024-05-14 18:24:14.000000 coc_py-3.5.3/tests/test_clans.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-14 18:24:14.000000 coc_py-3.5.3/tests/test_clash_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:24:14.000000 coc_py-3.5.3/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:24:14.000000 coc_py-3.5.3/tests/test_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:24:14.000000 coc_py-3.5.3/tests/test_login.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:24:14.000000 coc_py-3.5.3/tests/test_miscmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)    10293 2024-05-14 18:24:14.000000 coc_py-3.5.3/tests/test_players.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-14 18:24:14.000000 coc_py-3.5.3/tests/test_troop_levels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-14 18:24:14.000000 coc_py-3.5.3/tests/test_wars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:52:29.361730 coc_py-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-17 16:52:24.000000 coc_py-3.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-17 16:52:24.000000 coc_py-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-05-17 16:52:29.361730 coc_py-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-05-17 16:52:24.000000 coc_py-3.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:52:29.349730 coc_py-3.6.0/coc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15861 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11864 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/clans.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83797 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9189 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/entry_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41186 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12992 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/events.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:52:29.341730 coc_py-3.6.0/coc/ext/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:52:29.349730 coc_py-3.6.0/coc/ext/discordlinks/
+-rw-r--r--   0 runner    (1001) docker     (127)     9498 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/ext/discordlinks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:52:29.349730 coc_py-3.6.0/coc/ext/fullwarapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/ext/fullwarapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:52:29.349730 coc_py-3.6.0/coc/ext/triggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/ext/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/ext/triggers/cron.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21905 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/ext/triggers/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/hero.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24332 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21685 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/miscmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/player_clan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29950 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/players.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19577 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/raid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/spell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:52:29.357730 coc_py-3.6.0/coc/static/
+-rw-r--r--   0 runner    (1001) docker     (127)  1291668 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/static/buildings.json
+-rw-r--r--   0 runner    (1001) docker     (127)  1965460 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/static/characters.json
+-rw-r--r--   0 runner    (1001) docker     (127)   220960 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/static/equipment.json
+-rw-r--r--   0 runner    (1001) docker     (127)   648975 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/static/heroes.json
+-rw-r--r--   0 runner    (1001) docker     (127)   255626 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/static/pets.json
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/static/spell_ids.json
+-rw-r--r--   0 runner    (1001) docker     (127)   566845 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/static/spells.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8699 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/static/supers.json
+-rw-r--r--   0 runner    (1001) docker     (127)  1025147 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/static/texts_EN.json
+-rw-r--r--   0 runner    (1001) docker     (127)    92590 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/static/townhall_levels.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/static/troop_ids.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/static/update_static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8451 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/troop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19780 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4595 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/war_attack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/war_clans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/war_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19658 2024-05-17 16:52:24.000000 coc_py-3.6.0/coc/wars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:52:29.361730 coc_py-3.6.0/coc.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-05-17 16:52:29.000000 coc_py-3.6.0/coc.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-17 16:52:29.000000 coc_py-3.6.0/coc.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 16:52:29.000000 coc_py-3.6.0/coc.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-17 16:52:29.000000 coc_py-3.6.0/coc.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-17 16:52:29.000000 coc_py-3.6.0/coc.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-17 16:52:24.000000 coc_py-3.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-17 16:52:24.000000 coc_py-3.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 16:52:29.361730 coc_py-3.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-17 16:52:24.000000 coc_py-3.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:52:29.361730 coc_py-3.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-05-17 16:52:24.000000 coc_py-3.6.0/tests/test_capitalraidseasons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12050 2024-05-17 16:52:24.000000 coc_py-3.6.0/tests/test_clans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-17 16:52:24.000000 coc_py-3.6.0/tests/test_clash_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 16:52:24.000000 coc_py-3.6.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 16:52:24.000000 coc_py-3.6.0/tests/test_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 16:52:24.000000 coc_py-3.6.0/tests/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 16:52:24.000000 coc_py-3.6.0/tests/test_miscmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10293 2024-05-17 16:52:24.000000 coc_py-3.6.0/tests/test_players.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-17 16:52:24.000000 coc_py-3.6.0/tests/test_troop_levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-17 16:52:24.000000 coc_py-3.6.0/tests/test_wars.py
```

### Comparing `coc_py-3.5.3/LICENSE` & `coc_py-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/PKG-INFO` & `coc_py-3.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coc.py
-Version: 3.5.3
+Version: 3.6.0
 Summary: A python wrapper for the Clash of Clans API
 Author: mathsman5133
 Maintainer: majordoobie, MagicTheDev, Kuchenmampfer, lukasthaler, doluk
 License: MIT
 Project-URL: documentation, https://cocpy.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/mathsman5133/coc.py
 Project-URL: changelog, https://cocpy.readthedocs.io/en/latest/miscellaneous/changelog.html
```

### Comparing `coc_py-3.5.3/README.rst` & `coc_py-3.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/coc/__init__.py` & `coc_py-3.6.0/coc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-__version__ = "3.5.3"
+__version__ = "3.6.0"
 
 from .abc import BasePlayer, BaseClan
 from .clans import RankedClan, Clan
 from .client import Client
 from .events import PlayerEvents, ClanEvents, WarEvents, EventsClient, ClientEvents
 from .enums import (
     PlayerHouseElementType,
```

### Comparing `coc_py-3.5.3/coc/abc.py` & `coc_py-3.6.0/coc/abc.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/coc/clans.py` & `coc_py-3.6.0/coc/clans.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,15 @@
             self._iter_capital_districts = (capital_district_cls(data=cddata, client=self._client) for cddata in
                                             data_get("clanCapital")["districts"])
         else:
             self._iter_capital_districts = ()
 
     @cached_property("_cs_labels")
     def labels(self) -> typing.List[Label]:
-        """List[:class:`Label`]: A :class:`List` of :class:`Label`s that the clan has."""
+        """List[:class:`Label`]: A :class:`List` of :class:`Label`\s that the clan has."""
         return list(self._iter_labels)
 
     @cached_property("_cs_members")
     def members(self) -> typing.List[ClanMember]:
         """List[:class:`ClanMember`]: A list of members that belong to the clan."""
         return list(self.members_dict.values())
```

### Comparing `coc_py-3.5.3/coc/client.py` & `coc_py-3.6.0/coc/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,22 +141,27 @@
         the original json data as returned by the API. This can be useful if you want to store a response in a database
         for later use or are interested in new things that coc.py does not support otherwise yet. But because this
         increases the memory footprint and is not needed for most use cases, this defaults to ``False``.
 
     base_url: :class:`str`
         The base URL to use for API requests. Defaults to "https://api.clashofclans.com/v1"
 
+    ip: :class:`str`
+        The IP address to use for API requests. Defaults to None, which means the IP address will be automatically
+        detected.
+
     Attributes
     ----------
     loop : :class:`asyncio.AbstractEventLoop`
         The loop that is used for HTTP requests
     """
 
     __slots__ = (
         "base_url",
+        "ip",
         "loop",
         "correct_key_count",
         "key_names",
         "key_scopes",
         "throttle_limit",
         "throttler",
         "timeout",
@@ -193,14 +198,15 @@
         timeout: float = 30.0,
         cache_max_size: int = 10000,
         stats_max_size: int = 1000,
         load_game_data: LoadGameData = LoadGameData(default=True),
         realtime=False,
         raw_attribute=False,
         base_url: str = "https://api.clashofclans.com/v1",
+        ip: Optional[str] = None,
         **kwargs,
     ):
 
         self.loop = loop or asyncio.get_event_loop()
 
         self.correct_key_count = max(min(KEY_MAXIMUM, key_count), KEY_MINIMUM)
 
@@ -218,14 +224,15 @@
 
         self.http = None  # set in method login()
         self.realtime = realtime
         self.raw_attribute = raw_attribute
         self.correct_tags = correct_tags
         self.load_game_data = load_game_data
         self.base_url = base_url
+        self.ip = ip
         # cache
         self._players = {}
         self._clans = {}
         self._wars = {}
 
     async def __aenter__(self):
         return self
@@ -243,14 +250,15 @@
             loop=self.loop,
             key_count=self.correct_key_count,
             throttle_limit=self.throttle_limit,
             throttler=self.throttler,
             cache_max_size=self.cache_max_size,
             stats_max_size=self.stats_max_size,
             base_url=self.base_url,
+            ip=self.ip,
         )
 
     def _load_holders(self):
         with open(ENGLISH_ALIAS_PATH) as fp:
             english_aliases = ujson.load(fp)
 
         with open(BUILDING_FILE_PATH) as fp:
```

### Comparing `coc_py-3.5.3/coc/entry_logs.py` & `coc_py-3.6.0/coc/entry_logs.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/coc/enums.py` & `coc_py-3.6.0/coc/enums.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/coc/errors.py` & `coc_py-3.6.0/coc/errors.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/coc/events.py` & `coc_py-3.6.0/coc/events.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/coc/events.pyi` & `coc_py-3.6.0/coc/events.pyi`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/coc/ext/discordlinks/__init__.py` & `coc_py-3.6.0/coc/ext/discordlinks/__init__.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/coc/ext/fullwarapi/__init__.py` & `coc_py-3.6.0/coc/ext/fullwarapi/__init__.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/coc/ext/triggers/cron.py` & `coc_py-3.6.0/coc/ext/triggers/cron.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/coc/ext/triggers/triggers.py` & `coc_py-3.6.0/coc/ext/triggers/triggers.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,15 @@
         have fully loaded and initialized. If you choose to disable autostart (which is the default),
         you can use `coc.ext.triggers.start_triggers()` to manually kick the trigger execution off once you
         have loaded all required resources
 
     error_handler: Optional[:class:`coc.ext.triggers.CoroFunction`]
         an optional coroutine function that will be called on each error incurred during the trigger execution.
         The handler will receive three arguments:
+
             function_name: :class:`str`
                 the name of the failing trigger's decorated function
             arg: Optional[:class:`Any`]
                 the failing `iter_args` element or None if no iter_args are defined
             exception: :class:`Exception`
                 the exception that occurred
 
@@ -316,14 +317,15 @@
         have fully loaded and initialized. If you choose to disable autostart (which is the default),
         you can use `coc.ext.triggers.start_triggers()` to manually kick the trigger execution off once you
         have loaded all required resources
 
     error_handler: Optional[:class:`coc.ext.triggers.CoroFunction`]
         an optional coroutine function that will be called on each error incurred during the trigger execution.
         The handler will receive three arguments:
+
             function_name: :class:`str`
                 the name of the failing trigger's decorated function
             arg: Optional[:class:`Any`]
                 the failing `iter_args` element or None if no iter_args are defined
             exception: :class:`Exception`
                 the exception that occurred
 
@@ -336,20 +338,21 @@
         the trigger will provision one using `asyncio.get_event_loop()`
 
     kwargs:
         any additional keyword arguments that will be passed to the decorated function every time it is called
 
 
     Example
-    ----------
+    -------
+
     .. code-block:: python3
 
         @CronTrigger(cron_schedule='0 0 * * *', iter_args=['#2PP', '#2PPP'])
         async def download_current_war(clan_tag: str):
-            # use your coc client to fetch war data, store it to a file or database, ...
+            # use your coc client to fetch war data, store it to a file or database,
             pass
 
     """
 
     def __init__(self,
                  *,  # disable positional arguments
                  cron_schedule: Union[CronSchedule, str],
```

### Comparing `coc_py-3.5.3/coc/hero.py` & `coc_py-3.6.0/coc/hero.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/coc/http.py` & `coc_py-3.6.0/coc/http.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,14 +196,15 @@
             key_count,
             key_scopes,
             throttle_limit,
             throttler=BasicThrottler,
             cache_max_size=10000,
             stats_max_size=1000,
             base_url="https://api.clashofclans.com/v1",
+            ip=None,
     ):
         self.client = client
         self.loop = loop
         self.email = email
         self.password = password
         self.key_names = key_names
         self.key_count = key_count
@@ -218,14 +219,15 @@
         self.stats = stats_max_size and HTTPStats(max_size=stats_max_size)
         if base_url and isinstance(base_url, str) and len(base_url) > 0:
             if base_url.endswith("/"):
                 base_url = base_url[:-1]
             self.base_url = base_url
         else:
             raise ValueError("base_url must be a string and not empty.")
+        self.ip = ip
         if issubclass(throttler, BasicThrottler):
             self.__throttle = throttler(1 / per_second)
         elif issubclass(throttler, BatchThrottler):
             self.__throttle = throttler(per_second)
         else:
             raise TypeError("throttler must be either BasicThrottler or BatchThrottler.")
 
@@ -503,16 +505,18 @@
                 LOG.error("Invalid credentials used when attempting to log in")
                 await self.close()
                 raise InvalidCredentials()
 
             LOG.info("Successfully logged into the developer site.")
 
             resp_payload = await resp.json()
-            ip = json_loads(base64_b64decode(resp_payload["temporaryAPIToken"].split(".")[1] + "====").decode("utf-8"))["limits"][1]["cidrs"][0].split("/")[0]
-
+            if not self.ip:
+                ip = json_loads(base64_b64decode(resp_payload["temporaryAPIToken"].split(".")[1] + "====").decode("utf-8"))["limits"][1]["cidrs"][0].split("/")[0]
+            else:
+                ip = self.ip
             LOG.info("Found IP address to be %s", ip)
 
             resp = await session.post("https://developer.clashofclans.com/api/apikey/list")
             keys = (await resp.json())["keys"]
             for key in keys:
                 LOG.debug(f"Key {key}")
                 if key["name"] != self.key_names or ip not in key["cidrRanges"]:
```

### Comparing `coc_py-3.5.3/coc/iterators.py` & `coc_py-3.6.0/coc/iterators.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/coc/miscmodels.py` & `coc_py-3.6.0/coc/miscmodels.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,15 +386,15 @@
         :class:`str` - URL for a small sized badge (70x70).
     medium:
         :class:`str` - URL for a medium sized badge (200x200).
     large:
         :class:`str` - URL for a large sized badge (512x512).
     """
 
-    __slots__ = ("small", "medium", "large", "url", "_client")
+    __slots__ = ("small", "medium", "large", "_client")
 
     def __repr__(self):
         attrs = [
             ("url", self.url),
         ]
         return "<%s %s>" % (self.__class__.__name__, " ".join("%s=%r" % t for t in attrs),)
 
@@ -455,15 +455,15 @@
         :class:`str`: URL for a tiny sized icon (32x32).
     small:
         :class:`str`: URL for a small sized icon (72x72).
     medium:
         :class:`str`: URL for a medium sized icon (288x288).
     """
 
-    __slots__ = ("small", "medium", "tiny", "url", "_client")
+    __slots__ = ("small", "medium", "tiny", "_client")
 
     def __repr__(self):
         attrs = [
             ("url", self.url),
         ]
         return "<%s %s>" % (self.__class__.__name__, " ".join("%s=%r" % t for t in attrs),)
```

### Comparing `coc_py-3.5.3/coc/player_clan.py` & `coc_py-3.6.0/coc/player_clan.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/coc/players.py` & `coc_py-3.6.0/coc/players.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,20 +168,21 @@
             player = await client.get_player('tag')
             clan = await player.get_detailed_clan()
         """
         return self.clan and await self._client.get_clan(self.clan.tag)
 
     @cached_property("_cs_player_house_elements")
     def player_house_elements(self) -> List[PlayerHouseElement]:
-        """List[:class:`PlayerHouseElement`]: A :class:`List` of :class:`PlayerHouseElement`s that the player has."""
+        """List[:class:`PlayerHouseElement`]: A :class:`List` of :class:`PlayerHouseElement`\s that the player has."""
         return list(self._iter_player_house_elements)
 
 
 class RankedPlayer(ClanMember):
-    """Represents a leaderboard-ranked player.
+    """
+    Represents a leaderboard-ranked player.
 
     Attributes
     ----------
     attack_wins: :class:`int`
         The player's number of attack wins. If retrieving info for builder base leader-boards, this will be ``None``.
     defense_wins: :class:`int`
         The player's number of defense wins. If retrieving info for builder base leader-boards, this will be ``None``.
@@ -205,15 +206,16 @@
         self.defense_wins: int = data_get("defenseWins")
         self.builder_base_trophies: int = data_get("builderBaseTrophies")
         self.rank: int = data_get("rank")
         self.previous_rank: int = data_get("previousRank")
 
 
 class Player(ClanMember):
-    """Represents a Clash of Clans Player.
+    """
+    Represents a Clash of Clans Player.
 
     Attributes
     ----------
     achievement_cls: :class:`Achievement`
         The constructor used to create the :attr:`Player.achievements` list.
         This must inherit from :class:`Achievement`.
     hero_cls: :class:`Hero`
@@ -243,16 +245,14 @@
     clan_capital_contributions: :class:`int`
         The player's total contribution to clan capitals
     legend_statistics: Optional[:class:`LegendStatistics`]
         The player's legend statistics, or ``None`` if they have never been in the legend league.
     war_opted_in: Optional[:class:`bool`]
         Whether the player has selected that they are opted "in" (True) for wars, or opted "out" (False).
         This will be ``None`` if the player is not in a clan.
-    equipment: List[:class:`Equipment`]
-        The player's unlocked hero equipment
     """
 
     __slots__ = (
         "clan",
         "attack_wins",
         "defense_wins",
         "best_trophies",
@@ -358,15 +358,15 @@
         except KeyError:
             # not in a clan / war preference not there
             self.war_opted_in: Optional[bool] = None
 
         label_cls = self.label_cls
         achievement_cls = self.achievement_cls
         troop_loader = self._client._troop_holder.load if self._client else None
-        hero_loader =  self._client._hero_holder.load if self._client else None
+        hero_loader = self._client._hero_holder.load if self._client else None
         spell_loader = self._client._spell_holder.load if self._client else None
         pet_loader = self._client._pet_holder.load if self._client else None
         equipment_loader = self._client._equipment_holder.load if self._client else None
 
         if self._game_files_loaded:
             pet_lookup = [p.name for p in self._client._pet_holder.items]
             equipment_lookup = [e.name for e in self._client._equipment_holder.items]
@@ -458,15 +458,15 @@
                         base = holder.get(item.name, item.is_home_base)
                         item._load_from_parent(base)
                     else:
                         item._load_from_parent(holder.get(item.name))
 
     @cached_property("_cs_labels")
     def labels(self) -> List[Label]:
-        """List[:class:`Label`]: A :class:`List` of :class:`Label`s that the player has."""
+        """List[:class:`Label`]: A :class:`List` of :class:`Label`\s that the player has."""
         return list(self._iter_labels)
 
     @cached_property("_cs_achievements")
     def achievements(self) -> List[Achievement]:
         """List[:class:`Achievement`]: A list of the player's achievements."""
         # at the time of writing, the API presents achievements in the order
         # added to the game which doesn't match in-game order.
@@ -543,15 +543,15 @@
 
         return troops
 
     @cached_property("_cs_home_troops")
     def home_troops(self) -> List[Troop]:
         """List[:class:`Troop`]: A :class:`List` of the player's home-base :class:`Troop`.
 
-        This will return troops in the order found in both barracks and labatory in-game.
+        This will return troops in the order found in both barracks and laboratory in-game.
 
         This includes:
         - Elixir Troops (Barbarian, Balloon, etc.)
         - Dark Elixir Troops (Minion, Hog Rider, etc.)
         - Siege Machines (Log Launcher, etc.)
         - **Boosted** Super Troops
         """
@@ -562,15 +562,15 @@
 
         return list(sorted(self._home_troops.values(), key=lambda t: order.get(t.name, 0)))
 
     @cached_property("_cs_builder_troops")
     def builder_troops(self) -> List[Troop]:
         """List[:class:`Troop`]: A :class:`List` of the player's builder-base :class:`Troop`.
 
-        This will return troops in the order found in both barracks and labatory in-game.
+        This will return troops in the order found in both barracks and laboratory in-game.
 
         This includes:
         - Builder troops
         """
         order = {k: v for v, k in enumerate(BUILDER_TROOPS_ORDER)}
 
         if not self._builder_troops:
@@ -578,15 +578,15 @@
 
         return list(sorted(self._builder_troops.values(), key=lambda t: order.get(t.name, 0)))
 
     @cached_property("_cs_siege_machines")
     def siege_machines(self) -> List[Troop]:
         """List[:class:`Troop`]: A :class:`List` of the player's siege-machine :class:`Troop`.
 
-        This will return siege machines in the order found in both barracks and labatory in-game.
+        This will return siege machines in the order found in both barracks and laboratory in-game.
 
         This includes:
         - Siege machines only.
         """
         order = {k: v for v, k in enumerate(SIEGE_MACHINE_ORDER)}
         troops = (t for t in self.troops if t.name in SIEGE_MACHINE_ORDER or t.is_siege_machine)
         return list(sorted(troops, key=lambda t: order.get(t.name, 0)))
@@ -695,15 +695,15 @@
             builder and home troops.
         default_value
             The value to return if the ``name`` is not found. Defaults to ``None``.
 
         Returns
         --------
         Optional[:class:`Troop`]
-            The returned troop or the ``default_value`` if not found, which defaults to ``None``..
+            The returned troop or the ``default_value`` if not found, which defaults to ``None``.
         """
         _ = self.troops
 
         if is_home_troop is None:
             lookup = {**self._builder_troops, **self._home_troops}
         elif is_home_troop is True:
             lookup = self._home_troops
@@ -717,15 +717,15 @@
         except KeyError:
             return default_value
 
     @cached_property("_cs_heroes")
     def heroes(self) -> List[Hero]:
         """List[:class:`Hero`]: A :class:`List` of the player's :class:`Hero`.
 
-        This will return heroes in the order found in the store and labatory in-game.
+        This will return heroes in the order found in the store and laboratory in-game.
         """
         heroes_dict = {h.name: h for h in self._iter_heroes}
         sorted_heroes = {}
         for name in HERO_ORDER:
             # have to do it this way because it's less expensive than removing None's if they don't have a troop.
             try:
                 sorted_heroes[name] = heroes_dict[name]
@@ -759,38 +759,38 @@
         except KeyError:
             return default_value
 
     @cached_property("_cs_spells")
     def spells(self) -> List[Spell]:
         """List[:class:`Spell`]: A :class:`List` of the player's :class:`Spell` ordered as they appear in-game.
 
-        This will return spells in the order found in both spell factory and labatory in-game.
+        This will return spells in the order found in both spell factory and laboratory in-game.
         """
         self._spells = {s.name: s for s in self._iter_spells}
         dict_spells = self._spells
         order = {k: v for v, k in enumerate(SPELL_ORDER)}
 
         return list(sorted(
-                    dict_spells.values(),
-                    key=lambda s: order.get(s.name, 0)))
+                dict_spells.values(),
+                key=lambda s: order.get(s.name, 0)))
 
     def get_spell(self, name: str, default_value=None) -> Optional[Spell]:
         """Gets the spell with the given name.
 
         Parameters
         -----------
         name: :class:`str`
             The name of a spell as found in-game.
         default_value:
             The default value to return if a spell with ``name`` is not found. Defaults to ``None``.
 
         Returns
         --------
         Optional[:class:`Spell`]
-            The returned spell or the ``default_value`` if not found, which defaults to ``None``..
+            The returned spell or the ``default_value`` if not found, which defaults to ``None``.
         """
         if not self._spells:
             _ = self.spells
 
         try:
             return self._spells[name]
         except KeyError:
```

### Comparing `coc_py-3.5.3/coc/raid.py` & `coc_py-3.6.0/coc/raid.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/coc/spell.py` & `coc_py-3.6.0/coc/spell.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/coc/static/buildings.json` & `coc_py-3.6.0/coc/static/buildings.json`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/coc/static/characters.json` & `coc_py-3.6.0/coc/static/characters.json`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/coc/static/equipment.json` & `coc_py-3.6.0/coc/static/equipment.json`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/coc/static/heroes.json` & `coc_py-3.6.0/coc/static/heroes.json`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/coc/static/pets.json` & `coc_py-3.6.0/coc/static/pets.json`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/coc/static/spells.json` & `coc_py-3.6.0/coc/static/spells.json`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/coc/static/supers.json` & `coc_py-3.6.0/coc/static/supers.json`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/coc/static/texts_EN.json` & `coc_py-3.6.0/coc/static/texts_EN.json`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/coc/static/townhall_levels.json` & `coc_py-3.6.0/coc/static/townhall_levels.json`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/coc/static/troop_ids.json` & `coc_py-3.6.0/coc/static/troop_ids.json`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/coc/static/update_static.py` & `coc_py-3.6.0/coc/static/update_static.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/coc/troop.py` & `coc_py-3.6.0/coc/troop.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/coc/utils.py` & `coc_py-3.6.0/coc/utils.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/coc/war_attack.py` & `coc_py-3.6.0/coc/war_attack.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/coc/war_clans.py` & `coc_py-3.6.0/coc/war_clans.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/coc/war_members.py` & `coc_py-3.6.0/coc/war_members.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/coc/wars.py` & `coc_py-3.6.0/coc/wars.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/coc.py.egg-info/PKG-INFO` & `coc_py-3.6.0/coc.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coc.py
-Version: 3.5.3
+Version: 3.6.0
 Summary: A python wrapper for the Clash of Clans API
 Author: mathsman5133
 Maintainer: majordoobie, MagicTheDev, Kuchenmampfer, lukasthaler, doluk
 License: MIT
 Project-URL: documentation, https://cocpy.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/mathsman5133/coc.py
 Project-URL: changelog, https://cocpy.readthedocs.io/en/latest/miscellaneous/changelog.html
```

### Comparing `coc_py-3.5.3/coc.py.egg-info/SOURCES.txt` & `coc_py-3.6.0/coc.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/pyproject.toml` & `coc_py-3.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coc.py"
 authors = [{ name = "mathsman5133" }]
 maintainers = [{ name = "majordoobie" }, { name = "MagicTheDev" }, { name = "Kuchenmampfer" },
     { name = "lukasthaler"}, { name = "doluk"}]
-version = "3.5.3"
+version = "3.6.0"
 description = "A python wrapper for the Clash of Clans API"
 requires-python = ">=3.7.3"
 readme = "README.rst"
 license = { text = "MIT" }
 keywords = ["coc", "clash of clans", "coc.py", "clash api"]
 classifiers = ["Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
```

### Comparing `coc_py-3.5.3/tests/test_capitalraidseasons.py` & `coc_py-3.6.0/tests/test_capitalraidseasons.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/tests/test_clans.py` & `coc_py-3.6.0/tests/test_clans.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/tests/test_clash_meta.py` & `coc_py-3.6.0/tests/test_clash_meta.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/tests/test_players.py` & `coc_py-3.6.0/tests/test_players.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/tests/test_troop_levels.py` & `coc_py-3.6.0/tests/test_troop_levels.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.5.3/tests/test_wars.py` & `coc_py-3.6.0/tests/test_wars.py`

 * *Files identical despite different names*

