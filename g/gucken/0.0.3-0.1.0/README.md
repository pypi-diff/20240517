# Comparing `tmp/gucken-0.0.3.tar.gz` & `tmp/gucken-0.1.0.tar.gz`

## Comparing `gucken-0.0.3.tar` & `gucken-0.1.0.tar`

### file list

```diff
@@ -1,38 +1,43 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/__main__.py
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/aniskip.py
--rw-r--r--   0        0        0    23099 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/gucken.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/gucken.tcss
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/update.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/hoster/__init__.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/hoster/common.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/hoster/doodstream.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/hoster/streamtape.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/hoster/veo.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/hoster/vidoza.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/player/__init__.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/player/android.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/player/common.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/player/ffplay.py
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/player/flatpak.py
--rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/player/mpv.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/player/vlc.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/player/wmplayer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/provider/__init__.py
--rw-r--r--   0        0        0     9785 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/provider/aniworld.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/provider/burningseries.py
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/provider/common.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/provider/crunchyroll.py
--rw-r--r--   0        0        0     9824 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/provider/serienstream.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/provider/streamcloud.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/tracker/__init__.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/tracker/anilist.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/tracker/aniworld.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/tracker/common.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/tracker/myanimelist.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.0.3/src/gucken/tracker/serienstream.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 gucken-0.0.3/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 gucken-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 gucken-0.0.3/README.md
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 gucken-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     6802 2020-02-02 00:00:00.000000 gucken-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/__main__.py
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/aniskip.py
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/custom_widgets.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/default_settings.toml
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/gucken.css
+-rw-r--r--   0        0        0    23834 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/gucken.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/rome.py
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/settings.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/update.py
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/hoster/__init__.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/hoster/common.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/hoster/doodstream.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/hoster/streamtape.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/hoster/veo.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/hoster/vidoza.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/player/__init__.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/player/android.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/player/common.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/player/ffplay.py
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/player/flatpak.py
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/player/mpv.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/player/vlc.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/player/wmplayer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/provider/__init__.py
+-rw-r--r--   0        0        0    10145 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/provider/aniworld.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/provider/burningseries.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/provider/common.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/provider/crunchyroll.py
+-rw-r--r--   0        0        0    10182 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/provider/serienstream.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/provider/streamcloud.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/tracker/__init__.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/tracker/anilist.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/tracker/aniworld.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/tracker/common.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/tracker/myanimelist.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.0/src/gucken/tracker/serienstream.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 gucken-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 gucken-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 gucken-0.1.0/README.md
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 gucken-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     9296 2020-02-02 00:00:00.000000 gucken-0.1.0/PKG-INFO
```

### Comparing `gucken-0.0.3/src/gucken/aniskip.py` & `gucken-0.1.0/src/gucken/aniskip.py`

 * *Files identical despite different names*

### Comparing `gucken-0.0.3/src/gucken/gucken.py` & `gucken-0.1.0/src/gucken/gucken.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import logging
-import sys
 from atexit import register as register_atexit
 from asyncio import gather
-from os import name as os_name, getenv, remove
-from os.path import join
-from pathlib import Path
+from os import name as os_name, remove
+from .settings import gucken_settings_manager
 from random import choice
 from shutil import which
 from subprocess import PIPE, Popen, DEVNULL
 from time import sleep, time
-from typing import Union
+from typing import Union, ClassVar, List
 
 from pypresence import AioPresence, DiscordNotFound
 from textual import events, on, work
 from textual.app import App, ComposeResult
+from textual.binding import BindingType, Binding
 from textual.containers import Center, Container, Horizontal, ScrollableContainer
 from textual.reactive import reactive
 from textual.screen import ModalScreen
 from textual.widgets import (
     Button,
     Checkbox,
     DataTable,
@@ -29,125 +28,65 @@
     ListView,
     Markdown,
     RadioButton,
     TabbedContent,
     TabPane,
 )
 
+from .utils import detect_player, is_android
+from .custom_widgets import SortableTable
 from .update import check
 from .aniskip import (
     get_timings_from_search,
     timings_to_mpv_options,
     generate_chapters_file,
     get_chapters_file_mpv_option,
 )
 from .hoster.common import DirectLink, Hoster
 from .hoster.doodstream import DoodstreamHoster
 from .hoster.streamtape import StreamtapeHoster
 from .hoster.veo import VOEHoster
 from .hoster.vidoza import VidozaHoster
-from .player.android import AndroidChoosePlayer, AndroidMPVPlayer, AndroidVLCPlayer
-from .player.common import Player
-from .player.ffplay import FFPlayPlayer
-from .player.mpv import MPVPlayer, MPVNETPlayer, CelluloidPlayer
+from .player.mpv import MPVPlayer
 from .player.vlc import VLCPlayer
-from .player.wmplayer import WMPlayer
-from .player.flatpak import FlatpakMPVPlayer, FlatpakVLCPlayer, FlatpakCelluloidPlayer
 from .provider.aniworld import AniWorldProvider
 from .provider.common import Episode, Language, SearchResult, Series
 from .provider.serienstream import SerienStreamProvider
+from platformdirs import user_log_path, user_config_path
 
-# TODO: fix this mess
-logs_path = Path(__file__).parent.parent.parent.joinpath("logs")
-logs_path.mkdir(exist_ok=True, parents=True)
+logs_path = user_log_path("gucken", ensure_exists=True)
 logging.basicConfig(
-    filename=logs_path.joinpath("gucken.log"), encoding="utf-8", level=logging.INFO
+    filename=logs_path.joinpath("gucken.log"),
+    encoding="utf-8",
+    level=logging.INFO
 )
 
+register_atexit(gucken_settings_manager.save)
 
-def detect_player() -> Union[Player, None]:
-    if hasattr(sys, "getandroidapilevel"):
-        # TODO: detect right
-        return AndroidMPVPlayer()
-        # return AndroidVLCPlayer()
-        # return AndroidChoosePlayer()
-        # return None
-
-    if os_name == "nt":
-        if which("mpv.exe"):
-            return MPVPlayer("mpv.exe")
-    elif which("mpv"):
-        return MPVPlayer()
-
-    if os_name == "nt":
-        if which("mpvnet.exe"):
-            return MPVNETPlayer()
-        if getenv("LOCALAPPDATA"):
-            mpvnet = join(getenv("LOCALAPPDATA"), "Programs", "mpv.net", "mpvnet.exe")
-            if which(mpvnet):
-                return MPVNETPlayer(mpvnet)
-
-    if os_name == "posix":
-        if which("celluloid"):
-            return CelluloidPlayer()
-
-    if which("vlc"):
-        return VLCPlayer()
-
-    if os_name == "posix":
-        # TODO: fix this will slow down
-        if which("flatpak"):
-            p = Popen(
-                ["flatpak", "info", "io.mpv.Mpv"],
-                stdout=DEVNULL,
-                stderr=DEVNULL,
-                stdin=DEVNULL,
-            )
-            if p.wait() == 0:
-                return FlatpakMPVPlayer()
-            p = Popen(
-                ["flatpak", "info", "io.github.celluloid_player.Celluloid"],
-                stdout=DEVNULL,
-                stderr=DEVNULL,
-                stdin=DEVNULL,
-            )
-            if p.wait() == 0:
-                return FlatpakCelluloidPlayer()
-            p = Popen(
-                ["flatpak", "info", "org.videolan.VLC"],
-                stdout=DEVNULL,
-                stderr=DEVNULL,
-                stdin=DEVNULL,
-            )
-            if p.wait() == 0:
-                return FlatpakVLCPlayer()
 
-    if os_name == "nt":
-        vlc = r"C:\Program Files\VideoLAN\VLC\vlc.exe"
-        if which(vlc):
-            return VLCPlayer(vlc)
+def sort_favorite_lang(language_list: List[Language], pio_list: List[str]) -> List[Language]:
+    def lang_sort_key(hoster: Language) -> int:
+        try:
+            return pio_list.index(hoster.name)
+        except ValueError:
+            return len(pio_list)
 
-    if which("ffplay"):
-        return FFPlayPlayer()
+    return sorted(language_list, key=lang_sort_key)
 
-    if os_name == "nt":
-        return WMPlayer()
 
-    return None
+"""
+def sort_favorite_hoster(hoster_list: List[Hoster], pio_list: List[Type[Hoster]]) -> List[Hoster]:
+    def hoster_sort_key(hoster: Hoster) -> int:
+        try:
+            return pio_list.index(type(hoster))
+        except ValueError:
+            return len(pio_list)
 
-
-def sort_favorite_lang(language_list: list[Language]) -> list[Language]:
-    return sorted(
-        language_list,
-        key=lambda x: (
-            x != Language.DE,
-            x != Language.JP_DESUB,
-            x != Language.JP_ENSUB,
-        ),
-    )
+    return sorted(hoster_list, key=hoster_sort_key)
+"""
 
 
 def sort_favorite_hoster(hoster_list: list[Hoster]) -> list[Hoster]:
     return sorted(
         hoster_list,
         key=lambda x: (
             not isinstance(x, StreamtapeHoster),
@@ -229,67 +168,116 @@
         if row_index <= -1:
             return
         if self.last_click.get(row_index) and time() - self.last_click[row_index] < 0.5:
             self.app.play_selected()
         self.last_click[row_index] = time()
 
 
+def remove_duplicates(lst: list) -> list:
+    """
+    Why this instead of a set you ask ?
+    Because a set cant maintaining the original order.
+    """
+    seen = set()
+    result = []
+    for item in lst:
+        if item not in seen:
+            seen.add(item)
+            result.append(item)
+    return result
+
+
+def remove_none_lang_keys(lst: list) -> list:
+    valid_languages = {lang.name for lang in Language}
+    return [item for item in lst if item in valid_languages]
+
+
+def move_item(lst: list, from_index: int, to_index: int) -> list:
+    item = lst.pop(from_index)
+    lst.insert(to_index, item)
+    return lst
+
+
 client_id = "1238219157464416266"
 
 
 class GuckenApp(App):
     TITLE = "Gucken TUI"
     # TODO: color theme https://textual.textualize.io/guide/design/#designing-with-colors
-    CSS_PATH = "gucken.tcss"
+
+    CSS_PATH = ["gucken.css"]
+    custom_css = user_config_path("gucken").joinpath("custom.css")
+    if custom_css.exists():
+        CSS_PATH.append(custom_css)
+    BINDINGS: ClassVar[list[BindingType]] = [
+        Binding("q", "quit", "Quit", show=True, priority=False),
+    ]
 
     def __init__(self):
         super().__init__()
         self.current: Union[list[SearchResult], None] = None
         self.current_info: Union[Series, None] = None
         self.player = detect_player()
         self.RPC: Union[AioPresence, None] = None
 
+        language: list = gucken_settings_manager.settings["settings"]["language"]
+        language = remove_none_lang_keys(language)
+
+        for ll in Language:
+            language.append(ll.name)
+
+        gucken_settings_manager.settings["settings"]["language"] = remove_duplicates(language)
+        self.language = gucken_settings_manager.settings["settings"]["language"]
+
     def compose(self) -> ComposeResult:
+        settings = gucken_settings_manager.settings["settings"]
+        providers = settings["providers"]
         yield Header()
         with TabbedContent():
             with TabPane("Search", id="search"):  # Search "🔎"
                 with Horizontal(id="hosters"):
-                    yield Checkbox("AniWorld.to", True, id="aniworld_to")
-                    yield Checkbox("SerienStream.to", id="serienstream_to")
+                    yield Checkbox("AniWorld.to", value=providers["aniworld_to"], id="aniworld_to")
+                    yield Checkbox("SerienStream.to", value=providers["serienstream_to"], id="serienstream_to")
                 yield Input(id="input", placeholder="Search for a Anime")
                 yield ListView(id="results")
             with TabPane("Info", id="info", disabled=True):  # Info "ℹ"
                 with ScrollableContainer(id="res_con"):
                     yield Markdown(id="markdown")
                     yield ClickableDataTable(id="season_list")
             with TabPane("Settings", id="setting"):  # Settings "⚙"
                 # TODO: dont show unneeded on android
-                yield RadioButton("Fullscreen", id="fullscreen", value=True)
-                yield RadioButton("Syncplay", id="syncplay", value=False)
-                yield RadioButton("ani-skip", id="ani_skip", value=True)
-                yield RadioButton("Discord Presence", id="discord_presence", value=False)
+                with Container():
+                    yield SortableTable(id="lang")
+                    yield RadioButton("Fullscreen", id="fullscreen", value=settings["fullscreen"])
+                    yield RadioButton("Syncplay", id="syncplay", value=settings["syncplay"])
+                    yield RadioButton("ani-skip", id="ani-skip", value=settings["ani-skip"])
+                    yield RadioButton("Discord Presence", id="discord_presence", value=settings["discord_presence"])
             # with RadioSet():
             #    yield RadioButton("VOE", id="voe", value=True)
             #    yield RadioButton("Doodstream", id="doodstream")
             #    yield RadioButton("Vidoza", id="vidoza")
             #    yield RadioButton("Streamtape", id="streamtape")
         with Footer():
             with Center():
-                yield Label("Made by Commandcracker with ❤")
+                yield Label("Made by Commandcracker with [red]:heart:[/red]")
 
     # TODO: dont lock - no async
     async def on_mount(self) -> None:
+        lang = self.query_one("#lang", DataTable)
+        lang.add_columns("Language")
+        for l in self.language:
+            lang.add_row(l)
         self.query_one(Input).focus()
         # TODO: FIx sometimes not disabling loading
         # TODO: dont lock
         self.query_one("#info", TabPane).loading = True
-        table = self.query_one(DataTable)
+        table = self.query_one("#season_list", DataTable)
         table.cursor_type = "row"
         # TODO: make them scale
-        table.add_columns("FT", "S", "F", "Name", "Title", "Hoster", "Sprache")
+        table.add_columns("FT", "S", "F", "Title", "Hoster", "Sprache")
         if self.player is None:
             self.notify(
                 "You wont be able to play videos.\n"
                 "Without an supported video player!",
                 title="No player found",
                 severity="warning",
             )
@@ -312,24 +300,29 @@
         if self.RPC is not None:
             await self.RPC.clear()
             # close without closing event loop
             self.RPC.send_data(2, {"v": 1, "client_id": self.RPC.client_id})
             self.RPC.sock_writer.close()
             self.RPC = None
 
-    async def on_checkbox_changed(self):
+    async def on_checkbox_changed(self, event: Checkbox.Changed):
+        gucken_settings_manager.settings["settings"]["providers"][event.control.id] = event.value
         self.lookup_anime(self.query_one("#input", Input).value)
 
     async def on_radio_button_changed(self, event: RadioButton.Changed):
+        gucken_settings_manager.settings["settings"][event.control.id] = event.value
         if event.radio_button.id == "discord_presence":
             if event.value is True:
                 await self.enable_RPC()
             else:
                 await self.disable_RPC()
 
+    async def on_sortable_table_sort_changed(self, event: SortableTable.SortChanged) -> None:
+        move_item(self.language, event.previous, event.now)
+
     async def on_input_changed(self, message: Input.Changed) -> None:
         if message.value:
             self.lookup_anime(message.value)
         else:
             # TODO: fix sometimes wont clear
             await self.query_one("#results", ListView).clear()
 
@@ -355,15 +348,15 @@
 
         # TODO: Sort final_results with fuzzy-sort
         if len(final_results) > 0:
             self.current = final_results
             for series in final_results:
                 # TODO: show provider
                 await results_list_view.append(ClickableListItem(Markdown(
-                    f"##### **{series.name}** {series.production_year}\n{series.description}"
+                    f"##### {series.name} {series.production_year}\n{series.description}"
                 )))
         results_list_view.loading = False
         if len(final_results) > 0:
 
             def select_first_index():
                 try:
                     results_list_view.index = 0
@@ -394,20 +387,20 @@
                 if key not in ["down", "up", "enter"]:
                     if lv.has_focus:
                         inp.focus()
                         if key == "backspace":
                             inp.action_delete_left()
                         else:
                             await inp.on_event(event)
-            if key == "enter" and self.query_one(DataTable).has_focus:
+            if key == "enter" and self.query_one("#season_list", DataTable).has_focus:
                 self.play_selected()
 
     @work(exclusive=True)
     async def play_selected(self):
-        dt = self.query_one(DataTable)
+        dt = self.query_one("#season_list", DataTable)
         # TODO: show loading
         dt.loading = True
         index = self.app.query_one("#results", ListView).index
         series_search_result = self.current[index]
         self.play(series_search_result=series_search_result, episodes=self.current_info.episodes, index=dt.cursor_row)
         dt.loading = False
 
@@ -419,15 +412,15 @@
         info_tab.loading = True
         self.query_one(TabbedContent).active = "info"
         md = self.query_one("#markdown", Markdown)
         series = await series_search_result.get_series()
         self.current_info = series
         await md.update(series.to_markdown())
 
-        table = self.query_one(DataTable)
+        table = self.query_one("#season_list", DataTable)
         table.clear()
         c = 0
         for ep in series.episodes:
             hl = []
             for h in ep.available_hoster:
                 if h is VOEHoster:
                     hl.append("VEO")
@@ -436,30 +429,24 @@
                 if h is VidozaHoster:
                     hl.append("VZ")
                 if h is StreamtapeHoster:
                     hl.append("ST")
 
             ll = []
             for l in ep.available_language:
-                if l == Language.DE:
-                    ll.append("DE")
-                if l == Language.JP_DESUB:
-                    ll.append("JP_DESUB")
-                if l == Language.JP_ENSUB:
-                    ll.append("JP_ENSUB")
+                ll.append(l.name)
 
             c += 1
             table.add_row(
                 c,
                 ep.season,
                 ep.episode_number,
                 ep.title,
-                "",
-                ", ".join(hl),
-                ", ".join(ll)
+                " ".join(hl),
+                " ".join(ll)
             )
         table.focus(scroll_visible=False)
         info_tab.loading = False
 
     @work(exclusive=True, thread=True)
     async def update_check(self):
         res = await check()
@@ -476,15 +463,23 @@
             series_search_result: SearchResult,
             episodes: list[Episode],
             index: int
     ) -> None:
         episode: Episode = episodes[index]
         processed_hoster = await episode.process_hoster()
 
-        lang = sort_favorite_lang(episode.available_language)[0]
+        if len(episode.available_language) <= 0:
+            self.notify(
+                "The episode you are trying to watch has no stream available.",
+                title="No stream available",
+                severity="error",
+            )
+            return
+
+        lang = sort_favorite_lang(episode.available_language, self.language)[0]
         sorted_hoster = sort_favorite_hoster(processed_hoster.get(lang))
         direct_link = await get_working_direct_link(sorted_hoster)
 
         # TODO: check for header support
 
         if self.player is None:
             self.notify(
@@ -493,15 +488,15 @@
                 title="No player found",
                 severity="error",
             )
             return
 
         # TODO: ani_skip, syncplay, fullscreen as cli arg
         # TODO: pass ani_skip as script
-        ani_skip = self.query_one("#ani_skip", RadioButton).value
+        ani_skip = self.query_one("#ani-skip", RadioButton).value
         syncplay = self.query_one("#syncplay", RadioButton).value
         fullscreen = self.query_one("#fullscreen", RadioButton).value
 
         title = f"{series_search_result.name} - {episode.title}"
         args = self.player.play(direct_link.url, title, fullscreen, direct_link.headers)
 
         if self.RPC and self.RPC.sock_writer:
@@ -520,15 +515,15 @@
 
             self.app.call_later(update)
 
         chapters_file = None
 
         # TODO: cache more
         if isinstance(self.player, MPVPlayer):
-            if ani_skip:
+            if ani_skip is True:
                 timings = await get_timings_from_search(series_search_result.name, index + 1)
                 if timings:
                     chapters_file = generate_chapters_file(timings)
 
                     def delete_chapters_file():
                         try:
                             remove(chapters_file.name)
@@ -570,14 +565,18 @@
                     self.notify(
                         "Your player is not supported by Syncplay",
                         title="Player not supported",
                         severity="warning",
                     )
 
         logging.info("Running: %s", args)
+        # TODO: detach on linux
+        # multiprocessing
+        # child_pid = os.fork()
+        # if child_pid == 0:
         process = Popen(args, stderr=PIPE, stdout=DEVNULL, stdin=DEVNULL)
         while not self.app._exit:
             sleep(0.1)
 
             resume_time = None
 
             # only if mpv
@@ -612,17 +611,21 @@
                             self.play(
                                 series_search_result,
                                 episodes,
                                 index + 1,
                             )
 
                     await self.app.push_screen(
-                        Next("Playing next episode in", no_time=hasattr(sys, 'getandroidapilevel')), callback=play_next)
+                        Next("Playing next episode in", no_time=is_android), callback=play_next)
 
-                self.app.call_later(push_next_screen)
+                if not len(episodes) <= index + 1:
+                    self.app.call_later(push_next_screen)
+                else:
+                    # TODO: ask to mark as completed
+                    pass
                 return
 
 
 exit_quotes = [
     "Closing one anime is just an invitation to open another.",
     "You finished one, now finish the next.",
     "Don't stop now, there's a whole universe waiting to be explored.",
```

### Comparing `gucken-0.0.3/src/gucken/gucken.tcss` & `gucken-0.1.0/src/gucken/gucken.css`

 * *Files 11% similar despite different names*

```diff
@@ -30,26 +30,34 @@
 
 #input {
     margin: 1 0;
 }
 
 #markdown {
     margin: 0 0;
+    margin-top: -1;
 }
 
+/*TODO: make height 100 of what the table needs, so there is only one scroll*/
 #season_list {
     margin: 1 0;
+    margin-top: 0;
     margin-bottom: 0;
+    min-height: 3;
 }
 
 TabbedContent #--content-tab-setting {
     dock: right;
     margin-right: 1;
 }
 
 #setting > RadioButton {
     margin-bottom: 1;
 }
 
 ClickableListItem {
     padding-bottom: -1;
+    padding-left: -2;
+    padding-right: -2;
 }
+
+/*$accent: lime;*/
```

### Comparing `gucken-0.0.3/src/gucken/update.py` & `gucken-0.1.0/src/gucken/update.py`

 * *Files identical despite different names*

### Comparing `gucken-0.0.3/src/gucken/hoster/common.py` & `gucken-0.1.0/src/gucken/hoster/common.py`

 * *Files identical despite different names*

### Comparing `gucken-0.0.3/src/gucken/hoster/doodstream.py` & `gucken-0.1.0/src/gucken/hoster/doodstream.py`

 * *Files identical despite different names*

### Comparing `gucken-0.0.3/src/gucken/hoster/streamtape.py` & `gucken-0.1.0/src/gucken/hoster/streamtape.py`

 * *Files identical despite different names*

### Comparing `gucken-0.0.3/src/gucken/hoster/veo.py` & `gucken-0.1.0/src/gucken/hoster/veo.py`

 * *Files identical despite different names*

### Comparing `gucken-0.0.3/src/gucken/hoster/vidoza.py` & `gucken-0.1.0/src/gucken/hoster/vidoza.py`

 * *Files identical despite different names*

### Comparing `gucken-0.0.3/src/gucken/player/android.py` & `gucken-0.1.0/src/gucken/player/android.py`

 * *Files identical despite different names*

### Comparing `gucken-0.0.3/src/gucken/player/common.py` & `gucken-0.1.0/src/gucken/player/common.py`

 * *Files identical despite different names*

### Comparing `gucken-0.0.3/src/gucken/player/ffplay.py` & `gucken-0.1.0/src/gucken/player/ffplay.py`

 * *Files identical despite different names*

### Comparing `gucken-0.0.3/src/gucken/player/flatpak.py` & `gucken-0.1.0/src/gucken/player/flatpak.py`

 * *Files identical despite different names*

### Comparing `gucken-0.0.3/src/gucken/player/mpv.py` & `gucken-0.1.0/src/gucken/player/mpv.py`

 * *Files identical despite different names*

### Comparing `gucken-0.0.3/src/gucken/player/vlc.py` & `gucken-0.1.0/src/gucken/player/vlc.py`

 * *Files identical despite different names*

### Comparing `gucken-0.0.3/src/gucken/player/wmplayer.py` & `gucken-0.1.0/src/gucken/player/wmplayer.py`

 * *Files identical despite different names*

### Comparing `gucken-0.0.3/src/gucken/provider/aniworld.py` & `gucken-0.1.0/src/gucken/provider/aniworld.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,34 +9,38 @@
 from ..hoster.doodstream import DoodstreamHoster
 from ..hoster.streamtape import StreamtapeHoster
 from ..hoster.veo import VOEHoster
 from ..hoster.vidoza import VidozaHoster
 from .common import Episode, Hoster, Language, Provider, SearchResult, Series
 
 
-def data_lang_key_to_lang(data_lang_key: str) -> Language:
-    if data_lang_key == "1":
-        return Language.DE
-    if data_lang_key == "2":
-        return Language.JP_ENSUB
-    if data_lang_key == "3":
-        return Language.JP_DESUB
-
-
 def provider_to_hoster(provider: str, url: str) -> Hoster:
     if provider == "VOE":
         return VOEHoster(url)
     if provider == "Doodstream":
         return DoodstreamHoster(url)
     if provider == "Vidoza":
         return VidozaHoster(url)
     if provider == "Streamtape":
         return StreamtapeHoster(url)
 
 
+def lang_img_src_lang_name_to_lang(name: str) -> Language:
+    if name == "english":
+        return Language.EN
+    if name == "english-german":
+        return Language.EN_DESUB
+    if name == "japanese-english":
+        return Language.JP_ENSUB
+    if name == "japanese-german":
+        return Language.JP_DESUB
+    if name == "german":
+        return Language.DE
+
+
 @dataclass
 class AniWorldEpisode(Episode):
     url: str
 
     async def process_hoster(self) -> dict[Language, list[Hoster]]:
         async with AsyncClient(verify=False) as client:
             response = await client.get(f"{self.url}/staffel-{self.season}/episode-{self.episode_number}")
@@ -47,27 +51,31 @@
                 attrs={
                     "data-lang-key": True,
                     "data-link-id": True,
                     "data-link-target": True,
                     "data-external-embed": True
                 }
             )
-
-            processed_hoster = {
-                Language.DE: list(),
-                Language.JP_DESUB: list(),
-                Language.JP_ENSUB: list(),
-            }
+            processed_hoster = {}
+            for l in Language:
+                processed_hoster[l] = list()
+
+            langs = soup.find("div", class_="changeLanguage").find_all("img")
+            lang_map = {}
+            for lang in langs:
+                lang_name = lang.attrs.get("src").split("/")[-1].rsplit(".", 1)[0]
+                data_lang_key = lang.attrs.get("data-lang-key")
+                lang_map[data_lang_key] = lang_img_src_lang_name_to_lang(lang_name)
 
             for episode in watch_episode:
                 data_link_id = episode.attrs.get("data-link-id")
                 provider = episode.find_next("h4").text
 
                 data_lang_key = episode.attrs.get("data-lang-key")
-                lang = data_lang_key_to_lang(data_lang_key)
+                lang = lang_map[data_lang_key]
 
                 hoster = provider_to_hoster(provider, f"https://{AniWorldProvider.host}/redirect/{data_link_id}")
 
                 processed_hoster[lang].append(hoster)
 
             return processed_hoster
 
@@ -84,15 +92,15 @@
 
     def to_markdown(self) -> str:
         return (
             f"# {self.name} {self.production_year}\n{self.full_description}\n\n"
             f"**Regisseure**: {', '.join(self.regisseure)}\\\n"
             f"**Schauspieler**: {', '.join(self.schauspieler)}\\\n"
             f"**Produzent**: {', '.join(self.produzent)}\\\n"
-            f"**Land**: {', '.join(self.land)}\n\n"
+            f"**Land**: {', '.join(self.land)}\\\n"
             f"**Tags**: {', '.join(self.tags)}"
         )
 
 
 @dataclass
 class AniWorldSearchResult(SearchResult):
     link: str = None
@@ -117,15 +125,15 @@
             return None
         async with AsyncClient(verify=False) as client:
             response = await client.get(f"https://{AniWorldProvider.host}/ajax/seriesSearch?keyword={keyword}")
             results = response.json()
             search_results = []
             for series in results:
                 search_results.append(AniWorldSearchResult(
-                    name=unescape(series.get("name")),
+                    name=unescape(series.get("name")).strip(),
                     link=series.get("link"),
                     description=unescape(series.get("description")),
                     cover=f"https://{AniWorldProvider.host}{series.get('cover')}",
                     production_year=series.get("productionYear"),
                     host=AniWorldProvider.host
                 ))
             return search_results
@@ -176,16 +184,16 @@
             feps = []
             for e in eps:
                 for b in e:
                     feps.append(b)
 
             return AniWorldSeries(
                 # cover=f"https://{search_result.host}" + soup.find("div", class_="seriesCoverBox").find("img").attrs.get("data-src"),
-                name=unescape(soup.find("h1", attrs={"itemprop": "name"}).find("span").text),
-                production_year=unescape(soup.find("div", class_="series-title").find("small").text).lstrip(),
+                name=unescape(soup.find("h1", attrs={"itemprop": "name"}).find("span").text).strip(),
+                production_year=unescape(soup.find("div", class_="series-title").find("small").text).strip(),
                 # age=int(soup.find("div", class_="fsk").find("span").text),
                 # imdb_link=soup.find("a", class_="imdb-link").attrs.get("href"),
                 full_description=unescape(soup.find("p", class_="seri_des").attrs.get("data-full-description")),
                 regisseure=directors,
                 schauspieler=actors,
                 produzent=creators,
                 land=countrys,
@@ -211,40 +219,36 @@
     episodes = []
     e_count = 0
     for episode in soup.find("table", class_="seasonEpisodesList").find("tbody").find_all("tr"):
         title = episode.find_next("td", class_="seasonEpisodeTitle")
 
         language = set()
         for flag in episode.find_next("td", class_="editFunctions").find_all("img"):
-            t = flag.attrs.get("title")
-            if t == "Englisch":
-                language.add(Language.JP_ENSUB)
-            if t == "Deutsch/German":
-                language.add(Language.DE)
-            if t == "Mit deutschem Untertitel":
-                language.add(Language.JP_DESUB)
+            lang_name = flag.attrs.get("src").split("/")[-1].rsplit(".", 1)[0]
+            language.add(lang_img_src_lang_name_to_lang(lang_name))
 
         hoster = set()
         for h in episode.find_all_next("i", class_="icon"):
             t = h.attrs.get("title")
             if t == "VOE":
                 hoster.add(VOEHoster)
             if t == "Doodstream":
                 hoster.add(DoodstreamHoster)
             if t == "Vidoza":
                 hoster.add(VidozaHoster)
             if t == "Streamtape":
                 hoster.add(StreamtapeHoster)
 
         e_count += 1
-        title_en = title.find("span").text.lstrip()
-        title_de = title.find("strong").text.lstrip()
+        title_en = title.find("span").text.strip()
+        title_de = title.find("strong").text.strip()
+        title = f"{title_en} - {title_de}" if title_en and title_de else title_en or title_de
         episodes.append(AniWorldEpisode(
             url=url,
-            title=f"{title_en} - {title_de}",
+            title=title,
             season=staffel,
             episode_number=e_count,
             available_hoster=hoster,
             available_language=language,
             total_episode_number=None
             # language=language,
             # hoster=hoster,
```

### Comparing `gucken-0.0.3/src/gucken/provider/common.py` & `gucken-0.1.0/src/gucken/provider/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from typing import Union
 
 from ..hoster.common import Hoster
 
 
 class Language(Enum):
     DE = "Deutsch"
+    EN = "English"
+    EN_DESUB = "English mit deutschen untertitel"
     JP_DESUB = "Japanisch mit deutschen untertitel"
     JP_ENSUB = "Japanisch mit englischen untertitel"
 
 
 @dataclass
 class Episode:
     title: str
```

### Comparing `gucken-0.0.3/src/gucken/provider/serienstream.py` & `gucken-0.1.0/src/gucken/provider/serienstream.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,34 +9,38 @@
 from ..hoster.doodstream import DoodstreamHoster
 from ..hoster.streamtape import StreamtapeHoster
 from ..hoster.veo import VOEHoster
 from ..hoster.vidoza import VidozaHoster
 from .common import Episode, Hoster, Language, Provider, SearchResult, Series
 
 
-def data_lang_key_to_lang(data_lang_key: str) -> Language:
-    if data_lang_key == "1":
-        return Language.DE
-    if data_lang_key == "2":
-        return Language.JP_ENSUB
-    if data_lang_key == "3":
-        return Language.JP_DESUB
-
-
 def provider_to_hoster(provider: str, url: str) -> Hoster:
     if provider == "VOE":
         return VOEHoster(url)
     if provider == "Doodstream":
         return DoodstreamHoster(url)
     if provider == "Vidoza":
         return VidozaHoster(url)
     if provider == "Streamtape":
         return StreamtapeHoster(url)
 
 
+def lang_img_src_lang_name_to_lang(name: str) -> Language:
+    if name == "english":
+        return Language.EN
+    if name == "english-german":
+        return Language.EN_DESUB
+    if name == "japanese-english":
+        return Language.JP_ENSUB
+    if name == "japanese-german":
+        return Language.JP_DESUB
+    if name == "german":
+        return Language.DE
+
+
 @dataclass
 class SerienStreamEpisode(Episode):
     url: str
 
     async def process_hoster(self) -> dict[Language, list[Hoster]]:
         async with AsyncClient(verify=False) as client:
             response = await client.get(f"{self.url}/staffel-{self.season}/episode-{self.episode_number}")
@@ -47,27 +51,31 @@
                 attrs={
                     "data-lang-key": True,
                     "data-link-id": True,
                     "data-link-target": True,
                     "data-external-embed": True
                 }
             )
-
-            processed_hoster = {
-                Language.DE: list(),
-                Language.JP_DESUB: list(),
-                Language.JP_ENSUB: list(),
-            }
+            processed_hoster = {}
+            for l in Language:
+                processed_hoster[l] = list()
+
+            langs = soup.find("div", class_="changeLanguage").find_all("img")
+            lang_map = {}
+            for lang in langs:
+                lang_name = lang.attrs.get("src").split("/")[-1].rsplit(".", 1)[0]
+                data_lang_key = lang.attrs.get("data-lang-key")
+                lang_map[data_lang_key] = lang_img_src_lang_name_to_lang(lang_name)
 
             for episode in watch_episode:
                 data_link_id = episode.attrs.get("data-link-id")
                 provider = episode.find_next("h4").text
 
                 data_lang_key = episode.attrs.get("data-lang-key")
-                lang = data_lang_key_to_lang(data_lang_key)
+                lang = lang_map[data_lang_key]
 
                 hoster = provider_to_hoster(provider, f"https://{SerienStreamProvider.host}/redirect/{data_link_id}")
 
                 processed_hoster[lang].append(hoster)
 
             return processed_hoster
 
@@ -84,15 +92,15 @@
 
     def to_markdown(self) -> str:
         return (
             f"# {self.name} {self.production_year}\n{self.full_description}\n\n"
             f"**Regisseure**: {', '.join(self.regisseure)}\\\n"
             f"**Schauspieler**: {', '.join(self.schauspieler)}\\\n"
             f"**Produzent**: {', '.join(self.produzent)}\\\n"
-            f"**Land**: {', '.join(self.land)}\n\n"
+            f"**Land**: {', '.join(self.land)}\\\n"
             f"**Tags**: {', '.join(self.tags)}"
         )
 
 
 @dataclass
 class SerienStreamSearchResult(SearchResult):
     link: str = None
@@ -117,15 +125,15 @@
             return None
         async with AsyncClient(verify=False) as client:
             response = await client.get(f"https://{SerienStreamProvider.host}/ajax/seriesSearch?keyword={keyword}")
             results = response.json()
             search_results = []
             for series in results:
                 search_results.append(SerienStreamSearchResult(
-                    name=unescape(series.get("name")),
+                    name=unescape(series.get("name")).strip(),
                     link=series.get("link"),
                     description=unescape(series.get("description")),
                     cover=f"https://s.to{series.get('cover')}",
                     production_year=series.get("productionYear"),
                     host=SerienStreamProvider.host
                 ))
             return search_results
@@ -176,16 +184,16 @@
             feps = []
             for e in eps:
                 for b in e:
                     feps.append(b)
 
             return SerienStreamSeries(
                 # cover=f"https://{search_result.host}" + soup.find("div", class_="seriesCoverBox").find("img").attrs.get("data-src"),
-                name=unescape(soup.find("h1", attrs={"itemprop": "name"}).find("span").text),
-                production_year=unescape(soup.find("div", class_="series-title").find("small").text).lstrip(),
+                name=unescape(soup.find("h1", attrs={"itemprop": "name"}).find("span").text).strip(),
+                production_year=unescape(soup.find("div", class_="series-title").find("small").text).strip(),
                 # age=int(soup.find("div", class_="fsk").find("span").text),
                 # imdb_link=soup.find("a", class_="imdb-link").attrs.get("href"),
                 full_description=unescape(soup.find("p", class_="seri_des").attrs.get("data-full-description")),
                 regisseure=directors,
                 schauspieler=actors,
                 produzent=creators,
                 land=countrys,
@@ -211,41 +219,36 @@
     episodes = []
     e_count = 0
     for episode in soup.find("table", class_="seasonEpisodesList").find("tbody").find_all("tr"):
         title = episode.find_next("td", class_="seasonEpisodeTitle")
 
         language = set()
         for flag in episode.find_next("td", class_="editFunctions").find_all("img"):
-            t = flag.attrs.get("title")
-            if t == "Englisch":
-                language.add(Language.JP_ENSUB)
-            if t == "Deutsch/German":
-                language.add(Language.DE)
-            if t == "Mit deutschem Untertitel":
-                language.add(Language.JP_DESUB)
+            lang_name = flag.attrs.get("src").split("/")[-1].rsplit(".", 1)[0]
+            language.add(lang_img_src_lang_name_to_lang(lang_name))
 
         hoster = set()
         for h in episode.find_all_next("i", class_="icon"):
             t = h.attrs.get("title")
             if t == "VOE":
                 hoster.add(VOEHoster)
             if t == "Doodstream":
                 hoster.add(DoodstreamHoster)
             if t == "Vidoza":
                 hoster.add(VidozaHoster)
             if t == "Streamtape":
                 hoster.add(StreamtapeHoster)
 
         e_count += 1
-        title_en = title.find("span").text.lstrip()
-        title_de = title.find("strong").text.lstrip()
-
+        title_en = title.find("span").text.strip()
+        title_de = title.find("strong").text.strip()
+        title = f"{title_en} - {title_de}" if title_en and title_de else title_en or title_de
         episodes.append(SerienStreamEpisode(
             url=url,
-            title=f"{title_en} - {title_de}",
+            title=title,
             season=staffel,
             episode_number=e_count,
             available_hoster=hoster,
             available_language=language,
             total_episode_number=None
             #language=language,
             #hoster=hoster,
```

### Comparing `gucken-0.0.3/src/gucken/tracker/anilist.py` & `gucken-0.1.0/src/gucken/tracker/anilist.py`

 * *Files identical despite different names*

### Comparing `gucken-0.0.3/LICENSE.txt` & `gucken-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gucken-0.0.3/pyproject.toml` & `gucken-0.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 dynamic = ["version"]
 description = "Gucken is a Terminal User Interface which allows you to browse and watch your favorite anime's with style."
 authors = [{name="Commandcracker"}]
 maintainers = [{name="Commandcracker"}]
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 dependencies = [
-  "textual>=0.58.1",
+  "textual>=0.60.1",
   "beautifulsoup4>=4.12.3",
   "httpx>=0.27.0",
   "pypresence>=4.3.0",
-  "packaging>=24.0"
+  "packaging>=24.0",
+  "platformdirs>=4.2.2",
+  "toml>=0.10.2"
   #"yt-dlp>=2024.4.9",
   #"mpv>=1.0.6",
   #"httpx[socks]",
 ]
 keywords = [
   "gucken",
   "anime",
```

### Comparing `gucken-0.0.3/PKG-INFO` & `gucken-0.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gucken
-Version: 0.0.3
+Version: 0.1.0
 Summary: Gucken is a Terminal User Interface which allows you to browse and watch your favorite anime's with style.
 Project-URL: Repository, https://github.com/Commandcracker/gucken
 Author: Commandcracker
 Maintainer: Commandcracker
 License: MIT License
         
         Copyright (c) 2024 Commandcracker
@@ -43,82 +43,112 @@
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Video
 Requires-Dist: beautifulsoup4>=4.12.3
 Requires-Dist: httpx>=0.27.0
 Requires-Dist: packaging>=24.0
+Requires-Dist: platformdirs>=4.2.2
 Requires-Dist: pypresence>=4.3.0
-Requires-Dist: textual>=0.58.1
+Requires-Dist: textual>=0.60.1
+Requires-Dist: toml>=0.10.2
 Description-Content-Type: text/markdown
 
 # Gucken
 
+Project state: **Pre-Alpha**
+
 ## Description
 
 Gucken is a Terminal User Interface which allows you to browse and watch your favorite anime's with style. 
 
 ## Usage
 
-Search
-![Search](.README/Search.png)
-and watch
-![Watch](.README/Watch.png)
+<img alt="Search" src="https://github.com/Commandcracker/gucken/assets/49335821/d91de2af-c086-485c-8aec-1e68cdb02aa3"/>
+<img alt="Watch" src="https://github.com/Commandcracker/gucken/assets/49335821/7354eeff-bd97-4226-91b9-317939128a81"/> 
 
 ## Installation
 
-### Windows
+<details><summary><b>Windows</b></summary>
 
 Install [Python] and if you are **on Windows 10** [Windows Terminal] for a better experience.
 
 ```
 pip install gucken
 gucken
 ```
 
-### Linux
+</details>
+
+<details><summary><b>Linux</b></summary>
 
 Install [Python] and then
 
 ```
 pip install gucken
 gucken
 ```
 
-### Android
+</details>
+
+<details><summary><b>Android</b></summary>
 
 Install [Termux](https://termux.dev/en/) and run:
 
 ```
-pkg update -y
-pkg upgrade -y
+yes|pkg update
 pkg install python ffmpeg -y
 pip install gucken
 gucken
 ```
 
-#### Optional
+#### Shortcut
+
+Install [Termux:Widget](https://github.com/termux/termux-widget?tab=readme-ov-file#Installation).
+
+##### Lunch shortcut
+
+```
+echo gucken>~/.shortcuts/Gucken
+```
 
-Setup storage for downloads.
+##### Update shortcut
+
+```
+echo pip install -U gucken>~/.shortcuts/Update\ Gucken
+```
+
+#### Custom Font
+
+If you want a custom font then just pace the ttf in `~/.termux/font.ttf`. Recommended fonts: [Nerd fonts](https://www.nerdfonts.com/font-downloads) (**Only use Mono fonts!**)
+
+#### Downloads
+
+Setup storage for downloads. (Default download location: `/data/data/com.termux/files/home/storage/movies`)
 
 ```
 termux-setup-storage
 ```
 
+</details>
+
 ## Features
 
 - [x] Update checker
+- [x] Language priority list
+- [ ] Hoster priority list
+- [x] Automatically use working hoster
 - [x] Browsing
   - [x] Descriptions
 - [x] Watching
   - [x] Automatically start next episode
   - [x] Discord Presence **WIP**
   - [MPV] only
-    - [X] [ani-skip](https://github.com/synacktraa/ani-skip) support **Very WIP**
-    - [x] [Syncplay](https://github.com/Syncplay/syncplay) support
+    - [X] [ani-skip](https://github.com/synacktraa/ani-skip) support **Very WIP** (need skip plugin)
+    - [x] [Syncplay](https://github.com/Syncplay/syncplay) support (almost out of WIP)
     - [ ] Remember watch time **WIP**
     - [ ] Remember completed Episodes (and series)
   - [ ] Tracker support
     - [ ] [MyAnimeList](https://myanimelist.net/)
     - [ ] [AniList](https://anilist.co/)
     - [ ] [AniWorld.to] & [SerienStream.to]
 - [ ] Downloading
@@ -126,25 +156,28 @@
 
 ## Provider
 
 List of supported Anime sites
 
 - [x] [AniWorld.to] & [SerienStream.to]
   - [ ] Filme
-  - [ ] Language Selection
-  - [x] Automatically use working provider
-    - [x] Streamtape
-    - [x] VEO
-    - [x] Vidoza
-    - [x] Doodstream
 - [ ] [bs.to](https://bs.to/)
 - [ ] [www3.streamcloud.info](https://www3.streamcloud.info/)
 - [ ] [www.crunchyroll.com](https://www.crunchyroll.com)
 - [ ] Add some from [International Piracy Sites German](https://fmhy.net/non-english#german-deutsch)
 
+## Hoster
+
+List of supported video hoster.
+
+- [x] Streamtape
+- [x] VEO
+- [x] Vidoza
+- [x] Doodstream
+
 ## Player
 
 List of supported video players
 
 - [x] [MPV] (most features, recommended)
 - [x] [VLC]
 - [x] [ffplay](https://www.ffmpeg.org/ffplay.html)
@@ -161,18 +194,30 @@
   - [x] [VLC](https://flathub.org/apps/org.videolan.VLC)
   - [x] [Celluloid](https://flathub.org/apps/io.github.celluloid_player.Celluloid)
 - Linux
   - [x] [Celluloid](https://celluloid-player.github.io/)
 - MacOS
   - [ ] [IINA](https://iina.io/)
 
+## Custom CSS
+
+**For power users only**
+
+Place your custom CSS in `user_config_path("gucken").joinpath("custom.css")` and it will be automatically loaded by Gucken.
+
+- [Textual CSS Guide](https://textual.textualize.io/guide/CSS/)
+- [Textual CSS Reference](https://textual.textualize.io/css_types/)
+
 ## Todo
 
 - [ ] Up-scaling (after download)
   - [ ] [video2x](https://github.com/k4yt3x/video2x)
+  - [ ] [waifu2x](https://github.com/nagadomi/waifu2x)
+  - [ ] [Real-ESRGAN](https://github.com/xinntao/Real-ESRGAN)
+  - [ ] [FSRCNN](https://github.com/igv/FSRCNN-TensorFlow)
   - [ ] [Anime4k]
 - [ ] Proxy support
   ```
   Note:
   Proxies can easiely be implented
   
   for the http client in python
@@ -192,15 +237,14 @@
   AniWorld.to need Cloudflare captcha and JS challange
   SerienStream.to can be bypassed by using diract ip
   
   Cloudflare captcha and JS challange can be solved by using something like
   selenium or playwright
   ```
 - [ ] [MPV] Screen selection
-- [ ] Save settings
 - [ ] Custom player args
 - [ ] Custom player
 - [ ] Colors themes
 - [ ] Installation helper
   - [ ] [MPV]
     - [ ] [Anime4k]
   - [ ] [VLC]
@@ -211,21 +255,47 @@
 - [ ] [Anime4k] options
 - [ ] Modular (Custom extractors/players, API)
 - [ ] Proper error handling
 - [ ] Logging and Crash reports
 - [ ] Pre-fetching
 - [ ] improve [ani-skip](https://github.com/synacktraa/ani-skip) support
 - [ ] Use something like opencv to time match a sub from aniworld with a high quality video form another site.
-- [ ] Image preview
+- [ ] Image preview (Kitty protocol, iterm protocol, Sixel, textual-web)
+- [ ] Support textual-web
 - [ ] Blacklist detection & bypass
 - [ ] Syncplay on Android
 - [ ] Mac support
 - [ ] IOS support
 - [ ] Option to disable update checker
 - [ ] Update checker option to perform update
+- [ ] Snap support ?
+- [ ] 404 detection inside Hoster and don't crash whole program on http error + crash reports/logs
+- [ ] s.to, aniworld.to scrape episode description
+- [ ] search in episodes
+- [ ] Focus window when ask next
+- [ ] next and cancel hotkeys
+- [ ] show hotkeys in Footer
+- [ ] ani-skip load skip plugin from src
+- [ ] ani-skip only to get chapters
+- [ ] Window in settings menu to show where files are located (data, logs, config, downloads)
+- [ ] Utilize next and previous buttons in mpv
+- [ ] Nix
+- [ ] Docker
+- [ ] Flatpack ?
+- [ ] Merge anime's from SerienStream.to to AniWorld.to to get more langs
+- [ ] Fix title
+- [ ] Do unescape and stripe only on render
+- [ ] Dont coppy code from SerienStream.to to AniWorld.to
+- [ ] FIX TYPING SOMETIMES CAUSES CRASH
+- [ ] option to disable debug logging
+- [ ] BIG CODE CLEANUP
+- [ ] Player selection
+- [ ] Hoster prio list
+- [ ] Translation
+- [ ] detect existing chapters and use them for skip
 
 [Anime4k]: https://github.com/bloc97/Anime4K
 [MPV]: https://mpv.io/
 [VLC]: https://www.videolan.org/vlc/
 [AniWorld.to]: https://aniworld.to
 [SerienStream.to]: https://186.2.175.5
 [Python]: https://www.python.org/downloads/
```

