# Comparing `tmp/retrodevem-0.1.tar.gz` & `tmp/retrodevem-0.2.tar.gz`

## Comparing `retrodevem-0.1.tar` & `retrodevem-0.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 retrodevem-0.1/doc/mechanical.md
--rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 retrodevem-0.1/doc/sourcing.md
--rw-r--r--   0        0        0  1598431 2020-02-02 00:00:00.000000 retrodevem-0.1/pictures/pcb-v2.0.jpg
--rw-r--r--   0        0        0  1056877 2020-02-02 00:00:00.000000 retrodevem-0.1/pictures/retrodevem-illustration-1024x673.png
--rw-r--r--   0        0        0   483539 2020-02-02 00:00:00.000000 retrodevem-0.1/pictures/retrodevem-pen-mechanical-drawing.pdf
--rw-r--r--   0        0        0   430287 2020-02-02 00:00:00.000000 retrodevem-0.1/pictures/retrodevem-pencil-mechanical-drawing.pdf
--rw-r--r--   0        0        0   127549 2020-02-02 00:00:00.000000 retrodevem-0.1/pictures/retrodevem-v2.0-schematic.png
--rw-r--r--   0        0        0    72582 2020-02-02 00:00:00.000000 retrodevem-0.1/pictures/retrodevem-v2.1-schematic.png
--rw-r--r--   0        0        0   766653 2020-02-02 00:00:00.000000 retrodevem-0.1/rde-board/rde-board.kicad_pcb
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 retrodevem-0.1/rde-board/rde-board.kicad_prl
--rw-r--r--   0        0        0     9311 2020-02-02 00:00:00.000000 retrodevem-0.1/rde-board/rde-board.kicad_pro
--rw-r--r--   0        0        0    75405 2020-02-02 00:00:00.000000 retrodevem-0.1/rde-board/rde-board.kicad_sch
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 retrodevem-0.1/src/retrodevem/1khz_square.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 retrodevem-0.1/src/retrodevem/__init__.py
--rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 retrodevem-0.1/src/retrodevem/atarist_joystick.py
--rw-r--r--   0        0        0     7174 2020-02-02 00:00:00.000000 retrodevem-0.1/src/retrodevem/atarist_mouse.py
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 retrodevem-0.1/src/retrodevem/inputdevice.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 retrodevem-0.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 retrodevem-0.1/LICENSE
--rw-r--r--   0        0        0     9427 2020-02-02 00:00:00.000000 retrodevem-0.1/README.md
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 retrodevem-0.1/pyproject.toml
--rw-r--r--   0        0        0    10271 2020-02-02 00:00:00.000000 retrodevem-0.1/PKG-INFO
+prw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 retrodevem-0.2/.lgd-nfy0
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 retrodevem-0.2/doc/mechanical.md
+-rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 retrodevem-0.2/doc/sourcing.md
+-rw-r--r--   0        0        0  1598431 2020-02-02 00:00:00.000000 retrodevem-0.2/pictures/pcb-v2.0.jpg
+-rw-r--r--   0        0        0  1056877 2020-02-02 00:00:00.000000 retrodevem-0.2/pictures/retrodevem-illustration-1024x673.png
+-rw-r--r--   0        0        0   483539 2020-02-02 00:00:00.000000 retrodevem-0.2/pictures/retrodevem-pen-mechanical-drawing.pdf
+-rw-r--r--   0        0        0   430287 2020-02-02 00:00:00.000000 retrodevem-0.2/pictures/retrodevem-pencil-mechanical-drawing.pdf
+-rw-r--r--   0        0        0   127549 2020-02-02 00:00:00.000000 retrodevem-0.2/pictures/retrodevem-v2.0-schematic.png
+-rw-r--r--   0        0        0    72582 2020-02-02 00:00:00.000000 retrodevem-0.2/pictures/retrodevem-v2.1-schematic.png
+-rw-r--r--   0        0        0   766653 2020-02-02 00:00:00.000000 retrodevem-0.2/rde-board/rde-board.kicad_pcb
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 retrodevem-0.2/rde-board/rde-board.kicad_prl
+-rw-r--r--   0        0        0     9311 2020-02-02 00:00:00.000000 retrodevem-0.2/rde-board/rde-board.kicad_pro
+-rw-r--r--   0        0        0    75405 2020-02-02 00:00:00.000000 retrodevem-0.2/rde-board/rde-board.kicad_sch
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 retrodevem-0.2/src/retrodevem/1khz_square.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 retrodevem-0.2/src/retrodevem/__init__.py
+-rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 retrodevem-0.2/src/retrodevem/atarist_joystick.py
+-rw-r--r--   0        0        0     7174 2020-02-02 00:00:00.000000 retrodevem-0.2/src/retrodevem/atarist_mouse.py
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 retrodevem-0.2/src/retrodevem/inputdevice.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 retrodevem-0.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 retrodevem-0.2/LICENSE
+-rw-r--r--   0        0        0     9427 2020-02-02 00:00:00.000000 retrodevem-0.2/README.md
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 retrodevem-0.2/pyproject.toml
+-rw-r--r--   0        0        0    10292 2020-02-02 00:00:00.000000 retrodevem-0.2/PKG-INFO
```

### Comparing `retrodevem-0.1/doc/mechanical.md` & `retrodevem-0.2/doc/mechanical.md`

 * *Files identical despite different names*

### Comparing `retrodevem-0.1/doc/sourcing.md` & `retrodevem-0.2/doc/sourcing.md`

 * *Files identical despite different names*

### Comparing `retrodevem-0.1/pictures/pcb-v2.0.jpg` & `retrodevem-0.2/pictures/pcb-v2.0.jpg`

 * *Files identical despite different names*

### Comparing `retrodevem-0.1/pictures/retrodevem-illustration-1024x673.png` & `retrodevem-0.2/pictures/retrodevem-illustration-1024x673.png`

 * *Files identical despite different names*

### Comparing `retrodevem-0.1/pictures/retrodevem-pen-mechanical-drawing.pdf` & `retrodevem-0.2/pictures/retrodevem-pen-mechanical-drawing.pdf`

 * *Files identical despite different names*

### Comparing `retrodevem-0.1/pictures/retrodevem-pencil-mechanical-drawing.pdf` & `retrodevem-0.2/pictures/retrodevem-pencil-mechanical-drawing.pdf`

 * *Files identical despite different names*

### Comparing `retrodevem-0.1/pictures/retrodevem-v2.0-schematic.png` & `retrodevem-0.2/pictures/retrodevem-v2.0-schematic.png`

 * *Files identical despite different names*

### Comparing `retrodevem-0.1/pictures/retrodevem-v2.1-schematic.png` & `retrodevem-0.2/pictures/retrodevem-v2.1-schematic.png`

 * *Files identical despite different names*

### Comparing `retrodevem-0.1/rde-board/rde-board.kicad_pcb` & `retrodevem-0.2/rde-board/rde-board.kicad_pcb`

 * *Files identical despite different names*

### Comparing `retrodevem-0.1/rde-board/rde-board.kicad_prl` & `retrodevem-0.2/rde-board/rde-board.kicad_prl`

 * *Files identical despite different names*

### Comparing `retrodevem-0.1/rde-board/rde-board.kicad_pro` & `retrodevem-0.2/rde-board/rde-board.kicad_pro`

 * *Files identical despite different names*

### Comparing `retrodevem-0.1/rde-board/rde-board.kicad_sch` & `retrodevem-0.2/rde-board/rde-board.kicad_sch`

 * *Files identical despite different names*

### Comparing `retrodevem-0.1/src/retrodevem/atarist_joystick.py` & `retrodevem-0.2/src/retrodevem/atarist_joystick.py`

 * *Files identical despite different names*

### Comparing `retrodevem-0.1/src/retrodevem/atarist_mouse.py` & `retrodevem-0.2/src/retrodevem/atarist_mouse.py`

 * *Files identical despite different names*

### Comparing `retrodevem-0.1/src/retrodevem/inputdevice.py` & `retrodevem-0.2/src/retrodevem/inputdevice.py`

 * *Files identical despite different names*

### Comparing `retrodevem-0.1/LICENSE` & `retrodevem-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `retrodevem-0.1/README.md` & `retrodevem-0.2/README.md`

 * *Files identical despite different names*

### Comparing `retrodevem-0.1/pyproject.toml` & `retrodevem-0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "retrodevem"
-version = "0.1"
+version = "0.2"
 authors = [
   { name="Florent Flament", email="contact@florentflament.com" },
 ]
 
 description = "RetroDevEm (Retro Device Emulator) is a free (as in Free Software) input devices (mouse and joystick) emulator for retro consoles and computers (Atari 2600, Atari ST, Amstrad CPC, ...)."
 
 readme = "README.md"
 requires-python = ">=3"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: POSIX :: Linux",
 ]
 
-dependencies = ["gpiozero", "click"]
+dependencies = ["lgpio", "gpiozero", "click"]
 keywords = ["mouse", "joystick", "gamepad", "USB", "Atari 2600", "Atari 2600", "Atari ST", "Amstrad CPC", "retrogaming", "retrocomputing"]
 
 [project.urls]
 Homepage = "https://github.com/FlorentFlament/RetroDevEm"
 Issues = "https://github.com/FlorentFlament/RetroDevEm/issues"
 
 [project.scripts]
```

### Comparing `retrodevem-0.1/PKG-INFO` & `retrodevem-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.3
 Name: retrodevem
-Version: 0.1
+Version: 0.2
 Summary: RetroDevEm (Retro Device Emulator) is a free (as in Free Software) input devices (mouse and joystick) emulator for retro consoles and computers (Atari 2600, Atari ST, Amstrad CPC, ...).
 Project-URL: Homepage, https://github.com/FlorentFlament/RetroDevEm
 Project-URL: Issues, https://github.com/FlorentFlament/RetroDevEm/issues
 Author-email: Florent Flament <contact@florentflament.com>
 License-File: LICENSE
 Keywords: Amstrad CPC,Atari 2600,Atari ST,USB,gamepad,joystick,mouse,retrocomputing,retrogaming
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Requires-Dist: click
 Requires-Dist: gpiozero
+Requires-Dist: lgpio
 Description-Content-Type: text/markdown
 
 # RetroDevEm
 
 RetroDevEm (Retro Device Emulator) is a free (as in Free Software)
 input devices (mouse and joystick) emulator for retro consoles and
 computers (Atari 2600, Atari ST, Amstrad CPC, ...).  It allows using
```

