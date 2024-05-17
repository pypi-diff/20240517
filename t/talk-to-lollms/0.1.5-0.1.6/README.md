# Comparing `tmp/talk_to_lollms-0.1.5.tar.gz` & `tmp/talk_to_lollms-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_to_lollms-0.1.5.tar", last modified: Fri May 17 19:36:41 2024, max compression
+gzip compressed data, was "talk_to_lollms-0.1.6.tar", last modified: Fri May 17 20:01:20 2024, max compression
```

## Comparing `talk_to_lollms-0.1.5.tar` & `talk_to_lollms-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 19:36:41.098109 talk_to_lollms-0.1.5/
--rw-rw-rw-   0        0        0    11558 2024-05-15 21:15:31.000000 talk_to_lollms-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      329 2024-05-17 19:36:41.097109 talk_to_lollms-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0       57 2024-05-15 21:15:31.000000 talk_to_lollms-0.1.5/README.md
--rw-rw-rw-   0        0        0      531 2024-05-17 19:36:29.000000 talk_to_lollms-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-17 19:36:41.099107 talk_to_lollms-0.1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-17 19:36:41.081072 talk_to_lollms-0.1.5/talk_to_lollms/
--rw-rw-rw-   0        0        0        0 2024-05-15 23:47:06.000000 talk_to_lollms-0.1.5/talk_to_lollms/__init__.py
--rw-rw-rw-   0        0        0    23212 2024-05-17 19:35:47.000000 talk_to_lollms-0.1.5/talk_to_lollms/main.py
-drwxrwxrwx   0        0        0        0 2024-05-17 19:36:41.096108 talk_to_lollms-0.1.5/talk_to_lollms.egg-info/
--rw-rw-rw-   0        0        0      329 2024-05-17 19:36:41.000000 talk_to_lollms-0.1.5/talk_to_lollms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2024-05-17 19:36:41.000000 talk_to_lollms-0.1.5/talk_to_lollms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 19:36:41.000000 talk_to_lollms-0.1.5/talk_to_lollms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-05-17 19:36:41.000000 talk_to_lollms-0.1.5/talk_to_lollms.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       48 2024-05-17 19:36:41.000000 talk_to_lollms-0.1.5/talk_to_lollms.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-17 19:36:41.000000 talk_to_lollms-0.1.5/talk_to_lollms.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 20:01:20.834388 talk_to_lollms-0.1.6/
+-rw-rw-rw-   0        0        0    11558 2024-05-15 21:15:31.000000 talk_to_lollms-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0       45 2024-05-17 20:01:07.000000 talk_to_lollms-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      329 2024-05-17 20:01:20.833384 talk_to_lollms-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       57 2024-05-15 21:15:31.000000 talk_to_lollms-0.1.6/README.md
+-rw-rw-rw-   0        0        0      602 2024-05-17 20:01:12.000000 talk_to_lollms-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-17 20:01:20.834388 talk_to_lollms-0.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 20:01:20.819864 talk_to_lollms-0.1.6/talk_to_lollms/
+-rw-rw-rw-   0        0        0        0 2024-05-15 23:47:06.000000 talk_to_lollms-0.1.6/talk_to_lollms/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 20:01:20.831388 talk_to_lollms-0.1.6/talk_to_lollms/assets/
+-rw-rw-rw-   0        0        0     3205 2024-05-15 23:43:16.000000 talk_to_lollms-0.1.6/talk_to_lollms/assets/settings.svg
+-rw-rw-rw-   0        0        0    24346 2024-05-17 19:59:18.000000 talk_to_lollms-0.1.6/talk_to_lollms/main.py
+drwxrwxrwx   0        0        0        0 2024-05-17 20:01:20.832389 talk_to_lollms-0.1.6/talk_to_lollms.egg-info/
+-rw-rw-rw-   0        0        0      329 2024-05-17 20:01:20.000000 talk_to_lollms-0.1.6/talk_to_lollms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2024-05-17 20:01:20.000000 talk_to_lollms-0.1.6/talk_to_lollms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 20:01:20.000000 talk_to_lollms-0.1.6/talk_to_lollms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-17 20:01:20.000000 talk_to_lollms-0.1.6/talk_to_lollms.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       48 2024-05-17 20:01:20.000000 talk_to_lollms-0.1.6/talk_to_lollms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-17 20:01:20.000000 talk_to_lollms-0.1.6/talk_to_lollms.egg-info/top_level.txt
```

### Comparing `talk_to_lollms-0.1.5/LICENSE` & `talk_to_lollms-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `talk_to_lollms-0.1.5/pyproject.toml` & `talk_to_lollms-0.1.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "talk_to_lollms"
-version = "0.1.5"
+version = "0.1.6"
 description = "A client for Lollms that allows audio to audio full interaction with Lollms"
 authors = [
     { name = "ParisNeo", email = "parisneoai@gmail.com" }
 ]
 dependencies = [
     "requests",
     "pydantic",
@@ -17,7 +17,10 @@
 ]
 
 [project.scripts]
 talk_to_lollms = "talk_to_lollms:main"
 
 [tool.setuptools]
 packages = ["talk_to_lollms"]
+
+[tool.setuptools.package-data]
+"talk_to_lollms" = ["assets/*.svg"]
```

### Comparing `talk_to_lollms-0.1.5/talk_to_lollms/main.py` & `talk_to_lollms-0.1.6/talk_to_lollms/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import whisper
 from ascii_colors import ASCIIColors, trace_exception
 from lollms_client import LollmsClient, LollmsDiscussion, LollmsXTTS
 import gc
 import requests
 from pathlib import Path
 import re
+import importlib
 class TranscriptionSignal(QObject):
     new_user_transcription = pyqtSignal(str, str)
     new_lollms_transcription = pyqtSignal(str, str)
     update_status = pyqtSignal(str)
 
 class AudioRecorder:
     def __init__(self, lollms_address="http://localhost:9600", cond="Act as a helpful AI assistant called lollms.", threshold=1000, silence_duration=2, sound_threshold_percentage=10, gain=1.0, rate=44100, channels=1, buffer_size=10, model="small.en", snd_device=None, logs_folder="logs", voice=None, block_while_talking=True, context_size=4096):
@@ -302,30 +303,40 @@
         # Title Label
         title_label = QLabel('Talk to LoLLMs')
         title_font = QFont('Arial', 24, QFont.Bold)
         title_label.setFont(title_font)
         title_label.setAlignment(Qt.AlignCenter)
 
         # Record Button
+        
         self.record_button = QPushButton('Start Recording')
         self.record_button.setFont(QFont('Arial', 14))
         self.record_button.setStyleSheet("background-color: #4CAF50; color: white; padding: 10px; border-radius: 5px;")
         self.record_button.clicked.connect(self.toggle_recording)
 
         # Settings Button
         self.settings_button = QPushButton()
-        self.settings_button.setIcon(QIcon('assets/settings.svg'))  # Load the SVG icon
+
+        # Get the path to the SVG file
+        try:
+            icon_path = importlib.resources.files('talk_to_lollms.assets').joinpath('settings.svg')
+            # Load the SVG icon
+            self.settings_button.setIcon(QIcon(str(icon_path)))
+        except:
+            try:
+                self.settings_button.setIcon(QIcon("talk_to_lollms/assets/settings.svg"))
+            except:
+                pass
         self.settings_button.setIconSize(QSize(24, 24))
         self.settings_button.clicked.connect(self.show_settings_dialog)
 
         # Text Edit for Transcriptions
         self.text_edit = QTextEdit()
         self.text_edit.setFont(QFont('Arial', 12))
-        self.text_edit.setStyleSheet("background-color: #f0f0f0; padding: 10px; border-radius: 5px;")
-
+        self.text_edit.setStyleSheet("background-color: #ffffff; font-family: Arial, sans-serif; font-size: 14px; padding: 10px;")
         # Status Bar
         self.status_bar = QStatusBar()
         self.setStatusBar(self.status_bar)
 
         layout = QVBoxLayout()
         layout.addWidget(title_label)
         layout.addWidget(self.record_button)
@@ -380,15 +391,15 @@
         voices_list.setCurrentText(str(self.recorder.snd_device))
 
         block_while_talking_input = QCheckBox()
         block_while_talking_input.setChecked(self.recorder.block_while_talking)
 
         context_size_input = QSpinBox()
         context_size_input.setMaximum(100000000)
-        context_size_input.setValue(self.recorder.context_size)
+        context_size_input.setValue(self.recorder.context_size if type(self.recorder.context_size)==int else 4096)
         
 
         def open_folder_dialog():
             folder_path = QFileDialog.getExistingDirectory(dialog, "Select Logs Folder")
             if folder_path:
                 logs_folder_input.setText(folder_path)
         
@@ -508,21 +519,33 @@
                 self.recorder.voice = settings.get('voice',"")
                 self.recorder.context_size = settings.get('context_size',"")
                 
                 
         except FileNotFoundError:
             pass
 
-    def display_user_transcription(self, filename, transcription:str):
-        transcription = transcription.replace('\n','<br>')
-        self.text_edit.append(f"<b>User:</b><br>{transcription}<br>")
-
-    def display_lollms_transcription(self, filename, transcription:str):
-        transcription = transcription.replace('\n','<br>')
-        self.text_edit.append(f"<b>LoLLMs:</b><br>{transcription}<br>")
+    def display_user_transcription(self, filename, transcription: str):
+        transcription = transcription.replace('\n', '<br>')
+        user_html = f"""
+        <div style="background-color: #e1f5fe; border: 1px solid #0277bd; border-radius: 10px; padding: 10px; margin: 5px 0; max-width: 70%; word-wrap: break-word;">
+            <b style="color: #0277bd;">User:</b><br>
+            <span>{transcription}</span>
+        </div>
+        """
+        self.text_edit.append(user_html)
+
+    def display_lollms_transcription(self, filename, transcription: str):
+        transcription = transcription.replace('\n', '<br>')
+        lollms_html = f"""
+        <div style="background-color: #e8f5e9; border: 1px solid #388e3c; border-radius: 10px; padding: 10px; margin: 5px 0; max-width: 70%; word-wrap: break-word; align-self: flex-end; text-align: right;">
+            <b style="color: #388e3c;">LoLLMs:</b><br>
+            <span>{transcription}</span>
+        </div>
+        """
+        self.text_edit.append(f'<div style="display: flex; justify-content: flex-end;">{lollms_html}</div>')
 
     def update_status_bar(self, message:str):
         self.status_bar.showMessage(message)  # Display message for 5 seconds
 
 
 
 if __name__ == '__main__':
```

