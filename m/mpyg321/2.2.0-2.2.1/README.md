# Comparing `tmp/mpyg321-2.2.0.tar.gz` & `tmp/mpyg321-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpyg321-2.2.0.tar", last modified: Sat May  4 21:42:37 2024, max compression
+gzip compressed data, was "mpyg321-2.2.1.tar", last modified: Fri May 17 12:07:26 2024, max compression
```

## Comparing `mpyg321-2.2.0.tar` & `mpyg321-2.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:42:37.405925 mpyg321-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-04 21:42:33.000000 mpyg321-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-04 21:42:37.405925 mpyg321-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-04 21:42:33.000000 mpyg321-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:42:37.405925 mpyg321-2.2.0/mpyg321/
--rw-r--r--   0 runner    (1001) docker     (127)     8978 2024-05-04 21:42:33.000000 mpyg321-2.2.0/mpyg321/BasePlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-04 21:42:33.000000 mpyg321-2.2.0/mpyg321/EventContext.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-04 21:42:33.000000 mpyg321-2.2.0/mpyg321/MPyg123Player.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-04 21:42:33.000000 mpyg321-2.2.0/mpyg321/MPyg321Player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-04 21:42:33.000000 mpyg321-2.2.0/mpyg321/MpygError.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-04 21:42:33.000000 mpyg321-2.2.0/mpyg321/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-04 21:42:33.000000 mpyg321-2.2.0/mpyg321/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-04 21:42:33.000000 mpyg321-2.2.0/mpyg321/mpyg321.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:42:37.405925 mpyg321-2.2.0/mpyg321.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-04 21:42:37.000000 mpyg321-2.2.0/mpyg321.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-04 21:42:37.000000 mpyg321-2.2.0/mpyg321.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 21:42:37.000000 mpyg321-2.2.0/mpyg321.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 21:42:37.000000 mpyg321-2.2.0/mpyg321.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 21:42:37.000000 mpyg321-2.2.0/mpyg321.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 21:42:37.405925 mpyg321-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-04 21:42:33.000000 mpyg321-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:07:26.897015 mpyg321-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-17 12:07:23.000000 mpyg321-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-17 12:07:26.897015 mpyg321-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-05-17 12:07:23.000000 mpyg321-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:07:26.893015 mpyg321-2.2.1/mpyg321/
+-rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-05-17 12:07:23.000000 mpyg321-2.2.1/mpyg321/BasePlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-17 12:07:23.000000 mpyg321-2.2.1/mpyg321/EventContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-17 12:07:23.000000 mpyg321-2.2.1/mpyg321/MPyg123Player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-17 12:07:23.000000 mpyg321-2.2.1/mpyg321/MPyg321Player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-17 12:07:23.000000 mpyg321-2.2.1/mpyg321/MpygError.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-17 12:07:23.000000 mpyg321-2.2.1/mpyg321/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-17 12:07:23.000000 mpyg321-2.2.1/mpyg321/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-17 12:07:23.000000 mpyg321-2.2.1/mpyg321/mpyg321.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:07:26.897015 mpyg321-2.2.1/mpyg321.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-17 12:07:26.000000 mpyg321-2.2.1/mpyg321.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-17 12:07:26.000000 mpyg321-2.2.1/mpyg321.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 12:07:26.000000 mpyg321-2.2.1/mpyg321.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-17 12:07:26.000000 mpyg321-2.2.1/mpyg321.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-17 12:07:26.000000 mpyg321-2.2.1/mpyg321.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 12:07:26.897015 mpyg321-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-17 12:07:23.000000 mpyg321-2.2.1/setup.py
```

### Comparing `mpyg321-2.2.0/LICENSE` & `mpyg321-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mpyg321-2.2.0/PKG-INFO` & `mpyg321-2.2.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,18 @@
-Metadata-Version: 2.1
-Name: mpyg321
-Version: 2.2.0
-Summary: mpg321 wrapper for python - command line music player
-Home-page: https://github.com/4br3mm0rd/mpyg321
-Author: 4br3mm0rd
-Author-email: 4br3mm0rd@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pexpect
-
 [![Downloads](https://pepy.tech/badge/mpyg321)](https://pepy.tech/project/mpyg321)
 [![Downloads](https://pepy.tech/badge/mpyg321/month)](https://pepy.tech/project/mpyg321)
 [![Downloads](https://pepy.tech/badge/mpyg321/week)](https://pepy.tech/project/mpyg321)
+
 # mpyg321
 
 mpyg321 is a simple python wrapper for mpg321 and mpg123. It allows you to easily play mp3 sounds in python, do basic operations on the music and implement callbacks for events like the end of a sound.
 
 # Installation
 
-mpyg321 requires the installation of mpg123 (or mpg321 depending on your usage) software for reading mp3. This section describes the installation of the library on MacOS, Linux and Windows. **For now, the library has only been tested on mac, but it should work on any platform.**
+mpyg321 requires the installation of mpg123 (or mpg321 depending on your usage) software for reading mp3. This section describes the installation of the library on MacOS, Linux and Windows.
 
 We recommend using mpg123 since the project is more up to date. However, you can also use this library with mpg321 (using the `MPyg321Player` class)
 
 ## MacOS
 
 ```
 $ brew install mpg123 # or mpg321
@@ -54,20 +41,53 @@
 
 ```
 from mpyg321.MPyg123Player import MPyg123Player # or MPyg321Player if you installed mpg321
 player = MPyg123Player()
 player.play_song("/path/to/some_mp3.mp3")
 ```
 
-## Calbacks
+## Calbacks and Events
+
+### Callbacks
 
 You can implement callbacks for several events such as: end of song, user paused the music, ...
 All the callbacks can be found inside the code of the `BasePlayer` class and the `MPyg123Player` class.
 Most of the callbacks are implemented in the `callbacks.py` example file.
 
+### Events
+
+Starting **from version 2.2.0**, you can now subscribe to events using decorators and/or the `subscribe_event` function.
+Here is an example usage. You can find more details in the `events.py` example file.
+
+```
+player = MPyg123Player()
+
+@player.on(MPyg321Events.ANY_STOP)
+def callback(context):
+    print("Any stop event occured")
+
+# or
+def my_func(context):
+    print("Other event subscribed")
+
+player.subscribe_event(MPyg321Events.ANY_STOP, my_func)
+```
+
+Here is an exhaustive list of the available events and their compatibilities with the different players (MPyg123 and MPyg321):
+|Event|Description|MPyg123Player|MPyg321Player|
+|------|------|:---------:|:-------:|
+|USER_STOP|When you stop the music (call `player.stop`)|X|X|
+|USER_PAUSE|When you pause the music (call `player.pause`)|X|X|
+|USER_RESUME|When you resume the music (call `player.resume`)|X|X|
+|ANY_STOP|When any stop occures (pause, stop, end of music)|X|X|
+|MUSIC_END|When the music ends|X|X|
+|ERROR|When an error occurs (The error info is within the context using the class `MPyg321ErrorContext`)|X|X|
+|USER_MUTE|When you mute the player|X|-|
+|USER_MUTE|When you unmute the player|X|-|
+
 ## Loops
 
 In order to loop (replay the song when it ended), you can either set the loop mode when calling the `play_song` function:
 
 ```
 player.play_song("/path/to/sample.mp3", loop=True)
 ```
```

### Comparing `mpyg321-2.2.0/mpyg321/BasePlayer.py` & `mpyg321-2.2.1/mpyg321/BasePlayer.py`

 * *Files 5% similar despite different names*

```diff
@@ -145,14 +145,21 @@
 
     def pause(self):
         """Pauses the player"""
         if self.status == PlayerStatus.PLAYING:
             self.player.sendline("PAUSE")
             self.status = PlayerStatus.PAUSED
 
+    def toggle_pause(self):
+        """Pause if playing, else resume if paused"""
+        if self.status == PlayerStatus.PLAYING:
+            self.pause()
+        elif self.status == PlayerStatus.PAUSED:
+            self.resume()            
+
     def resume(self):
         """Resume the player"""
         if self.status == PlayerStatus.PAUSED:
             self.player.sendline("PAUSE")
             self._trigger_event(MPyg321Events.USER_RESUME)
             self.on_user_resume()
```

### Comparing `mpyg321-2.2.0/mpyg321/MPyg123Player.py` & `mpyg321-2.2.1/mpyg321/MPyg123Player.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .BasePlayer import BasePlayer
 from .consts import MPyg321Events, PlayerStatus
 from .EventContext import MPyg321EventContext
 
 
 class MPyg123Player(BasePlayer):
-    """Player for legacy mpg321"""
+    """Player for mpg123"""
 
     def __init__(
         self,
         player=None,
         audiodevice=None,
         performance_mode=True,
         custom_args="",
@@ -16,21 +16,24 @@
     ):
         self.suitable_versions = ["mpg123"]
         self.default_player = "mpg123"
         custom_args += " --rva-mix " if rva_mix else ""
         super().__init__(player, audiodevice, performance_mode, custom_args)
         if performance_mode:
             self.silence_mpyg_output()
+        self._is_muted = False            
 
     def process_output_ext(self, action):
         """Processes specific output for mpg123 player"""
         if action == "user_mute":
+            self._is_muted = True
             self.on_user_mute()
             self._trigger_event(MPyg321Events.USER_MUTE, MPyg321EventContext(self))
         elif action == "user_unmute":
+            self._is_muted = False
             self._trigger_event(MPyg321Events.USER_UNMUTE, MPyg321EventContext(self))
             self.on_user_unmute()
 
     def load_list(self, entry, filepath):
         """Load an entry in a list
         Parameters:
         entry (int): index of the song in the list - first is 0
@@ -47,14 +50,21 @@
         """Mutes the player"""
         self.player.sendline("MUTE")
 
     def unmute(self):
         """Unmutes the player"""
         self.player.sendline("UNMUTE")
 
+    def toggle_mute(self):
+        """Mute or UnMute if playing"""
+        if self._is_muted:
+            self.unmute()
+        else:
+            self.mute()
+
     def volume(self, percent):
         """Adjust player's volume"""
         self.player.sendline("VOLUME {}".format(percent))
 
     # # # Public Callbacks # # #
     def on_user_mute(self):
         """Callback when user mutes player"""
```

### Comparing `mpyg321-2.2.0/mpyg321/MPyg321Player.py` & `mpyg321-2.2.1/mpyg321/MPyg321Player.py`

 * *Files identical despite different names*

### Comparing `mpyg321-2.2.0/mpyg321/MpygError.py` & `mpyg321-2.2.1/mpyg321/MpygError.py`

 * *Files identical despite different names*

### Comparing `mpyg321-2.2.0/mpyg321/consts.py` & `mpyg321-2.2.1/mpyg321/consts.py`

 * *Files identical despite different names*

### Comparing `mpyg321-2.2.0/setup.py` & `mpyg321-2.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mpyg321",
-    version="2.2.0",
+    version="2.2.1",
     author="4br3mm0rd",
     author_email="4br3mm0rd@gmail.com",
     description="mpg321 wrapper for python - command line music player",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/4br3mm0rd/mpyg321",
     packages=setuptools.find_packages(),
```

