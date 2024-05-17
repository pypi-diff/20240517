# Comparing `tmp/talk_to_lollms-0.1.0.tar.gz` & `tmp/talk_to_lollms-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_to_lollms-0.1.0.tar", last modified: Thu May 16 00:30:42 2024, max compression
+gzip compressed data, was "talk_to_lollms-0.1.1.tar", last modified: Fri May 17 18:26:42 2024, max compression
```

## Comparing `talk_to_lollms-0.1.0.tar` & `talk_to_lollms-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 00:30:42.954887 talk_to_lollms-0.1.0/
--rw-rw-rw-   0        0        0    11558 2024-05-15 21:15:31.000000 talk_to_lollms-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      304 2024-05-16 00:30:42.953825 talk_to_lollms-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       57 2024-05-15 21:15:31.000000 talk_to_lollms-0.1.0/README.md
--rw-rw-rw-   0        0        0      514 2024-05-16 00:30:34.000000 talk_to_lollms-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-16 00:30:42.954887 talk_to_lollms-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-16 00:30:42.924727 talk_to_lollms-0.1.0/talk_to_lollms/
--rw-rw-rw-   0        0        0        0 2024-05-15 23:47:06.000000 talk_to_lollms-0.1.0/talk_to_lollms/__init__.py
--rw-rw-rw-   0        0        0    16904 2024-05-16 00:29:16.000000 talk_to_lollms-0.1.0/talk_to_lollms/main.py
-drwxrwxrwx   0        0        0        0 2024-05-16 00:30:42.952752 talk_to_lollms-0.1.0/talk_to_lollms.egg-info/
--rw-rw-rw-   0        0        0      304 2024-05-16 00:30:42.000000 talk_to_lollms-0.1.0/talk_to_lollms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2024-05-16 00:30:42.000000 talk_to_lollms-0.1.0/talk_to_lollms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 00:30:42.000000 talk_to_lollms-0.1.0/talk_to_lollms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-05-16 00:30:42.000000 talk_to_lollms-0.1.0/talk_to_lollms.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       39 2024-05-16 00:30:42.000000 talk_to_lollms-0.1.0/talk_to_lollms.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-16 00:30:42.000000 talk_to_lollms-0.1.0/talk_to_lollms.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 18:26:42.340556 talk_to_lollms-0.1.1/
+-rw-rw-rw-   0        0        0    11558 2024-05-15 21:15:31.000000 talk_to_lollms-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      304 2024-05-17 18:26:42.339558 talk_to_lollms-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       57 2024-05-15 21:15:31.000000 talk_to_lollms-0.1.1/README.md
+-rw-rw-rw-   0        0        0      514 2024-05-17 18:24:22.000000 talk_to_lollms-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-17 18:26:42.340556 talk_to_lollms-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 18:26:42.315528 talk_to_lollms-0.1.1/talk_to_lollms/
+-rw-rw-rw-   0        0        0        0 2024-05-15 23:47:06.000000 talk_to_lollms-0.1.1/talk_to_lollms/__init__.py
+-rw-rw-rw-   0        0        0    19113 2024-05-17 18:24:10.000000 talk_to_lollms-0.1.1/talk_to_lollms/main.py
+drwxrwxrwx   0        0        0        0 2024-05-17 18:26:42.338561 talk_to_lollms-0.1.1/talk_to_lollms.egg-info/
+-rw-rw-rw-   0        0        0      304 2024-05-17 18:26:42.000000 talk_to_lollms-0.1.1/talk_to_lollms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2024-05-17 18:26:42.000000 talk_to_lollms-0.1.1/talk_to_lollms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 18:26:42.000000 talk_to_lollms-0.1.1/talk_to_lollms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-17 18:26:42.000000 talk_to_lollms-0.1.1/talk_to_lollms.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       39 2024-05-17 18:26:42.000000 talk_to_lollms-0.1.1/talk_to_lollms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-17 18:26:42.000000 talk_to_lollms-0.1.1/talk_to_lollms.egg-info/top_level.txt
```

### Comparing `talk_to_lollms-0.1.0/LICENSE` & `talk_to_lollms-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `talk_to_lollms-0.1.0/pyproject.toml` & `talk_to_lollms-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "talk_to_lollms"
-version = "0.1.0"
+version = "0.1.1"
 description = "A client for Lollms that allows audio to audio full interaction with Lollms"
 authors = [
     { name = "ParisNeo", email = "parisneoai@gmail.com" }
 ]
 dependencies = [
     "requests",
     "pydantic",
```

### Comparing `talk_to_lollms-0.1.0/talk_to_lollms/main.py` & `talk_to_lollms-0.1.1/talk_to_lollms/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,43 +4,51 @@
 import numpy as np
 import sounddevice as sd
 import wave
 import matplotlib.pyplot as plt
 from collections import deque
 from PyQt5.QtCore import pyqtSignal, QObject
 import json
-from PyQt5.QtWidgets import QStatusBar, QMainWindow, QLabel, QPushButton, QTextEdit, QVBoxLayout, QWidget, QDialog, QFormLayout, QLineEdit, QDialogButtonBox
+from PyQt5.QtWidgets import QMessageBox, QHBoxLayout, QFileDialog, QComboBox, QStatusBar, QMainWindow, QLabel, QPushButton, QTextEdit, QVBoxLayout, QWidget, QDialog, QFormLayout, QLineEdit, QDialogButtonBox
 from PyQt5.QtGui import QFont, QIcon
 from PyQt5.QtWidgets import QApplication, QMainWindow, QPushButton, QTextEdit, QVBoxLayout, QWidget
 from PyQt5.QtWidgets import QMainWindow, QWidget, QVBoxLayout, QPushButton, QTextEdit, QLabel
 from PyQt5.QtCore import Qt, QSize
 from PyQt5.QtGui import QFont
 import whisper
 from ascii_colors import ASCIIColors, trace_exception
 from lollms_client import LollmsClient, LollmsDiscussion, LollmsXTTS
 import gc
+from pathlib import Path
 
 class TranscriptionSignal(QObject):
     new_user_transcription = pyqtSignal(str, str)
     new_lollms_transcription = pyqtSignal(str, str)
     update_status = pyqtSignal(str)
 
 class AudioRecorder:
-    def __init__(self, lollms_address="http://localhost:9600", cond="Act as a helpful AI assistant called lollms.", threshold=500, silence_duration=2, sound_threshold_percentage=10, gain=1.0, rate=44100, channels=1, buffer_size=10, model="small.en"):
+    def __init__(self, lollms_address="http://localhost:9600", cond="Act as a helpful AI assistant called lollms.", threshold=500, silence_duration=2, sound_threshold_percentage=10, gain=1.0, rate=44100, channels=1, buffer_size=10, model="small.en", snd_device=None, logs_folder="logs"):
         self.lc = LollmsClient(lollms_address)
         self.tts = LollmsXTTS(self.lc)
         self.cond = cond
         self.rate = rate
         self.channels = channels
         self.threshold = threshold
         self.silence_duration = silence_duration
         self.buffer_size = buffer_size
         self.gain = gain
         self.sound_threshold_percentage = sound_threshold_percentage
 
+        if snd_device is None:
+            devices = sd.query_devices()
+            snd_device = [device['name'] for device in devices][0]
+
+        self.snd_device = snd_device
+        self.logs_folder = logs_folder
+
         self.frames = []
         self.silence_counter = 0
         self.current_silence_duration = 0
         self.longest_silence_duration = 0
         self.sound_frames = 0
         self.audio_values = []
 
@@ -72,23 +80,24 @@
         threading.Thread(target=self._record).start()
         threading.Thread(target=self._process_files).start()
 
     def stop_recording(self):
         self.stop_flag = True
 
     def _record(self):
+        sd.default.device = self.snd_device
         with sd.InputStream(channels=self.channels, samplerate=self.rate, callback=self.callback, dtype='int16'):
             while not self.stop_flag:
                 time.sleep(0.1)
 
         if self.frames:
             self._save_wav(self.frames)
         self.recording = False
 
-        self._save_histogram(self.audio_values)
+        # self._save_histogram(self.audio_values)
 
     def callback(self, indata, frames, time, status):
         audio_data = np.frombuffer(indata, dtype=np.int16)
         max_value = np.max(audio_data)
         min_value = np.min(audio_data)
 
         if max_value > self.max_audio_value:
@@ -158,14 +167,16 @@
         ASCIIColors.green("<<SEGMENT_RECOVERED>>")
         self.transcription_signal.update_status.emit("Segment detected and saved")
         filename = f"recording_{self.file_index}.wav"
         self.file_index += 1
 
         amplified_frames = self._apply_gain(frames)
         trimmed_frames = self._trim_silence([amplified_frames])
+        logs_file = Path(self.logs_folder)/filename
+        logs_file.parent.mkdir(exist_ok=True, parents=True)
 
         wf = wave.open("logs/"+ filename, 'wb')
         wf.setnchannels(self.channels)
         wf.setsampwidth(2)
         wf.setframerate(self.rate)
         wf.writeframes(trimmed_frames)
         wf.close()
@@ -206,14 +217,15 @@
                     self.transcribed_lock.notify()
                 self.transcription_signal.new_user_transcription.emit(filename, result["text"])
                 self.discussion.add_message("user",result["text"])
                 if result["text"]!="":
                     discussion = self.discussion.format_discussion(4096)
                     print(discussion)
                     self.transcription_signal.update_status.emit("Generating answer")
+                    ASCIIColors.green("<<RESPONDING>>")
                     lollms_text = self.lc.generate_text('!@>system:' + self.cond + discussion+"\n!@>lollms:", personality=0)
                     self.discussion.add_message("lollms",lollms_text)
                     print(lollms_text)
                     self.transcription_signal.update_status.emit("Listening")
                     self.transcription_signal.new_lollms_transcription.emit(filename, lollms_text)
                     self.tts.text2Audio(lollms_text)
 class MainWindow(QMainWindow):
@@ -292,59 +304,82 @@
         silence_duration_input = QLineEdit(str(self.recorder.silence_duration))
         sound_threshold_percentage_input = QLineEdit(str(self.recorder.sound_threshold_percentage))
         gain_input = QLineEdit(str(self.recorder.gain))
         rate_input = QLineEdit(str(self.recorder.rate))
         channels_input = QLineEdit(str(self.recorder.channels))
         buffer_size_input = QLineEdit(str(self.recorder.buffer_size))
         model_input =  QLineEdit(self.recorder.model)
-
+        devices_list = QComboBox(self)
+        devices = sd.query_devices()
+        device_names = [device['name'] for device in devices]
+        devices_list.addItems(device_names)        
+        devices_list.setCurrentText(str(self.recorder.snd_device))
+
+        logs_folder_input = QLineEdit(self.recorder.logs_folder)
+        logs_folder_input.setText(self.recorder.logs_folder)
+        logs_folder_button = QPushButton("...")
         
+        def open_folder_dialog():
+            folder_path = QFileDialog.getExistingDirectory(dialog, "Select Logs Folder")
+            if folder_path:
+                logs_folder_input.setText(folder_path)
+        
+        logs_folder_button.clicked.connect(open_folder_dialog)
+        logs_folder_layout = QHBoxLayout()
+        logs_folder_layout.addWidget(logs_folder_input)
+        logs_folder_layout.addWidget(logs_folder_button)        
+
         form_layout.addRow("LoLLMs Conditionning:", cond_input)
         form_layout.addRow("LoLLMs Address:", lollms_address_input)
         form_layout.addRow("Threshold:", threshold_input)
         form_layout.addRow("Silence Duration:", silence_duration_input)
         form_layout.addRow("Sound Threshold Percentage:", sound_threshold_percentage_input)
         form_layout.addRow("Gain:", gain_input)
         form_layout.addRow("Rate:", rate_input)
         form_layout.addRow("Channels:", channels_input)
         form_layout.addRow("Buffer Size:", buffer_size_input)
         form_layout.addRow("Whisper Model:", model_input)
+        form_layout.addRow("Audio Devices:", devices_list)
+        form_layout.addRow("Logs Folder:", logs_folder_layout)
 
         button_box = QDialogButtonBox(QDialogButtonBox.Ok | QDialogButtonBox.Cancel)
         button_box.accepted.connect(lambda: self.save_settings_and_close(
             dialog,
             cond_input.toPlainText(),
             lollms_address_input.text(),
             int(threshold_input.text()),
             int(silence_duration_input.text()),
             int(sound_threshold_percentage_input.text()),
             float(gain_input.text()),
             int(rate_input.text()),
             int(channels_input.text()),
             int(buffer_size_input.text()),
             model_input.text(),
-            
+            devices_list.currentText(),
+            logs_folder_input.text()
         ))
         button_box.rejected.connect(dialog.reject)
 
         form_layout.addWidget(button_box)
         dialog.setLayout(form_layout)
         dialog.exec_()
 
-    def save_settings_and_close(self, dialog, cond, lollms_address, threshold, silence_duration, sound_threshold_percentage, gain, rate, channels, buffer_size, model):
+    def save_settings_and_close(self, dialog, cond, lollms_address, threshold, silence_duration, sound_threshold_percentage, gain, rate, channels, buffer_size, model, snd_device, logs_folder):
         
         self.recorder.cond = cond
         self.recorder.lc.host_address = lollms_address
         self.recorder.threshold = threshold
         self.recorder.silence_duration = silence_duration
         self.recorder.sound_threshold_percentage = sound_threshold_percentage
         self.recorder.gain = gain
         self.recorder.rate = rate
         self.recorder.channels = channels
         self.recorder.buffer_size = buffer_size
+        self.recorder.snd_device = snd_device
+        self.recorder.logs_folder = logs_folder
         if self.recorder.model != model:
             self.recorder.whisper = None
             gc.collect
             self.recorder.whisper = whisper.load_model(model)
             self.recorder.model = model
 
         settings = {
@@ -352,36 +387,46 @@
             'lollms_address': lollms_address,
             'threshold': threshold,
             'silence_duration': silence_duration,
             'sound_threshold_percentage': sound_threshold_percentage,
             'gain': gain,
             'rate': rate,
             'channels': channels,
-            'buffer_size': buffer_size
+            'buffer_size': buffer_size,
+            'snd_device': snd_device,
+            'logs_folder': logs_folder
         }
 
         with open('settings.json', 'w') as f:
             json.dump(settings, f)
         
         self.update_status_bar("Settings saved")
         dialog.accept()
+        try:
+            sd.default.device = snd_device
+        except Exception as e:
+            QMessageBox.critical(dialog, "Error", f"Failed to set sound device: {e}")
+            return       
 
     def load_settings(self):
         try:
             with open('settings.json', 'r') as f:
                 settings = json.load(f)
                 self.recorder.cond = settings['cond']
                 self.recorder.lc.host_address = settings['lollms_address']
                 self.recorder.threshold = settings['threshold']
                 self.recorder.silence_duration = settings['silence_duration']
                 self.recorder.sound_threshold_percentage = settings['sound_threshold_percentage']
                 self.recorder.gain = settings['gain']
                 self.recorder.rate = settings['rate']
                 self.recorder.channels = settings['channels']
                 self.recorder.buffer_size = settings['buffer_size']
+                self.recorder.snd_device = settings.get('snd_device',"")
+                self.recorder.logs_folder = settings.get('logs_folder',"")
+                
         except FileNotFoundError:
             pass
 
     def display_user_transcription(self, filename, transcription:str):
         transcription = transcription.replace('\n','<br>')
         self.text_edit.append(f"<b>User:</b><br>{transcription}<br>")
```

