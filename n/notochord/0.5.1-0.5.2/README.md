# Comparing `tmp/notochord-0.5.1.tar.gz` & `tmp/notochord-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notochord-0.5.1.tar", max compression
+gzip compressed data, was "notochord-0.5.2.tar", max compression
```

## Comparing `notochord-0.5.1.tar` & `notochord-0.5.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0     1084 2023-11-28 17:22:02.563723 notochord-0.5.1/LICENSE
--rw-r--r--   0        0        0     4650 2024-05-15 20:23:17.997516 notochord-0.5.1/README.md
--rw-r--r--   0        0        0      833 2024-05-15 20:38:01.811173 notochord-0.5.1/pyproject.toml
--rw-r--r--   0        0        0       87 2023-11-28 17:22:02.566423 notochord-0.5.1/src/notochord/__init__.py
--rw-r--r--   0        0        0      898 2024-05-15 20:23:17.997905 notochord-0.5.1/src/notochord/__main__.py
--rw-r--r--   0        0        0      163 2023-11-28 17:22:02.566552 notochord-0.5.1/src/notochord/app/__init__.py
--rw-r--r--   0        0        0      316 2023-11-28 17:22:02.566610 notochord-0.5.1/src/notochord/app/harmonizer.css
--rw-r--r--   0        0        0    10522 2023-11-28 17:22:02.566797 notochord-0.5.1/src/notochord/app/harmonizer.py
--rw-r--r--   0        0        0     1479 2024-05-15 20:23:17.998076 notochord-0.5.1/src/notochord/app/homunculus.css
--rw-r--r--   0        0        0    44887 2024-05-15 20:23:17.998440 notochord-0.5.1/src/notochord/app/homunculus.py
--rw-r--r--   0        0        0    18983 2023-11-28 17:22:02.567055 notochord-0.5.1/src/notochord/app/improviser-txala.py
--rw-r--r--   0        0        0      385 2023-11-28 17:22:02.567122 notochord-0.5.1/src/notochord/app/improviser.css
--rw-r--r--   0        0        0    19710 2024-04-24 13:59:31.571434 notochord-0.5.1/src/notochord/app/improviser.py
--rw-r--r--   0        0        0     4842 2024-05-15 20:23:17.998613 notochord-0.5.1/src/notochord/app/preset.json
--rw-r--r--   0        0        0     4413 2024-05-15 20:23:17.998802 notochord-0.5.1/src/notochord/app/server.py
--rw-r--r--   0        0        0     3073 2023-11-28 17:22:02.567375 notochord-0.5.1/src/notochord/app/simple_harmonizer.py
--rw-r--r--   0        0        0    10631 2024-04-24 13:59:31.572536 notochord-0.5.1/src/notochord/data.py
--rw-r--r--   0        0        0    12790 2023-11-28 17:22:02.567536 notochord-0.5.1/src/notochord/distributions.py
--rw-r--r--   0        0        0    47353 2024-05-15 20:23:17.999241 notochord-0.5.1/src/notochord/model.py
--rw-r--r--   0        0        0    12706 2024-04-24 13:59:31.573908 notochord-0.5.1/src/notochord/perform.py
--rw-r--r--   0        0        0     2528 2023-11-28 17:22:02.567874 notochord-0.5.1/src/notochord/rnn.py
--rw-r--r--   0        0        0    13940 2024-04-24 13:59:31.574327 notochord-0.5.1/src/notochord/train.py
--rw-r--r--   0        0        0     2488 2023-11-28 17:22:02.568040 notochord-0.5.1/src/notochord/util.py
--rw-r--r--   0        0        0     5443 1970-01-01 00:00:00.000000 notochord-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-11-28 17:22:02.563723 notochord-0.5.2/LICENSE
+-rw-r--r--   0        0        0     4726 2024-05-17 00:10:44.090539 notochord-0.5.2/README.md
+-rw-r--r--   0        0        0      833 2024-05-17 00:16:02.481173 notochord-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0       87 2023-11-28 17:22:02.566423 notochord-0.5.2/src/notochord/__init__.py
+-rw-r--r--   0        0        0      898 2024-05-15 20:23:17.997905 notochord-0.5.2/src/notochord/__main__.py
+-rw-r--r--   0        0        0      163 2023-11-28 17:22:02.566552 notochord-0.5.2/src/notochord/app/__init__.py
+-rw-r--r--   0        0        0      316 2023-11-28 17:22:02.566610 notochord-0.5.2/src/notochord/app/harmonizer.css
+-rw-r--r--   0        0        0    10522 2023-11-28 17:22:02.566797 notochord-0.5.2/src/notochord/app/harmonizer.py
+-rw-r--r--   0        0        0     1479 2024-05-15 20:23:17.998076 notochord-0.5.2/src/notochord/app/homunculus.css
+-rw-r--r--   0        0        0    45875 2024-05-17 00:10:44.091633 notochord-0.5.2/src/notochord/app/homunculus.py
+-rw-r--r--   0        0        0    18983 2023-11-28 17:22:02.567055 notochord-0.5.2/src/notochord/app/improviser-txala.py
+-rw-r--r--   0        0        0      385 2023-11-28 17:22:02.567122 notochord-0.5.2/src/notochord/app/improviser.css
+-rw-r--r--   0        0        0    19710 2024-04-24 13:59:31.571434 notochord-0.5.2/src/notochord/app/improviser.py
+-rw-r--r--   0        0        0     1558 2024-05-16 11:58:41.020109 notochord-0.5.2/src/notochord/app/preset-zeno.json
+-rw-r--r--   0        0        0     4842 2024-05-16 23:35:41.902339 notochord-0.5.2/src/notochord/app/preset.json
+-rw-r--r--   0        0        0     4413 2024-05-15 20:23:17.998802 notochord-0.5.2/src/notochord/app/server.py
+-rw-r--r--   0        0        0     3073 2023-11-28 17:22:02.567375 notochord-0.5.2/src/notochord/app/simple_harmonizer.py
+-rw-r--r--   0        0        0    10631 2024-04-24 13:59:31.572536 notochord-0.5.2/src/notochord/data.py
+-rw-r--r--   0        0        0    12790 2023-11-28 17:22:02.567536 notochord-0.5.2/src/notochord/distributions.py
+-rw-r--r--   0        0        0    47550 2024-05-17 00:10:44.092251 notochord-0.5.2/src/notochord/model.py
+-rw-r--r--   0        0        0    12706 2024-04-24 13:59:31.573908 notochord-0.5.2/src/notochord/perform.py
+-rw-r--r--   0        0        0     2528 2023-11-28 17:22:02.567874 notochord-0.5.2/src/notochord/rnn.py
+-rw-r--r--   0        0        0    13940 2024-04-24 13:59:31.574327 notochord-0.5.2/src/notochord/train.py
+-rw-r--r--   0        0        0     2488 2023-11-28 17:22:02.568040 notochord-0.5.2/src/notochord/util.py
+-rw-r--r--   0        0        0     5519 1970-01-01 00:00:00.000000 notochord-0.5.2/PKG-INFO
```

### Comparing `notochord-0.5.1/LICENSE` & `notochord-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `notochord-0.5.1/README.md` & `notochord-0.5.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Notochord ([Paper](https://zenodo.org/record/7088404 "Notochord AIMC 2022 paper") | [Video](https://www.youtube.com/watch?v=mkBKAyudL0A "Notochord AIMC 2022 video"))
+# Notochord ([Documentation](https://intelligent-instruments-lab.github.io/notochord/) | [Paper](https://zenodo.org/record/7088404 "Notochord AIMC 2022 paper") | [Video](https://www.youtube.com/watch?v=mkBKAyudL0A "Notochord AIMC 2022 video"))
  
 <div align="middle">
 <img alt="Max Ernst, Stratified Rocks, Nature's Gift of Gneiss Lava Iceland Moss 2 kinds of lungwort 2 kinds of ruptures of the perinaeum growths of the heart b) the same thing in a well-polished little box somewhat more expensive, 1920" src="https://user-images.githubusercontent.com/4522484/223191876-251d461a-5bfc-439a-8df0-3841e7c76c4a.jpeg" width="60%" />
 </div>
 
 Notochord is a neural network model for MIDI performances. This package contains the training and inference model implemented in pytorch, as well as interactive MIDI processing apps using iipyper. 
 <!-- Some further examples involving SuperCollider and TidalCycles can be found in the parent repo under `examples`. -->
```

### Comparing `notochord-0.5.1/pyproject.toml` & `notochord-0.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "notochord"
-version = "0.5.1"
+version = "0.5.2"
 description = "Notochord is a real-time neural network model for MIDI performances."
 authors = ["Victor Shepardson <victor.shepardson@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
 torch = ">=1.13,<2.3"
 numpy = "^1.23"
 pandas = "^2.0"
 tqdm = "^4.64"
 sf2utils = "^0.9"
 appdirs = "^1.4.4"
-iipyper = "~0.1.2"
+iipyper = "~0.1.3"
 
 [tool.poetry.group.dev.dependencies]
 mkdocs = "^1.5.3"
 mkdocstrings = {extras = ["python"], version = "^0.23.0"}
 mkdocs-gen-files = "^0.5.0"
 mkdocs-include-markdown-plugin = "^6.0.4"
 mkdocs-material = "^9.4.8"
```

### Comparing `notochord-0.5.1/src/notochord/__main__.py` & `notochord-0.5.2/src/notochord/__main__.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.1/src/notochord/app/harmonizer.py` & `notochord-0.5.2/src/notochord/app/harmonizer.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.1/src/notochord/app/homunculus.css` & `notochord-0.5.2/src/notochord/app/homunculus.css`

 * *Files identical despite different names*

### Comparing `notochord-0.5.1/src/notochord/app/homunculus.py` & `notochord-0.5.2/src/notochord/app/homunculus.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,16 @@
 from textual.widgets import Header, Footer, Static, Button, Log, RichLog, Label
 from textual.screen import Screen
 from textual.containers import Grid
 
 def main(
     checkpoint="notochord-latest.ckpt", # Notochord checkpoint
     config:Dict[int,Dict[str,Any]]=None, # map MIDI channel : GM instrument
+    preset:str=None,
+    preset_file:Path=None,
 
     initial_mute=False, # start with Notochord muted
     initial_query=False, # let Notochord start playing immediately
 
     midi_in:Optional[str]=None, # MIDI port for player input
     midi_out:Optional[str]=None, # MIDI port for Notochord output
     thru=False, # copy player input to output
@@ -132,14 +134,16 @@
                 4:{
                     'mode':'follow', 'source':3, 'inst':10, 'range':(72,96)
                 }, # harmonize channel 3 within upper registers of the glockenspiel
             }
             Notes:
             no 'input' or 'auto' channels should use the same instrument,
             but 'follow' channels may have the same as an 'input' or 'auto'
+        preset: preset name (in preset file) to load config from
+        preset_file: path to JSON file containing dict of name:config (as above)
 
         initial_mute: start 'auto' voices muted so it won't play with input.
         initial_query: query Notochord immediately,
             so 'auto' voices begin playing  without input.
 
         midi_in: MIDI ports for input. 
             default is to use all input ports.
@@ -211,36 +215,46 @@
             assert lo<hi, (i-1,lo,hi)
             return lo, hi
         sf_inst_ranges = {i:_get_range(i) for i in range(1,129)}
         def get_range(i):
             return sf_inst_ranges.get(i, (0,127))
     else:
         def get_range(i):
-            return 0,127
-    
+            return 0,127  
 
     ### Textual UI
     tui = NotoTUI()
     print = notochord.print = iipyper.print = tui.print
     ###
 
-    with open(Path(__file__).parent / 'preset.json') as f:
-        presets = json.load(f)
+    ### presets and config
+    try:
+        if preset_file is None:
+            with open(Path(__file__).parent / 'preset.json') as f:
+                presets = json.load(f)
+        else:
+            with open(preset_file) as f:
+                presets = json.load(f)
+    except Exception:
+        print('WARNING: failed to load presets file')
+        presets = {}
+
     # convert MIDI channels to int
     presets = {p:{int(k):v for k,v in d.items()} for p,d in presets.items()}
 
-    if config is None: config = 'ens1'
-    if isinstance(config, str):
-        config = presets[config]
+    if preset is None and len(presets):
+        preset = list(presets)[0]
+    if isinstance(preset, str):
+        config = presets[preset]
 
     # defaults
     config_in = config
     def default_config_channel():
         return {'mode':'auto', 'inst':1, 'mute':False, 'mono':False, 'source':1}
-    config = {i:default_config_channel() for i in config_in}
+    config = {i:default_config_channel() for i in range(1,17)}
     for k,v in config_in.items():
         config[k].update(v)
 
     def validate_config():
         assert all(
             v['source'] in config for v in config.values() if v['mode']=='follow'
             ), 'ERROR: no source given for follow voice'
@@ -296,41 +310,54 @@
         print("WARNING: auto and input instruments shouldn't overlap")
         print('setting to an anonymous instrument')
         # TODO: set to anon insts without changing mel/drum
         # respecting anon insts selected for player
         raise NotImplementedError
     # TODO:
     # check for repeated insts/channels
+    
+    # load notochord model
+    try:
+        noto = Notochord.from_checkpoint(checkpoint)
+        noto.eval()
+        noto.feed(0,0,0,0)
+        noto.query()
+        noto.reset()
+    except Exception:
+        print("""error loading notochord model""")
+        raise
 
     def warn_inst(i):
         if i > 128:
             if i < 257:
                 print(f"WARNING: drum instrument {i} selected, be sure to select a drum bank in your synthesizer")
             else:
                 print(f"WARNING: instrument {i} is not General MIDI")
 
+    def dedup_inst(c, i):
+        # change to anon if already in use
+        def in_use():
+            return any(
+                c_other!=c and config[c_other]['inst']==i 
+                for c_other in config)
+        if in_use():
+            i = noto.first_anon_like(i)
+        while in_use():
+            i = i+1
+        return i
+
     def do_send_pc(c, i):
         warn_inst(i)
         # convert to 0-index
         midi.program_change(channel=c-1, program=(i-1)%128)
 
-    if send_pc:
-        for c,i in channel_insts():
+    for c,i in channel_insts():
+        if send_pc:
             do_send_pc(c, i)
-    
-    # load notochord model
-    try:
-        noto = Notochord.from_checkpoint(checkpoint)
-        noto.eval()
-        noto.feed(0,0,0,0)
-        noto.query()
-        noto.reset()
-    except Exception:
-        print("""error loading notochord model""")
-        raise
+        config[c]['inst'] = dedup_inst(c, i)
 
     # main stopwatch to track time difference between MIDI events
     stopwatch = Stopwatch()
 
     # simple class to hold pending event prediction
     class Prediction:
         def __init__(self):
@@ -897,36 +924,39 @@
             )
         def on_button_pressed(self, event: Button.Pressed) -> None:
             # print(event.button.id)
             # i = 1
             i = int(event.button.id.split('_')[-1])
             self.app.pop_screen()
             set_inst(self.channel, i)
+        # TODO: on key pressed esc, q: cancel
 
     def set_inst(c, i, update=True):
         print(f'SET INSTRUMENT {i}')
         if c in config:
             prev_i = config[c]['inst']
         else:
             prev_i = None
         if prev_i==i:
-            print('SAME INSTRUMENT')
+            # print('SAME INSTRUMENT')
             return
-        # TODO: warn if instrument already in use?
 
         # for (chan,inst,pitch) in history.note_triples:
         for note in history.notes:
             if note.chan==c and config[note.chan]['mode']!='input':
                 play_event(
                     dict(inst=note.inst, pitch=note.pitch, vel=0),
                     channel=note.chan, 
                     tag='NOTO', memo='change instrument')
         # send pc if appropriate
         if send_pc:
             do_send_pc(c, i)
+
+        i = dedup_inst(c, i)
+        
         # then set config
         config[c]['inst'] = i
         # and call:
         if update:
             update_config()
 
     def set_mute(c, b, update=True):
@@ -1220,15 +1250,15 @@
     'SITAR\n     ', 'BANJO\n     ', 'SHAM \n ISEN', 'KOTO \n     ',
     'KAL  \n IMBA', 'BAG  \n PIPE', 'FID  \n  DLE', 'SHA  \n  NAI',  
     'TINKL\nBELL ', 'AGO  \n   GÔ', 'STEEL\nDRUM ', 'WOOD \nBLOCK', 
     'TAIKO\nDRUM ', 'MELO \n  TOM', 'SYNTH\nDRUM ', ' REV \nCYMBL',  
     'GTR  \n FRET', 'BRE  \n  ATH', ' SEA \nSHORE', 'BIRD \nTWEET',
     'TELE \nPHONE', 'HELI \nCOPTR', 'APP  \nLAUSE', 'GUN  \n SHOT',  
     ' STD \nDRUMS'
-]
+] + ['DRUM \n  KIT']*127 + ['ANON \n MEL ']*32 + ['ANON \nDRUMS']*32
 def inst_label(i):
     if i is None:
         return f"--- \n-----\n-----"
     return f'{i:03d} \n{gm_names[i-1]}'
 ### end def TUI components###
```

### Comparing `notochord-0.5.1/src/notochord/app/improviser-txala.py` & `notochord-0.5.2/src/notochord/app/improviser-txala.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.1/src/notochord/app/improviser.py` & `notochord-0.5.2/src/notochord/app/improviser.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.1/src/notochord/app/preset.json` & `notochord-0.5.2/src/notochord/app/preset.json`

 * *Files identical despite different names*

### Comparing `notochord-0.5.1/src/notochord/app/server.py` & `notochord-0.5.2/src/notochord/app/server.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.1/src/notochord/app/simple_harmonizer.py` & `notochord-0.5.2/src/notochord/app/simple_harmonizer.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.1/src/notochord/data.py` & `notochord-0.5.2/src/notochord/data.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.1/src/notochord/distributions.py` & `notochord-0.5.2/src/notochord/distributions.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.1/src/notochord/model.py` & `notochord-0.5.2/src/notochord/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,14 +322,18 @@
         return r
 
 
     def is_drum(self, inst):
         # TODO: add a constructor argument to specify which are drums
         # hardcoded for now
         return inst > 128 and inst < 257 or inst > 288
+    def first_anon_like(self, inst):
+        # TODO: add a constructor argument to specify how many anon
+        # hardcoded for now
+        return 288 if self.is_drum(inst) else 257
 
     
     def feed(self, inst, pitch, time, vel, **kw):
         """consume an event and advance hidden state
         
         Args:
             inst: int. instrument of current note.
@@ -1188,15 +1192,15 @@
 
         Args:
             path: file path to Notochord model
         """
         if path=="notochord-latest.ckpt":
             import appdirs
             d = Path(appdirs.user_data_dir('Notochord', 'IIL'))
-            d.mkdir(exist_ok=True)
+            d.mkdir(exist_ok=True, parents=True)
             path = d / path
             # maybe download
             if not path.is_file():
                 while True:
                     answer = input("Do you want to download a notochord model? (y/n)")
                     if answer.lower() in ["y","yes"]:
                         download_url('https://github.com/Intelligent-Instruments-Lab/iil-python-tools/releases/download/notochord-v0.4.0/notochord_lakh_50G_deep.pt', path)
```

### Comparing `notochord-0.5.1/src/notochord/perform.py` & `notochord-0.5.2/src/notochord/perform.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.1/src/notochord/rnn.py` & `notochord-0.5.2/src/notochord/rnn.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.1/src/notochord/train.py` & `notochord-0.5.2/src/notochord/train.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.1/src/notochord/util.py` & `notochord-0.5.2/src/notochord/util.py`

 * *Files identical despite different names*

### Comparing `notochord-0.5.1/PKG-INFO` & `notochord-0.5.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: notochord
-Version: 0.5.1
+Version: 0.5.2
 Summary: Notochord is a real-time neural network model for MIDI performances.
 License: MIT
 Author: Victor Shepardson
 Author-email: victor.shepardson@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
-Requires-Dist: iipyper (>=0.1.2,<0.2.0)
+Requires-Dist: iipyper (>=0.1.3,<0.2.0)
 Requires-Dist: numpy (>=1.23,<2.0)
 Requires-Dist: pandas (>=2.0,<3.0)
 Requires-Dist: sf2utils (>=0.9,<0.10)
 Requires-Dist: torch (>=1.13,<2.3)
 Requires-Dist: tqdm (>=4.64,<5.0)
 Description-Content-Type: text/markdown
 
-# Notochord ([Paper](https://zenodo.org/record/7088404 "Notochord AIMC 2022 paper") | [Video](https://www.youtube.com/watch?v=mkBKAyudL0A "Notochord AIMC 2022 video"))
+# Notochord ([Documentation](https://intelligent-instruments-lab.github.io/notochord/) | [Paper](https://zenodo.org/record/7088404 "Notochord AIMC 2022 paper") | [Video](https://www.youtube.com/watch?v=mkBKAyudL0A "Notochord AIMC 2022 video"))
  
 <div align="middle">
 <img alt="Max Ernst, Stratified Rocks, Nature's Gift of Gneiss Lava Iceland Moss 2 kinds of lungwort 2 kinds of ruptures of the perinaeum growths of the heart b) the same thing in a well-polished little box somewhat more expensive, 1920" src="https://user-images.githubusercontent.com/4522484/223191876-251d461a-5bfc-439a-8df0-3841e7c76c4a.jpeg" width="60%" />
 </div>
 
 Notochord is a neural network model for MIDI performances. This package contains the training and inference model implemented in pytorch, as well as interactive MIDI processing apps using iipyper. 
 <!-- Some further examples involving SuperCollider and TidalCycles can be found in the parent repo under `examples`. -->
```

