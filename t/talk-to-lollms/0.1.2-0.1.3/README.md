# Comparing `tmp/talk_to_lollms-0.1.2.tar.gz` & `tmp/talk_to_lollms-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_to_lollms-0.1.2.tar", last modified: Fri May 17 18:29:03 2024, max compression
+gzip compressed data, was "talk_to_lollms-0.1.3.tar", last modified: Fri May 17 18:40:09 2024, max compression
```

## Comparing `talk_to_lollms-0.1.2.tar` & `talk_to_lollms-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 18:29:03.245350 talk_to_lollms-0.1.2/
--rw-rw-rw-   0        0        0    11558 2024-05-15 21:15:31.000000 talk_to_lollms-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      304 2024-05-17 18:29:03.244349 talk_to_lollms-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       57 2024-05-15 21:15:31.000000 talk_to_lollms-0.1.2/README.md
--rw-rw-rw-   0        0        0      514 2024-05-17 18:28:54.000000 talk_to_lollms-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-17 18:29:03.246345 talk_to_lollms-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-17 18:29:03.227804 talk_to_lollms-0.1.2/talk_to_lollms/
--rw-rw-rw-   0        0        0        0 2024-05-15 23:47:06.000000 talk_to_lollms-0.1.2/talk_to_lollms/__init__.py
--rw-rw-rw-   0        0        0    19152 2024-05-17 18:28:49.000000 talk_to_lollms-0.1.2/talk_to_lollms/main.py
-drwxrwxrwx   0        0        0        0 2024-05-17 18:29:03.243346 talk_to_lollms-0.1.2/talk_to_lollms.egg-info/
--rw-rw-rw-   0        0        0      304 2024-05-17 18:29:03.000000 talk_to_lollms-0.1.2/talk_to_lollms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2024-05-17 18:29:03.000000 talk_to_lollms-0.1.2/talk_to_lollms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 18:29:03.000000 talk_to_lollms-0.1.2/talk_to_lollms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-05-17 18:29:03.000000 talk_to_lollms-0.1.2/talk_to_lollms.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       39 2024-05-17 18:29:03.000000 talk_to_lollms-0.1.2/talk_to_lollms.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-17 18:29:03.000000 talk_to_lollms-0.1.2/talk_to_lollms.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 18:40:09.705042 talk_to_lollms-0.1.3/
+-rw-rw-rw-   0        0        0    11558 2024-05-15 21:15:31.000000 talk_to_lollms-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      304 2024-05-17 18:40:09.704044 talk_to_lollms-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       57 2024-05-15 21:15:31.000000 talk_to_lollms-0.1.3/README.md
+-rw-rw-rw-   0        0        0      514 2024-05-17 18:39:46.000000 talk_to_lollms-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-17 18:40:09.705042 talk_to_lollms-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 18:40:09.678308 talk_to_lollms-0.1.3/talk_to_lollms/
+-rw-rw-rw-   0        0        0        0 2024-05-15 23:47:06.000000 talk_to_lollms-0.1.3/talk_to_lollms/__init__.py
+-rw-rw-rw-   0        0        0    19144 2024-05-17 18:39:42.000000 talk_to_lollms-0.1.3/talk_to_lollms/main.py
+drwxrwxrwx   0        0        0        0 2024-05-17 18:40:09.703041 talk_to_lollms-0.1.3/talk_to_lollms.egg-info/
+-rw-rw-rw-   0        0        0      304 2024-05-17 18:40:09.000000 talk_to_lollms-0.1.3/talk_to_lollms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2024-05-17 18:40:09.000000 talk_to_lollms-0.1.3/talk_to_lollms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 18:40:09.000000 talk_to_lollms-0.1.3/talk_to_lollms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-17 18:40:09.000000 talk_to_lollms-0.1.3/talk_to_lollms.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       39 2024-05-17 18:40:09.000000 talk_to_lollms-0.1.3/talk_to_lollms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-17 18:40:09.000000 talk_to_lollms-0.1.3/talk_to_lollms.egg-info/top_level.txt
```

### Comparing `talk_to_lollms-0.1.2/LICENSE` & `talk_to_lollms-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `talk_to_lollms-0.1.2/pyproject.toml` & `talk_to_lollms-0.1.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "talk_to_lollms"
-version = "0.1.2"
+version = "0.1.3"
 description = "A client for Lollms that allows audio to audio full interaction with Lollms"
 authors = [
     { name = "ParisNeo", email = "parisneoai@gmail.com" }
 ]
 dependencies = [
     "requests",
     "pydantic",
```

### Comparing `talk_to_lollms-0.1.2/talk_to_lollms/main.py` & `talk_to_lollms-0.1.3/talk_to_lollms/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
         self.file_index += 1
 
         amplified_frames = self._apply_gain(frames)
         trimmed_frames = self._trim_silence([amplified_frames])
         logs_file = Path(self.logs_folder)/filename
         logs_file.parent.mkdir(exist_ok=True, parents=True)
 
-        wf = wave.open("logs/"+ filename, 'wb')
+        wf = wave.open(logs_file, 'wb')
         wf.setnchannels(self.channels)
         wf.setsampwidth(2)
         wf.setframerate(self.rate)
         wf.writeframes(trimmed_frames)
         wf.close()
 
         with self.buffer_lock:
```

