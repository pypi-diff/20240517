# Comparing `tmp/gaycore-2.0.1.tar.gz` & `tmp/gaycore-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gaycore-2.0.1.tar", last modified: Mon Nov  2 04:56:56 2020, max compression
+gzip compressed data, was "gaycore-3.0.tar", last modified: Fri May 17 11:00:26 2024, max compression
```

## Comparing `gaycore-2.0.1.tar` & `gaycore-3.0.tar`

### file list

```diff
@@ -1,25 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-02 04:56:56.000000 gaycore-2.0.1/
--rw-r--r--   0 root         (0) root         (0)       39 2020-10-26 02:07:33.000000 gaycore-2.0.1/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1093 2020-10-26 02:07:33.000000 gaycore-2.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      820 2020-11-02 04:56:56.000000 gaycore-2.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2020-11-02 03:48:09.000000 gaycore-2.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-02 04:56:56.000000 gaycore-2.0.1/gaycore/
--rw-r--r--   0 root         (0) root         (0)       45 2020-10-26 02:07:33.000000 gaycore-2.0.1/gaycore/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2020-11-02 03:48:09.000000 gaycore-2.0.1/gaycore/cli.py
--rw-r--r--   0 root         (0) root         (0)     1298 2020-11-02 03:48:09.000000 gaycore-2.0.1/gaycore/config.py
--rw-r--r--   0 root         (0) root         (0)    13347 2020-11-02 04:54:04.000000 gaycore-2.0.1/gaycore/gcore_box.py
--rw-r--r--   0 root         (0) root         (0)     2155 2020-11-02 03:48:09.000000 gaycore-2.0.1/gaycore/player.py
--rw-r--r--   0 root         (0) root         (0)     2974 2020-11-02 04:52:03.000000 gaycore-2.0.1/gaycore/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-02 04:56:56.000000 gaycore-2.0.1/gaycore.egg-info/
--rw-r--r--   0 root         (0) root         (0)      820 2020-11-02 04:56:56.000000 gaycore-2.0.1/gaycore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      402 2020-11-02 04:56:56.000000 gaycore-2.0.1/gaycore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-11-02 04:56:56.000000 gaycore-2.0.1/gaycore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2020-11-02 04:56:56.000000 gaycore-2.0.1/gaycore.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        9 2020-11-02 04:56:56.000000 gaycore-2.0.1/gaycore.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2020-11-02 04:56:56.000000 gaycore-2.0.1/gaycore.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-11-02 04:56:56.000000 gaycore-2.0.1/gaycore.egg-info/zip-safe
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-02 04:56:56.000000 gaycore-2.0.1/img/
--rw-r--r--   0 root         (0) root         (0)  2429626 2020-10-26 02:07:33.000000 gaycore-2.0.1/img/gcore1.gif
--rw-r--r--   0 root         (0) root         (0)       18 2020-11-02 03:48:09.000000 gaycore-2.0.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       79 2020-11-02 04:56:56.000000 gaycore-2.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1277 2020-11-02 04:55:50.000000 gaycore-2.0.1/setup.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-05-17 11:00:26.228393 gaycore-3.0/
+-rw-r--r--   0 hyi        (502) staff       (20)     1074 2024-05-11 04:50:29.000000 gaycore-3.0/LICENSE
+-rw-r--r--   0 hyi        (502) staff       (20)      967 2024-05-17 11:00:26.228021 gaycore-3.0/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)     1089 2024-05-17 10:51:16.000000 gaycore-3.0/README.md
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-05-17 11:00:26.214247 gaycore-3.0/gaycore/
+-rw-r--r--   0 hyi        (502) staff       (20)       42 2024-05-11 04:50:29.000000 gaycore-3.0/gaycore/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)      139 2024-05-17 10:59:50.000000 gaycore-3.0/gaycore/__main__.py
+-rw-r--r--   0 hyi        (502) staff       (20)      154 2024-05-11 04:50:29.000000 gaycore-3.0/gaycore/cli.py
+-rw-r--r--   0 hyi        (502) staff       (20)     6431 2024-05-17 10:59:50.000000 gaycore-3.0/gaycore/config.py
+-rw-r--r--   0 hyi        (502) staff       (20)    13679 2024-05-17 10:59:50.000000 gaycore-3.0/gaycore/gcore_box.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2089 2024-05-11 04:52:05.000000 gaycore-3.0/gaycore/player.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3546 2024-05-17 10:59:50.000000 gaycore-3.0/gaycore/utils.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-05-17 11:00:26.224447 gaycore-3.0/gaycore.egg-info/
+-rw-r--r--   0 hyi        (502) staff       (20)      967 2024-05-17 11:00:26.000000 gaycore-3.0/gaycore.egg-info/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)      379 2024-05-17 11:00:26.000000 gaycore-3.0/gaycore.egg-info/SOURCES.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        1 2024-05-17 11:00:26.000000 gaycore-3.0/gaycore.egg-info/dependency_links.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       44 2024-05-17 11:00:26.000000 gaycore-3.0/gaycore.egg-info/entry_points.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       24 2024-05-17 11:00:26.000000 gaycore-3.0/gaycore.egg-info/requires.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        8 2024-05-17 11:00:26.000000 gaycore-3.0/gaycore.egg-info/top_level.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        1 2024-05-17 11:00:25.000000 gaycore-3.0/gaycore.egg-info/zip-safe
+-rw-r--r--   0 hyi        (502) staff       (20)       79 2024-05-17 11:00:26.228872 gaycore-3.0/setup.cfg
+-rw-r--r--   0 hyi        (502) staff       (20)     1242 2024-05-17 11:00:10.000000 gaycore-3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `gaycore-2.0.1/LICENSE` & `gaycore-3.0/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2018 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+Copyright (c) 2018 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `gaycore-2.0.1/gaycore/gcore_box.py` & `gaycore-3.0/gaycore/gcore_box.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,352 +1,366 @@
-# Author: Yi Hong
-# Date: 2019.01.29
-import curses
-import threading
-import time
-import webbrowser
-
-from gaycore.config import BOX_HEIGHT, BOX_WIDTH, PAD_HEIGHT, PAD_WIDTH, AUDIO_API
-from gaycore.player import Player
-from gaycore.utils import (
-    get_audio_info,
-    recent_func,
-    chunkstring,
-    likes_func,
-    comments_func,
-    bookmarks_func,
-    make_cate_dict,
-)
-
-try:
-    from urllib.request import urlretrieve
-except:
-    from urllib import urlretrieve
-
-
-MENU_DICT = {
-    "最近电台": recent_func,
-    "分类电台": make_cate_dict(),
-    "最热电台": {"点赞排行": likes_func, "收藏排行": bookmarks_func, "评论排行": comments_func},
-}
-
-
-class GcoreBox:
-    def __init__(self):
-        self.BOX_WIDTH = BOX_WIDTH
-        self.BOX_HEIGHT = BOX_HEIGHT
-
-        self.PAD_WIDTH = PAD_WIDTH
-        self.PAD_HEIGHT = PAD_HEIGHT
-        self.windows = []
-        self.flow_info = {}
-        self.flow_img = ""
-        self.quote = ""
-        self.last_flag = False
-        self.menu_dict = MENU_DICT
-        self.dict_stack = []  # 定义一个stack 方便进入下个目录和返回下个目录
-        self.page_num = -1  # 用于翻页
-        self.player = Player()
-        self._init_curses()
-
-    def _init_curses(self):
-        self.stdscr = curses.initscr()
-        self.stdscr.keypad(1)
-        curses.noecho()
-        curses.cbreak()
-        curses.curs_set(0)
-        curses.start_color()
-        try:
-            curses.init_pair(1, curses.COLOR_BLACK, 197)  # 接近机核主题的颜色
-        except:
-            # 树莓派 windows无法使用机核like色
-            curses.init_pair(1, curses.COLOR_BLACK, curses.COLOR_RED)
-        curses.init_pair(2, curses.COLOR_WHITE, curses.COLOR_BLACK)
-        self.stdscr.bkgd(curses.color_pair(2))
-        self.stdscr.timeout(100)
-        self.stdscr.refresh()
-
-    def make_text_box(self, boxes):
-        self.boxes = boxes
-        self.pad = curses.newpad(self.PAD_WIDTH, self.PAD_HEIGHT)
-
-        self.pad.box()
-        height = 1
-        for num, text in enumerate(boxes, 1):
-            box = self.pad.derwin(
-                self.BOX_HEIGHT,
-                self.BOX_WIDTH,
-                height,
-                self.PAD_WIDTH // 2 - self.BOX_WIDTH // 2,
-            )
-            box.box()
-            if len(text) > 37:
-                text = text[:36] + "..."
-            box.addstr(1, 0, "{}. {}".format(num, text))
-            yield box
-            height += self.BOX_HEIGHT
-        self.max_height = height
-
-    def _center(self, window):
-        cy, cx = window.getbegyx()
-        maxy, maxx = self.stdscr.getmaxyx()
-        self.pad.timeout(-1)
-        self.pad.refresh(cy, cx, 1, maxx // 2 - self.BOX_WIDTH // 2, maxy - 1, maxx - 1)
-        return (cy, cx)
-
-    def _end_curses(self):
-        """ Terminates the curses application. """
-        curses.nocbreak()
-        self.stdscr.keypad(0)
-        curses.echo()
-        curses.endwin()
-
-    def start_to_play(self, url):
-        thread = threading.Thread(target=self.player.run_mpg123, args=(url,))
-        thread.start()
-        time.sleep(0.1)
-        return thread
-
-    def start_to_download(self, mp3_url, audio_name):
-        thread = threading.Thread(target=self._download_mp3, args=(mp3_url, audio_name))
-        thread.start()
-
-    def mainloop(self):
-
-        try:
-            topy, _ = self._center(self.windows[0])
-
-            current_num = 0
-            last = 1
-            top = self.windows[0]
-            while True:
-                # 处理只有一个box的情况
-                if len(self.windows) == 1:
-                    last = 0
-                self.windows[last].bkgd(curses.color_pair(2))
-                self.windows[current_num].bkgd(curses.color_pair(1))
-
-                maxy, _ = self.stdscr.getmaxyx()
-                cy, _ = self.windows[current_num].getbegyx()
-
-                if (topy + maxy - self.BOX_HEIGHT) <= cy:
-                    top = self.windows[current_num]
-
-                if topy >= cy + self.BOX_HEIGHT:
-                    top = self.windows[current_num]
-
-                if last != current_num:
-                    last = current_num
-
-                topy, _ = self._center(top)
-                c = self.stdscr.getch()
-
-                if c == curses.KEY_RESIZE:
-                    self.stdscr.clear()
-
-                if c in [ord("j"), curses.KEY_DOWN]:
-                    current_num = (
-                        current_num + 1 if current_num < len(self.windows) - 1 else 0
-                    )
-
-                if c in [ord("k"), curses.KEY_UP]:
-                    current_num = (
-                        current_num - 1 if current_num > 0 else len(self.windows) - 1
-                    )
-
-                # enter the menu selected
-                if c in [curses.KEY_RIGHT, ord("l")]:
-                    try:
-                        if not callable(self.menu_dict):
-                            self.page_num = -1  # 恢复翻页处理，翻页过多的问题
-                            self.dict_stack.append(self.menu_dict)
-                            self.menu_dict = self.menu_dict.get(self.boxes[current_num])
-                        if isinstance(self.menu_dict, dict):
-                            self.boxes = list(self.menu_dict.keys())
-                        else:
-                            # 利用函数一等对象特性（可能需要重构）
-                            if callable(self.menu_dict):
-                                if self.last_flag:
-                                    break
-                                self.dict_stack.append(self.menu_dict)
-                                self.page_num += 1
-                                self.info_dict = self.menu_dict(self.page_num)
-                                self.boxes = list(self.info_dict.keys())
-                                # 处理翻页到头情况
-                                if len(self.boxes) < 10 and (not self.last_flag):
-                                    self.last_flag = True
-                                    self.last_flag_num = self.page_num
-                            else:
-                                self.boxes = self.menu_dict
-                        break
-                    except:
-                        self.dict_stack.pop()
-
-                # back to last menu
-                if c in [curses.KEY_LEFT, ord("h")]:
-                    try:
-                        # stack pop
-                        last_menu = self.dict_stack.pop()
-                        if callable(last_menu):
-                            # 处理翻页到头情况
-                            if self.last_flag:
-                                self.page_num = self.last_flag_num
-                                self.last_flag = False
-                            self.page_num = self.page_num - 1
-                            if self.page_num >= 0:
-                                self.info_dict = last_menu(self.page_num)
-                                self.boxes = list(self.info_dict.keys())
-                            else:
-                                self.menu_dict = self.dict_stack.pop()
-                                self.boxes = list(self.menu_dict.keys())
-                        else:
-                            self.menu_dict = last_menu
-                            self.boxes = list(last_menu.keys())
-                        break
-                    except:
-                        pass
-                # 退出
-                if c == ord("q"):
-                    self._end_curses()
-                    self.player.q_mp3()
-                    return
-
-                # 打开浏览器查看
-                if c == ord("w"):
-                    try:
-                        info_list = self.info_dict.get(self.boxes[current_num])
-                        gcore_url = info_list[0]
-                        webbrowser.open(gcore_url)
-                    except:
-                        # 查看图片
-                        webbrowser.open(self.flow_img)
-
-                # 打开来源
-                if c == ord("o"):
-                    try:
-                        webbrowser.open(self.quote)
-                    except:
-                        pass
-
-                # 下载
-                if c == ord("d"):
-                    if self.dict_stack and callable(self.dict_stack[-1]):
-                        audio_name = self.boxes[current_num]
-                        audio_id = self.info_dict.get(audio_name)
-                        _, mp3_url = get_audio_info(AUDIO_API, audio_id)
-
-                        # 下载当前MP3
-                        self.start_to_download(mp3_url, audio_name + ".mp3")
-
-                if c == ord("\n"):
-                    try:
-                        if self.player.popen_handler:
-
-                            if current_num == len(self.windows) - 1:
-                                webbrowser.open(self.flow_img)
-                                continue
-                            self.player.q_mp3()
-                            self.windows.pop()
-                        if self.info_dict:
-                            audio_id = self.info_dict.get(self.boxes[current_num])
-                            flow_info, mp3_url = get_audio_info(AUDIO_API, audio_id)
-                            # 播放当前选择的音乐
-                            self.start_to_play(mp3_url)
-                            # 生成播放信息
-                            self.flow_info = flow_info
-                            # 添加播放时间轴
-                            self._add_info_box()
-                    except Exception as e:
-                        pass
-
-                # 暂停或继续播放
-                if c == ord(" "):
-                    self.player.pause_or_resume_mp3()
-
-                # 快进/倒退
-                if c == ord("f"):
-                    self.player.forward_mp3(5)
-
-                # 播放时间轴
-                self._play_timeflow_info()
-
-            self.pick(self.boxes)
-        except:
-            # handle ctrl + c break
-            self._end_curses()
-            self.player.q_mp3()
-            return
-
-    def _play_timeflow_info(self):
-
-        # 播放时间轴
-        if self.player.popen_handler:
-            flow_info = dict(self.flow_info.get(self.player.process_length, ""))
-            self.windows[-1].box()
-            self.windows[-1].addstr(1, 1, "时间轴")
-            play_time_hrs, play_time_min = divmod(self.player.process_location, 3600)
-            play_time_min, play_time_sec = divmod(self.player.process_location, 60)
-
-            self.windows[-1].addstr(
-                3,
-                1,
-                "time:  "
-                + str(play_time_hrs).zfill(2)
-                + ":"
-                + str(play_time_min).zfill(2)
-                + ":"
-                + str(play_time_sec).zfill(2),
-            )
-            if flow_info.get("content"):
-                try:
-                    self.flow_img = flow_info.get("img", "")
-                    self.quote = flow_info.get("quote_href", "")
-                    self.windows[-1].clear()
-                    self.windows[-1].bkgd(curses.color_pair(2))
-                    self.windows[-1].addstr(
-                        4, 1, "title: " + flow_info.get("title", "")
-                    )
-                    self.windows[-1].addstr(5, 1, "content:")
-                    content = flow_info.get("content", "")
-                    # 去掉换行符
-                    content = content.replace("\n", "")
-                    content_length = len(content)
-                    if content_length > 230:
-                        content = content[:230] + "..."
-                    content_list = chunkstring(content, 37)
-                    for i, j in enumerate(content_list):
-                        self.windows[-1].addstr(6 + i, 1, "  " + j)
-                    if self.quote:
-                        self.windows[-1].addstr(13, 1, "打开来源请按o键")
-                except:
-                    pass
-
-    def _add_info_box(self):
-        box = self.pad.derwin(
-            self.BOX_HEIGHT * 5,
-            self.BOX_WIDTH,
-            self.max_height,
-            self.PAD_WIDTH // 2 - self.BOX_WIDTH // 2,
-        )
-        box.box()
-        self.windows.append(box)
-
-    def _download_mp3(self, mp3_url, audio_name):
-
-        # 下载进度
-        def report(count, blockSize, totalSize):
-            percent = int(count * blockSize * 100 / totalSize)
-            self.stdscr.addstr(0, 0, "\r%d%%" % percent + " complete")
-
-        try:
-            urlretrieve(mp3_url, audio_name, reporthook=report)
-            self.stdscr.addstr(0, 0, audio_name + ": 下载完成")
-            time.sleep(1)
-            self.stdscr.clear()
-        except:
-            self.stdscr.addstr(0, 0, "download error")
-
-    def pick(self, boxes):
-        self.windows = list(self.make_text_box(boxes))
-        if self.player.popen_handler:
-            self._add_info_box()
-        self.mainloop()
+# Author: Yi Hong
+# Date: 2019.01.29
+import curses
+import threading
+import time
+import webbrowser
+import subprocess
+
+from gaycore.config import BOX_HEIGHT, BOX_WIDTH, PAD_HEIGHT, PAD_WIDTH, AUDIO_API
+from gaycore.player import Player
+from gaycore.utils import (
+    get_audio_info,
+    recent_func,
+    chunkstring,
+    make_cate_dict,
+    make_playlist_dict,
+)
+
+try:
+    from urllib.request import urlretrieve
+except:
+    from urllib import urlretrieve
+
+
+MENU_DICT = {
+    "最近电台": recent_func,
+    "分类电台": make_cate_dict(),
+    "机核播单": make_playlist_dict(),
+}
+
+
+class GcoreBox:
+    def __init__(self):
+        self.BOX_WIDTH = BOX_WIDTH
+        self.BOX_HEIGHT = BOX_HEIGHT
+
+        self.PAD_WIDTH = PAD_WIDTH
+        self.PAD_HEIGHT = PAD_HEIGHT
+        self.windows = []
+        self.flow_info = {}
+        self.flow_img = ""
+        self.quote = ""
+        self.last_flag = False
+        self.menu_dict = MENU_DICT
+        self.dict_stack = []  # 定义一个 stack 方便进入下个目录和返回下个目录
+        self.page_num = -1  # 用于翻页
+        self.player = Player()
+        self._init_curses()
+
+    def _init_curses(self):
+        self.stdscr = curses.initscr()
+        self.stdscr.keypad(1)
+        curses.noecho()
+        curses.cbreak()
+        curses.curs_set(0)
+        curses.start_color()
+        try:
+            curses.init_pair(1, curses.COLOR_BLACK, 197)  # 接近机核主题的颜色
+        except:
+            # 树莓派 windows无法使用机核like色
+            curses.init_pair(1, curses.COLOR_BLACK, curses.COLOR_RED)
+        curses.init_pair(2, curses.COLOR_WHITE, curses.COLOR_BLACK)
+        self.stdscr.bkgd(curses.color_pair(2))
+        self.stdscr.timeout(100)
+        self.stdscr.refresh()
+
+    def make_text_box(self, boxes):
+        self.boxes = boxes
+        self.pad = curses.newpad(self.PAD_WIDTH, self.PAD_HEIGHT)
+
+        self.pad.box()
+        height = 1
+        for num, text in enumerate(boxes, 1):
+            box = self.pad.derwin(
+                self.BOX_HEIGHT,
+                self.BOX_WIDTH,
+                height,
+                self.PAD_WIDTH // 2 - self.BOX_WIDTH // 2,
+            )
+            box.box()
+            if len(text) > 37:
+                text = text[:36] + "..."
+            box.addstr(1, 0, "{}. {}".format(num, text))
+            yield box
+            height += self.BOX_HEIGHT
+        self.max_height = height
+
+    def _center(self, window):
+        cy, cx = window.getbegyx()
+        maxy, maxx = self.stdscr.getmaxyx()
+        self.pad.timeout(-1)
+        self.pad.refresh(cy, cx, 1, maxx // 2 - self.BOX_WIDTH // 2, maxy - 1, maxx - 1)
+        return (cy, cx)
+
+    def _end_curses(self):
+        """Terminates the curses application."""
+        curses.nocbreak()
+        self.stdscr.keypad(0)
+        curses.echo()
+        curses.endwin()
+
+    def start_to_play(self, url):
+        thread = threading.Thread(target=self.player.run_mpg123, args=(url,))
+        thread.start()
+        time.sleep(0.1)
+        return thread
+
+    def start_to_download(self, mp3_url, audio_name):
+        thread = threading.Thread(target=self._download_mp3, args=(mp3_url, audio_name))
+        thread.start()
+
+    def mainloop(self):
+
+        try:
+            topy, _ = self._center(self.windows[0])
+
+            current_num = 0
+            last = 1
+            top = self.windows[0]
+            while True:
+                # 处理只有一个box的情况
+                if len(self.windows) == 1:
+                    last = 0
+                self.windows[last].bkgd(curses.color_pair(2))
+                self.windows[current_num].bkgd(curses.color_pair(1))
+
+                maxy, _ = self.stdscr.getmaxyx()
+                cy, _ = self.windows[current_num].getbegyx()
+
+                if (topy + maxy - self.BOX_HEIGHT) <= cy:
+                    top = self.windows[current_num]
+
+                if topy >= cy + self.BOX_HEIGHT:
+                    top = self.windows[current_num]
+
+                if last != current_num:
+                    last = current_num
+
+                topy, _ = self._center(top)
+                c = self.stdscr.getch()
+
+                if c == curses.KEY_RESIZE:
+                    self.stdscr.clear()
+
+                if c in [ord("j"), curses.KEY_DOWN]:
+                    current_num = (
+                        current_num + 1 if current_num < len(self.windows) - 1 else 0
+                    )
+
+                if c in [ord("k"), curses.KEY_UP]:
+                    current_num = (
+                        current_num - 1 if current_num > 0 else len(self.windows) - 1
+                    )
+
+                # enter the menu selected
+                if c in [curses.KEY_RIGHT, ord("l")]:
+                    try:
+                        if not callable(self.menu_dict):
+                            self.page_num = -1  # 恢复翻页处理，翻页过多的问题
+                            self.dict_stack.append(self.menu_dict)
+                            self.menu_dict = self.menu_dict.get(self.boxes[current_num])
+                        if isinstance(self.menu_dict, dict):
+                            self.boxes = list(self.menu_dict.keys())
+                        else:
+                            # 利用函数一等对象特性（可能需要重构）
+                            if callable(self.menu_dict):
+                                if self.last_flag:
+                                    break
+                                self.dict_stack.append(self.menu_dict)
+                                self.page_num += 1
+                                self.info_dict = self.menu_dict(self.page_num)
+                                self.boxes = list(self.info_dict.keys())
+                                # 处理翻页到头情况
+                                if len(self.boxes) < 10 and (not self.last_flag):
+                                    self.last_flag = True
+                                    self.last_flag_num = self.page_num
+                            else:
+                                self.boxes = self.menu_dict
+                        break
+                    except:
+                        self.dict_stack.pop()
+
+                # back to last menu
+                if c in [curses.KEY_LEFT, ord("h")]:
+                    try:
+                        # stack pop
+                        last_menu = self.dict_stack.pop()
+                        if callable(last_menu):
+                            # 处理翻页到头情况
+                            if self.last_flag:
+                                self.page_num = self.last_flag_num
+                                self.last_flag = False
+                            self.page_num = self.page_num - 1
+                            if self.page_num >= 0:
+                                self.info_dict = last_menu(self.page_num)
+                                self.boxes = list(self.info_dict.keys())
+                            else:
+                                self.menu_dict = self.dict_stack.pop()
+                                self.boxes = list(self.menu_dict.keys())
+                        else:
+                            self.menu_dict = last_menu
+                            self.boxes = list(last_menu.keys())
+                        break
+                    except:
+                        pass
+                # 退出
+                if c == ord("q"):
+                    self._end_curses()
+                    self.player.q_mp3()
+                    return
+
+                # 打开浏览器查看
+                if c == ord("w"):
+                    try:
+                        info_list = self.info_dict.get(self.boxes[current_num])
+                        gcore_url = info_list[0]
+                        webbrowser.open(gcore_url)
+                    except:
+                        # 查看图片
+                        webbrowser.open(self.flow_img)
+
+                # 打开来源
+                if c == ord("o"):
+                    try:
+                        webbrowser.open(self.quote)
+                    except:
+                        pass
+
+                # 下载
+                if c == ord("d"):
+                    if self.dict_stack and callable(self.dict_stack[-1]):
+                        audio_name = self.boxes[current_num]
+                        audio_id = self.info_dict.get(audio_name)
+                        _, mp3_url = get_audio_info(AUDIO_API, audio_id)
+
+                        # 下载当前MP3
+                        self.start_to_download(mp3_url, audio_name + ".mp3")
+
+                if c == ord("\n"):
+                    try:
+                        if self.player.popen_handler:
+
+                            if current_num == len(self.windows) - 1:
+                                webbrowser.open(self.flow_img)
+                                continue
+                            self.player.q_mp3()
+                            self.windows.pop()
+                        if self.info_dict:
+                            audio_id = self.info_dict.get(self.boxes[current_num])
+                            flow_info, mp3_url = get_audio_info(AUDIO_API, audio_id)
+                            # 播放当前选择的音乐
+                            self.start_to_play(mp3_url)
+                            # 生成播放信息
+                            self.flow_info = flow_info
+                            # 添加播放时间轴
+                            self._add_info_box()
+                    except Exception as e:
+                        pass
+                if c == ord("m"):
+                    try:
+                        audio_id = self.info_dict.get(self.boxes[current_num])
+                        _, mp3_url = get_audio_info(AUDIO_API, audio_id)
+                        # 播放当前选择的音乐
+                        subprocess.check_output(["micli", "play", mp3_url])
+                        self._add_info_box()
+                        self.windows[-1].box()
+                        self.windows[-1].addstr(
+                            1, 1, f"  正在用小爱播放\n  : {self.boxes[current_num]}"
+                        )
+                    except Exception as e:
+                        pass
+                if c == ord("p"):
+                    subprocess.check_output(["micli", "stop"])
+
+                # 暂停或继续播放
+                if c == ord(" "):
+                    self.player.pause_or_resume_mp3()
+
+                # 快进/倒退
+                if c == ord("f"):
+                    self.player.forward_mp3(5)
+
+                # 播放时间轴
+                self._play_timeflow_info()
+
+            self.pick(self.boxes)
+        except:
+            # handle ctrl + c break
+            self._end_curses()
+            self.player.q_mp3()
+            return
+
+    def _play_timeflow_info(self):
+
+        # 播放时间轴
+        if self.player.popen_handler:
+            flow_info = dict(self.flow_info.get(self.player.process_length, ""))
+            self.windows[-1].box()
+            self.windows[-1].addstr(1, 1, "时间轴")
+            play_time_hrs, play_time_min = divmod(self.player.process_location, 3600)
+            play_time_min, play_time_sec = divmod(self.player.process_location, 60)
+
+            self.windows[-1].addstr(
+                3,
+                1,
+                "time:  "
+                + str(play_time_hrs).zfill(2)
+                + ":"
+                + str(play_time_min).zfill(2)
+                + ":"
+                + str(play_time_sec).zfill(2),
+            )
+            if flow_info.get("content"):
+                try:
+                    self.flow_img = flow_info.get("img", "")
+                    self.quote = flow_info.get("quote_href", "")
+                    self.windows[-1].clear()
+                    self.windows[-1].bkgd(curses.color_pair(2))
+                    self.windows[-1].addstr(
+                        4, 1, "title: " + flow_info.get("title", "")
+                    )
+                    self.windows[-1].addstr(5, 1, "content:")
+                    content = flow_info.get("content", "")
+                    # 去掉换行符
+                    content = content.replace("\n", "")
+                    content_length = len(content)
+                    if content_length > 230:
+                        content = content[:230] + "..."
+                    content_list = chunkstring(content, 37)
+                    for i, j in enumerate(content_list):
+                        self.windows[-1].addstr(6 + i, 1, "  " + j)
+                    if self.quote:
+                        self.windows[-1].addstr(13, 1, "打开来源请按o键")
+                except:
+                    pass
+
+    def _add_info_box(self):
+        box = self.pad.derwin(
+            self.BOX_HEIGHT * 5,
+            self.BOX_WIDTH,
+            self.max_height,
+            self.PAD_WIDTH // 2 - self.BOX_WIDTH // 2,
+        )
+        box.box()
+        self.windows.append(box)
+
+    def _download_mp3(self, mp3_url, audio_name):
+
+        # 下载进度
+        def report(count, blockSize, totalSize):
+            percent = int(count * blockSize * 100 / totalSize)
+            self.stdscr.addstr(0, 0, "\r%d%%" % percent + " complete")
+
+        try:
+            urlretrieve(mp3_url, audio_name, reporthook=report)
+            self.stdscr.addstr(0, 0, audio_name + ": 下载完成")
+            time.sleep(1)
+            self.stdscr.clear()
+        except:
+            self.stdscr.addstr(0, 0, "download error")
+
+    def pick(self, boxes):
+        self.windows = list(self.make_text_box(boxes))
+        if self.player.popen_handler:
+            self._add_info_box()
+        self.mainloop()
```

### Comparing `gaycore-2.0.1/gaycore/player.py` & `gaycore-3.0/gaycore/player.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-import subprocess
-
-
-class Player:
-    def __init__(self):
-        self.popen_handler = None
-        self.process_location = 0
-        self.process_length = 0
-        self.fps = 0
-
-    # 参考musicibox代码
-    def run_mpg123(self, url, expires=-1, get_time=-1):
-        para = ["mpg123", "-R"] + []
-        self.popen_handler = subprocess.Popen(
-            para, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.PIPE
-        )
-
-        self.popen_handler.stdin.write(b"L " + url.encode("utf-8") + b"\n")
-        self.popen_handler.stdin.flush()
-
-        endless_loop_cnt = 0
-        # some code from musicbox
-        while True:
-            if not self.popen_handler:
-                break
-
-            strout = self.popen_handler.stdout.readline().decode("utf-8").strip()
-            if strout[:2] == "@F":
-                out = strout.split(" ")
-                self.process_location = int(float(out[3]))
-                self.process_length = int(float(out[3]) + float(out[4]))
-                if float(out[3]) != 0:
-                    self.fps = float(out[1]) / float(out[3])
-
-            elif strout == "@P 0":
-                # end, moving to next
-                playing_flag = True
-                break
-            elif strout == "":
-                endless_loop_cnt += 1
-                if endless_loop_cnt > 100:
-                    break
-
-    # 停止播放
-    def pause_or_resume_mp3(self):
-        if not self.popen_handler:
-            return
-        self.popen_handler.stdin.write(b"P\n")
-        self.popen_handler.stdin.flush()
-
-    # 快进/倒退10s
-    def forward_mp3(self, seconds):
-        if not self.popen_handler:
-            return
-        self.popen_handler.stdin.write(
-            b"J +" + str(seconds * int(self.fps)).encode("utf-8") + b"\n"
-        )
-        self.popen_handler.stdin.flush()
-
-    # 退出播放
-    def q_mp3(self):
-        if self.popen_handler:
-            self.popen_handler.stdin.write(b"Q\n")
-            self.popen_handler.stdin.flush()
-            self.popen_handler.kill()
-            self.popen_handler = None
+import subprocess
+
+
+class Player:
+    def __init__(self):
+        self.popen_handler = None
+        self.process_location = 0
+        self.process_length = 0
+        self.fps = 0
+
+    # 参考musicibox代码
+    def run_mpg123(self, url, expires=-1, get_time=-1):
+        para = ["mpg123", "-R"] + []
+        self.popen_handler = subprocess.Popen(
+            para, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.PIPE
+        )
+
+        self.popen_handler.stdin.write(b"L " + url.encode("utf-8") + b"\n")
+        self.popen_handler.stdin.flush()
+
+        endless_loop_cnt = 0
+        # some code from musicbox
+        while True:
+            if not self.popen_handler:
+                break
+
+            strout = self.popen_handler.stdout.readline().decode("utf-8").strip()
+            if strout[:2] == "@F":
+                out = strout.split(" ")
+                self.process_location = int(float(out[3]))
+                self.process_length = int(float(out[3]) + float(out[4]))
+                if float(out[3]) != 0:
+                    self.fps = float(out[1]) / float(out[3])
+
+            elif strout == "@P 0":
+                # end, moving to next
+                playing_flag = True
+                break
+            elif strout == "":
+                endless_loop_cnt += 1
+                if endless_loop_cnt > 100:
+                    break
+
+    # 停止播放
+    def pause_or_resume_mp3(self):
+        if not self.popen_handler:
+            return
+        self.popen_handler.stdin.write(b"P\n")
+        self.popen_handler.stdin.flush()
+
+    # 快进/倒退10s
+    def forward_mp3(self, seconds):
+        if not self.popen_handler:
+            return
+        self.popen_handler.stdin.write(
+            b"J +" + str(seconds * int(self.fps)).encode("utf-8") + b"\n"
+        )
+        self.popen_handler.stdin.flush()
+
+    # 退出播放
+    def q_mp3(self):
+        if self.popen_handler:
+            self.popen_handler.stdin.write(b"Q\n")
+            self.popen_handler.stdin.flush()
+            self.popen_handler.kill()
+            self.popen_handler = None
```

