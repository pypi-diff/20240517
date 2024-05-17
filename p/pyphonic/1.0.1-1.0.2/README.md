# Comparing `tmp/pyphonic-1.0.1.tar.gz` & `tmp/pyphonic-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyphonic-1.0.1.tar", last modified: Sat Apr 20 04:09:05 2024, max compression
+gzip compressed data, was "pyphonic-1.0.2.tar", last modified: Fri May 17 03:03:09 2024, max compression
```

## Comparing `pyphonic-1.0.1.tar` & `pyphonic-1.0.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:09:05.341449 pyphonic-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-04-20 04:09:05.341449 pyphonic-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-20 04:09:00.000000 pyphonic-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-20 04:09:00.000000 pyphonic-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 04:09:05.341449 pyphonic-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:09:05.333449 pyphonic-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:09:05.337449 pyphonic-1.0.1/src/pyphonic/
--rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-04-20 04:09:00.000000 pyphonic-1.0.1/src/pyphonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-20 04:09:00.000000 pyphonic-1.0.1/src/pyphonic/arp.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-20 04:09:00.000000 pyphonic-1.0.1/src/pyphonic/butterworth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-20 04:09:00.000000 pyphonic-1.0.1/src/pyphonic/circular_buffer_overlap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-20 04:09:00.000000 pyphonic-1.0.1/src/pyphonic/demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-20 04:09:00.000000 pyphonic-1.0.1/src/pyphonic/fft.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-20 04:09:00.000000 pyphonic-1.0.1/src/pyphonic/flipper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-04-20 04:09:00.000000 pyphonic-1.0.1/src/pyphonic/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-20 04:09:00.000000 pyphonic-1.0.1/src/pyphonic/midi_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-20 04:09:00.000000 pyphonic-1.0.1/src/pyphonic/midirando.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-20 04:09:00.000000 pyphonic-1.0.1/src/pyphonic/multithreaded_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-20 04:09:00.000000 pyphonic-1.0.1/src/pyphonic/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-20 04:09:00.000000 pyphonic-1.0.1/src/pyphonic/stretcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-20 04:09:00.000000 pyphonic-1.0.1/src/pyphonic/syncd_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-20 04:09:00.000000 pyphonic-1.0.1/src/pyphonic/torch_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-20 04:09:00.000000 pyphonic-1.0.1/src/pyphonic/torch_saturator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 04:09:05.341449 pyphonic-1.0.1/src/pyphonic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-04-20 04:09:05.000000 pyphonic-1.0.1/src/pyphonic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-20 04:09:05.000000 pyphonic-1.0.1/src/pyphonic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 04:09:05.000000 pyphonic-1.0.1/src/pyphonic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 04:09:05.000000 pyphonic-1.0.1/src/pyphonic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:03:09.166270 pyphonic-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-05-17 03:03:09.166270 pyphonic-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-05-17 03:03:04.000000 pyphonic-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-17 03:03:04.000000 pyphonic-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 03:03:09.166270 pyphonic-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:03:09.162270 pyphonic-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:03:09.166270 pyphonic-1.0.2/src/pyphonic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/10_fftramp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/11_polysynth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/12_syncdnoise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/13_sccompressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/4_butterworth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/5_midiarp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/6_wavetable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/7_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/8_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/9_saturator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/circular_buffer_overlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/flipper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/midi_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/midirando.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/multithreaded_noise.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:03:09.166270 pyphonic-1.0.2/src/pyphonic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-05-17 03:03:09.000000 pyphonic-1.0.2/src/pyphonic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-17 03:03:09.000000 pyphonic-1.0.2/src/pyphonic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 03:03:09.000000 pyphonic-1.0.2/src/pyphonic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 03:03:09.000000 pyphonic-1.0.2/src/pyphonic.egg-info/top_level.txt
```

### Comparing `pyphonic-1.0.1/PKG-INFO` & `pyphonic-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pyphonic
-Version: 1.0.1
+Version: 1.0.2
 Summary: Make a VST plugin for your DAW using Python
 Author-email: AudioFluff <tom@audiofluff.com>, Tom Grek <tom.grek@gmail.com>
-Project-URL: Homepage, https://github.com/tomgrek/pyphonic
-Project-URL: Issues, https://github.com/tomgrek/pyphonic/issues
+Project-URL: Homepage, https://github.com/audiofluff/pyphonic
+Project-URL: Issues, https://github.com/audiofluff/pyphonic/issues
 Classifier: License :: Free for non-commercial use
 Classifier: Topic :: Artistic Software
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: MIDI
 Classifier: Topic :: Multimedia :: Sound/Audio :: Sound Synthesis
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
@@ -27,15 +27,15 @@
 
 The VST streams audio and midi to some server; the server responds with some processed audio.
 
 This library is (one implementation of) the server component.
 
 ## Where do I get the VST?
 
-The VST is not yet released. It's in the final stages of development with release expected in April 2024. If you're interested in beta testing, please get in touch.
+The VST is not yet released. It's in the final stages of development with release expected in May 2024; you can sign up at https://audiofluff.com to get notified when it's released.
 
 ## Quickstart
 
 ##### Super Quick Demo
 
 ```bash
 python -c "import pyphonic; from pyphonic.demo import process;  pyphonic.start(process, 8020)"
@@ -110,15 +110,15 @@
 11. (TODO) `pyphonic.deverb` - A deep learning model trained to remove reverb
 12. (TODO) `pyphonic.source_separation` - A [deep learning model](https://pytorch.org/audio/stable/tutorials/hybrid_demucs_tutorial.html#sphx-glr-tutorials-hybrid-demucs-tutorial-py) trained to separate music into drums, bass, vocals and other
 
 ## Status
 
 The VST is fully functional, rarely crashes, and stays quite performant even under heavy load. Before releasing it (hopefully to the KVR community), I need to 1. make a few more presets that push performance boundaries and check edge cases - dogfooding, basically - 2. write more docs and 3. make a Windows installer. A Mac installer will follow (and Linux if there's interest).
 
-As at mid-March 2024 I reckon this could be by April 2024.
+As at early May 2024 I reckon this should be this month.
 
 ## Development
 
 Contributions welcome!
 
 In particular, the VST plugin automatically pulls `presets.json` and uses that to populate the presets dropdown. If you come up with a great preset and want to share it, please consider making a pull request.
```

### Comparing `pyphonic-1.0.1/README.md` & `pyphonic-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 The VST streams audio and midi to some server; the server responds with some processed audio.
 
 This library is (one implementation of) the server component.
 
 ## Where do I get the VST?
 
-The VST is not yet released. It's in the final stages of development with release expected in April 2024. If you're interested in beta testing, please get in touch.
+The VST is not yet released. It's in the final stages of development with release expected in May 2024; you can sign up at https://audiofluff.com to get notified when it's released.
 
 ## Quickstart
 
 ##### Super Quick Demo
 
 ```bash
 python -c "import pyphonic; from pyphonic.demo import process;  pyphonic.start(process, 8020)"
@@ -93,15 +93,15 @@
 11. (TODO) `pyphonic.deverb` - A deep learning model trained to remove reverb
 12. (TODO) `pyphonic.source_separation` - A [deep learning model](https://pytorch.org/audio/stable/tutorials/hybrid_demucs_tutorial.html#sphx-glr-tutorials-hybrid-demucs-tutorial-py) trained to separate music into drums, bass, vocals and other
 
 ## Status
 
 The VST is fully functional, rarely crashes, and stays quite performant even under heavy load. Before releasing it (hopefully to the KVR community), I need to 1. make a few more presets that push performance boundaries and check edge cases - dogfooding, basically - 2. write more docs and 3. make a Windows installer. A Mac installer will follow (and Linux if there's interest).
 
-As at mid-March 2024 I reckon this could be by April 2024.
+As at early May 2024 I reckon this should be this month.
 
 ## Development
 
 Contributions welcome!
 
 In particular, the VST plugin automatically pulls `presets.json` and uses that to populate the presets dropdown. If you come up with a great preset and want to share it, please consider making a pull request.
```

### Comparing `pyphonic-1.0.1/pyproject.toml` & `pyphonic-1.0.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyphonic"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="AudioFluff", email="tom@audiofluff.com" },
   { name="Tom Grek", email="tom.grek@gmail.com" },
 ]
 description = "Make a VST plugin for your DAW using Python"
 readme = "README.md"
 requires-python = ">=3.8"
@@ -22,9 +22,9 @@
     'Topic :: Multimedia :: Sound/Audio :: MIDI',
     'Topic :: Multimedia :: Sound/Audio :: Sound Synthesis',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'Programming Language :: Python :: 3'
 ]
 
 [project.urls]
-Homepage = "https://github.com/tomgrek/pyphonic"
-Issues = "https://github.com/tomgrek/pyphonic/issues"
+Homepage = "https://github.com/audiofluff/pyphonic"
+Issues = "https://github.com/audiofluff/pyphonic/issues"
```

### Comparing `pyphonic-1.0.1/src/pyphonic/__init__.py` & `pyphonic-1.0.2/src/pyphonic/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,17 +104,15 @@
         return process_fn(midi_messages, audio)
 
     while not should_stop.wait(0.0001):
         while len(in_buffer) and not should_stop.is_set():
             seq_num, audio_in, midi_in = in_buffer.pop(0)
             try:
                 audio_in = struct.unpack(f"<{_state.block_size*_state.num_channels}f", audio_in)
-                new_audio = []
-                for i in range(0, _state.num_channels):
-                    new_audio.append(audio_in[i*_state.block_size:(i+1)*_state.block_size])
+
                 if fn_expects == "npy":
                     audio_in = np.array(audio_in, dtype=np.float32).reshape((_state.num_channels, -1))
                 elif fn_expects == "torch":
                     audio_in = torch.tensor(audio_in, dtype=torch.float32).view((_state.num_channels, -1))
                 elif fn_expects == "list":
                     if _state.num_channels == 1:
                         audio_in = [audio_in]
```

### Comparing `pyphonic-1.0.1/src/pyphonic/butterworth.py` & `pyphonic-1.0.2/src/pyphonic/4_butterworth.py`

 * *Files identical despite different names*

### Comparing `pyphonic-1.0.1/src/pyphonic/circular_buffer_overlap.py` & `pyphonic-1.0.2/src/pyphonic/circular_buffer_overlap.py`

 * *Files identical despite different names*

### Comparing `pyphonic-1.0.1/src/pyphonic/demo.py` & `pyphonic-1.0.2/src/pyphonic/11_polysynth.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,16 @@
                 self.delay_position = 0
 
         return cur
 
 poly = Poly()
 
 def process(midi_messages, audio):
-    poly.set_sample_rate_block_size(pyphonic.getSampleRate(), pyphonic.getBlockSize())
+    num_samples = len(audio[0])
+    poly.set_sample_rate_block_size(pyphonic.getSampleRate(), num_samples)
     for m in midi_messages:
         if m.type == "note_on":
             if m.note < 20:
                 continue
             poly.start_note(m.note, m.velocity/10)
         elif m.type == "note_off":
             poly.stop_note(m.note)
```

### Comparing `pyphonic-1.0.1/src/pyphonic/flipper.py` & `pyphonic-1.0.2/src/pyphonic/flipper.py`

 * *Files identical despite different names*

### Comparing `pyphonic-1.0.1/src/pyphonic/functions.py` & `pyphonic-1.0.2/src/pyphonic/functions.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,66 +22,55 @@
 
 def getSampleRate():
     """
     Returns the sample rate of the audio stream
     """
     return _state.sample_rate
 
-def getBlockSize():
-    """
-    Returns the block size of the audio stream. This is the number of samples
-    per block of audio - each call to the process() function will contain this
-    many samples (per channel).
-    """
-    return _state.block_size
-
-def getNumChannels():
-    """
-    Returns the number of channels in the audio stream. This is typically 1 for
-    mono audio and 2 for stereo audio.
-
-    Currently, > 2 channels are not supported.
-
-    This is the `audio` input into your `process()` function. If the audio is mono, the right channel data will be all zeros.
-    The audio is always shaped as (num_channels, block_size).
-
-    Note that the shape of the audio returned by `process()` must match the shape of the audio input.
-    """
-    return _state.num_channels
-
 def getBPM():
     """
     Returns the current BPM (beats per minute) of the incoming data. This is
     set in the DAW, or defaults to 120 in the standalone plugin.
     """
     return _state.bpm
 
 def getTransport():
     """
-    Returns the current transport state of the DAW. Properties are:
-    - sample_num: the current sample number
-    - bar: the current bar number
-    - beat: the current beat number
-    - ticks: the current tick number
-    - is_playing: whether the DAW is currently playing
+    Returns the current transport state of the DAW.
+
+    Attributes of the returned dict: 
+        ``sample_num``: the current sample number
+
+        ``bar``: the current bar number
+
+        ``beat``: the current beat number
+
+        ``ticks``: the current tick number
+
+        ``is_playing``: whether the DAW is currently playing
+
     """
     return {
         "sample_num": _state.sample_num,
         "bar": _state.bar,
         "beat": _state.beat,
         "ticks": _state.ticks,
         "is_playing": _state.is_playing
     }
 
 def getSignalStats():
     """
-    Returns the current signal statistics of the incoming audio. Properties are:
-    - min: the minimum value of the audio signal
-    - max: the maximum value of the audio signal
-    - rms: the root mean square value of the audio signal
+    Returns the current signal statistics of the incoming audio.
+    
+    Attributes of the returned dict:
+        ``min``: the minimum value of the audio signal
+
+        ``max``: the maximum value of the audio signal
+
+        ``rms``: the root mean square value of the audio signal
 
     Note that stats are calculated over the audio as a whole, not per-channel -
     in other words, the max is the highest value whether left or right. The
     stats are only true for the current block of audio, there's no sliding windows.
 
     Also note that the stats are calculated on the incoming audio before any
     processing/synthesis by Pyphonic.
@@ -95,15 +84,15 @@
 def getDataDir():
     """
     Returns the directory where Pyphonic can store data. This is a directory
     that is guaranteed to be writable by the plugin, and is unique to the
     current user. This is useful for storing samples, presets, and other
     user-specific data.
 
-    On Windows this is typically C:/Users/<username>/AppData/Roaming/AudioFluff/PyPhonic
+    On Windows this is typically ``C:/Users/<username>/AppData/Roaming/AudioFluff/PyPhonic``
     """
     dir_ = Path(platformdirs.user_data_dir("PyPhonic", "AudioFluff", roaming=True))
     if "WSL" in platform.platform():
         paths = os.environ.get("PATH", "").split(":")
         for path in paths:
             if "AppData" in path:
                 path = Path(path.split("AppData")[0])
```

### Comparing `pyphonic-1.0.1/src/pyphonic/midi_parser.py` & `pyphonic-1.0.2/src/pyphonic/midi_parser.py`

 * *Files identical despite different names*

### Comparing `pyphonic-1.0.1/src/pyphonic/sampler.py` & `pyphonic-1.0.2/src/pyphonic/6_wavetable.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# wavetable_synth
+# First builds wavetables from a sample by pitch shifting, then playable with MIDI.
+
 from pathlib import Path
 
 import pyphonic
 from pyphonic import MidiMessage
 import numpy as np
 import librosa
 
@@ -23,38 +26,40 @@
     left = librosa.effects.pitch_shift(sample[0], sr=44100, n_steps=(note - 60))
     right = librosa.effects.pitch_shift(sample[1], sr=44100, n_steps=(note - 60))
     joined = np.array([left, right])
     voices[note] = {"wave": joined, "position": 0, "playing": False, "velocity": 0}
 
 def process_npy(midi, audio):
 
+    num_channels, num_samples = audio.shape
+
     for msg in midi:
         if msg.note not in voices:
             continue
         if msg.type == "note_on":
             if voices[msg.note]["playing"]:
                 voices[msg.note]["position"] = 0
             else:
                 voices[msg.note]["playing"] = True
             voices[msg.note]["velocity"] = msg.velocity
         elif msg.type == "note_off":
             voices[msg.note]["position"] = 0
             voices[msg.note]["playing"] = False
             # Could add some tail off instead of dead stop
     
-    new_audio = np.zeros((pyphonic.getNumChannels(), pyphonic.getBlockSize()))
+    new_audio = np.zeros((num_channels, num_samples))
 
     for voice, data in voices.items():
         if not data["playing"]:
             continue
         start_pos = data["position"] % data["wave"].shape[1]
-        end_pos = (start_pos + pyphonic.getBlockSize())
+        end_pos = (start_pos + num_samples)
         if end_pos >= data["wave"].shape[1]:
             end_pos = data["wave"].shape[1]
             new_audio[:, :end_pos - start_pos] += data["wave"][:, start_pos:end_pos]
             voices[voice]["position"] = 0
             voices[voice]["playing"] = False
         else:
             new_audio += data["wave"][:, start_pos:end_pos] * (data["velocity"] / 127)
-            voices[voice]["position"] += pyphonic.getBlockSize()
+            voices[voice]["position"] += num_samples
     
     return midi, new_audio
```

### Comparing `pyphonic-1.0.1/src/pyphonic/stretcher.py` & `pyphonic-1.0.2/src/pyphonic/7_sampler.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# time_stretching_sampler
+# Stretches the duration of a sample without affecting pitch. Playable with MIDI; samples will start looping faster as they get shorter.
+
 from pathlib import Path
 
 import pyphonic
 from pyphonic import MidiMessage
 import numpy as np
 import librosa
 
@@ -23,36 +26,38 @@
     left = librosa.effects.time_stretch(sample[0], rate=ratio)
     right = librosa.effects.time_stretch(sample[1], rate=ratio)
     joined = np.array([left, right])
     voices[note] = {"wave": joined, "position": 0, "playing": False, "velocity": 0}
 
 def process_npy(midi, audio):
 
+    num_channels, num_samples = audio.shape
+
     for msg in midi:
         if msg.note not in voices:
             continue
         if msg.type == "note_on":
             if voices[msg.note]["playing"]:
                 voices[msg.note]["position"] = 0
             else:
                 voices[msg.note]["playing"] = True
             voices[msg.note]["velocity"] = msg.velocity
         elif msg.type == "note_off":
             voices[msg.note]["position"] = 0
             voices[msg.note]["playing"] = False
     
-    new_audio = np.zeros((pyphonic.getNumChannels(), pyphonic.getBlockSize()))
+    new_audio = np.zeros((num_samples, num_channels))
 
     for voice, data in voices.items():
         if not data["playing"]:
             continue
         start_pos = data["position"] % data["wave"].shape[1]
-        end_pos = (start_pos + pyphonic.getBlockSize())
+        end_pos = (start_pos + num_samples)
         if end_pos >= data["wave"].shape[1]:
             end_pos = data["wave"].shape[1]
             new_audio[:, :end_pos - start_pos] += data["wave"][:, start_pos:end_pos]
             voices[voice]["position"] = 0
         else:
             new_audio += data["wave"][:, start_pos:end_pos] * (data["velocity"] / 127)
-            voices[voice]["position"] += pyphonic.getBlockSize()
+            voices[voice]["position"] += num_samples
     
     return midi, new_audio
```

### Comparing `pyphonic-1.0.1/src/pyphonic/torch_saturator.py` & `pyphonic-1.0.2/src/pyphonic/9_saturator.py`

 * *Files identical despite different names*

### Comparing `pyphonic-1.0.1/src/pyphonic.egg-info/PKG-INFO` & `pyphonic-1.0.2/src/pyphonic.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pyphonic
-Version: 1.0.1
+Version: 1.0.2
 Summary: Make a VST plugin for your DAW using Python
 Author-email: AudioFluff <tom@audiofluff.com>, Tom Grek <tom.grek@gmail.com>
-Project-URL: Homepage, https://github.com/tomgrek/pyphonic
-Project-URL: Issues, https://github.com/tomgrek/pyphonic/issues
+Project-URL: Homepage, https://github.com/audiofluff/pyphonic
+Project-URL: Issues, https://github.com/audiofluff/pyphonic/issues
 Classifier: License :: Free for non-commercial use
 Classifier: Topic :: Artistic Software
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: MIDI
 Classifier: Topic :: Multimedia :: Sound/Audio :: Sound Synthesis
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
@@ -27,15 +27,15 @@
 
 The VST streams audio and midi to some server; the server responds with some processed audio.
 
 This library is (one implementation of) the server component.
 
 ## Where do I get the VST?
 
-The VST is not yet released. It's in the final stages of development with release expected in April 2024. If you're interested in beta testing, please get in touch.
+The VST is not yet released. It's in the final stages of development with release expected in May 2024; you can sign up at https://audiofluff.com to get notified when it's released.
 
 ## Quickstart
 
 ##### Super Quick Demo
 
 ```bash
 python -c "import pyphonic; from pyphonic.demo import process;  pyphonic.start(process, 8020)"
@@ -110,15 +110,15 @@
 11. (TODO) `pyphonic.deverb` - A deep learning model trained to remove reverb
 12. (TODO) `pyphonic.source_separation` - A [deep learning model](https://pytorch.org/audio/stable/tutorials/hybrid_demucs_tutorial.html#sphx-glr-tutorials-hybrid-demucs-tutorial-py) trained to separate music into drums, bass, vocals and other
 
 ## Status
 
 The VST is fully functional, rarely crashes, and stays quite performant even under heavy load. Before releasing it (hopefully to the KVR community), I need to 1. make a few more presets that push performance boundaries and check edge cases - dogfooding, basically - 2. write more docs and 3. make a Windows installer. A Mac installer will follow (and Linux if there's interest).
 
-As at mid-March 2024 I reckon this could be by April 2024.
+As at early May 2024 I reckon this should be this month.
 
 ## Development
 
 Contributions welcome!
 
 In particular, the VST plugin automatically pulls `presets.json` and uses that to populate the presets dropdown. If you come up with a great preset and want to share it, please consider making a pull request.
```

### Comparing `pyphonic-1.0.1/src/pyphonic.egg-info/SOURCES.txt` & `pyphonic-1.0.2/src/pyphonic.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 README.md
 pyproject.toml
+src/pyphonic/10_fftramp.py
+src/pyphonic/11_polysynth.py
+src/pyphonic/12_syncdnoise.py
+src/pyphonic/13_sccompressor.py
+src/pyphonic/4_butterworth.py
+src/pyphonic/5_midiarp.py
+src/pyphonic/6_wavetable.py
+src/pyphonic/7_sampler.py
+src/pyphonic/8_noise.py
+src/pyphonic/9_saturator.py
 src/pyphonic/__init__.py
-src/pyphonic/arp.py
-src/pyphonic/butterworth.py
 src/pyphonic/circular_buffer_overlap.py
-src/pyphonic/demo.py
-src/pyphonic/fft.py
 src/pyphonic/flipper.py
 src/pyphonic/functions.py
 src/pyphonic/midi_parser.py
 src/pyphonic/midirando.py
 src/pyphonic/multithreaded_noise.py
-src/pyphonic/sampler.py
-src/pyphonic/stretcher.py
-src/pyphonic/syncd_noise.py
-src/pyphonic/torch_noise.py
-src/pyphonic/torch_saturator.py
 src/pyphonic.egg-info/PKG-INFO
 src/pyphonic.egg-info/SOURCES.txt
 src/pyphonic.egg-info/dependency_links.txt
 src/pyphonic.egg-info/top_level.txt
```

