# Comparing `tmp/noveler-0.1.1.tar.gz` & `tmp/noveler-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noveler-0.1.1.tar", max compression
+gzip compressed data, was "noveler-0.1.2.tar", max compression
```

## Comparing `noveler-0.1.1.tar` & `noveler-0.1.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     1073 2024-04-05 16:46:40.584169 noveler-0.1.1/LICENSE
--rw-r--r--   0        0        0     2812 2024-04-05 23:46:41.029817 noveler-0.1.1/README.md
--rw-r--r--   0        0        0       72 2024-03-27 02:28:45.063002 noveler-0.1.1/noveler/__init__.py
--rw-r--r--   0        0        0     7397 2024-05-16 16:29:47.881622 noveler-0.1.1/noveler/application.py
--rw-r--r--   0        0        0     5138 2024-04-26 23:37:57.167329 noveler-0.1.1/noveler/controllers/ActivityController.py
--rw-r--r--   0        0        0    26678 2024-04-26 23:26:37.587556 noveler-0.1.1/noveler/controllers/AssistantController.py
--rw-r--r--   0        0        0    11098 2024-04-26 23:42:46.902640 noveler-0.1.1/noveler/controllers/AuthorController.py
--rw-r--r--   0        0        0      984 2024-04-29 20:02:53.981822 noveler-0.1.1/noveler/controllers/BaseController.py
--rw-r--r--   0        0        0    13579 2024-04-29 20:07:01.963452 noveler-0.1.1/noveler/controllers/BibliographyController.py
--rw-r--r--   0        0        0    25404 2024-04-29 23:40:17.360757 noveler-0.1.1/noveler/controllers/ChapterController.py
--rw-r--r--   0        0        0    75357 2024-04-30 18:57:39.408452 noveler-0.1.1/noveler/controllers/CharacterController.py
--rw-r--r--   0        0        0    20297 2024-04-29 22:11:35.716251 noveler-0.1.1/noveler/controllers/EventController.py
--rw-r--r--   0        0        0    16728 2024-04-30 18:44:07.987106 noveler-0.1.1/noveler/controllers/ExportController.py
--rw-r--r--   0        0        0    10472 2024-04-29 22:15:45.985866 noveler-0.1.1/noveler/controllers/ImageController.py
--rw-r--r--   0        0        0     7221 2024-04-29 23:00:47.199253 noveler-0.1.1/noveler/controllers/LinkController.py
--rw-r--r--   0        0        0    23864 2024-04-29 23:07:38.798422 noveler-0.1.1/noveler/controllers/LocationController.py
--rw-r--r--   0        0        0     6655 2024-04-29 23:14:13.518805 noveler-0.1.1/noveler/controllers/NoteController.py
--rw-r--r--   0        0        0     2865 2024-04-29 23:14:38.879658 noveler-0.1.1/noveler/controllers/OllamaModelController.py
--rw-r--r--   0        0        0    21926 2024-04-29 23:22:47.753481 noveler-0.1.1/noveler/controllers/SceneController.py
--rw-r--r--   0        0        0    23049 2024-04-29 23:29:10.431386 noveler-0.1.1/noveler/controllers/StoryController.py
--rw-r--r--   0        0        0     9149 2024-04-29 23:31:13.876182 noveler-0.1.1/noveler/controllers/SubmissionController.py
--rw-r--r--   0        0        0    17444 2024-04-29 23:31:13.774179 noveler-0.1.1/noveler/controllers/UserController.py
--rw-r--r--   0        0        0     1221 2024-03-30 00:37:25.669229 noveler-0.1.1/noveler/controllers/__init__.py
--rw-r--r--   0        0        0     3374 2024-04-18 17:39:28.714791 noveler-0.1.1/noveler/models/Activity.py
--rw-r--r--   0        0        0     6358 2024-05-03 01:08:29.388098 noveler-0.1.1/noveler/models/Assistance.py
--rw-r--r--   0        0        0     4790 2024-03-26 17:54:58.737034 noveler-0.1.1/noveler/models/Author.py
--rw-r--r--   0        0        0     3316 2024-05-05 19:32:49.704937 noveler-0.1.1/noveler/models/AuthorStory.py
--rw-r--r--   0        0        0       70 2024-03-24 02:35:40.239112 noveler-0.1.1/noveler/models/Base.py
--rw-r--r--   0        0        0     7430 2024-05-05 18:44:03.133809 noveler-0.1.1/noveler/models/Bibliography.py
--rw-r--r--   0        0        0     4817 2024-05-05 19:15:35.689588 noveler-0.1.1/noveler/models/BibliographyAuthor.py
--rw-r--r--   0        0        0     6709 2024-03-30 20:19:56.562647 noveler-0.1.1/noveler/models/Chapter.py
--rw-r--r--   0        0        0     3799 2024-03-30 15:06:41.382174 noveler-0.1.1/noveler/models/ChapterLink.py
--rw-r--r--   0        0        0     3798 2024-03-30 15:06:11.516345 noveler-0.1.1/noveler/models/ChapterNote.py
--rw-r--r--   0        0        0    27269 2024-05-15 04:11:34.202461 noveler-0.1.1/noveler/models/Character.py
--rw-r--r--   0        0        0     3594 2024-04-03 17:49:52.714571 noveler-0.1.1/noveler/models/CharacterEvent.py
--rw-r--r--   0        0        0     4529 2024-04-03 04:05:10.789780 noveler-0.1.1/noveler/models/CharacterImage.py
--rw-r--r--   0        0        0     3483 2024-04-03 04:06:41.377737 noveler-0.1.1/noveler/models/CharacterLink.py
--rw-r--r--   0        0        0     3609 2024-04-03 04:05:52.527628 noveler-0.1.1/noveler/models/CharacterNote.py
--rw-r--r--   0        0        0     7615 2024-04-03 16:14:05.483259 noveler-0.1.1/noveler/models/CharacterRelationship.py
--rw-r--r--   0        0        0      649 2024-03-23 23:08:42.545496 noveler-0.1.1/noveler/models/CharacterRelationshipTypes.py
--rw-r--r--   0        0        0     3589 2024-04-03 17:54:57.531181 noveler-0.1.1/noveler/models/CharacterStory.py
--rw-r--r--   0        0        0     5186 2024-03-26 17:58:57.654914 noveler-0.1.1/noveler/models/CharacterTrait.py
--rw-r--r--   0        0        0     6119 2024-05-15 17:30:41.019205 noveler-0.1.1/noveler/models/Event.py
--rw-r--r--   0        0        0     3366 2024-03-26 17:59:36.066040 noveler-0.1.1/noveler/models/EventLink.py
--rw-r--r--   0        0        0     3353 2024-03-26 18:00:15.887213 noveler-0.1.1/noveler/models/EventNote.py
--rw-r--r--   0        0        0     7577 2024-05-15 17:34:54.008689 noveler-0.1.1/noveler/models/Image.py
--rw-r--r--   0        0        0     4309 2024-03-26 18:00:46.640121 noveler-0.1.1/noveler/models/ImageLocation.py
--rw-r--r--   0        0        0      403 2024-03-24 00:00:16.388632 noveler-0.1.1/noveler/models/ImageMimeTypes.py
--rw-r--r--   0        0        0     6190 2024-05-15 17:41:06.577136 noveler-0.1.1/noveler/models/Link.py
--rw-r--r--   0        0        0     3414 2024-03-24 02:51:56.610270 noveler-0.1.1/noveler/models/LinkLocation.py
--rw-r--r--   0        0        0     3366 2024-03-30 14:28:11.555374 noveler-0.1.1/noveler/models/LinkScene.py
--rw-r--r--   0        0        0     3397 2024-03-30 15:15:20.441603 noveler-0.1.1/noveler/models/LinkStory.py
--rw-r--r--   0        0        0    11025 2024-05-15 17:44:44.416398 noveler-0.1.1/noveler/models/Location.py
--rw-r--r--   0        0        0     3311 2024-03-24 02:53:02.016031 noveler-0.1.1/noveler/models/LocationNote.py
--rw-r--r--   0        0        0     6026 2024-05-15 18:39:18.266390 noveler-0.1.1/noveler/models/Note.py
--rw-r--r--   0        0        0     3366 2024-03-30 14:29:01.876861 noveler-0.1.1/noveler/models/NoteScene.py
--rw-r--r--   0        0        0     3397 2024-03-30 15:16:00.109707 noveler-0.1.1/noveler/models/NoteStory.py
--rw-r--r--   0        0        0     5644 2024-05-15 18:41:45.146555 noveler-0.1.1/noveler/models/OllamaModel.py
--rw-r--r--   0        0        0     7206 2024-05-15 18:42:51.323681 noveler-0.1.1/noveler/models/Scene.py
--rw-r--r--   0        0        0     7248 2024-05-15 18:44:18.920291 noveler-0.1.1/noveler/models/Story.py
--rw-r--r--   0        0        0     9722 2024-05-15 18:45:30.881700 noveler-0.1.1/noveler/models/Submission.py
--rw-r--r--   0        0        0      768 2024-05-15 18:46:35.155017 noveler-0.1.1/noveler/models/SubmissionResultType.py
--rw-r--r--   0        0        0     9026 2024-05-15 18:47:38.667364 noveler-0.1.1/noveler/models/User.py
--rw-r--r--   0        0        0     2059 2024-03-27 21:58:27.857198 noveler-0.1.1/noveler/models/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 19:38:44.012362 noveler-0.1.1/noveler/tmp/empty
--rw-r--r--   0        0        0      781 2024-05-16 16:44:12.587280 noveler-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3206 1970-01-01 00:00:00.000000 noveler-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-05 16:46:40.584169 noveler-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2812 2024-04-05 23:46:41.029817 noveler-0.1.2/README.md
+-rw-r--r--   0        0        0       72 2024-03-27 02:28:45.063002 noveler-0.1.2/noveler/__init__.py
+-rw-r--r--   0        0        0     7397 2024-05-16 16:29:47.881622 noveler-0.1.2/noveler/application.py
+-rw-r--r--   0        0        0     5138 2024-04-26 23:37:57.167329 noveler-0.1.2/noveler/controllers/ActivityController.py
+-rw-r--r--   0        0        0    26678 2024-04-26 23:26:37.587556 noveler-0.1.2/noveler/controllers/AssistantController.py
+-rw-r--r--   0        0        0    11098 2024-04-26 23:42:46.902640 noveler-0.1.2/noveler/controllers/AuthorController.py
+-rw-r--r--   0        0        0      984 2024-04-29 20:02:53.981822 noveler-0.1.2/noveler/controllers/BaseController.py
+-rw-r--r--   0        0        0    13579 2024-04-29 20:07:01.963452 noveler-0.1.2/noveler/controllers/BibliographyController.py
+-rw-r--r--   0        0        0    25404 2024-04-29 23:40:17.360757 noveler-0.1.2/noveler/controllers/ChapterController.py
+-rw-r--r--   0        0        0    75357 2024-04-30 18:57:39.408452 noveler-0.1.2/noveler/controllers/CharacterController.py
+-rw-r--r--   0        0        0    17439 2024-05-17 18:13:22.445990 noveler-0.1.2/noveler/controllers/EventController.py
+-rw-r--r--   0        0        0    16728 2024-04-30 18:44:07.987106 noveler-0.1.2/noveler/controllers/ExportController.py
+-rw-r--r--   0        0        0    10472 2024-04-29 22:15:45.985866 noveler-0.1.2/noveler/controllers/ImageController.py
+-rw-r--r--   0        0        0     7221 2024-04-29 23:00:47.199253 noveler-0.1.2/noveler/controllers/LinkController.py
+-rw-r--r--   0        0        0    23864 2024-04-29 23:07:38.798422 noveler-0.1.2/noveler/controllers/LocationController.py
+-rw-r--r--   0        0        0     6655 2024-04-29 23:14:13.518805 noveler-0.1.2/noveler/controllers/NoteController.py
+-rw-r--r--   0        0        0     2865 2024-04-29 23:14:38.879658 noveler-0.1.2/noveler/controllers/OllamaModelController.py
+-rw-r--r--   0        0        0    21926 2024-04-29 23:22:47.753481 noveler-0.1.2/noveler/controllers/SceneController.py
+-rw-r--r--   0        0        0    23049 2024-04-29 23:29:10.431386 noveler-0.1.2/noveler/controllers/StoryController.py
+-rw-r--r--   0        0        0     9149 2024-04-29 23:31:13.876182 noveler-0.1.2/noveler/controllers/SubmissionController.py
+-rw-r--r--   0        0        0    17444 2024-04-29 23:31:13.774179 noveler-0.1.2/noveler/controllers/UserController.py
+-rw-r--r--   0        0        0     1221 2024-03-30 00:37:25.669229 noveler-0.1.2/noveler/controllers/__init__.py
+-rw-r--r--   0        0        0     3374 2024-04-18 17:39:28.714791 noveler-0.1.2/noveler/models/Activity.py
+-rw-r--r--   0        0        0     6358 2024-05-03 01:08:29.388098 noveler-0.1.2/noveler/models/Assistance.py
+-rw-r--r--   0        0        0     4790 2024-03-26 17:54:58.737034 noveler-0.1.2/noveler/models/Author.py
+-rw-r--r--   0        0        0     3316 2024-05-05 19:32:49.704937 noveler-0.1.2/noveler/models/AuthorStory.py
+-rw-r--r--   0        0        0       70 2024-03-24 02:35:40.239112 noveler-0.1.2/noveler/models/Base.py
+-rw-r--r--   0        0        0     7430 2024-05-05 18:44:03.133809 noveler-0.1.2/noveler/models/Bibliography.py
+-rw-r--r--   0        0        0     4817 2024-05-05 19:15:35.689588 noveler-0.1.2/noveler/models/BibliographyAuthor.py
+-rw-r--r--   0        0        0     6709 2024-03-30 20:19:56.562647 noveler-0.1.2/noveler/models/Chapter.py
+-rw-r--r--   0        0        0     3799 2024-03-30 15:06:41.382174 noveler-0.1.2/noveler/models/ChapterLink.py
+-rw-r--r--   0        0        0     3798 2024-03-30 15:06:11.516345 noveler-0.1.2/noveler/models/ChapterNote.py
+-rw-r--r--   0        0        0    27269 2024-05-15 04:11:34.202461 noveler-0.1.2/noveler/models/Character.py
+-rw-r--r--   0        0        0     3594 2024-04-03 17:49:52.714571 noveler-0.1.2/noveler/models/CharacterEvent.py
+-rw-r--r--   0        0        0     4529 2024-04-03 04:05:10.789780 noveler-0.1.2/noveler/models/CharacterImage.py
+-rw-r--r--   0        0        0     3483 2024-04-03 04:06:41.377737 noveler-0.1.2/noveler/models/CharacterLink.py
+-rw-r--r--   0        0        0     3609 2024-04-03 04:05:52.527628 noveler-0.1.2/noveler/models/CharacterNote.py
+-rw-r--r--   0        0        0     7615 2024-04-03 16:14:05.483259 noveler-0.1.2/noveler/models/CharacterRelationship.py
+-rw-r--r--   0        0        0      649 2024-03-23 23:08:42.545496 noveler-0.1.2/noveler/models/CharacterRelationshipTypes.py
+-rw-r--r--   0        0        0     3589 2024-04-03 17:54:57.531181 noveler-0.1.2/noveler/models/CharacterStory.py
+-rw-r--r--   0        0        0     5186 2024-03-26 17:58:57.654914 noveler-0.1.2/noveler/models/CharacterTrait.py
+-rw-r--r--   0        0        0     5923 2024-05-17 18:15:18.785448 noveler-0.1.2/noveler/models/Event.py
+-rw-r--r--   0        0        0     3366 2024-03-26 17:59:36.066040 noveler-0.1.2/noveler/models/EventLink.py
+-rw-r--r--   0        0        0     3353 2024-03-26 18:00:15.887213 noveler-0.1.2/noveler/models/EventNote.py
+-rw-r--r--   0        0        0     7577 2024-05-15 17:34:54.008689 noveler-0.1.2/noveler/models/Image.py
+-rw-r--r--   0        0        0     4309 2024-03-26 18:00:46.640121 noveler-0.1.2/noveler/models/ImageLocation.py
+-rw-r--r--   0        0        0      403 2024-03-24 00:00:16.388632 noveler-0.1.2/noveler/models/ImageMimeTypes.py
+-rw-r--r--   0        0        0     6190 2024-05-15 17:41:06.577136 noveler-0.1.2/noveler/models/Link.py
+-rw-r--r--   0        0        0     3414 2024-03-24 02:51:56.610270 noveler-0.1.2/noveler/models/LinkLocation.py
+-rw-r--r--   0        0        0     3366 2024-03-30 14:28:11.555374 noveler-0.1.2/noveler/models/LinkScene.py
+-rw-r--r--   0        0        0     3397 2024-03-30 15:15:20.441603 noveler-0.1.2/noveler/models/LinkStory.py
+-rw-r--r--   0        0        0    10829 2024-05-17 18:15:41.119110 noveler-0.1.2/noveler/models/Location.py
+-rw-r--r--   0        0        0     3311 2024-03-24 02:53:02.016031 noveler-0.1.2/noveler/models/LocationNote.py
+-rw-r--r--   0        0        0     6026 2024-05-15 18:39:18.266390 noveler-0.1.2/noveler/models/Note.py
+-rw-r--r--   0        0        0     3366 2024-03-30 14:29:01.876861 noveler-0.1.2/noveler/models/NoteScene.py
+-rw-r--r--   0        0        0     3397 2024-03-30 15:16:00.109707 noveler-0.1.2/noveler/models/NoteStory.py
+-rw-r--r--   0        0        0     5644 2024-05-15 18:41:45.146555 noveler-0.1.2/noveler/models/OllamaModel.py
+-rw-r--r--   0        0        0     7206 2024-05-15 18:42:51.323681 noveler-0.1.2/noveler/models/Scene.py
+-rw-r--r--   0        0        0     7248 2024-05-15 18:44:18.920291 noveler-0.1.2/noveler/models/Story.py
+-rw-r--r--   0        0        0     9722 2024-05-15 18:45:30.881700 noveler-0.1.2/noveler/models/Submission.py
+-rw-r--r--   0        0        0      768 2024-05-15 18:46:35.155017 noveler-0.1.2/noveler/models/SubmissionResultType.py
+-rw-r--r--   0        0        0     9026 2024-05-15 18:47:38.667364 noveler-0.1.2/noveler/models/User.py
+-rw-r--r--   0        0        0     2004 2024-05-17 18:14:04.813251 noveler-0.1.2/noveler/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:38:44.012362 noveler-0.1.2/noveler/tmp/empty
+-rw-r--r--   0        0        0      781 2024-05-17 18:17:19.063008 noveler-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3206 1970-01-01 00:00:00.000000 noveler-0.1.2/PKG-INFO
```

### Comparing `noveler-0.1.1/LICENSE` & `noveler-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/README.md` & `noveler-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/application.py` & `noveler-0.1.2/noveler/application.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/controllers/ActivityController.py` & `noveler-0.1.2/noveler/controllers/ActivityController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/controllers/AssistantController.py` & `noveler-0.1.2/noveler/controllers/AssistantController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/controllers/AuthorController.py` & `noveler-0.1.2/noveler/controllers/AuthorController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/controllers/BaseController.py` & `noveler-0.1.2/noveler/controllers/BaseController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/controllers/BibliographyController.py` & `noveler-0.1.2/noveler/controllers/BibliographyController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/controllers/ChapterController.py` & `noveler-0.1.2/noveler/controllers/ChapterController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/controllers/CharacterController.py` & `noveler-0.1.2/noveler/controllers/CharacterController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/controllers/EventController.py` & `noveler-0.1.2/noveler/controllers/EventController.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from datetime import datetime
 from typing import Type, List
 from sqlalchemy.orm import Session
 from noveler.controllers.BaseController import BaseController
-from noveler.models import User, Event, CharacterEvent, Character, Activity, EventLocation, Location, Link, EventLink, \
-    Note, EventNote
+from noveler.models import User, Event, CharacterEvent, Character, Activity, Location, Link, EventLink, Note, EventNote
 
 
 class EventController(BaseController):
     """Event controller encapsulates event management functionality
 
     Attributes
     ----------
@@ -30,18 +29,14 @@
         Get all events associated with a user
     get_all_events_page(page: int, per_page: int)
         Get a single page of events associated with a user from the database
     append_characters_to_event(event_id: int, characters: list)
         Append characters to an event
     get_characters_by_event_id(event_id: int)
         Get all characters associated with an event
-    append_locations_to_event(event_id: int, locations: list)
-        Append locations to an event
-    get_locations_by_event_id(event_id: int)
-        Get all locations associated with an event
     append_links_to_event(event_id: int, links: list)
         Append links to an event
     get_links_by_event_id(event_id: int)
         Get all links associated with an event
     get_links_page_by_event_id(event_id: int, page: int, per_page: int)
         Get a single page of links associated with an event from the database
     append_notes_to_event(event_id: int, notes: list)
@@ -352,98 +347,14 @@
                 CharacterEvent.user_id == self._owner.id
             ).offset(offset).limit(per_page).all():
                 yield session.query(Character).filter(
                     Character.id == character_event.character_id,
                     Character.user_id == self._owner.id
                 ).first()
 
-    def append_locations_to_event(
-        self, event_id: int, location_ids: list
-    ) -> Type[Event]:
-        """Append locations to an event
-
-        Parameters
-        ----------
-        event_id : int
-            The id of the event
-        location_ids : list
-            A list of location ids
-
-        Returns
-        -------
-        Event
-            The updated event object
-        """
-
-        with self._session as session:
-            try:
-                event = session.query(Event).filter(
-                    Event.id == event_id,
-                    Event.user_id == self._owner.id
-                ).first()
-
-                if not event:
-                    raise ValueError('Event not found.')
-
-                for location_id in location_ids:
-                    location = session.query(Location).filter(
-                        Location.id == location_id,
-                        Location.user_id == self._owner.id
-                    ).first()
-
-                    if not location:
-                        raise ValueError('Location not found.')
-
-                    event_location = EventLocation(
-                        user_id=self._owner.id, event_id=event_id,
-                        location_id=location_id, created=datetime.now()
-                    )
-
-                    activity = Activity(
-                        user_id=self._owner.id, summary=f'Location \
-                        {location.name[:50]} associated with event \
-                        {event.title[:50]} by {self._owner.username}',
-                        created=datetime.now()
-                    )
-
-                    session.add(event_location)
-                    session.add(activity)
-
-            except Exception as e:
-                session.rollback()
-                raise e
-
-            else:
-                session.commit()
-                return event
-
-    def get_locations_by_event_id(self, event_id: int) -> List[Type[Location]]:
-        """Get all locations associated with an event
-
-        Parameters
-        ----------
-        event_id : int
-            The id of the event
-
-        Returns
-        -------
-        list
-            A list of location objects
-        """
-
-        with self._session as session:
-            for event_location in session.query(EventLocation).filter(
-                EventLocation.event_id == event_id,
-                    EventLocation.user_id == self._owner.id
-            ).all():
-                yield session.query(Location).filter(
-                    Location.id == event_location.location_id,
-                    Location.user_id == self._owner.id
-                ).first()
-
     def append_links_to_event(
         self, event_id: int, link_ids: list
     ) -> Type[Event]:
         """Append links to an event
 
         Parameters
         ----------
```

### Comparing `noveler-0.1.1/noveler/controllers/ExportController.py` & `noveler-0.1.2/noveler/controllers/ExportController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/controllers/ImageController.py` & `noveler-0.1.2/noveler/controllers/ImageController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/controllers/LinkController.py` & `noveler-0.1.2/noveler/controllers/LinkController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/controllers/LocationController.py` & `noveler-0.1.2/noveler/controllers/LocationController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/controllers/NoteController.py` & `noveler-0.1.2/noveler/controllers/NoteController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/controllers/OllamaModelController.py` & `noveler-0.1.2/noveler/controllers/OllamaModelController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/controllers/SceneController.py` & `noveler-0.1.2/noveler/controllers/SceneController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/controllers/StoryController.py` & `noveler-0.1.2/noveler/controllers/StoryController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/controllers/SubmissionController.py` & `noveler-0.1.2/noveler/controllers/SubmissionController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/controllers/UserController.py` & `noveler-0.1.2/noveler/controllers/UserController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/controllers/__init__.py` & `noveler-0.1.2/noveler/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/Activity.py` & `noveler-0.1.2/noveler/models/Activity.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/Assistance.py` & `noveler-0.1.2/noveler/models/Assistance.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/Author.py` & `noveler-0.1.2/noveler/models/Author.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/AuthorStory.py` & `noveler-0.1.2/noveler/models/AuthorStory.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/Bibliography.py` & `noveler-0.1.2/noveler/models/Bibliography.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/BibliographyAuthor.py` & `noveler-0.1.2/noveler/models/BibliographyAuthor.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/Chapter.py` & `noveler-0.1.2/noveler/models/Chapter.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/ChapterLink.py` & `noveler-0.1.2/noveler/models/ChapterLink.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/ChapterNote.py` & `noveler-0.1.2/noveler/models/ChapterNote.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/Character.py` & `noveler-0.1.2/noveler/models/Character.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/CharacterEvent.py` & `noveler-0.1.2/noveler/models/CharacterEvent.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/CharacterImage.py` & `noveler-0.1.2/noveler/models/CharacterImage.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/CharacterLink.py` & `noveler-0.1.2/noveler/models/CharacterLink.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/CharacterNote.py` & `noveler-0.1.2/noveler/models/CharacterNote.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/CharacterRelationship.py` & `noveler-0.1.2/noveler/models/CharacterRelationship.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/CharacterRelationshipTypes.py` & `noveler-0.1.2/noveler/models/CharacterRelationshipTypes.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/CharacterStory.py` & `noveler-0.1.2/noveler/models/CharacterStory.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/CharacterTrait.py` & `noveler-0.1.2/noveler/models/CharacterTrait.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/Event.py` & `noveler-0.1.2/noveler/models/Event.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime
 from typing import Optional, List
 from sqlalchemy import Integer, ForeignKey, String, DateTime, Text
 from sqlalchemy.orm import Mapped, mapped_column, relationship, validates
-from noveler.models import User, EventLink, CharacterEvent, EventNote, EventLocation, Base
+from noveler.models import User, EventLink, CharacterEvent, EventNote, Base
 
 
 class Event(Base):
     """The Event class represents an event that is referenced by one or more stories.
 
     Attributes
     ----------
@@ -74,17 +74,14 @@
         cascade="all, delete, delete-orphan")
     characters: Mapped[Optional[List["CharacterEvent"]]] = relationship(
         "CharacterEvent", back_populates="event", lazy="joined",
         cascade="all, delete, delete-orphan")
     notes: Mapped[Optional[List["EventNote"]]] = relationship(
         "EventNote", back_populates="event", lazy="joined",
         cascade="all, delete, delete-orphan")
-    locations: Mapped[Optional[List["EventLocation"]]] = relationship(
-        "EventLocation", back_populates="event", lazy="joined",
-        cascade="all, delete, delete-orphan")
 
     def __repr__(self):
         """Returns a string representation of the event.
 
         Returns
         -------
         str
```

### Comparing `noveler-0.1.1/noveler/models/EventLink.py` & `noveler-0.1.2/noveler/models/EventLink.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/EventNote.py` & `noveler-0.1.2/noveler/models/EventNote.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/Image.py` & `noveler-0.1.2/noveler/models/Image.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/ImageLocation.py` & `noveler-0.1.2/noveler/models/ImageLocation.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/Link.py` & `noveler-0.1.2/noveler/models/Link.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/LinkLocation.py` & `noveler-0.1.2/noveler/models/LinkLocation.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/LinkScene.py` & `noveler-0.1.2/noveler/models/LinkScene.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/LinkStory.py` & `noveler-0.1.2/noveler/models/LinkStory.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/Location.py` & `noveler-0.1.2/noveler/models/Location.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime
 from typing import Optional, List
 from sqlalchemy import Integer, ForeignKey, String, Text, Float, DateTime
 from sqlalchemy.orm import Mapped, mapped_column, relationship, validates
-from noveler.models import User, ImageLocation, LinkLocation, EventLocation, LocationNote, Base
+from noveler.models import User, ImageLocation, LinkLocation, LocationNote, Base
 
 
 class Location(Base):
     """The Location class represents a location associated with one or more stories.
 
     Attributes
     ----------
@@ -94,17 +94,14 @@
     user: Mapped["User"] = relationship("User", back_populates="locations")
     images: Mapped[Optional[List["ImageLocation"]]] = relationship(
         "ImageLocation", back_populates="location",
         cascade="all, delete, delete-orphan")
     links: Mapped[Optional[List["LinkLocation"]]] = relationship(
         "LinkLocation", back_populates="location",
         cascade="all, delete, delete-orphan", lazy="joined")
-    events: Mapped[Optional[List["EventLocation"]]] = relationship(
-        "EventLocation", back_populates="location",
-        cascade="all, delete, delete-orphan", lazy="joined")
     notes: Mapped[Optional[List["LocationNote"]]] = relationship(
         "LocationNote", back_populates="location",
         cascade="all, delete, delete-orphan", lazy="joined")
 
     def __repr__(self):
         """Returns a string representation of the location.
```

### Comparing `noveler-0.1.1/noveler/models/LocationNote.py` & `noveler-0.1.2/noveler/models/LocationNote.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/Note.py` & `noveler-0.1.2/noveler/models/Note.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/NoteScene.py` & `noveler-0.1.2/noveler/models/NoteScene.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/NoteStory.py` & `noveler-0.1.2/noveler/models/NoteStory.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/OllamaModel.py` & `noveler-0.1.2/noveler/models/OllamaModel.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/Scene.py` & `noveler-0.1.2/noveler/models/Scene.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/Story.py` & `noveler-0.1.2/noveler/models/Story.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/Submission.py` & `noveler-0.1.2/noveler/models/Submission.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/SubmissionResultType.py` & `noveler-0.1.2/noveler/models/SubmissionResultType.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/User.py` & `noveler-0.1.2/noveler/models/User.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.1/noveler/models/__init__.py` & `noveler-0.1.2/noveler/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from noveler.models.CharacterNote import CharacterNote
 from noveler.models.CharacterRelationship import CharacterRelationship
 from noveler.models.CharacterRelationshipTypes import CharacterRelationshipTypes
 from noveler.models.CharacterStory import CharacterStory
 from noveler.models.CharacterTrait import CharacterTrait
 from noveler.models.Event import Event
 from noveler.models.EventLink import EventLink
-from noveler.models.EventLocation import EventLocation
 from noveler.models.EventNote import EventNote
 from noveler.models.Image import Image
 from noveler.models.ImageLocation import ImageLocation
 from noveler.models.ImageMimeTypes import ImageMimeTypes
 from noveler.models.Link import Link
 from noveler.models.LinkLocation import LinkLocation
 from noveler.models.LinkScene import LinkScene
```

### Comparing `noveler-0.1.1/pyproject.toml` & `noveler-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "noveler"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Richard Lucas <webmaster@applebiter.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [project]
 name = "noveler"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Richard Lucas", email="webmaster@applebiter.com" },
 ]
 description = "Novel, short story, and serial authoring software"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `noveler-0.1.1/PKG-INFO` & `noveler-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noveler
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Richard Lucas
 Author-email: webmaster@applebiter.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

