# Comparing `tmp/talk_to_lollms-0.1.1.tar.gz` & `tmp/talk_to_lollms-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_to_lollms-0.1.1.tar", last modified: Fri May 17 18:26:42 2024, max compression
+gzip compressed data, was "talk_to_lollms-0.1.2.tar", last modified: Fri May 17 18:29:03 2024, max compression
```

## Comparing `talk_to_lollms-0.1.1.tar` & `talk_to_lollms-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 18:26:42.340556 talk_to_lollms-0.1.1/
--rw-rw-rw-   0        0        0    11558 2024-05-15 21:15:31.000000 talk_to_lollms-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      304 2024-05-17 18:26:42.339558 talk_to_lollms-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       57 2024-05-15 21:15:31.000000 talk_to_lollms-0.1.1/README.md
--rw-rw-rw-   0        0        0      514 2024-05-17 18:24:22.000000 talk_to_lollms-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-17 18:26:42.340556 talk_to_lollms-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-17 18:26:42.315528 talk_to_lollms-0.1.1/talk_to_lollms/
--rw-rw-rw-   0        0        0        0 2024-05-15 23:47:06.000000 talk_to_lollms-0.1.1/talk_to_lollms/__init__.py
--rw-rw-rw-   0        0        0    19113 2024-05-17 18:24:10.000000 talk_to_lollms-0.1.1/talk_to_lollms/main.py
-drwxrwxrwx   0        0        0        0 2024-05-17 18:26:42.338561 talk_to_lollms-0.1.1/talk_to_lollms.egg-info/
--rw-rw-rw-   0        0        0      304 2024-05-17 18:26:42.000000 talk_to_lollms-0.1.1/talk_to_lollms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2024-05-17 18:26:42.000000 talk_to_lollms-0.1.1/talk_to_lollms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 18:26:42.000000 talk_to_lollms-0.1.1/talk_to_lollms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-05-17 18:26:42.000000 talk_to_lollms-0.1.1/talk_to_lollms.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       39 2024-05-17 18:26:42.000000 talk_to_lollms-0.1.1/talk_to_lollms.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-17 18:26:42.000000 talk_to_lollms-0.1.1/talk_to_lollms.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 18:29:03.245350 talk_to_lollms-0.1.2/
+-rw-rw-rw-   0        0        0    11558 2024-05-15 21:15:31.000000 talk_to_lollms-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      304 2024-05-17 18:29:03.244349 talk_to_lollms-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       57 2024-05-15 21:15:31.000000 talk_to_lollms-0.1.2/README.md
+-rw-rw-rw-   0        0        0      514 2024-05-17 18:28:54.000000 talk_to_lollms-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-17 18:29:03.246345 talk_to_lollms-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 18:29:03.227804 talk_to_lollms-0.1.2/talk_to_lollms/
+-rw-rw-rw-   0        0        0        0 2024-05-15 23:47:06.000000 talk_to_lollms-0.1.2/talk_to_lollms/__init__.py
+-rw-rw-rw-   0        0        0    19152 2024-05-17 18:28:49.000000 talk_to_lollms-0.1.2/talk_to_lollms/main.py
+drwxrwxrwx   0        0        0        0 2024-05-17 18:29:03.243346 talk_to_lollms-0.1.2/talk_to_lollms.egg-info/
+-rw-rw-rw-   0        0        0      304 2024-05-17 18:29:03.000000 talk_to_lollms-0.1.2/talk_to_lollms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2024-05-17 18:29:03.000000 talk_to_lollms-0.1.2/talk_to_lollms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 18:29:03.000000 talk_to_lollms-0.1.2/talk_to_lollms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-17 18:29:03.000000 talk_to_lollms-0.1.2/talk_to_lollms.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       39 2024-05-17 18:29:03.000000 talk_to_lollms-0.1.2/talk_to_lollms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-17 18:29:03.000000 talk_to_lollms-0.1.2/talk_to_lollms.egg-info/top_level.txt
```

### Comparing `talk_to_lollms-0.1.1/LICENSE` & `talk_to_lollms-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `talk_to_lollms-0.1.1/pyproject.toml` & `talk_to_lollms-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "talk_to_lollms"
-version = "0.1.1"
+version = "0.1.2"
 description = "A client for Lollms that allows audio to audio full interaction with Lollms"
 authors = [
     { name = "ParisNeo", email = "parisneoai@gmail.com" }
 ]
 dependencies = [
     "requests",
     "pydantic",
```

### Comparing `talk_to_lollms-0.1.1/talk_to_lollms/main.py` & `talk_to_lollms-0.1.2/talk_to_lollms/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,16 +203,16 @@
                 if self.buffer:
                     filename = self.buffer.popleft()
                     self.buffer_lock.notify()
 
             if filename:
                 self.transcription_signal.update_status.emit("Transcribing")
                 ASCIIColors.green("<<TRANSCRIBING>>")
-                result = self.whisper.transcribe("logs/"+filename)
-                transcription_fn = "logs/"+ filename + ".txt"
+                result = self.whisper.transcribe(str(Path(self.logs_folder)/filename))
+                transcription_fn = str(Path(self.logs_folder)/filename) + ".txt"
                 with open(transcription_fn, "w", encoding="utf-8") as f:
                     f.write(result["text"])
 
                 with self.transcribed_lock:
                     self.transcribed_files.append((filename, result["text"]))
                     self.transcribed_lock.notify()
                 self.transcription_signal.new_user_transcription.emit(filename, result["text"])
```

