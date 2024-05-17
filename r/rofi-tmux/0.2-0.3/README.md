# Comparing `tmp/rofi-tmux-0.2.tar.gz` & `tmp/rofi-tmux-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rofi-tmux-0.2.tar", last modified: Sat May  5 14:20:34 2018, max compression
+gzip compressed data, was "dist/rofi-tmux-0.3.tar", last modified: Wed Mar 18 14:37:24 2020, max compression
```

## Comparing `rofi-tmux-0.2.tar` & `rofi-tmux-0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 arcanjo   (1000) arcanjo   (1000)        0 2018-05-05 14:20:34.000000 rofi-tmux-0.2/
-drwxr-xr-x   0 arcanjo   (1000) arcanjo   (1000)        0 2018-05-05 14:20:34.000000 rofi-tmux-0.2/rofi_tmux.egg-info/
--rw-r--r--   0 arcanjo   (1000) arcanjo   (1000)       12 2018-05-05 14:20:33.000000 rofi-tmux-0.2/rofi_tmux.egg-info/top_level.txt
--rw-r--r--   0 arcanjo   (1000) arcanjo   (1000)        1 2018-01-16 18:05:49.000000 rofi-tmux-0.2/rofi_tmux.egg-info/not-zip-safe
--rw-r--r--   0 arcanjo   (1000) arcanjo   (1000)       39 2018-05-05 14:20:33.000000 rofi-tmux-0.2/rofi_tmux.egg-info/requires.txt
--rw-r--r--   0 arcanjo   (1000) arcanjo   (1000)      352 2018-05-05 14:20:33.000000 rofi-tmux-0.2/rofi_tmux.egg-info/PKG-INFO
--rw-r--r--   0 arcanjo   (1000) arcanjo   (1000)       97 2018-05-05 14:20:33.000000 rofi-tmux-0.2/rofi_tmux.egg-info/entry_points.txt
--rw-r--r--   0 arcanjo   (1000) arcanjo   (1000)        1 2018-05-05 14:20:33.000000 rofi-tmux-0.2/rofi_tmux.egg-info/dependency_links.txt
--rw-r--r--   0 arcanjo   (1000) arcanjo   (1000)      342 2018-05-05 14:20:33.000000 rofi-tmux-0.2/rofi_tmux.egg-info/SOURCES.txt
--rw-r--r--   0 arcanjo   (1000) arcanjo   (1000)      679 2018-05-05 14:11:49.000000 rofi-tmux-0.2/setup.py
--rw-r--r--   0 arcanjo   (1000) arcanjo   (1000)       38 2018-05-05 14:20:34.000000 rofi-tmux-0.2/setup.cfg
--rw-r--r--   0 arcanjo   (1000) arcanjo   (1000)      352 2018-05-05 14:20:34.000000 rofi-tmux-0.2/PKG-INFO
--rw-r--r--   0 arcanjo   (1000) arcanjo   (1000)     1642 2018-01-24 02:00:16.000000 rofi-tmux-0.2/README.md
-drwxr-xr-x   0 arcanjo   (1000) arcanjo   (1000)        0 2018-05-05 14:20:34.000000 rofi-tmux-0.2/rft/
--rw-r--r--   0 arcanjo   (1000) arcanjo   (1000)        0 2018-01-15 11:56:12.000000 rofi-tmux-0.2/rft/__init__.py
--rw-r--r--   0 arcanjo   (1000) arcanjo   (1000)       67 2018-05-05 13:54:14.000000 rofi-tmux-0.2/rft/version.py
--rw-r--r--   0 arcanjo   (1000) arcanjo   (1000)      591 2018-01-24 01:08:40.000000 rofi-tmux-0.2/rft/window_manager.py
--rw-r--r--   0 arcanjo   (1000) arcanjo   (1000)     2244 2018-01-24 01:08:40.000000 rofi-tmux-0.2/rft/i3wm.py
--rwxr-xr-x   0 arcanjo   (1000) arcanjo   (1000)    12274 2018-05-05 14:10:15.000000 rofi-tmux-0.2/rft/rft.py
-drwxr-xr-x   0 arcanjo   (1000) arcanjo   (1000)        0 2018-05-05 14:20:34.000000 rofi-tmux-0.2/rft/bin/
--rwxr-xr-x   0 arcanjo   (1000) arcanjo   (1000)     1944 2018-05-05 14:04:39.000000 rofi-tmux-0.2/rft/bin/main.py
+drwxr-xr-x   0 viniarck  (1000) viniarck  (1000)        0 2020-03-18 14:37:24.511271 rofi-tmux-0.3/
+-rw-r--r--   0 viniarck  (1000) viniarck  (1000)      337 2020-03-18 14:37:24.511271 rofi-tmux-0.3/PKG-INFO
+-rw-r--r--   0 viniarck  (1000) viniarck  (1000)     1737 2020-03-18 14:05:58.000000 rofi-tmux-0.3/README.md
+drwxr-xr-x   0 viniarck  (1000) viniarck  (1000)        0 2020-03-18 14:37:24.507938 rofi-tmux-0.3/rft/
+-rw-r--r--   0 viniarck  (1000) viniarck  (1000)        0 2018-06-16 12:24:36.000000 rofi-tmux-0.3/rft/__init__.py
+drwxr-xr-x   0 viniarck  (1000) viniarck  (1000)        0 2020-03-18 14:37:24.507938 rofi-tmux-0.3/rft/bin/
+-rwxr-xr-x   0 viniarck  (1000) viniarck  (1000)     1944 2018-06-16 12:24:36.000000 rofi-tmux-0.3/rft/bin/main.py
+-rw-r--r--   0 viniarck  (1000) viniarck  (1000)     3896 2020-03-18 14:35:38.000000 rofi-tmux-0.3/rft/i3wm.py
+-rwxr-xr-x   0 viniarck  (1000) viniarck  (1000)    12484 2020-03-18 14:35:38.000000 rofi-tmux-0.3/rft/rft.py
+-rw-r--r--   0 viniarck  (1000) viniarck  (1000)       67 2020-03-18 14:35:38.000000 rofi-tmux-0.3/rft/version.py
+-rw-r--r--   0 viniarck  (1000) viniarck  (1000)      600 2020-03-18 14:15:22.000000 rofi-tmux-0.3/rft/window_manager.py
+drwxr-xr-x   0 viniarck  (1000) viniarck  (1000)        0 2020-03-18 14:37:24.511271 rofi-tmux-0.3/rofi_tmux.egg-info/
+-rw-r--r--   0 viniarck  (1000) viniarck  (1000)      337 2020-03-18 14:37:24.000000 rofi-tmux-0.3/rofi_tmux.egg-info/PKG-INFO
+-rw-r--r--   0 viniarck  (1000) viniarck  (1000)      342 2020-03-18 14:37:24.000000 rofi-tmux-0.3/rofi_tmux.egg-info/SOURCES.txt
+-rw-r--r--   0 viniarck  (1000) viniarck  (1000)        1 2020-03-18 14:37:24.000000 rofi-tmux-0.3/rofi_tmux.egg-info/dependency_links.txt
+-rw-r--r--   0 viniarck  (1000) viniarck  (1000)       97 2020-03-18 14:37:24.000000 rofi-tmux-0.3/rofi_tmux.egg-info/entry_points.txt
+-rw-r--r--   0 viniarck  (1000) viniarck  (1000)        1 2020-03-18 12:56:46.000000 rofi-tmux-0.3/rofi_tmux.egg-info/not-zip-safe
+-rw-r--r--   0 viniarck  (1000) viniarck  (1000)       46 2020-03-18 14:37:24.000000 rofi-tmux-0.3/rofi_tmux.egg-info/requires.txt
+-rw-r--r--   0 viniarck  (1000) viniarck  (1000)       12 2020-03-18 14:37:24.000000 rofi-tmux-0.3/rofi_tmux.egg-info/top_level.txt
+-rw-r--r--   0 viniarck  (1000) viniarck  (1000)       38 2020-03-18 14:37:24.511271 rofi-tmux-0.3/setup.cfg
+-rw-r--r--   0 viniarck  (1000) viniarck  (1000)      671 2020-03-18 14:35:38.000000 rofi-tmux-0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rofi-tmux-0.2/setup.py` & `rofi-tmux-0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 desc = 'Quickly manages tmux sessions, windows and tmuxinator projects on Rofi'
 
 setup(
     name='rofi-tmux',
     version=__version__,
     description=desc,
     author='Vinicius Arcanjo',
-    author_email='viniciusarcanjov@gmail.com',
+    author_email='viniarck@gmail.com',
     keywords='rofi tmux tmuxinator i3 manage switch',
-    url='http://github.com/viniciusarcanjo/rofi-tmux',
+    url='http://github.com/viniarck/rofi-tmux',
     packages=['rft', 'rft/bin'],
     license='MIT',
-    install_requires=['python-rofi==1.0.1', 'libtmux', 'i3ipc', 'click'],
+    install_requires=['python-rofi==1.0.1', 'libtmux', 'i3ipc>=2.0.1', 'click'],
     entry_points='''
         [console_scripts]
         rft=rft.bin.main:main
         rofi-tmux=rft.bin.main:main
     ''',
     zip_safe=False,
 )
```

### Comparing `rofi-tmux-0.2/README.md` & `rofi-tmux-0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+[![Documentation Status](https://readthedocs.org/projects/rofi-tmux/badge/?version=latest)](http://rofi-tmux.readthedocs.io/en/latest/?badge=latest) [![PyPI](https://img.shields.io/pypi/v/rofi-tmux.svg)](https://pypi.python.org/pypi/rofi-tmux)
+
 ## rft (rofi-tmux)
 
 ![rft](docs/images/rft.png)
 
-[![Documentation Status](https://readthedocs.org/projects/rofi-tmux/badge/?version=latest)](http://rofi-tmux.readthedocs.io/en/latest/?badge=latest)
-
 Quickly switches tmux sessions, windows and tmuxinator projects on rofi. Integrates with [i3wm](http://www.i3wm.org) for a smoother switching workflow, if you have multiple workspaces.
 
 ### Use Case
 
 I developed rft (rofi-tmux) to optimize my context-switching workflow. As a user who rely completely on tmux for anything shell related, I wanted to have a fuzzy finder switcher, to locate any tmux session or window with seamless integration with i3wm. I guess I've got spoiled by fuzzy finders. Watch the screencast bellow and you'll see what I mean :)
 
 ### Features
```

### Comparing `rofi-tmux-0.2/rft/rft.py` & `rofi-tmux-0.3/rft/rft.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,52 +15,55 @@
     """Abstraction to interface with rofi, tmux, tmuxinator."""
 
     def __init__(self, debug=False):
         """Initialize ."""
         self._rofi = rofi.Rofi()
         self._libts = libtmux.Server()
         self._sessions = None
-        self._wm = None
         self._cur_tmux_s = None
-        self._cur_i3_s = None
         self.logger = logging.getLogger(__name__)
         if debug:
             self.logger.setLevel(logging.DEBUG)
-        self._cache_f = os.path.join(os.environ.get('HOME'), '.rft.cache')
-        self._cache = {}
-        self._config_f = os.path.join(os.environ.get('HOME'), '.rft')
 
+        homedir = os.environ.get('HOME')
+        self._cache_f = os.path.join(homedir, '.rft.cache')
+        self._cache = self._load_cache()
+        self._config = self._load_config(os.path.join(homedir, '.rft'))
         self._register_cur_sessions()
-        self._load_cache()
-        self._load_config()
+        if self._config.get('wm') == 'i3':
+            self._wm = i3WM(self._config, logger_lvl = self.logger.getEffectiveLevel())
+        else:
+            self._wm = None
 
-    def _load_config(self) -> None:
+    def _load_config(self, conf_file_loc) -> None:
         """Load json config file ~/.rft.
 
         Currently supported window managers: 'i3'
 
         """
-        config = {'wm': ''}
-        try:
-            with open(self._config_f, 'r') as f:
-                config = json.load(f)
-                if config.get('wm') == 'i3':
-                    self._wm = i3WM()
-        except FileNotFoundError as e:
-            pass
-        self.logger.debug('loaded config: {}'.format(config))
+        conf = {
+                'wm': 'i3',
+                'tmux_title_rgx': '{session}',
+                'ignored_sessions': []
+        }
+        conf.update(_read_dict_from_file(conf_file_loc))
+        self.logger.debug('effective config: {}'.format(conf))
+        return conf
+
 
     def _load_cache(self) -> None:
         """Load last tmux sessions and window cache."""
-        try:
-            with open(self._cache_f, 'r') as f:
-                self._cache = json.load(f)
-        except FileNotFoundError as e:
-            self._cache = {'last_tmux_s': None, 'last_tmux_w': None}
-        self.logger.debug('loaded cache: {}'.format(self._cache))
+
+        cache = {
+                'last_tmux_s': None,
+                'last_tmux_w': None
+        }
+        cache.update(_read_dict_from_file(self._cache_f))
+        self.logger.debug('loaded cache: {}'.format(cache))
+        return cache
 
     def _write_cache(self) -> None:
         """Write cache."""
         try:
             with open(self._cache_f, 'w') as f:
                 f.write(
                     json.dumps(
@@ -69,44 +72,47 @@
                         sort_keys=True,
                         separators=(',', ': '),
                         ensure_ascii=False))
             self.logger.debug('wrote cache: {}'.format(self._cache))
         except IOError as e:
             raise e
 
+    def _get_sessions_filtered(self) -> list:
+        """Return list of tmux sessions, sans ones explicitly blacklisted
+        by self._config.ignored_sessions"""
+        return [s for s in self._libts.list_sessions() if s.name not in self._config['ignored_sessions']]
+
     def _register_cur_sessions(self) -> None:
-        """Register the current tmux sessions."""
+        """Register the current tmux sessions _sessions, and
+        store current active session in _cur_tmux_s"""
         try:
-            self._sessions = self._libts.list_sessions()
+            self._sessions = self._get_sessions_filtered()
             self.logger.debug('_sessions: {}'.format(self._sessions))
         except libtmux.exc.LibTmuxException as e:
             # if there are no sessions running load_project takes place
             self.load_tmuxinator()
         self._cur_tmux_s = self._get_cur_session()
-        self.logger.debug('_cur_tmux_s: {}'.format(self._cur_tmux_s))
+        self.logger.debug('_cur_tmux_s: {}'.format(self._cur_tmux_s.name if self._cur_tmux_s else self._cur_tmux_s))
 
-    def _get_cur_session(self) -> str:
-        """Get current tmux session name."""
-        out, err = subprocess.Popen(
-            "tmux list-panes -F '#{session_name}'",
-            shell=True,
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE).communicate()
-        for line in out.splitlines():
-            return line.decode('utf-8').split()[-1]
+    def _get_cur_session(self) -> libtmux.session.Session:
+        """Return reference to our current tmux session."""
+        for s in self._sessions:
+            if str(s.attached) != '0':
+                return s
+        return None
 
-    def _get_cur_window(self) -> str:
+    def _get_cur_tmux_win(self) -> str:
         """Get current tmux window."""
-        if self._cur_tmux_s:
-            for w in self._libts._list_windows():
-                if w.get('session_name') == self._cur_tmux_s:
-                    if w.get('window_active') == '1':
-                        return "{}:{}:{}".format(
-                            w.get('session_name'), w.get('window_index'),
-                            w.get('window_name'))
+        if not self._cur_tmux_s:
+            return None
+        else:
+            return '{}:{}:{}'.format(
+                self._cur_tmux_s.name,
+                self._cur_tmux_s.attached_window.index,
+                self._cur_tmux_s.attached_window.name)
 
     def _get_tmuxinator_projects(self) -> list:
         """Get tmuxinator projects name."""
         out, err = subprocess.Popen(
             "tmuxinator list",
             shell=True,
             stdout=subprocess.PIPE,
@@ -125,14 +131,15 @@
         :session_name: session name
 
         """
         if self._sessions:
             for s in self._sessions:
                 if s.name == session_name:
                     return s
+        return None
 
     def _rofi_tmuxinator(self, rofi_msg, rofi_err) -> None:
         """Launch rofi for loading a tmuxinator project.
 
         :rofi_msg: rofi displayed message
         :err_msg: rofi error message
 
@@ -143,29 +150,28 @@
             if key == 0:
                 out, err = subprocess.Popen(
                     "tmuxinator {}".format(projects[res]),
                     shell=True,
                     stdout=subprocess.PIPE,
                     stderr=subprocess.PIPE).communicate()
                 # update sessions.
-                self._sessions = self._libts.list_sessions()
+                self._sessions = self._get_sessions_filtered()
                 session = self._get_session_by_name(projects[res])
-                workspace = None
+                if not session:
+                    return
                 if self._wm:
-                    workspace = self._wm.is_tmux_not_in_cur_workspace(
-                        self._cur_tmux_s)
-                    if workspace:
-                        self._wm.switch_tmux_workspace(session.name)
+                    self._wm.focus_tmux_window(self._cur_tmux_s)
                 try:
                     session.attach_session()
                 except libtmux.exc.LibTmuxException as e:
                     # there are no attached clients just switch instead.
                     session.switch_client()
-                self._cache['last_tmux_s'] = self._cur_tmux_s
-                self._write_cache()
+                if self._cur_tmux_s:
+                    self._cache['last_tmux_s'] = self._cur_tmux_s.name
+                    self._write_cache()
         else:
             self._rofi.error(rofi_err)
 
     def load_tmuxinator(self) -> None:
         """Load tmuxinator project."""
         self._rofi_tmuxinator(
             rofi_msg='Tmuxinator project',
@@ -176,41 +182,41 @@
 
         :action: 'switch', 'kill'
         :rofi_msg: rofi displayed message
 
         """
         if self._sessions:
             sessions_list = [s.name for s in self._sessions]
-            tmux_wkps = None
+            is_tmux_win_visible = False
             if self._wm:
-                tmux_wkps = self._wm.is_tmux_not_in_cur_workspace(
-                    self._cur_tmux_s)
+                self.logger.debug('resolving is_tmux_win_visible...')
+                is_tmux_win_visible = self._wm.is_tmux_win_visible(self._cur_tmux_s)
+                self.logger.debug('is_tmux_win_visible: {}'.format(is_tmux_win_visible))
             try:
-                # select cur session if it's not int the same workspace
-                if tmux_wkps:
-                    sel = sessions_list.index(self._cur_tmux_s)
-                # otherwise selected the last session
-                else:
+                if is_tmux_win_visible:
                     sel = sessions_list.index(self._cache.get('last_tmux_s'))
+                elif self._cur_tmux_s:
+                    sel = sessions_list.index(self._cur_tmux_s.name)
+                else:
+                    sel = 0
             except ValueError as e:
                 sel = 0
             res, key = self._rofi.select(rofi_msg, sessions_list, select=sel)
             if key == 0:
                 session = self._sessions[res]
                 if action == 'switch':
-                    # if cur tmux session is not in the current workspace
-                    if tmux_wkps:
-                        self._wm.switch_tmux_workspace(session.name)
+                    if self._wm:
+                        self._wm.focus_tmux_window(self._cur_tmux_s)
                     try:
-                        session.attach_session()
-                    except libtmux.exc.LibTmuxException as e:
-                        # there are no attached clients just switch instead.
                         session.switch_client()
-                    self._cache['last_tmux_s'] = self._cur_tmux_s
-                    self._write_cache()
+                    except libtmux.exc.LibTmuxException as e:
+                        session.attach_session()
+                    if self._cur_tmux_s:
+                        self._cache['last_tmux_s'] = self._cur_tmux_s.name
+                        self._write_cache()
                 elif action == 'kill':
                     session.kill_session()
                 else:
                     self._rofi.error('This action is not implemented')
         else:
             self._rofi.error("There are no sessions yet")
 
@@ -230,69 +236,67 @@
         :session_name: if it's not None, the scope is limited to this session
         :global_scope: if True, it will take into account all existent windows
         :rofi_msg: rofi displayed message
 
         """
         windows = None
         if session_name:
-            session = self._get_session_by_name(session_name=session_name)
+            session = self._get_session_by_name(session_name = session_name)
             windows = session.list_windows()
         else:
-            session = self._get_session_by_name(
-                session_name=self._get_cur_session())
+            session = self._cur_tmux_s
             if session:
                 if global_scope:
                     windows = []
                     for s in self._sessions:
                         windows += s.list_windows()
                 else:
                     windows = session.list_windows()
 
         if windows:
             windows_str = [
                 "{}:{}:{}".format(w.session.name, w.index, w.name)
                 for w in windows
             ]
-            tmux_wkps = None
-            cur_win = self._get_cur_window()
+            is_tmux_win_visible = False
+            cur_win = self._get_cur_tmux_win()
             if self._wm:
-                tmux_wkps = self._wm.is_tmux_not_in_cur_workspace(
-                    self._cur_tmux_s)
+                self.logger.debug('resolving is_tmux_win_visible...')
+                is_tmux_win_visible = self._wm.is_tmux_win_visible(self._cur_tmux_s)
+                self.logger.debug('is_tmux_win_visible: {}'.format(is_tmux_win_visible))
             try:
-                # if it's not in the cur workspace
-                if tmux_wkps:
-                    sel = windows_str.index(cur_win)
-                else:
+                if is_tmux_win_visible:
                     sel = windows_str.index(self._cache.get('last_tmux_w'))
+                else:
+                    sel = windows_str.index(cur_win)
             except ValueError as e:
                 sel = 0
+
             res, key = self._rofi.select(rofi_msg, windows_str, select=sel)
             if key == 0:
                 win = windows[res]
                 if action == 'switch':
-                    self.logger.debug('selected: {}:{}:{}'.format(
-                        win.session.name, win.index, win.name))
-                    # only switch if workspace it's not in the same workspace
-                    if tmux_wkps:
-                        self._wm.switch_tmux_workspace(win.session.name)
+                    self.logger.debug('selected: {}'.format(windows_str[res]))
+
+                    if self._wm:
+                        self._wm.focus_tmux_window(self._cur_tmux_s)
                     try:
-                        self.logger.debug('tmux switching: {}'.format(
-                            win.session.name))
+                        self.logger.debug('tmux switching: {}'.format(win.session.name))
                         win.session.switch_client()
                         win.select_window()
                     except libtmux.exc.LibTmuxException as e:
                         # there are no attached clients yet
                         # attach if running in the shell
-                        self.logger.debug('tmux attaching: {}'.format(
-                            win.session.name))
+                        self.logger.debug('tmux attaching: {}'.format(win.session.name))
                         win.session.attach_session()
                     self._cache['last_tmux_w'] = cur_win
-                    # also updates last session accordingly
-                    self._cache['last_tmux_s'] = self._cur_tmux_s
-                    self._write_cache()
+                    # also update last session accordingly:
+                    if self._cur_tmux_s:
+                        self._cache['last_tmux_s'] = self._cur_tmux_s.name
+                        self._write_cache()
                 elif action == 'kill':
                     win.kill_window()
                 else:
                     self._rofi.error('This action is not implemented')
 
     def switch_window(self, session_name=None, global_scope=True) -> None:
         """Switch to a window of a particular session or any session.
@@ -315,7 +319,15 @@
 
         """
         self._rofi_tmux_window(
             action='kill',
             rofi_msg='Kill window',
             session_name=session_name,
             global_scope=global_scope)
+
+def _read_dict_from_file(file_loc):
+    try:
+        with open(file_loc, 'r') as f:
+            return json.load(f)
+    except Exception as e:
+        return {}
+
```

### Comparing `rofi-tmux-0.2/rft/bin/main.py` & `rofi-tmux-0.3/rft/bin/main.py`

 * *Files identical despite different names*

