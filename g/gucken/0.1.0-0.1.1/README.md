# Comparing `tmp/gucken-0.1.0.tar.gz` & `tmp/gucken-0.1.1.tar.gz`

## Comparing `gucken-0.1.0.tar` & `gucken-0.1.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/__main__.py
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/aniskip.py
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/custom_widgets.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/default_settings.toml
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/gucken.css
--rw-r--r--   0        0        0    23834 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/gucken.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/rome.py
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/settings.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/update.py
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/hoster/__init__.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/hoster/common.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/hoster/doodstream.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/hoster/streamtape.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/hoster/veo.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/hoster/vidoza.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/player/__init__.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/player/android.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/player/common.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/player/ffplay.py
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/player/flatpak.py
--rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/player/mpv.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/player/vlc.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/player/wmplayer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/provider/__init__.py
--rw-r--r--   0        0        0    10145 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/provider/aniworld.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/provider/burningseries.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/provider/common.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/provider/crunchyroll.py
--rw-r--r--   0        0        0    10182 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/provider/serienstream.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/provider/streamcloud.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/tracker/__init__.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/tracker/anilist.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/tracker/aniworld.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/tracker/common.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/tracker/myanimelist.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/tracker/serienstream.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 gucken-0.1.0/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 gucken-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 gucken-0.1.0/README.md
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 gucken-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     9296 2020-02-02 00:00:00.000000 gucken-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/__main__.py
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/aniskip.py
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/custom_widgets.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/default_settings.toml
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/gucken.css
+-rw-r--r--   0        0        0    23834 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/gucken.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/rome.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/settings.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/update.py
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/hoster/__init__.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/hoster/common.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/hoster/doodstream.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/hoster/streamtape.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/hoster/veo.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/hoster/vidoza.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/player/__init__.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/player/android.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/player/common.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/player/ffplay.py
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/player/flatpak.py
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/player/mpv.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/player/vlc.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/player/wmplayer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/provider/__init__.py
+-rw-r--r--   0        0        0    10145 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/provider/aniworld.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/provider/burningseries.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/provider/common.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/provider/crunchyroll.py
+-rw-r--r--   0        0        0    10182 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/provider/serienstream.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/provider/streamcloud.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/tracker/__init__.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/tracker/anilist.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/tracker/aniworld.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/tracker/common.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/tracker/myanimelist.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.1/src/gucken/tracker/serienstream.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 gucken-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 gucken-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     7028 2020-02-02 00:00:00.000000 gucken-0.1.1/README.md
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 gucken-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9324 2020-02-02 00:00:00.000000 gucken-0.1.1/PKG-INFO
```

### Comparing `gucken-0.1.0/src/gucken/aniskip.py` & `gucken-0.1.1/src/gucken/aniskip.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.0/src/gucken/custom_widgets.py` & `gucken-0.1.1/src/gucken/custom_widgets.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.0/src/gucken/gucken.css` & `gucken-0.1.1/src/gucken/gucken.css`

 * *Files identical despite different names*

### Comparing `gucken-0.1.0/src/gucken/gucken.py` & `gucken-0.1.1/src/gucken/gucken.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.0/src/gucken/rome.py` & `gucken-0.1.1/src/gucken/rome.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.0/src/gucken/settings.py` & `gucken-0.1.1/src/gucken/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 
         self.settings = _load_settings(self.settings_file, default_settings)
 
         if self.save_on_load:
             self.save()
 
     def save(self):
+        self.default_settings_file.parent.mkdir(exist_ok=True, parents=True)
         _save_settings(self.settings, self.settings_file)
 
 
 class Singleton:
     _instance = None
 
     def __new__(cls, *args, **kwargs):
```

### Comparing `gucken-0.1.0/src/gucken/update.py` & `gucken-0.1.1/src/gucken/update.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.0/src/gucken/utils.py` & `gucken-0.1.1/src/gucken/utils.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.0/src/gucken/hoster/common.py` & `gucken-0.1.1/src/gucken/hoster/common.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.0/src/gucken/hoster/doodstream.py` & `gucken-0.1.1/src/gucken/hoster/doodstream.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.0/src/gucken/hoster/streamtape.py` & `gucken-0.1.1/src/gucken/hoster/streamtape.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.0/src/gucken/hoster/veo.py` & `gucken-0.1.1/src/gucken/hoster/veo.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.0/src/gucken/hoster/vidoza.py` & `gucken-0.1.1/src/gucken/hoster/vidoza.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.0/src/gucken/player/android.py` & `gucken-0.1.1/src/gucken/player/android.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.0/src/gucken/player/common.py` & `gucken-0.1.1/src/gucken/player/common.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.0/src/gucken/player/ffplay.py` & `gucken-0.1.1/src/gucken/player/ffplay.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.0/src/gucken/player/flatpak.py` & `gucken-0.1.1/src/gucken/player/flatpak.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.0/src/gucken/player/mpv.py` & `gucken-0.1.1/src/gucken/player/mpv.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.0/src/gucken/player/vlc.py` & `gucken-0.1.1/src/gucken/player/vlc.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.0/src/gucken/player/wmplayer.py` & `gucken-0.1.1/src/gucken/player/wmplayer.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.0/src/gucken/provider/aniworld.py` & `gucken-0.1.1/src/gucken/provider/aniworld.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.0/src/gucken/provider/common.py` & `gucken-0.1.1/src/gucken/provider/common.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.0/src/gucken/provider/serienstream.py` & `gucken-0.1.1/src/gucken/provider/serienstream.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.0/src/gucken/tracker/anilist.py` & `gucken-0.1.1/src/gucken/tracker/anilist.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.0/LICENSE.txt` & `gucken-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gucken-0.1.0/README.md` & `gucken-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,18 @@
 gucken
 ```
 
 #### Shortcut
 
 Install [Termux:Widget](https://github.com/termux/termux-widget?tab=readme-ov-file#Installation).
 
+```
+mkdir ~/.shortcuts
+```
+
 ##### Lunch shortcut
 
 ```
 echo gucken>~/.shortcuts/Gucken
 ```
 
 ##### Update shortcut
```

### Comparing `gucken-0.1.0/pyproject.toml` & `gucken-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gucken-0.1.0/PKG-INFO` & `gucken-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gucken
-Version: 0.1.0
+Version: 0.1.1
 Summary: Gucken is a Terminal User Interface which allows you to browse and watch your favorite anime's with style.
 Project-URL: Repository, https://github.com/Commandcracker/gucken
 Author: Commandcracker
 Maintainer: Commandcracker
 License: MIT License
         
         Copyright (c) 2024 Commandcracker
@@ -101,14 +101,18 @@
 gucken
 ```
 
 #### Shortcut
 
 Install [Termux:Widget](https://github.com/termux/termux-widget?tab=readme-ov-file#Installation).
 
+```
+mkdir ~/.shortcuts
+```
+
 ##### Lunch shortcut
 
 ```
 echo gucken>~/.shortcuts/Gucken
 ```
 
 ##### Update shortcut
```

