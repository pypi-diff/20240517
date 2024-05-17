# Comparing `tmp/midi-beeper-1.79.tar.gz` & `tmp/midi_beeper-1.79.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midi-beeper-1.79.tar", last modified: Thu May 16 10:45:45 2024, max compression
+gzip compressed data, was "midi_beeper-1.79.1.tar", last modified: Thu May 16 10:51:22 2024, max compression
```

## Comparing `midi-beeper-1.79.tar` & `midi_beeper-1.79.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-16 10:45:45.913856 midi-beeper-1.79/
--rw-r--r--   0 silbrown   (501) staff       (20)    11357 2024-05-16 08:52:25.000000 midi-beeper-1.79/LICENSE
--rw-r--r--   0 silbrown   (501) staff       (20)     3750 2024-05-16 10:45:45.913014 midi-beeper-1.79/PKG-INFO
-drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-16 10:45:45.910728 midi-beeper-1.79/midi-beeper/
--rw-r--r--   0 silbrown   (501) staff       (20)      117 2024-05-16 10:45:45.000000 midi-beeper-1.79/midi-beeper/__init__.py
--rw-r--r--   0 silbrown   (501) staff       (20)    57594 2024-05-16 10:45:45.000000 midi-beeper-1.79/midi-beeper/__main__.py
-drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-16 10:45:45.912378 midi-beeper-1.79/midi_beeper.egg-info/
--rw-r--r--   0 silbrown   (501) staff       (20)     3750 2024-05-16 10:45:45.000000 midi-beeper-1.79/midi_beeper.egg-info/PKG-INFO
--rw-r--r--   0 silbrown   (501) staff       (20)      242 2024-05-16 10:45:45.000000 midi-beeper-1.79/midi_beeper.egg-info/SOURCES.txt
--rw-r--r--   0 silbrown   (501) staff       (20)        1 2024-05-16 10:45:45.000000 midi-beeper-1.79/midi_beeper.egg-info/dependency_links.txt
--rw-r--r--   0 silbrown   (501) staff       (20)       62 2024-05-16 10:45:45.000000 midi-beeper-1.79/midi_beeper.egg-info/entry_points.txt
--rw-r--r--   0 silbrown   (501) staff       (20)       12 2024-05-16 10:45:45.000000 midi-beeper-1.79/midi_beeper.egg-info/top_level.txt
--rw-r--r--   0 silbrown   (501) staff       (20)       38 2024-05-16 10:45:45.913993 midi-beeper-1.79/setup.cfg
--rw-r--r--   0 silbrown   (501) staff       (20)     3870 2024-05-16 10:45:45.000000 midi-beeper-1.79/setup.py
+drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-16 10:51:22.683353 midi_beeper-1.79.1/
+-rw-r--r--   0 silbrown   (501) staff       (20)    11357 2024-05-16 08:52:25.000000 midi_beeper-1.79.1/LICENSE
+-rw-r--r--   0 silbrown   (501) staff       (20)     3752 2024-05-16 10:51:22.682412 midi_beeper-1.79.1/PKG-INFO
+drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-16 10:51:22.679789 midi_beeper-1.79.1/midi_beeper/
+-rw-r--r--   0 silbrown   (501) staff       (20)      117 2024-05-16 10:51:22.000000 midi_beeper-1.79.1/midi_beeper/__init__.py
+-rw-r--r--   0 silbrown   (501) staff       (20)    57594 2024-05-16 10:51:22.000000 midi_beeper-1.79.1/midi_beeper/__main__.py
+drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-16 10:51:22.681781 midi_beeper-1.79.1/midi_beeper.egg-info/
+-rw-r--r--   0 silbrown   (501) staff       (20)     3752 2024-05-16 10:51:22.000000 midi_beeper-1.79.1/midi_beeper.egg-info/PKG-INFO
+-rw-r--r--   0 silbrown   (501) staff       (20)      242 2024-05-16 10:51:22.000000 midi_beeper-1.79.1/midi_beeper.egg-info/SOURCES.txt
+-rw-r--r--   0 silbrown   (501) staff       (20)        1 2024-05-16 10:51:22.000000 midi_beeper-1.79.1/midi_beeper.egg-info/dependency_links.txt
+-rw-r--r--   0 silbrown   (501) staff       (20)       62 2024-05-16 10:51:22.000000 midi_beeper-1.79.1/midi_beeper.egg-info/entry_points.txt
+-rw-r--r--   0 silbrown   (501) staff       (20)       12 2024-05-16 10:51:22.000000 midi_beeper-1.79.1/midi_beeper.egg-info/top_level.txt
+-rw-r--r--   0 silbrown   (501) staff       (20)       38 2024-05-16 10:51:22.683599 midi_beeper-1.79.1/setup.cfg
+-rw-r--r--   0 silbrown   (501) staff       (20)     3872 2024-05-16 10:51:22.000000 midi_beeper-1.79.1/setup.py
```

### Comparing `midi-beeper-1.79/LICENSE` & `midi_beeper-1.79.1/LICENSE`

 * *Files identical despite different names*

### Comparing `midi-beeper-1.79/PKG-INFO` & `midi_beeper-1.79.1/midi_beeper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midi-beeper
-Version: 1.79
+Version: 1.79.1
 Summary: Play MIDI files using piezo beepers and other sounders
 Home-page: http://ssb22.user.srcf.net/mwrhome/midi-beeper.html
 Author: Silas S. Brown
 Author-email: ssb22@cam.ac.uk
 License: Apache 2
 Platform: all
 Classifier: Programming Language :: Python :: 2
```

### Comparing `midi-beeper-1.79/midi-beeper/__main__.py` & `midi_beeper-1.79.1/midi_beeper/__main__.py`

 * *Files identical despite different names*

### Comparing `midi-beeper-1.79/midi_beeper.egg-info/PKG-INFO` & `midi_beeper-1.79.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: midi-beeper
-Version: 1.79
+Name: midi_beeper
+Version: 1.79.1
 Summary: Play MIDI files using piezo beepers and other sounders
 Home-page: http://ssb22.user.srcf.net/mwrhome/midi-beeper.html
 Author: Silas S. Brown
 Author-email: ssb22@cam.ac.uk
 License: Apache 2
 Platform: all
 Classifier: Programming Language :: Python :: 2
```

### Comparing `midi-beeper-1.79/setup.py` & `midi_beeper-1.79.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from setuptools import setup, find_packages;setup(name='midi-beeper',version='1.79',entry_points={'console_scripts':['midi-beeper=midi_beeper.__main__:placebo']},license='Apache 2',platforms='all',url='http://ssb22.user.srcf.net/mwrhome/midi-beeper.html',author='Silas S. Brown',author_email='ssb22@cam.ac.uk',description='Play MIDI files using piezo beepers and other sounders',long_description=r'''# midi-beeper
+from setuptools import setup, find_packages;setup(name='midi_beeper',version='1.79.1',entry_points={'console_scripts':['midi-beeper=midi_beeper.__main__:placebo']},license='Apache 2',platforms='all',url='http://ssb22.user.srcf.net/mwrhome/midi-beeper.html',author='Silas S. Brown',author_email='ssb22@cam.ac.uk',description='Play MIDI files using piezo beepers and other sounders',long_description=r'''# midi-beeper
 MIDI Beeper from http://ssb22.user.srcf.net/mwrhome/midi-beeper.html
 
 MIDI Beeper is a program to play MIDI files on Linux/BSD by beeping through the computer’s beeper instead of using proper sound circuits. If you try to play chords or polyphony, it will rapidly switch between alternate notes like an old office telephone. It sounds awful, but it might be useful when you really have to play a MIDI file but have no sound device attached. It should work on any machine that has the “beep” command (install “beep” package from your Linux/Unix package manager). It has been tested on a PC speaker and on an NSLU2’s internal speaker.
 
 On the NSLU2, playing music with beep works in Debian 4 (Etch, 2007) but not so well in Debian 5 (Lenny, 2012); you can try compiling this [modified beep.c](http://ssb22.user.srcf.net/mwrhome/beep.c) instead (remember the chmod 4755 mentioned in the man page). I haven’t tried it on more recent distros because my NSLU2 power supply failed and I upgraded to a Raspberry Pi.
 
 MIDI Beeper can also generate polyphonic square waves itself and feed them to `aplay`, which might be useful if you need a small MIDI player on a Raspberry Pi running Linux, although too many sound channels can slow this down as it’s only a Python script.
```

