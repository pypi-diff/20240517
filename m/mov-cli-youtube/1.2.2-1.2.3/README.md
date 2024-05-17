# Comparing `tmp/mov_cli_youtube-1.2.2.tar.gz` & `tmp/mov_cli_youtube-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov_cli_youtube-1.2.2.tar", last modified: Tue May  7 19:33:18 2024, max compression
+gzip compressed data, was "mov_cli_youtube-1.2.3.tar", last modified: Fri May 17 13:42:44 2024, max compression
```

## Comparing `mov_cli_youtube-1.2.2.tar` & `mov_cli_youtube-1.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-05-07 19:33:18.047351 mov_cli_youtube-1.2.2/
--rw-r--r--   0 ananas    (1000) ananas    (1000)     1064 2024-05-07 19:19:11.000000 mov_cli_youtube-1.2.2/LICENSE
--rw-r--r--   0 ananas    (1000) ananas    (1000)     2930 2024-05-07 19:33:18.047351 mov_cli_youtube-1.2.2/PKG-INFO
--rw-r--r--   0 ananas    (1000) ananas    (1000)      613 2024-05-07 19:19:11.000000 mov_cli_youtube-1.2.2/README.md
-drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-05-07 19:33:18.044017 mov_cli_youtube-1.2.2/mov_cli_youtube/
--rw-r--r--   0 ananas    (1000) ananas    (1000)      650 2024-05-07 19:32:46.000000 mov_cli_youtube-1.2.2/mov_cli_youtube/__init__.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     2462 2024-05-07 19:21:46.000000 mov_cli_youtube-1.2.2/mov_cli_youtube/pytube.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     3765 2024-05-07 19:19:11.000000 mov_cli_youtube-1.2.2/mov_cli_youtube/yt_dlp.py
-drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-05-07 19:33:18.044017 mov_cli_youtube-1.2.2/mov_cli_youtube.egg-info/
--rw-r--r--   0 ananas    (1000) ananas    (1000)     2930 2024-05-07 19:33:18.000000 mov_cli_youtube-1.2.2/mov_cli_youtube.egg-info/PKG-INFO
--rw-r--r--   0 ananas    (1000) ananas    (1000)      306 2024-05-07 19:33:18.000000 mov_cli_youtube-1.2.2/mov_cli_youtube.egg-info/SOURCES.txt
--rw-r--r--   0 ananas    (1000) ananas    (1000)        1 2024-05-07 19:33:18.000000 mov_cli_youtube-1.2.2/mov_cli_youtube.egg-info/dependency_links.txt
--rw-r--r--   0 ananas    (1000) ananas    (1000)      100 2024-05-07 19:33:18.000000 mov_cli_youtube-1.2.2/mov_cli_youtube.egg-info/requires.txt
--rw-r--r--   0 ananas    (1000) ananas    (1000)       16 2024-05-07 19:33:18.000000 mov_cli_youtube-1.2.2/mov_cli_youtube.egg-info/top_level.txt
--rw-r--r--   0 ananas    (1000) ananas    (1000)     1298 2024-05-07 19:32:06.000000 mov_cli_youtube-1.2.2/pyproject.toml
--rw-r--r--   0 ananas    (1000) ananas    (1000)       38 2024-05-07 19:33:18.047351 mov_cli_youtube-1.2.2/setup.cfg
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-05-17 13:42:44.072746 mov_cli_youtube-1.2.3/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1064 2024-05-17 13:41:24.000000 mov_cli_youtube-1.2.3/LICENSE
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     2930 2024-05-17 13:42:44.072746 mov_cli_youtube-1.2.3/PKG-INFO
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      613 2024-05-17 13:41:24.000000 mov_cli_youtube-1.2.3/README.md
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-05-17 13:42:44.072746 mov_cli_youtube-1.2.3/mov_cli_youtube/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      650 2024-05-17 13:41:24.000000 mov_cli_youtube-1.2.3/mov_cli_youtube/__init__.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     2731 2024-05-17 13:41:24.000000 mov_cli_youtube-1.2.3/mov_cli_youtube/pytube.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     4203 2024-05-17 13:41:24.000000 mov_cli_youtube-1.2.3/mov_cli_youtube/yt_dlp.py
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-05-17 13:42:44.072746 mov_cli_youtube-1.2.3/mov_cli_youtube.egg-info/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     2930 2024-05-17 13:42:44.000000 mov_cli_youtube-1.2.3/mov_cli_youtube.egg-info/PKG-INFO
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      306 2024-05-17 13:42:44.000000 mov_cli_youtube-1.2.3/mov_cli_youtube.egg-info/SOURCES.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)        1 2024-05-17 13:42:44.000000 mov_cli_youtube-1.2.3/mov_cli_youtube.egg-info/dependency_links.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      100 2024-05-17 13:42:44.000000 mov_cli_youtube-1.2.3/mov_cli_youtube.egg-info/requires.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       16 2024-05-17 13:42:44.000000 mov_cli_youtube-1.2.3/mov_cli_youtube.egg-info/top_level.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1298 2024-05-17 13:41:24.000000 mov_cli_youtube-1.2.3/pyproject.toml
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       38 2024-05-17 13:42:44.072746 mov_cli_youtube-1.2.3/setup.cfg
```

### Comparing `mov_cli_youtube-1.2.2/LICENSE` & `mov_cli_youtube-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mov_cli_youtube-1.2.2/PKG-INFO` & `mov_cli_youtube-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli-youtube
-Version: 1.2.2
+Version: 1.2.3
 Summary: A mov-cli v4 plugin for watching youtube.
 Author-email: Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mov_cli_youtube-1.2.2/README.md` & `mov_cli_youtube-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `mov_cli_youtube-1.2.2/mov_cli_youtube/__init__.py` & `mov_cli_youtube-1.2.3/mov_cli_youtube/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,8 +18,8 @@
         "IOS.DEFAULT": PyTubeScraper, 
 
         "yt-dlp": YTDlpScraper, 
         "pytube": PyTubeScraper, 
     }
 }
 
-__version__ = "1.2.2"
+__version__ = "1.2.3"
```

### Comparing `mov_cli_youtube-1.2.2/mov_cli_youtube/pytube.py` & `mov_cli_youtube-1.2.3/mov_cli_youtube/pytube.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import os
 import sys
 from pytubefix import YouTube, Search
 
 from mov_cli.scraper import Scraper
 from mov_cli.utils import EpisodeSelector
-from mov_cli import Single, Metadata, MetadataType
+from mov_cli import Single, Metadata, MetadataType, ExtraMetadata
 
 __all__ = ("PyTubeScraper",)
 
 class PyTubeScraper(Scraper):
     def __init__(self, config: Config, http_client: HTTPClient, options: Optional[ScraperOptionsT] = None) -> None:
         super().__init__(config, http_client, options)
 
@@ -35,15 +35,16 @@
             if (index + 1) == len(search_results) and not (index + 1) >= max_videos:
                 search_query.get_next_results()
 
             yield Metadata(
                 id = video.watch_url, 
                 title = f"{video.title} ~ {video.author}", 
                 type = MetadataType.MOVIE, 
-                year = str(video.publish_date.year)
+                year = str(video.publish_date.year),
+                extra_func = lambda: self.__scrape_extra(video)
             )
 
         # restore the console.
         sys.stderr = sys.__stderr__
 
     def scrape(self, metadata: Metadata, _: EpisodeSelector) -> Single:
         audio_only: bool = self.options.get("audio", False)
@@ -67,8 +68,14 @@
             url = url, 
             title = metadata.title, 
             year = metadata.year
         )
 
     def scrape_episodes(self, metadata: Metadata, **kwargs) -> Dict[None, int]:
         # Returning None as search does not return any metadata of type series.
-        return {None: 1}
+        return {None: 1}
+
+    def __scrape_extra(self, key: YouTube) -> ExtraMetadata:
+        return ExtraMetadata(
+            description = key.description,
+            image_url = key.thumbnail_url,
+        )
```

### Comparing `mov_cli_youtube-1.2.2/mov_cli_youtube/yt_dlp.py` & `mov_cli_youtube-1.2.3/mov_cli_youtube/yt_dlp.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     from mov_cli.http_client import HTTPClient
     from mov_cli.scraper import ScraperOptionsT
 
 import yt_dlp
 
 from mov_cli.scraper import Scraper
 from mov_cli.utils import EpisodeSelector
-from mov_cli import Single, Metadata, MetadataType
+from mov_cli import Single, Metadata, MetadataType, ExtraMetadata
 
 __all__ = ("YTDlpScraper",)
 
 class YTDlpScraper(Scraper):
     def __init__(self, config: Config, http_client: HTTPClient, options: Optional[ScraperOptionsT] = None) -> None:
         super().__init__(config, http_client, options)
 
@@ -35,19 +35,20 @@
             "match_filter": self.__yt_dlp_filter(**self.options)
         }
 
         with yt_dlp.YoutubeDL(yt_options) as ydl:
             info = ydl.extract_info(f"ytsearch{max_videos}:{query}", download = False)
 
             for key in info["entries"]:
-
                 yield Metadata(
                     id = key["url"], 
                     title = f"{key['title']} ~ {key['uploader']}", 
-                    type = MetadataType.SINGLE
+                    type = MetadataType.SINGLE,
+                    extra_func = lambda: self.__scrape_extra(key)
+                    
                 )
 
     def scrape(
         self, 
         metadata: Metadata, 
         _: EpisodeSelector
     ) -> Single:
@@ -107,8 +108,18 @@
 
         def filter(info, *, incomplete):
             url = info.get("url")
 
             if shorts is False and "/shorts" in url:
                 return "Video is a YouTube short. Pass '--shorts' to the scraper to scrape for them."
 
-        return filter
+        return filter
+
+    def __scrape_extra(self, key: dict) -> ExtraMetadata:
+        with yt_dlp.YoutubeDL() as ydl:
+            info = ydl.extract_info(key["url"], download = False)
+
+        return ExtraMetadata(
+            description = info["description"],
+            image_url = info["thumbnail"],
+            genres = info["categories"]
+        )
```

### Comparing `mov_cli_youtube-1.2.2/mov_cli_youtube.egg-info/PKG-INFO` & `mov_cli_youtube-1.2.3/mov_cli_youtube.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli-youtube
-Version: 1.2.2
+Version: 1.2.3
 Summary: A mov-cli v4 plugin for watching youtube.
 Author-email: Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mov_cli_youtube-1.2.2/pyproject.toml` & `mov_cli_youtube-1.2.3/pyproject.toml`

 * *Files identical despite different names*

