# Comparing `tmp/talk_to_lollms-0.1.4.tar.gz` & `tmp/talk_to_lollms-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_to_lollms-0.1.4.tar", last modified: Fri May 17 19:01:08 2024, max compression
+gzip compressed data, was "talk_to_lollms-0.1.5.tar", last modified: Fri May 17 19:36:41 2024, max compression
```

## Comparing `talk_to_lollms-0.1.4.tar` & `talk_to_lollms-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 19:01:08.163080 talk_to_lollms-0.1.4/
--rw-rw-rw-   0        0        0    11558 2024-05-15 21:15:31.000000 talk_to_lollms-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      329 2024-05-17 19:01:08.162073 talk_to_lollms-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       57 2024-05-15 21:15:31.000000 talk_to_lollms-0.1.4/README.md
--rw-rw-rw-   0        0        0      531 2024-05-17 18:43:05.000000 talk_to_lollms-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-17 19:01:08.163080 talk_to_lollms-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-17 19:01:08.140526 talk_to_lollms-0.1.4/talk_to_lollms/
--rw-rw-rw-   0        0        0        0 2024-05-15 23:47:06.000000 talk_to_lollms-0.1.4/talk_to_lollms/__init__.py
--rw-rw-rw-   0        0        0    20510 2024-05-17 18:59:15.000000 talk_to_lollms-0.1.4/talk_to_lollms/main.py
-drwxrwxrwx   0        0        0        0 2024-05-17 19:01:08.160566 talk_to_lollms-0.1.4/talk_to_lollms.egg-info/
--rw-rw-rw-   0        0        0      329 2024-05-17 19:01:08.000000 talk_to_lollms-0.1.4/talk_to_lollms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2024-05-17 19:01:08.000000 talk_to_lollms-0.1.4/talk_to_lollms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 19:01:08.000000 talk_to_lollms-0.1.4/talk_to_lollms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-05-17 19:01:08.000000 talk_to_lollms-0.1.4/talk_to_lollms.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       48 2024-05-17 19:01:08.000000 talk_to_lollms-0.1.4/talk_to_lollms.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-17 19:01:08.000000 talk_to_lollms-0.1.4/talk_to_lollms.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 19:36:41.098109 talk_to_lollms-0.1.5/
+-rw-rw-rw-   0        0        0    11558 2024-05-15 21:15:31.000000 talk_to_lollms-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      329 2024-05-17 19:36:41.097109 talk_to_lollms-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       57 2024-05-15 21:15:31.000000 talk_to_lollms-0.1.5/README.md
+-rw-rw-rw-   0        0        0      531 2024-05-17 19:36:29.000000 talk_to_lollms-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-17 19:36:41.099107 talk_to_lollms-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 19:36:41.081072 talk_to_lollms-0.1.5/talk_to_lollms/
+-rw-rw-rw-   0        0        0        0 2024-05-15 23:47:06.000000 talk_to_lollms-0.1.5/talk_to_lollms/__init__.py
+-rw-rw-rw-   0        0        0    23212 2024-05-17 19:35:47.000000 talk_to_lollms-0.1.5/talk_to_lollms/main.py
+drwxrwxrwx   0        0        0        0 2024-05-17 19:36:41.096108 talk_to_lollms-0.1.5/talk_to_lollms.egg-info/
+-rw-rw-rw-   0        0        0      329 2024-05-17 19:36:41.000000 talk_to_lollms-0.1.5/talk_to_lollms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2024-05-17 19:36:41.000000 talk_to_lollms-0.1.5/talk_to_lollms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 19:36:41.000000 talk_to_lollms-0.1.5/talk_to_lollms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-17 19:36:41.000000 talk_to_lollms-0.1.5/talk_to_lollms.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       48 2024-05-17 19:36:41.000000 talk_to_lollms-0.1.5/talk_to_lollms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-17 19:36:41.000000 talk_to_lollms-0.1.5/talk_to_lollms.egg-info/top_level.txt
```

### Comparing `talk_to_lollms-0.1.4/LICENSE` & `talk_to_lollms-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `talk_to_lollms-0.1.4/pyproject.toml` & `talk_to_lollms-0.1.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "talk_to_lollms"
-version = "0.1.4"
+version = "0.1.5"
 description = "A client for Lollms that allows audio to audio full interaction with Lollms"
 authors = [
     { name = "ParisNeo", email = "parisneoai@gmail.com" }
 ]
 dependencies = [
     "requests",
     "pydantic",
```

### Comparing `talk_to_lollms-0.1.4/talk_to_lollms/main.py` & `talk_to_lollms-0.1.5/talk_to_lollms/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,48 +4,51 @@
 import numpy as np
 import sounddevice as sd
 import wave
 import matplotlib.pyplot as plt
 from collections import deque
 from PyQt5.QtCore import pyqtSignal, QObject
 import json
-from PyQt5.QtWidgets import QMessageBox, QHBoxLayout, QFileDialog, QComboBox, QStatusBar, QMainWindow, QLabel, QPushButton, QTextEdit, QVBoxLayout, QWidget, QDialog, QFormLayout, QLineEdit, QDialogButtonBox
+from PyQt5.QtWidgets import QSpinBox, QCheckBox, QMessageBox, QHBoxLayout, QFileDialog, QComboBox, QStatusBar, QMainWindow, QLabel, QPushButton, QTextEdit, QVBoxLayout, QWidget, QDialog, QFormLayout, QLineEdit, QDialogButtonBox
 from PyQt5.QtGui import QFont, QIcon
 from PyQt5.QtWidgets import QApplication, QMainWindow, QPushButton, QTextEdit, QVBoxLayout, QWidget
 from PyQt5.QtWidgets import QMainWindow, QWidget, QVBoxLayout, QPushButton, QTextEdit, QLabel
 from PyQt5.QtCore import Qt, QSize
 from PyQt5.QtGui import QFont
 import whisper
 from ascii_colors import ASCIIColors, trace_exception
 from lollms_client import LollmsClient, LollmsDiscussion, LollmsXTTS
 import gc
 import requests
 from pathlib import Path
-
+import re
 class TranscriptionSignal(QObject):
     new_user_transcription = pyqtSignal(str, str)
     new_lollms_transcription = pyqtSignal(str, str)
     update_status = pyqtSignal(str)
 
 class AudioRecorder:
-    def __init__(self, lollms_address="http://localhost:9600", cond="Act as a helpful AI assistant called lollms.", threshold=1000, silence_duration=2, sound_threshold_percentage=10, gain=1.0, rate=44100, channels=1, buffer_size=10, model="small.en", snd_device=None, logs_folder="logs", voice=None):
+    def __init__(self, lollms_address="http://localhost:9600", cond="Act as a helpful AI assistant called lollms.", threshold=1000, silence_duration=2, sound_threshold_percentage=10, gain=1.0, rate=44100, channels=1, buffer_size=10, model="small.en", snd_device=None, logs_folder="logs", voice=None, block_while_talking=True, context_size=4096):
         self.lc = LollmsClient(lollms_address)
         self.tts = LollmsXTTS(self.lc)
+        self.block_listening = False
         if not voice:
             voices = self.get_voices(lollms_address)
             voice = voices[0]
         self.voice = voice
+        self.context_size = context_size
         self.cond = cond
         self.rate = rate
         self.channels = channels
         self.threshold = threshold
         self.silence_duration = silence_duration
         self.buffer_size = buffer_size
         self.gain = gain
         self.sound_threshold_percentage = sound_threshold_percentage
+        self.block_while_talking = block_while_talking
 
         if snd_device is None:
             devices = sd.query_devices()
             snd_device = [device['name'] for device in devices][0]
 
         self.snd_device = snd_device
         self.logs_folder = logs_folder
@@ -97,48 +100,60 @@
         if self.frames:
             self._save_wav(self.frames)
         self.recording = False
 
         # self._save_histogram(self.audio_values)
 
     def callback(self, indata, frames, time, status):
-        audio_data = np.frombuffer(indata, dtype=np.int16)
-        max_value = np.max(audio_data)
-        min_value = np.min(audio_data)
-
-        if max_value > self.max_audio_value:
-            self.max_audio_value = max_value
-        if min_value < self.min_audio_value:
-            self.min_audio_value = min_value
-
-        self.audio_values.extend(audio_data)
-
-        self.total_frames += frames
-        if max_value < self.threshold:
-            self.silence_counter += 1
-            self.current_silence_duration += frames
+        if not self.block_listening:
+            audio_data = np.frombuffer(indata, dtype=np.int16)
+            max_value = np.max(audio_data)
+            min_value = np.min(audio_data)
+
+            if max_value > self.max_audio_value:
+                self.max_audio_value = max_value
+            if min_value < self.min_audio_value:
+                self.min_audio_value = min_value
+
+            self.audio_values.extend(audio_data)
+
+            self.total_frames += frames
+            if max_value < self.threshold:
+                self.silence_counter += 1
+                self.current_silence_duration += frames
+            else:
+                self.silence_counter = 0
+                self.current_silence_duration = 0
+                self.sound_frames += frames
+
+            if self.current_silence_duration > self.longest_silence_duration:
+                self.longest_silence_duration = self.current_silence_duration
+
+            if self.silence_counter > (self.rate / frames * self.silence_duration):
+                trimmed_frames = self._trim_silence(self.frames)
+                sound_percentage = self._calculate_sound_percentage(trimmed_frames)
+                if sound_percentage >= self.sound_threshold_percentage:
+                    self._save_wav(self.frames)
+                self.frames = []
+                self.silence_counter = 0
+                self.total_frames = 0
+                self.sound_frames = 0
+            else:
+                self.frames.append(indata.copy())
         else:
-            self.silence_counter = 0
-            self.current_silence_duration = 0
-            self.sound_frames += frames
-
-        if self.current_silence_duration > self.longest_silence_duration:
-            self.longest_silence_duration = self.current_silence_duration
-
-        if self.silence_counter > (self.rate / frames * self.silence_duration):
-            trimmed_frames = self._trim_silence(self.frames)
-            sound_percentage = self._calculate_sound_percentage(trimmed_frames)
-            if sound_percentage >= self.sound_threshold_percentage:
-                self._save_wav(self.frames)
             self.frames = []
             self.silence_counter = 0
-            self.total_frames = 0
+            self.current_silence_duration = 0
+            self.longest_silence_duration = 0
             self.sound_frames = 0
-        else:
-            self.frames.append(indata.copy())
+            self.audio_values = []
+
+            self.max_audio_value = 0
+            self.min_audio_value = 0
+            self.total_frames = 0  # Initialize total_frames
 
     def _apply_gain(self, frames):
         audio_data = np.frombuffer(b''.join(frames), dtype=np.int16)
         audio_data = audio_data * self.gain
         audio_data = np.clip(audio_data, -32768, 32767)
         return audio_data.astype(np.int16).tobytes()
 
@@ -199,49 +214,67 @@
         plt.ylabel('Frequency')
         plt.savefig('audio_values_histogram.png')
         plt.close()
 
     def fix_string_for_xtts(self, input_string):
         # Remove excessive exclamation marks
         fixed_string = input_string.rstrip('!') + '!'
+        
+        # Convert to lower case
+        fixed_string = fixed_string.lower()
+        
+        # Remove any extra non-classical characters
+        fixed_string = re.sub(r'[^a-z0-9,.!?: ]', '', fixed_string)
+        
         return fixed_string
     
     def _process_files(self):
         while not self.stop_flag:
             with self.buffer_lock:
                 while not self.buffer and not self.stop_flag:
                     self.buffer_lock.wait()
                 if self.buffer:
                     filename = self.buffer.popleft()
                     self.buffer_lock.notify()
-
-            if filename:
-                self.transcription_signal.update_status.emit("Transcribing")
-                ASCIIColors.green("<<TRANSCRIBING>>")
-                result = self.whisper.transcribe(str(Path(self.logs_folder)/filename))
-                transcription_fn = str(Path(self.logs_folder)/filename) + ".txt"
-                with open(transcription_fn, "w", encoding="utf-8") as f:
-                    f.write(result["text"])
-
-                with self.transcribed_lock:
-                    self.transcribed_files.append((filename, result["text"]))
-                    self.transcribed_lock.notify()
-                self.transcription_signal.new_user_transcription.emit(filename, result["text"])
-                self.discussion.add_message("user",result["text"])
-                if result["text"]!="":
-                    discussion = self.discussion.format_discussion(4096)
-                    print(discussion)
-                    self.transcription_signal.update_status.emit("Generating answer")
-                    ASCIIColors.green("<<RESPONDING>>")
-                    lollms_text = self.fix_string_for_xtts(self.lc.generate_text('!@>system:' + self.cond + discussion+"\n!@>lollms:", personality=0))
-                    self.discussion.add_message("lollms",lollms_text)
-                    print(lollms_text)
-                    self.transcription_signal.update_status.emit("Listening")
-                    self.transcription_signal.new_lollms_transcription.emit(filename, lollms_text)
-                    self.tts.text2Audio(lollms_text, voice=self.voice)
+            if self.block_while_talking:
+                self.block_listening = True
+            try:
+                if filename:
+                    self.transcription_signal.update_status.emit("Transcribing")
+                    ASCIIColors.green("<<TRANSCRIBING>>")
+                    result = self.whisper.transcribe(str(Path(self.logs_folder)/filename))
+                    transcription_fn = str(Path(self.logs_folder)/filename) + ".txt"
+                    with open(transcription_fn, "w", encoding="utf-8") as f:
+                        f.write(result["text"])
+
+                    with self.transcribed_lock:
+                        self.transcribed_files.append((filename, result["text"]))
+                        self.transcribed_lock.notify()
+                    self.transcription_signal.new_user_transcription.emit(filename, result["text"])
+                    self.discussion.add_message("user",result["text"])
+                    if result["text"]!="":
+                        discussion = self.discussion.format_discussion(self.context_size)
+                        full_context = '!@>system:' + self.cond +"\n" + discussion+"\n!@>lollms:"
+                        ASCIIColors.red(" ---------------- Discussion ---------------------")
+                        ASCIIColors.yellow(full_context)
+                        ASCIIColors.red(" -------------------------------------------------")
+                        self.transcription_signal.update_status.emit("Generating answer")
+                        ASCIIColors.green("<<RESPONDING>>")
+                        lollms_text = self.fix_string_for_xtts(self.lc.generate_text(full_context, personality=0))
+                        self.discussion.add_message("lollms",lollms_text)
+                        ASCIIColors.red(" -------------- LOLLMS answer -------------------")
+                        ASCIIColors.yellow(lollms_text)
+                        ASCIIColors.red(" -------------------------------------------------")
+                        self.transcription_signal.new_lollms_transcription.emit(filename, lollms_text)
+                        self.transcription_signal.update_status.emit("Talking")
+                        self.tts.text2Audio(lollms_text, voice=self.voice)
+            except:
+                pass
+            self.block_listening = False
+            self.transcription_signal.update_status.emit("Listening")
 
     def get_voices(self, host_address):
         endpoint = f"{host_address}/list_voices"
         try:
             response = requests.get(endpoint)
             response.raise_for_status()  # Raise an error for bad status codes
             voices = response.json()  # Assuming the response is in JSON format
@@ -342,14 +375,21 @@
         logs_folder_button = QPushButton("...")
 
         voices_list = QComboBox(self)
         voices_list_values = self.recorder.get_voices(self.recorder.lc.host_address)
         voices_list.addItems(voices_list_values)        
         voices_list.setCurrentText(str(self.recorder.snd_device))
 
+        block_while_talking_input = QCheckBox()
+        block_while_talking_input.setChecked(self.recorder.block_while_talking)
+
+        context_size_input = QSpinBox()
+        context_size_input.setMaximum(100000000)
+        context_size_input.setValue(self.recorder.context_size)
+        
 
         def open_folder_dialog():
             folder_path = QFileDialog.getExistingDirectory(dialog, "Select Logs Folder")
             if folder_path:
                 logs_folder_input.setText(folder_path)
         
         logs_folder_button.clicked.connect(open_folder_dialog)
@@ -366,14 +406,17 @@
         form_layout.addRow("Rate:", rate_input)
         form_layout.addRow("Channels:", channels_input)
         form_layout.addRow("Buffer Size:", buffer_size_input)
         form_layout.addRow("Whisper Model:", model_input)
         form_layout.addRow("Audio Devices:", devices_list)
         form_layout.addRow("Logs Folder:", logs_folder_layout)
         form_layout.addRow("Voices List:", voices_list)
+        form_layout.addRow("Block While Talking:", block_while_talking_input)        
+        form_layout.addRow("Context Size:", context_size_input)
+        
         
 
         button_box = QDialogButtonBox(QDialogButtonBox.Ok | QDialogButtonBox.Cancel)
         button_box.accepted.connect(lambda: self.save_settings_and_close(
             dialog,
             cond_input.toPlainText(),
             lollms_address_input.text(),
@@ -383,36 +426,40 @@
             float(gain_input.text()),
             int(rate_input.text()),
             int(channels_input.text()),
             int(buffer_size_input.text()),
             model_input.text(),
             devices_list.currentText(),
             logs_folder_input.text(),
-            voices_list.currentText()
+            voices_list.currentText(),
+            block_while_talking_input.isChecked(),
+            context_size_input.value()
         ))
         button_box.rejected.connect(dialog.reject)
 
         form_layout.addWidget(button_box)
         dialog.setLayout(form_layout)
         dialog.exec_()
 
-    def save_settings_and_close(self, dialog, cond, lollms_address, threshold, silence_duration, sound_threshold_percentage, gain, rate, channels, buffer_size, model, snd_device, logs_folder, voice):
+    def save_settings_and_close(self, dialog, cond, lollms_address, threshold, silence_duration, sound_threshold_percentage, gain, rate, channels, buffer_size, model, snd_device, logs_folder, voice, block_while_talking, context_size):
         
         self.recorder.cond = cond
         self.recorder.lc.host_address = lollms_address
         self.recorder.threshold = threshold
         self.recorder.silence_duration = silence_duration
         self.recorder.sound_threshold_percentage = sound_threshold_percentage
         self.recorder.gain = gain
         self.recorder.rate = rate
         self.recorder.channels = channels
         self.recorder.buffer_size = buffer_size
         self.recorder.snd_device = snd_device
         self.recorder.logs_folder = logs_folder
         self.recorder.voice = voice
+        self.recorder.block_while_talking = block_while_talking
+        self.context_size = context_size
         if self.recorder.model != model:
             self.recorder.whisper = None
             gc.collect
             self.recorder.whisper = whisper.load_model(model)
             self.recorder.model = model
 
         settings = {
@@ -423,15 +470,17 @@
             'sound_threshold_percentage': sound_threshold_percentage,
             'gain': gain,
             'rate': rate,
             'channels': channels,
             'buffer_size': buffer_size,
             'snd_device': snd_device,
             'logs_folder': logs_folder,
-            'voice': voice
+            'voice': voice,
+            'block_while_talking': block_while_talking,
+            'context_size': context_size
         }
 
         with open('settings.json', 'w') as f:
             json.dump(settings, f)
         
         self.update_status_bar("Settings saved")
         dialog.accept()
@@ -453,14 +502,16 @@
                 self.recorder.gain = settings['gain']
                 self.recorder.rate = settings['rate']
                 self.recorder.channels = settings['channels']
                 self.recorder.buffer_size = settings['buffer_size']
                 self.recorder.snd_device = settings.get('snd_device',"")
                 self.recorder.logs_folder = settings.get('logs_folder',"")
                 self.recorder.voice = settings.get('voice',"")
+                self.recorder.context_size = settings.get('context_size',"")
+                
                 
         except FileNotFoundError:
             pass
 
     def display_user_transcription(self, filename, transcription:str):
         transcription = transcription.replace('\n','<br>')
         self.text_edit.append(f"<b>User:</b><br>{transcription}<br>")
```

