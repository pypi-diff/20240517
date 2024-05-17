# Comparing `tmp/iipyper-0.1.2.tar.gz` & `tmp/iipyper-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iipyper-0.1.2.tar", max compression
+gzip compressed data, was "iipyper-0.1.3.tar", max compression
```

## Comparing `iipyper-0.1.2.tar` & `iipyper-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1084 2023-11-28 17:22:02.521024 iipyper-0.1.2/LICENSE
--rw-r--r--   0        0        0     2138 2024-03-16 00:39:01.445389 iipyper-0.1.2/README.md
--rw-r--r--   0        0        0      984 2024-05-15 20:37:51.251964 iipyper-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4057 2024-03-15 23:43:00.590525 iipyper-0.1.2/src/iipyper/__init__.py
--rw-r--r--   0        0        0     1011 2024-03-15 23:43:00.590729 iipyper-0.1.2/src/iipyper/audio.py
--rw-r--r--   0        0        0     9349 2024-05-15 20:17:34.072216 iipyper-0.1.2/src/iipyper/midi.py
--rw-r--r--   0        0        0    32977 2024-05-15 20:17:34.072636 iipyper-0.1.2/src/iipyper/osc.py
--rw-r--r--   0        0        0      213 2023-11-28 17:22:02.524007 iipyper-0.1.2/src/iipyper/state.py
--rw-r--r--   0        0        0     1311 2023-12-07 13:43:17.591203 iipyper-0.1.2/src/iipyper/timing.py
--rw-r--r--   0        0        0     5108 2024-05-15 20:17:34.072912 iipyper-0.1.2/src/iipyper/tui.py
--rw-r--r--   0        0        0     1795 2024-01-04 17:20:53.154026 iipyper-0.1.2/src/iipyper/types.py
--rw-r--r--   0        0        0      937 2024-05-15 20:17:34.073139 iipyper-0.1.2/src/iipyper/util.py
--rw-r--r--   0        0        0     3215 1970-01-01 00:00:00.000000 iipyper-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-11-28 17:22:02.521024 iipyper-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2212 2024-05-17 00:13:01.654594 iipyper-0.1.3/README.md
+-rw-r--r--   0        0        0      984 2024-05-17 00:14:36.756461 iipyper-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4057 2024-05-17 00:13:01.655539 iipyper-0.1.3/src/iipyper/__init__.py
+-rw-r--r--   0        0        0     1011 2024-05-17 00:13:01.655924 iipyper-0.1.3/src/iipyper/audio.py
+-rw-r--r--   0        0        0     9580 2024-05-17 00:13:01.656183 iipyper-0.1.3/src/iipyper/midi.py
+-rw-r--r--   0        0        0    32977 2024-05-17 00:13:01.656770 iipyper-0.1.3/src/iipyper/osc.py
+-rw-r--r--   0        0        0      213 2023-11-28 17:22:02.524007 iipyper-0.1.3/src/iipyper/state.py
+-rw-r--r--   0        0        0     1311 2024-05-17 00:13:01.657191 iipyper-0.1.3/src/iipyper/timing.py
+-rw-r--r--   0        0        0     5108 2024-05-17 00:13:01.657648 iipyper-0.1.3/src/iipyper/tui.py
+-rw-r--r--   0        0        0     1795 2024-05-17 00:13:01.658088 iipyper-0.1.3/src/iipyper/types.py
+-rw-r--r--   0        0        0      937 2024-05-17 00:13:01.658421 iipyper-0.1.3/src/iipyper/util.py
+-rw-r--r--   0        0        0     3289 1970-01-01 00:00:00.000000 iipyper-0.1.3/PKG-INFO
```

### Comparing `iipyper-0.1.2/LICENSE` & `iipyper-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `iipyper-0.1.2/README.md` & `iipyper-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# iipyper
+# iipyper ([Documentation](https://intelligent-instruments-lab.github.io/iipyper/))
 
 `iipyper` is a Python package for fast creation of [Open Sound Control](https://en.wikipedia.org/wiki/Open_Sound_Control) (OSC) and [MIDI](https://en.wikipedia.org/wiki/MIDI)-based event loops.
 
 It is designed for creatives who want to explore the Python ecosystem and experiment with music and, for example, machine learning.
 
 For examples and tutorials of how to use `iipyper`, see our [examples repo](https://github.com/intelligent-instruments-lab/iil-examples) (TBC).
```

#### html2text {}

```diff
@@ -1,8 +1,9 @@
-# iipyper `iipyper` is a Python package for fast creation of [Open Sound
+# iipyper ([Documentation](https://intelligent-instruments-lab.github.io/
+iipyper/)) `iipyper` is a Python package for fast creation of [Open Sound
 Control](https://en.wikipedia.org/wiki/Open_Sound_Control) (OSC) and [MIDI]
 (https://en.wikipedia.org/wiki/MIDI)-based event loops. It is designed for
 creatives who want to explore the Python ecosystem and experiment with music
 and, for example, machine learning. For examples and tutorials of how to use
 `iipyper`, see our [examples repo](https://github.com/intelligent-instruments-
 lab/iil-examples) (TBC). ## Install `iipyper` can be installed via [PyPI]
 (https://pypi.org/project/iipyper): ```sh pip install iipyper ``` ## Develop
```

### Comparing `iipyper-0.1.2/pyproject.toml` & `iipyper-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iipyper"
-version = "0.1.2"
+version = "0.1.3"
 description = "python package for easy MIDI, OSC, event loops"
 authors = ["Victor Shepardson <victor.shepardson@gmail.com>", "Jack Armitage <jack.armitage@me.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Intelligent-Instruments-Lab/iipyper"
 documentation = "https://intelligent-instruments-lab.github.io/iipyper/"
```

### Comparing `iipyper-0.1.2/src/iipyper/__init__.py` & `iipyper-0.1.3/src/iipyper/__init__.py`

 * *Files identical despite different names*

### Comparing `iipyper-0.1.2/src/iipyper/audio.py` & `iipyper-0.1.3/src/iipyper/audio.py`

 * *Files identical despite different names*

### Comparing `iipyper-0.1.2/src/iipyper/midi.py` & `iipyper-0.1.3/src/iipyper/midi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import functools as ft
 import time
 import traceback
 from typing import Optional, List, Union
 
 import mido
 
@@ -35,15 +36,15 @@
     midi.note_on(channel=0, note=0, velocity=64, time=0)
     ```
     """
     @classmethod
     def print_ports(cls):
         print('Available MIDI inputs:')
         for s in set(mido.get_input_names()):
-            print(f'\t{s}')
+            print(f'\t{s}') 
         print('Available MIDI outputs:')
         for s in set(mido.get_output_names()):
             print(f'\t{s}')
         MIDI.ports_printed = True
 
     ports_printed = False
 
@@ -97,27 +98,32 @@
         for port in in_ports:
             try:
                 self.in_ports[port] = mido.open_input(
                     port, callback=self.get_callback(port))
             except Exception:
                 print(f"""WARNING: MIDI input {port} not found""")
         for i in range(virtual_in_ports):
-            virtual_in = f'To iipyper {i+1}'
-            self.in_ports[virtual_in] = mido.open_input(
-                virtual_in, virtual=True, callback=self.get_callback(port))
+            port = f'To iipyper {i+1}'
+            try:
+                self.in_ports[port] = mido.open_input(
+                    port, virtual=True, callback=self.get_callback(port))
+            except Exception: print(
+                f'WARNING: iipyper: failed to open virtual MIDI port {port}')
 
         if self.verbose:
             print(f"""opened MIDI input ports: {list(self.in_ports)}""")
 
         ##### WIP
         self.out_ports = {}
         for i in range(virtual_out_ports):
-            virtual_out = f'From iipyper {i+1}'
-            self.out_ports[virtual_out] = mido.open_output(
-                virtual_out, virtual=True)
+            port = f'From iipyper {i+1}'
+            try:
+                self.out_ports[port] = mido.open_output(port, virtual=True)
+            except Exception: print(
+                f'WARNING: iipyper: failed to open virtual MIDI port {port}')
 
         if out_ports is None:
             out_ports = []
         # if out_ports is None or len(out_ports)==0:
             # out_ports = set(mido.get_output_names())  
         # self.out_ports = {}
         for port in out_ports:
```

### Comparing `iipyper-0.1.2/src/iipyper/osc.py` & `iipyper-0.1.3/src/iipyper/osc.py`

 * *Files identical despite different names*

### Comparing `iipyper-0.1.2/src/iipyper/timing.py` & `iipyper-0.1.3/src/iipyper/timing.py`

 * *Files identical despite different names*

### Comparing `iipyper-0.1.2/src/iipyper/tui.py` & `iipyper-0.1.3/src/iipyper/tui.py`

 * *Files identical despite different names*

### Comparing `iipyper-0.1.2/src/iipyper/types.py` & `iipyper-0.1.3/src/iipyper/types.py`

 * *Files identical despite different names*

### Comparing `iipyper-0.1.2/src/iipyper/util.py` & `iipyper-0.1.3/src/iipyper/util.py`

 * *Files identical despite different names*

### Comparing `iipyper-0.1.2/PKG-INFO` & `iipyper-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iipyper
-Version: 0.1.2
+Version: 0.1.3
 Summary: python package for easy MIDI, OSC, event loops
 Home-page: https://github.com/Intelligent-Instruments-Lab/iipyper
 License: MIT
 Author: Victor Shepardson
 Author-email: victor.shepardson@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -20,15 +20,15 @@
 Requires-Dist: python-rtmidi (>=1.5.7,<2.0.0)
 Requires-Dist: sounddevice (>=0.4.6,<0.5.0)
 Requires-Dist: textual (>=0.41.0,<0.42.0)
 Project-URL: Documentation, https://intelligent-instruments-lab.github.io/iipyper/
 Project-URL: Repository, https://github.com/Intelligent-Instruments-Lab/iipyper
 Description-Content-Type: text/markdown
 
-# iipyper
+# iipyper ([Documentation](https://intelligent-instruments-lab.github.io/iipyper/))
 
 `iipyper` is a Python package for fast creation of [Open Sound Control](https://en.wikipedia.org/wiki/Open_Sound_Control) (OSC) and [MIDI](https://en.wikipedia.org/wiki/MIDI)-based event loops.
 
 It is designed for creatives who want to explore the Python ecosystem and experiment with music and, for example, machine learning.
 
 For examples and tutorials of how to use `iipyper`, see our [examples repo](https://github.com/intelligent-instruments-lab/iil-examples) (TBC).
```

#### html2text {}

```diff
@@ -1,27 +1,28 @@
-Metadata-Version: 2.1 Name: iipyper Version: 0.1.2 Summary: python package for
+Metadata-Version: 2.1 Name: iipyper Version: 0.1.3 Summary: python package for
 easy MIDI, OSC, event loops Home-page: https://github.com/Intelligent-
 Instruments-Lab/iipyper License: MIT Author: Victor Shepardson Author-email:
 victor.shepardson@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: fire (>=0.5.0,<0.6.0) Requires-Dist: mido (>=1.3.0,<2.0.0)
 Requires-Dist: pydantic (>=2.5.2,<3.0.0) Requires-Dist: pydantic-numpy
 (>=4.1.0,<5.0.0) Requires-Dist: python-osc (>=1.8.3,<2.0.0) Requires-Dist:
 python-rtmidi (>=1.5.7,<2.0.0) Requires-Dist: sounddevice (>=0.4.6,<0.5.0)
 Requires-Dist: textual (>=0.41.0,<0.42.0) Project-URL: Documentation, https://
 intelligent-instruments-lab.github.io/iipyper/ Project-URL: Repository, https:/
 /github.com/Intelligent-Instruments-Lab/iipyper Description-Content-Type: text/
-markdown # iipyper `iipyper` is a Python package for fast creation of [Open
-Sound Control](https://en.wikipedia.org/wiki/Open_Sound_Control) (OSC) and
-[MIDI](https://en.wikipedia.org/wiki/MIDI)-based event loops. It is designed
-for creatives who want to explore the Python ecosystem and experiment with
-music and, for example, machine learning. For examples and tutorials of how to
-use `iipyper`, see our [examples repo](https://github.com/intelligent-
+markdown # iipyper ([Documentation](https://intelligent-instruments-
+lab.github.io/iipyper/)) `iipyper` is a Python package for fast creation of
+[Open Sound Control](https://en.wikipedia.org/wiki/Open_Sound_Control) (OSC)
+and [MIDI](https://en.wikipedia.org/wiki/MIDI)-based event loops. It is
+designed for creatives who want to explore the Python ecosystem and experiment
+with music and, for example, machine learning. For examples and tutorials of
+how to use `iipyper`, see our [examples repo](https://github.com/intelligent-
 instruments-lab/iil-examples) (TBC). ## Install `iipyper` can be installed via
 [PyPI](https://pypi.org/project/iipyper): ```sh pip install iipyper ``` ##
 Develop ```sh git clone git@github.com:Intelligent-Instruments-Lab/iipyper.git
 cd iipyper poetry install iipyper ``` ## Contact `iipyper` is developed by the
 [Intelligent Instruments Lab](https://iil.is/about). Get in touch to
 [collaborate](https://iil.is/collaborate): â¦ _i_i_l_._i_s â¦ _F_a_c_e_b_o_o_k â¦
 _I_n_s_t_a_g_r_a_m â¦ _X_ _(_T_w_i_t_t_e_r_) â¦ _Y_o_u_T_u_b_e â¦ _D_i_s_c_o_r_d â¦ _G_i_t_H_u_b â¦ _L_i_n_k_e_d_I_n â¦
```

