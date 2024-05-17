# Comparing `tmp/talk_to_lollms-0.1.3.tar.gz` & `tmp/talk_to_lollms-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_to_lollms-0.1.3.tar", last modified: Fri May 17 18:40:09 2024, max compression
+gzip compressed data, was "talk_to_lollms-0.1.4.tar", last modified: Fri May 17 19:01:08 2024, max compression
```

## Comparing `talk_to_lollms-0.1.3.tar` & `talk_to_lollms-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 18:40:09.705042 talk_to_lollms-0.1.3/
--rw-rw-rw-   0        0        0    11558 2024-05-15 21:15:31.000000 talk_to_lollms-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      304 2024-05-17 18:40:09.704044 talk_to_lollms-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       57 2024-05-15 21:15:31.000000 talk_to_lollms-0.1.3/README.md
--rw-rw-rw-   0        0        0      514 2024-05-17 18:39:46.000000 talk_to_lollms-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-17 18:40:09.705042 talk_to_lollms-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-17 18:40:09.678308 talk_to_lollms-0.1.3/talk_to_lollms/
--rw-rw-rw-   0        0        0        0 2024-05-15 23:47:06.000000 talk_to_lollms-0.1.3/talk_to_lollms/__init__.py
--rw-rw-rw-   0        0        0    19144 2024-05-17 18:39:42.000000 talk_to_lollms-0.1.3/talk_to_lollms/main.py
-drwxrwxrwx   0        0        0        0 2024-05-17 18:40:09.703041 talk_to_lollms-0.1.3/talk_to_lollms.egg-info/
--rw-rw-rw-   0        0        0      304 2024-05-17 18:40:09.000000 talk_to_lollms-0.1.3/talk_to_lollms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2024-05-17 18:40:09.000000 talk_to_lollms-0.1.3/talk_to_lollms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 18:40:09.000000 talk_to_lollms-0.1.3/talk_to_lollms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-05-17 18:40:09.000000 talk_to_lollms-0.1.3/talk_to_lollms.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       39 2024-05-17 18:40:09.000000 talk_to_lollms-0.1.3/talk_to_lollms.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-17 18:40:09.000000 talk_to_lollms-0.1.3/talk_to_lollms.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 19:01:08.163080 talk_to_lollms-0.1.4/
+-rw-rw-rw-   0        0        0    11558 2024-05-15 21:15:31.000000 talk_to_lollms-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      329 2024-05-17 19:01:08.162073 talk_to_lollms-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       57 2024-05-15 21:15:31.000000 talk_to_lollms-0.1.4/README.md
+-rw-rw-rw-   0        0        0      531 2024-05-17 18:43:05.000000 talk_to_lollms-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-17 19:01:08.163080 talk_to_lollms-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 19:01:08.140526 talk_to_lollms-0.1.4/talk_to_lollms/
+-rw-rw-rw-   0        0        0        0 2024-05-15 23:47:06.000000 talk_to_lollms-0.1.4/talk_to_lollms/__init__.py
+-rw-rw-rw-   0        0        0    20510 2024-05-17 18:59:15.000000 talk_to_lollms-0.1.4/talk_to_lollms/main.py
+drwxrwxrwx   0        0        0        0 2024-05-17 19:01:08.160566 talk_to_lollms-0.1.4/talk_to_lollms.egg-info/
+-rw-rw-rw-   0        0        0      329 2024-05-17 19:01:08.000000 talk_to_lollms-0.1.4/talk_to_lollms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2024-05-17 19:01:08.000000 talk_to_lollms-0.1.4/talk_to_lollms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 19:01:08.000000 talk_to_lollms-0.1.4/talk_to_lollms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-17 19:01:08.000000 talk_to_lollms-0.1.4/talk_to_lollms.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       48 2024-05-17 19:01:08.000000 talk_to_lollms-0.1.4/talk_to_lollms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-17 19:01:08.000000 talk_to_lollms-0.1.4/talk_to_lollms.egg-info/top_level.txt
```

### Comparing `talk_to_lollms-0.1.3/LICENSE` & `talk_to_lollms-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `talk_to_lollms-0.1.3/pyproject.toml` & `talk_to_lollms-0.1.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "talk_to_lollms"
-version = "0.1.3"
+version = "0.1.4"
 description = "A client for Lollms that allows audio to audio full interaction with Lollms"
 authors = [
     { name = "ParisNeo", email = "parisneoai@gmail.com" }
 ]
 dependencies = [
     "requests",
     "pydantic",
-    "lollms_client>=0.5.9"
+    "lollms_client>=0.5.9",
+    "requests"
 ]
 
 [project.scripts]
 talk_to_lollms = "talk_to_lollms:main"
 
 [tool.setuptools]
 packages = ["talk_to_lollms"]
```

### Comparing `talk_to_lollms-0.1.3/talk_to_lollms/main.py` & `talk_to_lollms-0.1.4/talk_to_lollms/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,25 +14,30 @@
 from PyQt5.QtWidgets import QMainWindow, QWidget, QVBoxLayout, QPushButton, QTextEdit, QLabel
 from PyQt5.QtCore import Qt, QSize
 from PyQt5.QtGui import QFont
 import whisper
 from ascii_colors import ASCIIColors, trace_exception
 from lollms_client import LollmsClient, LollmsDiscussion, LollmsXTTS
 import gc
+import requests
 from pathlib import Path
 
 class TranscriptionSignal(QObject):
     new_user_transcription = pyqtSignal(str, str)
     new_lollms_transcription = pyqtSignal(str, str)
     update_status = pyqtSignal(str)
 
 class AudioRecorder:
-    def __init__(self, lollms_address="http://localhost:9600", cond="Act as a helpful AI assistant called lollms.", threshold=500, silence_duration=2, sound_threshold_percentage=10, gain=1.0, rate=44100, channels=1, buffer_size=10, model="small.en", snd_device=None, logs_folder="logs"):
+    def __init__(self, lollms_address="http://localhost:9600", cond="Act as a helpful AI assistant called lollms.", threshold=1000, silence_duration=2, sound_threshold_percentage=10, gain=1.0, rate=44100, channels=1, buffer_size=10, model="small.en", snd_device=None, logs_folder="logs", voice=None):
         self.lc = LollmsClient(lollms_address)
         self.tts = LollmsXTTS(self.lc)
+        if not voice:
+            voices = self.get_voices(lollms_address)
+            voice = voices[0]
+        self.voice = voice
         self.cond = cond
         self.rate = rate
         self.channels = channels
         self.threshold = threshold
         self.silence_duration = silence_duration
         self.buffer_size = buffer_size
         self.gain = gain
@@ -170,15 +175,15 @@
         self.file_index += 1
 
         amplified_frames = self._apply_gain(frames)
         trimmed_frames = self._trim_silence([amplified_frames])
         logs_file = Path(self.logs_folder)/filename
         logs_file.parent.mkdir(exist_ok=True, parents=True)
 
-        wf = wave.open(logs_file, 'wb')
+        wf = wave.open(str(logs_file), 'wb')
         wf.setnchannels(self.channels)
         wf.setsampwidth(2)
         wf.setframerate(self.rate)
         wf.writeframes(trimmed_frames)
         wf.close()
 
         with self.buffer_lock:
@@ -191,16 +196,21 @@
         plt.hist(audio_values, bins=50, edgecolor='black')
         plt.title('Histogram of Audio Values')
         plt.xlabel('Audio Value')
         plt.ylabel('Frequency')
         plt.savefig('audio_values_histogram.png')
         plt.close()
 
+    def fix_string_for_xtts(self, input_string):
+        # Remove excessive exclamation marks
+        fixed_string = input_string.rstrip('!') + '!'
+        return fixed_string
+    
     def _process_files(self):
-        while not self.stop_flag or len(self.buffer) > 0:
+        while not self.stop_flag:
             with self.buffer_lock:
                 while not self.buffer and not self.stop_flag:
                     self.buffer_lock.wait()
                 if self.buffer:
                     filename = self.buffer.popleft()
                     self.buffer_lock.notify()
 
@@ -218,20 +228,32 @@
                 self.transcription_signal.new_user_transcription.emit(filename, result["text"])
                 self.discussion.add_message("user",result["text"])
                 if result["text"]!="":
                     discussion = self.discussion.format_discussion(4096)
                     print(discussion)
                     self.transcription_signal.update_status.emit("Generating answer")
                     ASCIIColors.green("<<RESPONDING>>")
-                    lollms_text = self.lc.generate_text('!@>system:' + self.cond + discussion+"\n!@>lollms:", personality=0)
+                    lollms_text = self.fix_string_for_xtts(self.lc.generate_text('!@>system:' + self.cond + discussion+"\n!@>lollms:", personality=0))
                     self.discussion.add_message("lollms",lollms_text)
                     print(lollms_text)
                     self.transcription_signal.update_status.emit("Listening")
                     self.transcription_signal.new_lollms_transcription.emit(filename, lollms_text)
-                    self.tts.text2Audio(lollms_text)
+                    self.tts.text2Audio(lollms_text, voice=self.voice)
+
+    def get_voices(self, host_address):
+        endpoint = f"{host_address}/list_voices"
+        try:
+            response = requests.get(endpoint)
+            response.raise_for_status()  # Raise an error for bad status codes
+            voices = response.json()  # Assuming the response is in JSON format
+            return voices["voices"]
+        except requests.exceptions.RequestException as e:
+            print(f"Couldn't list voices: {e}")
+            return ["main_voice"]
+
 class MainWindow(QMainWindow):
     def __init__(self):
         super().__init__()
 
         self.recorder = AudioRecorder()
         self.recorder.transcription_signal.new_user_transcription.connect(self.display_user_transcription)
         self.recorder.transcription_signal.new_lollms_transcription.connect(self.display_lollms_transcription)
@@ -289,14 +311,15 @@
             self.update_status_bar("Recording stopped")
         else:
             self.recorder.start_recording()
             self.record_button.setText('Stop Recording')
             self.record_button.setStyleSheet("background-color: #f44336; color: white; padding: 10px; border-radius: 5px;")
             self.update_status_bar("Recording started")
 
+
     def show_settings_dialog(self):
         dialog = QDialog(self)
         dialog.setWindowTitle("Settings")
         form_layout = QFormLayout()
 
         cond_input =  QTextEdit(self.recorder.cond)
         lollms_address_input = QLineEdit(self.recorder.lc.host_address)
@@ -313,15 +336,21 @@
         device_names = [device['name'] for device in devices]
         devices_list.addItems(device_names)        
         devices_list.setCurrentText(str(self.recorder.snd_device))
 
         logs_folder_input = QLineEdit(self.recorder.logs_folder)
         logs_folder_input.setText(self.recorder.logs_folder)
         logs_folder_button = QPushButton("...")
-        
+
+        voices_list = QComboBox(self)
+        voices_list_values = self.recorder.get_voices(self.recorder.lc.host_address)
+        voices_list.addItems(voices_list_values)        
+        voices_list.setCurrentText(str(self.recorder.snd_device))
+
+
         def open_folder_dialog():
             folder_path = QFileDialog.getExistingDirectory(dialog, "Select Logs Folder")
             if folder_path:
                 logs_folder_input.setText(folder_path)
         
         logs_folder_button.clicked.connect(open_folder_dialog)
         logs_folder_layout = QHBoxLayout()
@@ -336,14 +365,16 @@
         form_layout.addRow("Gain:", gain_input)
         form_layout.addRow("Rate:", rate_input)
         form_layout.addRow("Channels:", channels_input)
         form_layout.addRow("Buffer Size:", buffer_size_input)
         form_layout.addRow("Whisper Model:", model_input)
         form_layout.addRow("Audio Devices:", devices_list)
         form_layout.addRow("Logs Folder:", logs_folder_layout)
+        form_layout.addRow("Voices List:", voices_list)
+        
 
         button_box = QDialogButtonBox(QDialogButtonBox.Ok | QDialogButtonBox.Cancel)
         button_box.accepted.connect(lambda: self.save_settings_and_close(
             dialog,
             cond_input.toPlainText(),
             lollms_address_input.text(),
             int(threshold_input.text()),
@@ -351,35 +382,37 @@
             int(sound_threshold_percentage_input.text()),
             float(gain_input.text()),
             int(rate_input.text()),
             int(channels_input.text()),
             int(buffer_size_input.text()),
             model_input.text(),
             devices_list.currentText(),
-            logs_folder_input.text()
+            logs_folder_input.text(),
+            voices_list.currentText()
         ))
         button_box.rejected.connect(dialog.reject)
 
         form_layout.addWidget(button_box)
         dialog.setLayout(form_layout)
         dialog.exec_()
 
-    def save_settings_and_close(self, dialog, cond, lollms_address, threshold, silence_duration, sound_threshold_percentage, gain, rate, channels, buffer_size, model, snd_device, logs_folder):
+    def save_settings_and_close(self, dialog, cond, lollms_address, threshold, silence_duration, sound_threshold_percentage, gain, rate, channels, buffer_size, model, snd_device, logs_folder, voice):
         
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
+        self.recorder.voice = voice
         if self.recorder.model != model:
             self.recorder.whisper = None
             gc.collect
             self.recorder.whisper = whisper.load_model(model)
             self.recorder.model = model
 
         settings = {
@@ -389,15 +422,16 @@
             'silence_duration': silence_duration,
             'sound_threshold_percentage': sound_threshold_percentage,
             'gain': gain,
             'rate': rate,
             'channels': channels,
             'buffer_size': buffer_size,
             'snd_device': snd_device,
-            'logs_folder': logs_folder
+            'logs_folder': logs_folder,
+            'voice': voice
         }
 
         with open('settings.json', 'w') as f:
             json.dump(settings, f)
         
         self.update_status_bar("Settings saved")
         dialog.accept()
@@ -418,14 +452,15 @@
                 self.recorder.sound_threshold_percentage = settings['sound_threshold_percentage']
                 self.recorder.gain = settings['gain']
                 self.recorder.rate = settings['rate']
                 self.recorder.channels = settings['channels']
                 self.recorder.buffer_size = settings['buffer_size']
                 self.recorder.snd_device = settings.get('snd_device',"")
                 self.recorder.logs_folder = settings.get('logs_folder',"")
+                self.recorder.voice = settings.get('voice',"")
                 
         except FileNotFoundError:
             pass
 
     def display_user_transcription(self, filename, transcription:str):
         transcription = transcription.replace('\n','<br>')
         self.text_edit.append(f"<b>User:</b><br>{transcription}<br>")
```

