# Comparing `tmp/librus_apix-0.7.7.tar.gz` & `tmp/librus_apix-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librus_apix-0.7.7.tar", last modified: Wed May 15 20:50:12 2024, max compression
+gzip compressed data, was "librus_apix-0.7.8.tar", last modified: Wed May 15 20:56:48 2024, max compression
```

## Comparing `librus_apix-0.7.7.tar` & `librus_apix-0.7.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:50:12.086392 librus_apix-0.7.7/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-15 20:50:04.000000 librus_apix-0.7.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-15 20:50:12.086392 librus_apix-0.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-05-15 20:50:04.000000 librus_apix-0.7.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:50:12.082392 librus_apix-0.7.7/librus_apix/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-15 20:50:04.000000 librus_apix-0.7.7/librus_apix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-15 20:50:04.000000 librus_apix-0.7.7/librus_apix/announcements.py
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-05-15 20:50:04.000000 librus_apix-0.7.7/librus_apix/attendance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-05-15 20:50:04.000000 librus_apix-0.7.7/librus_apix/completed_lessons.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-15 20:50:04.000000 librus_apix-0.7.7/librus_apix/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-05-15 20:50:04.000000 librus_apix-0.7.7/librus_apix/get_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     9740 2024-05-15 20:50:04.000000 librus_apix-0.7.7/librus_apix/grades.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-15 20:50:04.000000 librus_apix-0.7.7/librus_apix/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-15 20:50:04.000000 librus_apix-0.7.7/librus_apix/homework.py
--rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-05-15 20:50:04.000000 librus_apix-0.7.7/librus_apix/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-05-15 20:50:04.000000 librus_apix-0.7.7/librus_apix/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-15 20:50:04.000000 librus_apix-0.7.7/librus_apix/student_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-15 20:50:04.000000 librus_apix-0.7.7/librus_apix/timetable.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-15 20:50:04.000000 librus_apix-0.7.7/librus_apix/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:50:12.086392 librus_apix-0.7.7/librus_apix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-15 20:50:12.000000 librus_apix-0.7.7/librus_apix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-15 20:50:12.000000 librus_apix-0.7.7/librus_apix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:50:12.000000 librus_apix-0.7.7/librus_apix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 20:50:12.000000 librus_apix-0.7.7/librus_apix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 20:50:12.000000 librus_apix-0.7.7/librus_apix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-15 20:50:04.000000 librus_apix-0.7.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-15 20:50:12.086392 librus_apix-0.7.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 20:50:04.000000 librus_apix-0.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:56:48.318264 librus_apix-0.7.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-15 20:56:40.000000 librus_apix-0.7.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-15 20:56:48.318264 librus_apix-0.7.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-05-15 20:56:40.000000 librus_apix-0.7.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:56:48.318264 librus_apix-0.7.8/librus_apix/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-15 20:56:40.000000 librus_apix-0.7.8/librus_apix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-15 20:56:40.000000 librus_apix-0.7.8/librus_apix/announcements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-05-15 20:56:40.000000 librus_apix-0.7.8/librus_apix/attendance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-05-15 20:56:40.000000 librus_apix-0.7.8/librus_apix/completed_lessons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-15 20:56:40.000000 librus_apix-0.7.8/librus_apix/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-05-15 20:56:40.000000 librus_apix-0.7.8/librus_apix/get_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9740 2024-05-15 20:56:40.000000 librus_apix-0.7.8/librus_apix/grades.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-15 20:56:40.000000 librus_apix-0.7.8/librus_apix/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-15 20:56:40.000000 librus_apix-0.7.8/librus_apix/homework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-05-15 20:56:40.000000 librus_apix-0.7.8/librus_apix/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-05-15 20:56:40.000000 librus_apix-0.7.8/librus_apix/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-15 20:56:40.000000 librus_apix-0.7.8/librus_apix/student_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-15 20:56:40.000000 librus_apix-0.7.8/librus_apix/timetable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-15 20:56:40.000000 librus_apix-0.7.8/librus_apix/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:56:48.318264 librus_apix-0.7.8/librus_apix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-15 20:56:48.000000 librus_apix-0.7.8/librus_apix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-15 20:56:48.000000 librus_apix-0.7.8/librus_apix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:56:48.000000 librus_apix-0.7.8/librus_apix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 20:56:48.000000 librus_apix-0.7.8/librus_apix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 20:56:48.000000 librus_apix-0.7.8/librus_apix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-15 20:56:40.000000 librus_apix-0.7.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-15 20:56:48.318264 librus_apix-0.7.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 20:56:40.000000 librus_apix-0.7.8/setup.py
```

### Comparing `librus_apix-0.7.7/LICENSE` & `librus_apix-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.7/README.md` & `librus_apix-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.7/librus_apix/announcements.py` & `librus_apix-0.7.8/librus_apix/announcements.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.7/librus_apix/attendance.py` & `librus_apix-0.7.8/librus_apix/attendance.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.7/librus_apix/completed_lessons.py` & `librus_apix-0.7.8/librus_apix/completed_lessons.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.7/librus_apix/get_token.py` & `librus_apix-0.7.8/librus_apix/get_token.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.7/librus_apix/grades.py` & `librus_apix-0.7.8/librus_apix/grades.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.7/librus_apix/homework.py` & `librus_apix-0.7.8/librus_apix/homework.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.7/librus_apix/messages.py` & `librus_apix-0.7.8/librus_apix/messages.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     author, title, date = trs[:3]
     content = soup.find("div", attrs={"class": "container-message-content"})
     if content is None:
         raise ParseError("Error in parsing message content.")
     return MessageData(
         unwrap_message_data(author),
         unwrap_message_data(title),
-        content,
+        content.text,
         unwrap_message_data(date),
     )
 
 
 def parse_sent(message_soup: BeautifulSoup) -> List[Message]:
     msgs: List[Message] = []
     hasAttachment = False
```

### Comparing `librus_apix-0.7.7/librus_apix/schedule.py` & `librus_apix-0.7.8/librus_apix/schedule.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.7/librus_apix/student_information.py` & `librus_apix-0.7.8/librus_apix/student_information.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.7/librus_apix/timetable.py` & `librus_apix-0.7.8/librus_apix/timetable.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.7/librus_apix/urls.py` & `librus_apix-0.7.8/librus_apix/urls.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.7/librus_apix.egg-info/SOURCES.txt` & `librus_apix-0.7.8/librus_apix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.7/setup.cfg` & `librus_apix-0.7.8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [darglint]
 strictness = long
 docstring_style = google
 
 [metadata]
 name = librus_apix
-version = v0.7.7
+version = v0.7.8
 license = MIT
 description = Web Scraper for Librus Synergia
 long_description = ""
 author = Pascal Jodłowski
 url = https://github.com/poroknights/librus-apix
 keywords = librus, scraper, api, synergia
 classifiers =
```

