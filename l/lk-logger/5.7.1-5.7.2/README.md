# Comparing `tmp/lk_logger-5.7.1-py3-none-any.whl.zip` & `tmp/lk_logger-5.7.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,30 +1,30 @@
-Zip file size: 42425 bytes, number of entries: 28
+Zip file size: 44917 bytes, number of entries: 28
 -rw-r--r--  2.0 fat      955 b- defN 80-Jan-01 00:00 lk_logger/__init__.py
 -rw-r--r--  2.0 fat       34 b- defN 80-Jan-01 00:00 lk_logger/cache/__init__.py
 -rw-r--r--  2.0 fat     6970 b- defN 80-Jan-01 00:00 lk_logger/cache/cache.py
 -rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 lk_logger/cache/frame.py
 -rw-r--r--  2.0 fat     1875 b- defN 80-Jan-01 00:00 lk_logger/cache/legacy.py
 -rw-r--r--  2.0 fat      762 b- defN 80-Jan-01 00:00 lk_logger/cache/util.py
--rw-r--r--  2.0 fat     5815 b- defN 80-Jan-01 00:00 lk_logger/config.py
--rw-r--r--  2.0 fat     1267 b- defN 80-Jan-01 00:00 lk_logger/console.py
--rw-r--r--  2.0 fat     4988 b- defN 80-Jan-01 00:00 lk_logger/control.py
--rw-r--r--  2.0 fat     8992 b- defN 80-Jan-01 00:00 lk_logger/frame_info.py
--rw-r--r--  2.0 fat    13871 b- defN 80-Jan-01 00:00 lk_logger/logger.py
--rw-r--r--  2.0 fat    10376 b- defN 80-Jan-01 00:00 lk_logger/markup.py
--rw-r--r--  2.0 fat    11434 b- defN 80-Jan-01 00:00 lk_logger/message_builder.py
--rw-r--r--  2.0 fat    11258 b- defN 80-Jan-01 00:00 lk_logger/message_formatter.py
+-rw-r--r--  2.0 fat     5668 b- defN 80-Jan-01 00:00 lk_logger/config.py
+-rw-r--r--  2.0 fat     1230 b- defN 80-Jan-01 00:00 lk_logger/console.py
+-rw-r--r--  2.0 fat     4815 b- defN 80-Jan-01 00:00 lk_logger/control.py
+-rw-r--r--  2.0 fat     8737 b- defN 80-Jan-01 00:00 lk_logger/frame_info.py
+-rw-r--r--  2.0 fat    14614 b- defN 80-Jan-01 00:00 lk_logger/logger.py
+-rw-r--r--  2.0 fat    10730 b- defN 80-Jan-01 00:00 lk_logger/markup.py
+-rw-r--r--  2.0 fat    11636 b- defN 80-Jan-01 00:00 lk_logger/message_builder.py
+-rw-r--r--  2.0 fat    13323 b- defN 80-Jan-01 00:00 lk_logger/message_formatter.py
 -rw-r--r--  2.0 fat     4034 b- defN 80-Jan-01 00:00 lk_logger/path_helper.py
--rw-r--r--  2.0 fat     2543 b- defN 80-Jan-01 00:00 lk_logger/pipeline.py
--rw-r--r--  2.0 fat     2690 b- defN 80-Jan-01 00:00 lk_logger/printer.py
+-rw-r--r--  2.0 fat     2453 b- defN 80-Jan-01 00:00 lk_logger/pipeline.py
+-rw-r--r--  2.0 fat     2590 b- defN 80-Jan-01 00:00 lk_logger/printer.py
 -rw-r--r--  2.0 fat       73 b- defN 80-Jan-01 00:00 lk_logger/scanner/__init__.py
 -rw-r--r--  2.0 fat     6407 b- defN 80-Jan-01 00:00 lk_logger/scanner/analyser.py
 -rw-r--r--  2.0 fat     1164 b- defN 80-Jan-01 00:00 lk_logger/scanner/const.py
 -rw-r--r--  2.0 fat     1780 b- defN 80-Jan-01 00:00 lk_logger/scanner/exceptions.py
 -rw-r--r--  2.0 fat     9728 b- defN 80-Jan-01 00:00 lk_logger/scanner/scanner.py
 -rw-r--r--  2.0 fat     3306 b- defN 80-Jan-01 00:00 lk_logger/scanner/symbols.py
 -rw-r--r--  2.0 fat    19638 b- defN 80-Jan-01 00:00 lk_logger/scanner/text_scanner.py
 -rw-r--r--  2.0 fat      517 b- defN 80-Jan-01 00:00 lk_logger/scanner/typehint.py
--rw-r--r--  2.0 fat     4952 b- defN 80-Jan-01 00:00 lk_logger-5.7.1.dist-info/METADATA
--rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 lk_logger-5.7.1.dist-info/WHEEL
-?rw-r--r--  2.0 fat     2252 b- defN 16-Jan-01 00:00 lk_logger-5.7.1.dist-info/RECORD
-28 files, 137769 bytes uncompressed, 38841 bytes compressed:  71.8%
+-rw-r--r--  2.0 fat    10805 b- defN 80-Jan-01 00:00 lk_logger-5.7.2.dist-info/METADATA
+-rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 lk_logger-5.7.2.dist-info/WHEEL
+?rw-r--r--  2.0 fat     2253 b- defN 16-Jan-01 00:00 lk_logger-5.7.2.dist-info/RECORD
+28 files, 146185 bytes uncompressed, 41333 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -69,17 +69,17 @@
 
 Filename: lk_logger/scanner/text_scanner.py
 Comment: 
 
 Filename: lk_logger/scanner/typehint.py
 Comment: 
 
-Filename: lk_logger-5.7.1.dist-info/METADATA
+Filename: lk_logger-5.7.2.dist-info/METADATA
 Comment: 
 
-Filename: lk_logger-5.7.1.dist-info/WHEEL
+Filename: lk_logger-5.7.2.dist-info/WHEEL
 Comment: 
 
-Filename: lk_logger-5.7.1.dist-info/RECORD
+Filename: lk_logger-5.7.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lk_logger/__init__.py

```diff
@@ -30,8 +30,8 @@
     else:
         import IPython
         pipeline.add(IPython, bprint, scope=True)
         # pipeline.add('[ipython]', bprint)
 
 
 __init()
-__version__ = '5.7.1'
+__version__ = '5.7.2'
```

## lk_logger/config.py

 * *Ordering differences only*

```diff
@@ -1,147 +1,147 @@
-import sys
-import typing as t
-from sys import excepthook as _default_excepthook
-
-
-class LoggingConfig:
-    """
-    options:
-        show_source: bool[true]
-            add source info (filepath and line number) prefix to log messages.
-            example:
-                logger.log('hello world')
-                # enabled : './main.py:10  >>  hello world'
-                # disabled: 'hello world'
-        show_varnames: bool[false]
-            show both var names and values. (magic reflection)
-            example:
-                a, b = 1, 2
-                logger.log(a, b, a + b)
-                # enabled : 'main.py:11  >>  a = 1; b = 2; a + b = 3'
-                # disabled: 'main.py:11  >>  1, 2, 3'
-        show_external_lib: bool[true]
-            if `param source` came from an external library, whether to print.
-            for example, if a third-party library 'xxx' also used `logger.log`,
-            its source path (relative to current working dir) may be very long,
-            if you don't want to see any prints except your own project, you'd
-            set this to False.
-
-        # the following options are only available if `show_external_lib` is
-        # true.
-        path_style_for_external_lib: literal
-            literal:
-                'pretty_relpath': default
-                    trunscate the source path of external lib to be shorter.
-                    example:
-                        before:
-                            '../../../../site-packages/lk_logger/sourcemap.py'
-                            # there may be a lot of '../'.
-                        after:
-                            '[lk_logger]/sourcemap.py'
-                'relpath':
-                    a relative path to current working dir. (<- `os.getcwd()`)
-                    note there may be a lot of '../../../...' if external lib
-                    is far beyond the current working dir.
-                'lib_name_only':
-                    show only the library name (surrounded by brackets).
-                    example: '[lk_logger]'
-            ps: if you don't want to show anything, you should turn to set
-            `show_external_lib` to False.
-    """
-    async_: bool
-    clear_unfinished_stream: bool
-    console_width: t.Optional[int]
-    path_style_for_external_lib: str
-    rich_traceback: bool
-    separator: str
-    show_external_lib: bool
-    show_funcname: bool
-    show_source: bool
-    show_varnames: bool
-    sourcemap_alignment: t.Literal['left', 'right']
-    v2_meaning: t.Literal['info', 'success']  # TODO: not used.
-    
-    _preset_conf = {
-        'async_'                     : False,  # TODO
-        'clear_unfinished_stream'    : False,
-        'console_width'              : None,
-        'path_style_for_external_lib': 'pretty_relpath',
-        'rich_traceback'             : True,
-        'separator'                  : ';   ',
-        'show_external_lib'          : True,
-        'show_funcname'              : True,
-        'show_source'                : True,
-        'show_varnames'              : False,
-        'sourcemap_alignment'        : 'left',
-        'v2_meaning'                 : 'info',
-    }
-    
-    def __init__(self, **kwargs) -> None:
-        for k, v in self._merge_dict(self._preset_conf, kwargs).items():
-            self._apply(k, v)
-    
-    def update(self, **kwargs) -> None:
-        for k, v in kwargs.items():
-            if k in self._preset_conf and v != getattr(self, k, None):
-                self._apply(k, v)
-    
-    def reset(self) -> None:
-        for k, v in self._preset_conf.items():
-            if v != getattr(self, k, None):
-                self._apply(k, v)
-    
-    def _apply(self, key: str, val: t.Union[bool, int, str]) -> None:
-        setattr(self, key, val)
-        if key == 'console_width':
-            if val and isinstance(val, int):
-                from .console import console
-                console.width = val
-        elif key == 'rich_traceback':
-            import sys
-            from functools import partial
-            if val:
-                # https://rich.readthedocs.io/en/stable/traceback.html
-                from rich.traceback import install
-                from .console import console
-                install(console=console, show_locals=False)
-                modified = sys.excepthook
-                sys.excepthook = partial(
-                    self._wrap_system_excepthook,
-                    callback=modified
-                )
-            else:
-                sys.excepthook = self._wrap_system_excepthook
-    
-    @staticmethod
-    def _wrap_system_excepthook(
-        type_, value, traceback, callback=_default_excepthook
-    ) -> None:
-        # print(':r', '[red dim]drain out message queue[/]')
-        # from .logger import logger
-        # if hasattr(logger, '_stop_running'):
-        #     logger._stop_running()  # noqa
-        if type_ is KeyboardInterrupt:
-            print(':r', '[red dim]KeyboardInterrupt[/]')
-            sys.exit(0)
-        else:
-            callback(type_, value, traceback)
-    
-    # -------------------------------------------------------------------------
-    
-    def to_dict(self) -> t.Dict[str, t.Any]:
-        return {
-            k: getattr(self, k)
-            for k in self._preset_conf
-        }
-    
-    @staticmethod
-    def _merge_dict(base: dict, update: dict) -> dict:
-        return {k: update.get(k, default_v) for k, default_v in base.items()}
-    
-    @staticmethod
-    def _diff_dict(base: dict, update: dict) -> dict:
-        out = {}
-        for k, v0 in base.items():
-            if k in update and v0 != (v1 := update[k]):
-                out[k] = v1
-        return out
+import sys
+import typing as t
+from sys import excepthook as _default_excepthook
+
+
+class LoggingConfig:
+    """
+    options:
+        show_source: bool[true]
+            add source info (filepath and line number) prefix to log messages.
+            example:
+                logger.log('hello world')
+                # enabled : './main.py:10  >>  hello world'
+                # disabled: 'hello world'
+        show_varnames: bool[false]
+            show both var names and values. (magic reflection)
+            example:
+                a, b = 1, 2
+                logger.log(a, b, a + b)
+                # enabled : 'main.py:11  >>  a = 1; b = 2; a + b = 3'
+                # disabled: 'main.py:11  >>  1, 2, 3'
+        show_external_lib: bool[true]
+            if `param source` came from an external library, whether to print.
+            for example, if a third-party library 'xxx' also used `logger.log`,
+            its source path (relative to current working dir) may be very long,
+            if you don't want to see any prints except your own project, you'd
+            set this to False.
+
+        # the following options are only available if `show_external_lib` is
+        # true.
+        path_style_for_external_lib: literal
+            literal:
+                'pretty_relpath': default
+                    trunscate the source path of external lib to be shorter.
+                    example:
+                        before:
+                            '../../../../site-packages/lk_logger/sourcemap.py'
+                            # there may be a lot of '../'.
+                        after:
+                            '[lk_logger]/sourcemap.py'
+                'relpath':
+                    a relative path to current working dir. (<- `os.getcwd()`)
+                    note there may be a lot of '../../../...' if external lib
+                    is far beyond the current working dir.
+                'lib_name_only':
+                    show only the library name (surrounded by brackets).
+                    example: '[lk_logger]'
+            ps: if you don't want to show anything, you should turn to set
+            `show_external_lib` to False.
+    """
+    async_: bool
+    clear_unfinished_stream: bool
+    console_width: t.Optional[int]
+    path_style_for_external_lib: str
+    rich_traceback: bool
+    separator: str
+    show_external_lib: bool
+    show_funcname: bool
+    show_source: bool
+    show_varnames: bool
+    sourcemap_alignment: t.Literal['left', 'right']
+    v2_meaning: t.Literal['info', 'success']  # TODO: not used.
+    
+    _preset_conf = {
+        'async_'                     : False,  # TODO
+        'clear_unfinished_stream'    : False,
+        'console_width'              : None,
+        'path_style_for_external_lib': 'pretty_relpath',
+        'rich_traceback'             : True,
+        'separator'                  : ';   ',
+        'show_external_lib'          : True,
+        'show_funcname'              : True,
+        'show_source'                : True,
+        'show_varnames'              : False,
+        'sourcemap_alignment'        : 'left',
+        'v2_meaning'                 : 'info',
+    }
+    
+    def __init__(self, **kwargs) -> None:
+        for k, v in self._merge_dict(self._preset_conf, kwargs).items():
+            self._apply(k, v)
+    
+    def update(self, **kwargs) -> None:
+        for k, v in kwargs.items():
+            if k in self._preset_conf and v != getattr(self, k, None):
+                self._apply(k, v)
+    
+    def reset(self) -> None:
+        for k, v in self._preset_conf.items():
+            if v != getattr(self, k, None):
+                self._apply(k, v)
+    
+    def _apply(self, key: str, val: t.Union[bool, int, str]) -> None:
+        setattr(self, key, val)
+        if key == 'console_width':
+            if val and isinstance(val, int):
+                from .console import console
+                console.width = val
+        elif key == 'rich_traceback':
+            import sys
+            from functools import partial
+            if val:
+                # https://rich.readthedocs.io/en/stable/traceback.html
+                from rich.traceback import install
+                from .console import console
+                install(console=console, show_locals=False)
+                modified = sys.excepthook
+                sys.excepthook = partial(
+                    self._wrap_system_excepthook,
+                    callback=modified
+                )
+            else:
+                sys.excepthook = self._wrap_system_excepthook
+    
+    @staticmethod
+    def _wrap_system_excepthook(
+        type_, value, traceback, callback=_default_excepthook
+    ) -> None:
+        # print(':r', '[red dim]drain out message queue[/]')
+        # from .logger import logger
+        # if hasattr(logger, '_stop_running'):
+        #     logger._stop_running()  # noqa
+        if type_ is KeyboardInterrupt:
+            print(':r', '[red dim]KeyboardInterrupt[/]')
+            sys.exit(0)
+        else:
+            callback(type_, value, traceback)
+    
+    # -------------------------------------------------------------------------
+    
+    def to_dict(self) -> t.Dict[str, t.Any]:
+        return {
+            k: getattr(self, k)
+            for k in self._preset_conf
+        }
+    
+    @staticmethod
+    def _merge_dict(base: dict, update: dict) -> dict:
+        return {k: update.get(k, default_v) for k, default_v in base.items()}
+    
+    @staticmethod
+    def _diff_dict(base: dict, update: dict) -> dict:
+        out = {}
+        for k, v0 in base.items():
+            if k in update and v0 != (v1 := update[k]):
+                out[k] = v1
+        return out
```

## lk_logger/console.py

 * *Ordering differences only*

```diff
@@ -1,37 +1,37 @@
-from typing import Any
-
-from rich.console import Console as BaseConsole
-
-
-class Console(BaseConsole):
-    
-    def __init__(self) -> None:
-        super().__init__()
-        if self._color_system is None:
-            try:
-                # in rich version >= 12.5, the color system is changed to be a
-                # contant integer.
-                from rich.console import ColorSystem
-                self._color_system = ColorSystem.STANDARD
-            except:
-                # the older version is using a string.
-                self._color_system = 'standard'
-        
-        # TODO (width):
-        #   if width longer than default, use single line style; otherwise
-        #   split sourcemap and message into different lines.
-        pass
-    
-    def print(self, *objects: Any, soft_wrap: bool = True, **kwargs) -> None:
-        from .message_builder import MessageStruct
-        if len(objects) == 1 and isinstance(objects[0], MessageStruct):
-            super().print(
-                objects[0].text, overflow='fold', soft_wrap=soft_wrap, **kwargs
-            )
-        else:
-            super().print(
-                *objects, overflow='fold', soft_wrap=soft_wrap, **kwargs
-            )
-
-
-console = Console()
+from typing import Any
+
+from rich.console import Console as BaseConsole
+
+
+class Console(BaseConsole):
+    
+    def __init__(self) -> None:
+        super().__init__()
+        if self._color_system is None:
+            try:
+                # in rich version >= 12.5, the color system is changed to be a
+                # contant integer.
+                from rich.console import ColorSystem
+                self._color_system = ColorSystem.STANDARD
+            except:
+                # the older version is using a string.
+                self._color_system = 'standard'
+        
+        # TODO (width):
+        #   if width longer than default, use single line style; otherwise
+        #   split sourcemap and message into different lines.
+        pass
+    
+    def print(self, *objects: Any, soft_wrap: bool = True, **kwargs) -> None:
+        from .message_builder import MessageStruct
+        if len(objects) == 1 and isinstance(objects[0], MessageStruct):
+            super().print(
+                objects[0].text, overflow='fold', soft_wrap=soft_wrap, **kwargs
+            )
+        else:
+            super().print(
+                *objects, overflow='fold', soft_wrap=soft_wrap, **kwargs
+            )
+
+
+console = Console()
```

## lk_logger/control.py

 * *Ordering differences only*

```diff
@@ -1,173 +1,173 @@
-import builtins
-import typing as t
-
-from .logger import logger
-from .printer import bprint
-
-STATUS = 'unloaded'  # literal['enabled', 'disabled', 'unloaded']
-_HAS_WELCOME_MESSAGE_SHOWN = False
-
-
-def setup(
-    *,
-    quiet: bool = False,
-    clear_preset: bool = False,
-    _stdout: t.Callable = None,  # TODO: experimental
-    **kwargs
-) -> None:
-    """
-    args:
-        quiet:
-            True: show a welcome message in caller side.
-            False: do not show.
-
-            note: the welcome message is shown only once, if caller calls this
-                function multi times, only the first time when passes
-                `quiet=True` will show this message.
-            tip: if you are developing an intermediate/supporting library, it
-                is recommended to set `quiet=True`.
-        clear_preset:
-        kwargs: see `./logger.py > LoggingConfig`.
-    """
-    global _HAS_WELCOME_MESSAGE_SHOWN, STATUS
-    
-    logger.configure(clear_preset, **kwargs)
-    setattr(builtins, 'print', _stdout or logger.log)
-    
-    if not quiet and not _HAS_WELCOME_MESSAGE_SHOWN:
-        _HAS_WELCOME_MESSAGE_SHOWN = True
-        
-        from .markup import _Counter
-        random_color = _Counter._get_random_bright_color  # noqa
-        color_pair = (random_color(), random_color())
-        slogan = _blend_text('lk-logger is ready', color_pair)
-
-        # from random import choice
-        # color_pairs_group = (
-        #     ('#0a87ee', '#9294f0'),  # calm blue -> light blue
-        #     ('#2d34f1', '#9294f0'),  # ocean blue -> light blue
-        #     ('#ed3b3b', '#d08bf3'),  # rose red -> violet
-        #     ('#f38cfd', '#d08bf3'),  # light magenta -> violet
-        #     ('#f47fa4', '#f49364'),  # cold sandy -> camel tan
-        # )
-        # color_pair = choice(color_pairs_group)
-        # slogan = _blend_text('lk-logger is ready', color_pair)
-        
-        # dprint(slogan)
-        print(slogan, ':rsp')
-    
-    STATUS = 'enabled'
-
-
-def update(clear_preset=False, **kwargs) -> None:
-    logger.configure(clear_preset, **kwargs)
-
-
-def unload() -> None:
-    setattr(builtins, 'print', bprint)
-    global STATUS
-    STATUS = 'unloaded'
-
-
-def enable() -> None:
-    setattr(builtins, 'print', logger.log)
-    global STATUS
-    STATUS = 'enabled'
-
-
-def disable() -> None:
-    setattr(builtins, 'print', lambda *_, **__: None)
-    global STATUS
-    STATUS = 'disabled'
-
-
-# aliases
-mute = disable
-unmute = enable
-reload = enable
-
-
-# -----------------------------------------------------------------------------
-# other
-
-def start_ipython(
-        user_ns: t.Dict[str, t.Any] = None
-) -> None:
-    if _is_ipython_mode():
-        return
-    try:
-        import IPython  # noqa
-    except (ImportError, ModuleNotFoundError) as e:
-        print('ipython is not installed!', ':pv4')
-        raise e
-    else:
-        import sys
-        from IPython.core.getipython import get_ipython  # noqa
-        from IPython.terminal.ipapp import TerminalIPythonApp  # noqa
-        from rich.traceback import install
-        from .console import console
-        from .pipeline import pipeline
-    
-    pipeline.add(IPython, bprint, scope=True)
-    
-    backups = {
-        'lklogger_config': logger.config.copy(),
-        'sys.argv'       : sys.argv.copy(),
-    }
-    
-    setup(quiet=True, clear_preset=True,
-          show_source=False, show_funcname=False, show_varnames=False)
-    sys.argv = ['']  # avoid ipython to parse `sys.argv`.
-    
-    app = TerminalIPythonApp.instance(
-        user_ns={'print': logger.log, **(user_ns or {})}
-    )
-    app.initialize()
-    
-    # setup except hook for ipython
-    setattr(builtins, 'get_ipython', get_ipython)
-    install(console=console)
-    
-    app.start()
-    
-    # afterwards
-    logger.configure(**backups['lklogger_config'])
-    sys.argv = backups['sys.argv']
-    del backups
-
-
-# -----------------------------------------------------------------------------
-# neutral functions
-
-# DELETE
-def _blend_text(message: str, color_pair: t.Tuple[str, str]) -> str:
-    """ blend text from one color to another.
-    
-    source: [lib:rich_cli/__main__.py : blend_text()]
-    """
-    from rich.color import Color
-    from rich.text import Text
-    
-    color1, color2 = (Color.parse(x).triplet for x in color_pair)
-    r1, g1, b1 = color1
-    r2, g2, b2 = color2
-    dr = r2 - r1
-    dg = g2 - g1
-    db = b2 - b1
-    
-    text = Text(message)
-    size = len(text)
-    
-    for index in range(size):
-        blend = index / size
-        color = '#{}{}{}'.format(
-            f'{int(r1 + dr * blend):02X}',
-            f'{int(g1 + dg * blend):02X}',
-            f'{int(b1 + db * blend):02X}'
-        )
-        text.stylize(color, index, index + 1)
-    return text.markup
-
-
-def _is_ipython_mode() -> bool:
-    return getattr(builtins, '__IPYTHON__', False)
+import builtins
+import typing as t
+
+from .logger import logger
+from .printer import bprint
+
+STATUS = 'unloaded'  # literal['enabled', 'disabled', 'unloaded']
+_HAS_WELCOME_MESSAGE_SHOWN = False
+
+
+def setup(
+    *,
+    quiet: bool = False,
+    clear_preset: bool = False,
+    _stdout: t.Callable = None,  # TODO: experimental
+    **kwargs
+) -> None:
+    """
+    args:
+        quiet:
+            True: show a welcome message in caller side.
+            False: do not show.
+
+            note: the welcome message is shown only once, if caller calls this
+                function multi times, only the first time when passes
+                `quiet=True` will show this message.
+            tip: if you are developing an intermediate/supporting library, it
+                is recommended to set `quiet=True`.
+        clear_preset:
+        kwargs: see `./logger.py > LoggingConfig`.
+    """
+    global _HAS_WELCOME_MESSAGE_SHOWN, STATUS
+    
+    logger.configure(clear_preset, **kwargs)
+    setattr(builtins, 'print', _stdout or logger.log)
+    
+    if not quiet and not _HAS_WELCOME_MESSAGE_SHOWN:
+        _HAS_WELCOME_MESSAGE_SHOWN = True
+        
+        from .markup import _Counter
+        random_color = _Counter._get_random_bright_color  # noqa
+        color_pair = (random_color(), random_color())
+        slogan = _blend_text('lk-logger is ready', color_pair)
+
+        # from random import choice
+        # color_pairs_group = (
+        #     ('#0a87ee', '#9294f0'),  # calm blue -> light blue
+        #     ('#2d34f1', '#9294f0'),  # ocean blue -> light blue
+        #     ('#ed3b3b', '#d08bf3'),  # rose red -> violet
+        #     ('#f38cfd', '#d08bf3'),  # light magenta -> violet
+        #     ('#f47fa4', '#f49364'),  # cold sandy -> camel tan
+        # )
+        # color_pair = choice(color_pairs_group)
+        # slogan = _blend_text('lk-logger is ready', color_pair)
+        
+        # dprint(slogan)
+        print(slogan, ':rsp')
+    
+    STATUS = 'enabled'
+
+
+def update(clear_preset=False, **kwargs) -> None:
+    logger.configure(clear_preset, **kwargs)
+
+
+def unload() -> None:
+    setattr(builtins, 'print', bprint)
+    global STATUS
+    STATUS = 'unloaded'
+
+
+def enable() -> None:
+    setattr(builtins, 'print', logger.log)
+    global STATUS
+    STATUS = 'enabled'
+
+
+def disable() -> None:
+    setattr(builtins, 'print', lambda *_, **__: None)
+    global STATUS
+    STATUS = 'disabled'
+
+
+# aliases
+mute = disable
+unmute = enable
+reload = enable
+
+
+# -----------------------------------------------------------------------------
+# other
+
+def start_ipython(
+        user_ns: t.Dict[str, t.Any] = None
+) -> None:
+    if _is_ipython_mode():
+        return
+    try:
+        import IPython  # noqa
+    except (ImportError, ModuleNotFoundError) as e:
+        print('ipython is not installed!', ':pv4')
+        raise e
+    else:
+        import sys
+        from IPython.core.getipython import get_ipython  # noqa
+        from IPython.terminal.ipapp import TerminalIPythonApp  # noqa
+        from rich.traceback import install
+        from .console import console
+        from .pipeline import pipeline
+    
+    pipeline.add(IPython, bprint, scope=True)
+    
+    backups = {
+        'lklogger_config': logger.config.copy(),
+        'sys.argv'       : sys.argv.copy(),
+    }
+    
+    setup(quiet=True, clear_preset=True,
+          show_source=False, show_funcname=False, show_varnames=False)
+    sys.argv = ['']  # avoid ipython to parse `sys.argv`.
+    
+    app = TerminalIPythonApp.instance(
+        user_ns={'print': logger.log, **(user_ns or {})}
+    )
+    app.initialize()
+    
+    # setup except hook for ipython
+    setattr(builtins, 'get_ipython', get_ipython)
+    install(console=console)
+    
+    app.start()
+    
+    # afterwards
+    logger.configure(**backups['lklogger_config'])
+    sys.argv = backups['sys.argv']
+    del backups
+
+
+# -----------------------------------------------------------------------------
+# neutral functions
+
+# DELETE
+def _blend_text(message: str, color_pair: t.Tuple[str, str]) -> str:
+    """ blend text from one color to another.
+    
+    source: [lib:rich_cli/__main__.py : blend_text()]
+    """
+    from rich.color import Color
+    from rich.text import Text
+    
+    color1, color2 = (Color.parse(x).triplet for x in color_pair)
+    r1, g1, b1 = color1
+    r2, g2, b2 = color2
+    dr = r2 - r1
+    dg = g2 - g1
+    db = b2 - b1
+    
+    text = Text(message)
+    size = len(text)
+    
+    for index in range(size):
+        blend = index / size
+        color = '#{}{}{}'.format(
+            f'{int(r1 + dr * blend):02X}',
+            f'{int(g1 + dg * blend):02X}',
+            f'{int(b1 + db * blend):02X}'
+        )
+        text.stylize(color, index, index + 1)
+    return text.markup
+
+
+def _is_ipython_mode() -> bool:
+    return getattr(builtins, '__IPYTHON__', False)
```

## lk_logger/frame_info.py

 * *Ordering differences only*

```diff
@@ -1,255 +1,255 @@
-import inspect
-import re
-import typing as t
-from dataclasses import dataclass
-from os.path import abspath
-from os.path import exists
-from textwrap import dedent
-from types import FrameType
-
-from .scanner import get_all_blocks
-from .scanner import get_variables
-from .scanner.const import SUBSCRIPTABLE
-from .scanner.const import VARIABLE_NAME
-from .scanner.exceptions import ScanningError
-from .scanner.exceptions import UnresolvedCase
-
-
-class T:
-    VarNames = t.Tuple[str, ...]
-    SourceMap = t.Dict[str, t.Dict[int, VarNames]]
-
-
-class SourceMap:
-    _sourcemap: T.SourceMap
-    
-    def __init__(self):
-        self._sourcemap = {}
-    
-    def get_varnames(self, filepath: str, lineno: int) -> T.VarNames:
-        if filepath not in self._sourcemap:
-            self._indexing_filemap(filepath)
-        return self._sourcemap[filepath].get(lineno, ())
-    
-    def _indexing_filemap(self, filepath: str) -> None:
-        if filepath.startswith('<') or filepath.endswith('>') \
-                or not exists(filepath):
-            # see `FrameInfo > property filepath > docstring notice`
-            self._sourcemap.setdefault(filepath, {})
-            return
-        
-        def get_blocks(lines: t.Iterator[str]) -> t.Dict[int, T.VarNames]:
-            out = {}
-            for match in get_all_blocks(*lines):
-                text = match.fulltext.strip()
-                if not text:
-                    continue
-                if not text.startswith('print'):  # FIXME: this is not stable
-                    continue
-                try:
-                    varnames = _analyse_block(text)
-                    lineno = match.cursor.lineno + 1
-                    out[lineno] = tuple(varnames)
-                except ScanningError:
-                    raise ScanningError(
-                        match.cursor.lineno + 1, text,
-                        0, '<unknown>',
-                        f'<filepath: {filepath}>'
-                    )
-            return out
-        
-        def _analyse_block(text: str) -> t.List[str]:
-            varnames = []
-            try:
-                for element, type_ in get_variables(text):
-                    if type_ == VARIABLE_NAME:
-                        varnames.append(element)
-                    elif type_ == SUBSCRIPTABLE:
-                        varnames.append(_analyse_subscriptables(
-                            element, shorten_sub_substrings=True
-                        ))
-                    else:
-                        varnames.append('')
-            except UnresolvedCase:
-                varnames.clear()
-            finally:
-                return varnames
-        
-        _quotes_pattern_1 = re.compile(r'\'\'\'[\w\W]*\'\'\'|"""[\w\W]*"""')
-        _quotes_pattern_2 = re.compile(r'\'[^\']*\'|"[^"]*"')
-        
-        def _analyse_subscriptables(
-                text: str,
-                shorten_sub_substrings: bool = True,
-                threshold: int = 20
-        ) -> str:
-            """
-            shorten_sub_strings:
-                example:
-                    case 1: when captured a "varname" like "xxx('hello world')":
-                        if shorten_sub_strings is True:
-                            varname updated: "xxx('...')"
-                        if shorten_sub_strings is False:
-                            varname updated: "xxx('hello world')"
-                    case 2: when captured a "varname" like "xxx('''hello world\n
-                            hello world\nhello world\nhello world\nhello...''')"
-                            (which is a very long sentense):
-                        if shorten_sub_strings is True:
-                            varname updated: "xxx('...')"
-                        if shorten_sub_strings is False:
-                            varname updated: "xxx('''hello world\nhello world\n
-                                hello world\nhello world\nhello world\n...)"
-                note: the character threshold length to trigger shortening a
-                    string is adjustable, the default threshold is 10 chars and
-                    must with no line break in it.
-            """
-            if not shorten_sub_substrings:
-                return text
-            
-            backslash_mask = []
-            for i in re.findall(r'\\.', text):
-                backslash_mask.append(i)
-            if backslash_mask:
-                text = re.sub(r'\\.', '__BACKSLASK_MASK__', text)
-            
-            for i in set(_quotes_pattern_1.findall(text)):
-                if '\n' in i or len(i) > threshold:
-                    text = text.replace(i, '"""..."""')
-            
-            for i in set(_quotes_pattern_2.findall(text)):
-                if '\n' in i or len(i) > threshold:
-                    text = text.replace(i, '"..."')
-            
-            # restore backslashes
-            if backslash_mask:
-                for i in backslash_mask:
-                    text = text.replace('__BACKSLASK_MASK__', i, 1)
-                del backslash_mask
-            
-            text = re.sub(r'\s+', ' ', text)
-            #   note: this ^measure takes a side effect that it may replace
-            #   sequential whitespaces to one whitespace inside quote strings.
-            
-            return text
-        
-        with open(filepath, 'r', encoding='utf-8') as f:
-            self._sourcemap.setdefault(
-                filepath, get_blocks((x.rstrip('\n') for x in f.readlines()))
-            )
-
-
-sourcemap = SourceMap()
-
-
-class FrameInfo:
-    
-    def __init__(self, frame: FrameType):
-        self._frame = frame
-    
-    def __str__(self) -> str:
-        return self.info
-    
-    @property
-    def info(self) -> str:
-        return dedent(f'''
-            <FrameInfo object>
-                filepath: {self.filepath}
-                lineno: {self.lineno}
-                funcname: {self.funcname}
-        ''').rstrip()
-    
-    @property
-    def id(self) -> str:
-        return f'{self.filepath}:{self.lineno}'
-    
-    @property
-    def filepath(self) -> str:
-        """
-        notice:
-            - the returned value may be '<string>', '<unknown>' etc.
-            - (2023-05-22):
-                we do not use `__file__` anymore, because it may cause markup
-                analyser broken when the `__file__` is not real (for example
-                when caller passes `globals()` to `exec` function).
-                see also `examples/start_ipython.py : line 11`.
-            - in python 3.8, `co_filename` may be a relative path, so we need
-                to convert it to absolute.
-            - (2023-06-30):
-                the path may be unexisted, for example a kernel file using
-                `background_zmq_ipython` library.
-        """
-        # from ._print import debug
-        # debug(self._frame.f_code.co_filename,
-        #       self._frame.f_globals.get('__file__'))
-        return abspath(self._frame.f_code.co_filename).replace('\\', '/')
-    
-    @property
-    def lineno(self) -> int:
-        return self._frame.f_lineno
-    
-    @property
-    def indentation(self) -> int:
-        # https://stackoverflow.com/a/39172552
-        if x := inspect.getframeinfo(self._frame).code_context:
-            ctx = x[0]
-            return len(ctx) - len(ctx.lstrip())
-        return 0
-    
-    @property
-    def funcname(self) -> str:
-        return self._frame.f_code.co_name
-    
-    def collect_varnames(self) -> T.VarNames:
-        return sourcemap.get_varnames(self.filepath, self.lineno)
-    
-    def get_parent(self, traceback_level: int = 1) -> 'FrameInfo':
-        return FrameInfo(_get_parent_frame(self._frame, traceback_level))
-
-
-@dataclass
-class FrozenFrameInfo:
-    """
-    this is picklable. used for multiprocessing queue.
-    """
-    filepath: str
-    lineno: int
-    indentation: int
-    funcname: str
-    _parent: 'FrozenFrameInfo' = None
-
-    @property
-    def id(self) -> str:
-        return f'{self.filepath}:{self.lineno}'
-
-    def collect_varnames(self) -> T.VarNames:
-        return sourcemap.get_varnames(self.filepath, self.lineno)
-    
-    def get_parent(self, _) -> 'FrozenFrameInfo':
-        assert self._parent
-        return self._parent
-
-
-def freeze_frame_info(
-    frame: FrameType,
-    _traceback_level: int = 0,
-) -> FrozenFrameInfo:
-    info = FrameInfo(frame)
-    return FrozenFrameInfo(
-        info.filepath,
-        info.lineno,
-        info.indentation,
-        info.funcname,
-        (
-            _traceback_level > 0
-            and freeze_frame_info(
-                _get_parent_frame(frame, _traceback_level)
-            )
-            or None
-        )
-    )
-
-
-def _get_parent_frame(frame: FrameType, level: int = 1) -> FrameType:
-    for _ in range(level):
-        frame = frame.f_back
-    return frame
+import inspect
+import re
+import typing as t
+from dataclasses import dataclass
+from os.path import abspath
+from os.path import exists
+from textwrap import dedent
+from types import FrameType
+
+from .scanner import get_all_blocks
+from .scanner import get_variables
+from .scanner.const import SUBSCRIPTABLE
+from .scanner.const import VARIABLE_NAME
+from .scanner.exceptions import ScanningError
+from .scanner.exceptions import UnresolvedCase
+
+
+class T:
+    VarNames = t.Tuple[str, ...]
+    SourceMap = t.Dict[str, t.Dict[int, VarNames]]
+
+
+class SourceMap:
+    _sourcemap: T.SourceMap
+    
+    def __init__(self):
+        self._sourcemap = {}
+    
+    def get_varnames(self, filepath: str, lineno: int) -> T.VarNames:
+        if filepath not in self._sourcemap:
+            self._indexing_filemap(filepath)
+        return self._sourcemap[filepath].get(lineno, ())
+    
+    def _indexing_filemap(self, filepath: str) -> None:
+        if filepath.startswith('<') or filepath.endswith('>') \
+                or not exists(filepath):
+            # see `FrameInfo > property filepath > docstring notice`
+            self._sourcemap.setdefault(filepath, {})
+            return
+        
+        def get_blocks(lines: t.Iterator[str]) -> t.Dict[int, T.VarNames]:
+            out = {}
+            for match in get_all_blocks(*lines):
+                text = match.fulltext.strip()
+                if not text:
+                    continue
+                if not text.startswith('print'):  # FIXME: this is not stable
+                    continue
+                try:
+                    varnames = _analyse_block(text)
+                    lineno = match.cursor.lineno + 1
+                    out[lineno] = tuple(varnames)
+                except ScanningError:
+                    raise ScanningError(
+                        match.cursor.lineno + 1, text,
+                        0, '<unknown>',
+                        f'<filepath: {filepath}>'
+                    )
+            return out
+        
+        def _analyse_block(text: str) -> t.List[str]:
+            varnames = []
+            try:
+                for element, type_ in get_variables(text):
+                    if type_ == VARIABLE_NAME:
+                        varnames.append(element)
+                    elif type_ == SUBSCRIPTABLE:
+                        varnames.append(_analyse_subscriptables(
+                            element, shorten_sub_substrings=True
+                        ))
+                    else:
+                        varnames.append('')
+            except UnresolvedCase:
+                varnames.clear()
+            finally:
+                return varnames
+        
+        _quotes_pattern_1 = re.compile(r'\'\'\'[\w\W]*\'\'\'|"""[\w\W]*"""')
+        _quotes_pattern_2 = re.compile(r'\'[^\']*\'|"[^"]*"')
+        
+        def _analyse_subscriptables(
+                text: str,
+                shorten_sub_substrings: bool = True,
+                threshold: int = 20
+        ) -> str:
+            """
+            shorten_sub_strings:
+                example:
+                    case 1: when captured a "varname" like "xxx('hello world')":
+                        if shorten_sub_strings is True:
+                            varname updated: "xxx('...')"
+                        if shorten_sub_strings is False:
+                            varname updated: "xxx('hello world')"
+                    case 2: when captured a "varname" like "xxx('''hello world\n
+                            hello world\nhello world\nhello world\nhello...''')"
+                            (which is a very long sentense):
+                        if shorten_sub_strings is True:
+                            varname updated: "xxx('...')"
+                        if shorten_sub_strings is False:
+                            varname updated: "xxx('''hello world\nhello world\n
+                                hello world\nhello world\nhello world\n...)"
+                note: the character threshold length to trigger shortening a
+                    string is adjustable, the default threshold is 10 chars and
+                    must with no line break in it.
+            """
+            if not shorten_sub_substrings:
+                return text
+            
+            backslash_mask = []
+            for i in re.findall(r'\\.', text):
+                backslash_mask.append(i)
+            if backslash_mask:
+                text = re.sub(r'\\.', '__BACKSLASK_MASK__', text)
+            
+            for i in set(_quotes_pattern_1.findall(text)):
+                if '\n' in i or len(i) > threshold:
+                    text = text.replace(i, '"""..."""')
+            
+            for i in set(_quotes_pattern_2.findall(text)):
+                if '\n' in i or len(i) > threshold:
+                    text = text.replace(i, '"..."')
+            
+            # restore backslashes
+            if backslash_mask:
+                for i in backslash_mask:
+                    text = text.replace('__BACKSLASK_MASK__', i, 1)
+                del backslash_mask
+            
+            text = re.sub(r'\s+', ' ', text)
+            #   note: this ^measure takes a side effect that it may replace
+            #   sequential whitespaces to one whitespace inside quote strings.
+            
+            return text
+        
+        with open(filepath, 'r', encoding='utf-8') as f:
+            self._sourcemap.setdefault(
+                filepath, get_blocks((x.rstrip('\n') for x in f.readlines()))
+            )
+
+
+sourcemap = SourceMap()
+
+
+class FrameInfo:
+    
+    def __init__(self, frame: FrameType):
+        self._frame = frame
+    
+    def __str__(self) -> str:
+        return self.info
+    
+    @property
+    def info(self) -> str:
+        return dedent(f'''
+            <FrameInfo object>
+                filepath: {self.filepath}
+                lineno: {self.lineno}
+                funcname: {self.funcname}
+        ''').rstrip()
+    
+    @property
+    def id(self) -> str:
+        return f'{self.filepath}:{self.lineno}'
+    
+    @property
+    def filepath(self) -> str:
+        """
+        notice:
+            - the returned value may be '<string>', '<unknown>' etc.
+            - (2023-05-22):
+                we do not use `__file__` anymore, because it may cause markup
+                analyser broken when the `__file__` is not real (for example
+                when caller passes `globals()` to `exec` function).
+                see also `examples/start_ipython.py : line 11`.
+            - in python 3.8, `co_filename` may be a relative path, so we need
+                to convert it to absolute.
+            - (2023-06-30):
+                the path may be unexisted, for example a kernel file using
+                `background_zmq_ipython` library.
+        """
+        # from ._print import debug
+        # debug(self._frame.f_code.co_filename,
+        #       self._frame.f_globals.get('__file__'))
+        return abspath(self._frame.f_code.co_filename).replace('\\', '/')
+    
+    @property
+    def lineno(self) -> int:
+        return self._frame.f_lineno
+    
+    @property
+    def indentation(self) -> int:
+        # https://stackoverflow.com/a/39172552
+        if x := inspect.getframeinfo(self._frame).code_context:
+            ctx = x[0]
+            return len(ctx) - len(ctx.lstrip())
+        return 0
+    
+    @property
+    def funcname(self) -> str:
+        return self._frame.f_code.co_name
+    
+    def collect_varnames(self) -> T.VarNames:
+        return sourcemap.get_varnames(self.filepath, self.lineno)
+    
+    def get_parent(self, traceback_level: int = 1) -> 'FrameInfo':
+        return FrameInfo(_get_parent_frame(self._frame, traceback_level))
+
+
+@dataclass
+class FrozenFrameInfo:
+    """
+    this is picklable. used for multiprocessing queue.
+    """
+    filepath: str
+    lineno: int
+    indentation: int
+    funcname: str
+    _parent: 'FrozenFrameInfo' = None
+
+    @property
+    def id(self) -> str:
+        return f'{self.filepath}:{self.lineno}'
+
+    def collect_varnames(self) -> T.VarNames:
+        return sourcemap.get_varnames(self.filepath, self.lineno)
+    
+    def get_parent(self, _) -> 'FrozenFrameInfo':
+        assert self._parent
+        return self._parent
+
+
+def freeze_frame_info(
+    frame: FrameType,
+    _traceback_level: int = 0,
+) -> FrozenFrameInfo:
+    info = FrameInfo(frame)
+    return FrozenFrameInfo(
+        info.filepath,
+        info.lineno,
+        info.indentation,
+        info.funcname,
+        (
+            _traceback_level > 0
+            and freeze_frame_info(
+                _get_parent_frame(frame, _traceback_level)
+            )
+            or None
+        )
+    )
+
+
+def _get_parent_frame(frame: FrameType, level: int = 1) -> FrameType:
+    for _ in range(level):
+        frame = frame.f_back
+    return frame
```

## lk_logger/logger.py

```diff
@@ -13,15 +13,16 @@
 from .frame_info import FrameInfo
 from .frame_info import FrozenFrameInfo
 from .markup import MarkMeaning
 from .markup import MarkupAnalyser
 from .markup import T as T0
 from .message_builder import MessageStruct
 from .message_builder import T as T1
-from .message_builder import builder as message_builder
+from .message_builder import builder as msg_builder
+from .message_formatter import formatter as msg_formatter
 from .path_helper import path_helper
 from .pipeline import pipeline
 from .printer import con_print
 from .printer import dbg_print  # noqa
 from .printer import printer_manager
 from .printer import std_print
 
@@ -62,15 +63,15 @@
     def configure(self, clear_preset: bool = False, **kwargs) -> None:
         self._cache.clear_cache()
         if clear_preset:
             self._config.reset()
         if 'show_varname' in kwargs:  # workaround for compatibility
             kwargs['show_varnames'] = kwargs.pop('show_varname')
         self._config.update(**kwargs)
-        message_builder.update_config(separator=self._config.separator)
+        msg_builder.update_config(separator=self._config.separator)
     
     @property
     def config(self) -> dict:
         return self._config.to_dict()
     
     # -------------------------------------------------------------------------
     
@@ -151,15 +152,15 @@
             flush_scheme = 2
         elif MarkMeaning.FLUSH_EDDY in marks_meaning:
             flush_scheme = 3
         
         # check cache
         if self._cache.is_cached(frame_info.id, markup):
             cached_info = self._cache.get_cache(frame_info.id, markup)
-            return message_builder.compose(
+            return msg_builder.compose(
                 args, marks_meaning, cached_info,
                 self._config.show_source,
                 self._config.show_funcname,
                 self._config.show_varnames,
                 self._config.sourcemap_alignment,
             ), flush_scheme
         
@@ -167,27 +168,45 @@
         
         if not args:
             if (
                 MarkMeaning.MODERATE_PRUNE in marks_meaning or
                 MarkMeaning.AGRESSIVE_PRUNE in marks_meaning
             ):
                 return _NoMessage, flush_scheme
+        if (
+            MarkMeaning.RICH_OBJECT in marks_meaning or
+            MarkMeaning.RICHABLE_DATA in marks_meaning or
+            MarkMeaning.TABULAR_DATA in marks_meaning or
+            MarkMeaning.TRACEBACK_EXCEPTION in marks_meaning or
+            MarkMeaning.TRACEBACK_EXCEPTION_WITH_LOCALS in marks_meaning
+        ):
+            assert len(args) == 1
         if MarkMeaning.BUILTIN_PRINT in marks_meaning:
             return _RawArgs(args), flush_scheme
         elif MarkMeaning.RICH_OBJECT in marks_meaning:
-            assert len(args) == 1 and isinstance(args[0], RenderableType)
+            assert isinstance(args[0], RenderableType)
             return args[0], flush_scheme
+        elif (
+            MarkMeaning.RICHABLE_DATA in marks_meaning or
+            MarkMeaning.TABULAR_DATA in marks_meaning
+        ):
+            # TODO: need a better design.
+            print(':p2')
+            return msg_formatter.fmt_message(
+                arguments=args, varnames=(), rich=False, expand_rich=True,
+                _padding=4
+            ), flush_scheme
         elif MarkMeaning.TRACEBACK_EXCEPTION in marks_meaning:
-            assert len(args) == 1 and isinstance(args[0], BaseException)
-            return message_builder.compose_exception(
+            assert isinstance(args[0], BaseException)
+            return msg_builder.compose_exception(
                 args[0], show_locals=False
             ), flush_scheme
         elif MarkMeaning.TRACEBACK_EXCEPTION_WITH_LOCALS in marks_meaning:
-            assert len(args) == 1 and isinstance(args[0], BaseException)
-            return message_builder.compose_exception(
+            assert isinstance(args[0], BaseException)
+            return msg_builder.compose_exception(
                 args[0], show_locals=True
             ), flush_scheme
         
         info: T.Info = {
             'file_path'      : '',
             'line_number'    : '0',
             'is_external_lib': False,
@@ -247,15 +266,15 @@
                 elif markup_pos == 1:
                     info['variable_names'] = varnames[1:]
                 else:
                     info['variable_names'] = varnames[:-1]
         
         self._cache.store_info(frame_info.id, markup, info)
         
-        return message_builder.compose(
+        return msg_builder.compose(
             args, marks_meaning, info,
             show_source=show_source,
             show_funcname=show_funcname,
             show_varnames=show_varnames,
             sourcemap_alignment=self._config.sourcemap_alignment,
         ), flush_scheme
```

## lk_logger/markup.py

```diff
@@ -21,17 +21,19 @@
     FLUSH_EDDY = auto()
     MODERATE_PRUNE = auto()
     PARENT_POINTER = auto()
     RESET_INDEX = auto()
     RESET_TIMER = auto()
     RICH_FORMAT = auto()
     RICH_OBJECT = auto()
+    RICHABLE_DATA = auto()
     SCOPED_COUNTER = auto()
     SIMPLE_COUNTER = auto()
     STOP_TIMER = auto()
+    TABULAR_DATA = auto()
     TEMP_TIMER = auto()
     TRACEBACK_EXCEPTION = auto()
     TRACEBACK_EXCEPTION_WITH_LOCALS = auto()
     VERBOSITY = auto()
 
 
 class T:
@@ -41,15 +43,15 @@
         'e': int,  # exception trace back
         'i': int,  # index
         'f': int,  # flush
         'l': int,  # long / loose / expanded (multiple lines)
         'p': int,  # parent layer
         'r': int,  # rich style
         's': int,  # short / simple / single line
-        't': int,  # timer / timestamp
+        't': int,  # timer / timestamp / tabular
         'v': int,  # verbosity / log level
     })
     MarksMeaning = t.Dict[MarkMeaning, t.Any]
     
     class Counter:
         ColorHex = str
         Fid = str
@@ -174,17 +176,17 @@
             elif marks['f'] == 2:
                 out[MarkMeaning.FLUSH_EDDY] = True
             else:
                 raise E.UnsupportedMarkup(f':f{marks["f"]}')
         
         if marks['i'] >= 0:
             if marks['i'] == 0:
+                out[MarkMeaning.RICH_FORMAT] = True
                 out[MarkMeaning.RESET_INDEX] = \
                     self._counter.reset_simple_count()
-                out[MarkMeaning.RICH_FORMAT] = True
             elif marks['i'] == 1:
                 out[MarkMeaning.SIMPLE_COUNTER] = \
                     self._counter.update_simple_count()
             elif marks['i'] == 2:
                 info: FrameInfo = kwargs['frame_info']
                 out[MarkMeaning.SCOPED_COUNTER] = \
                     self._counter.update_scoped_count(
@@ -202,40 +204,46 @@
             out[MarkMeaning.PARENT_POINTER] = 0
         
         if marks['r'] >= 0:
             if marks['r'] == 0:
                 out[MarkMeaning.RICH_FORMAT] = True
             elif marks['r'] == 1:
                 out[MarkMeaning.RICH_OBJECT] = True
+            elif marks['r'] == 2:
+                out[MarkMeaning.RICHABLE_DATA] = True
             else:
                 raise E.UnsupportedMarkup(f':r{marks["r"]}')
         
         if marks['s'] >= 0:
             if marks['s'] == 0:
                 out[MarkMeaning.MODERATE_PRUNE] = True
             elif marks['s'] == 1:
                 out[MarkMeaning.AGRESSIVE_PRUNE] = True
             elif marks['s'] == 2:
                 out[MarkMeaning.BUILTIN_PRINT] = True
             else:
                 raise E.UnsupportedMarkup(f':s{marks["s"]}')
         
         if marks['t'] >= 0:
-            out[MarkMeaning.RICH_FORMAT] = True
             if marks['t'] == 0:
+                out[MarkMeaning.RICH_FORMAT] = True
                 t = self._simple_time = time()
                 out[MarkMeaning.RESET_TIMER] = t
             elif marks['t'] == 1:
+                out[MarkMeaning.RICH_FORMAT] = True
                 start, end = self._simple_time, time()
                 out[MarkMeaning.STOP_TIMER] = (start, end)
                 self._simple_time = end
             elif marks['t'] == 2:
+                out[MarkMeaning.RICH_FORMAT] = True
                 start, end = self._temp_time, time()
                 out[MarkMeaning.TEMP_TIMER] = (start, end)
                 self._temp_time = end
+            elif marks['t'] == 3:
+                out[MarkMeaning.TABULAR_DATA] = True
             else:
                 raise E.UnsupportedMarkup(f':t{marks["t"]}')
         
         if marks['v'] >= 1:
             levels = ('trace', 'debug', 'info', 'warn', 'error', 'fatal')
             out[MarkMeaning.VERBOSITY] = levels[marks['v']]
```

## lk_logger/message_builder.py

```diff
@@ -125,29 +125,29 @@
         info: T.Info,
         show_source: bool = True,
         show_funcname: bool = True,
         show_varnames: bool = False,
         sourcemap_alignment: t.Literal['left', 'right'] = 'left',
     ) -> T.MessageStruct:
         show_source = (
-            show_source  # fmt:skip
-            and MarkMeaning.AGRESSIVE_PRUNE not in marks_meaning
+            show_source and
+            MarkMeaning.AGRESSIVE_PRUNE not in marks_meaning
         )
         show_funcname = (
-            show_funcname  # fmt:skip
-            and MarkMeaning.AGRESSIVE_PRUNE not in marks_meaning
+            show_funcname and
+            MarkMeaning.AGRESSIVE_PRUNE not in marks_meaning
         )
         show_varnames = (
-            show_varnames
-            and MarkMeaning.MODERATE_PRUNE not in marks_meaning
-            and MarkMeaning.AGRESSIVE_PRUNE not in marks_meaning
+            show_varnames and
+            MarkMeaning.MODERATE_PRUNE not in marks_meaning and
+            MarkMeaning.AGRESSIVE_PRUNE not in marks_meaning
         )
         has_any_prune_scheme = (
-            MarkMeaning.MODERATE_PRUNE in marks_meaning
-            or MarkMeaning.AGRESSIVE_PRUNE in marks_meaning
+            MarkMeaning.MODERATE_PRUNE in marks_meaning or
+            MarkMeaning.AGRESSIVE_PRUNE in marks_meaning
         )
         
         head = Text()
         body = Text()
         
         # 1. source
         if show_source:
@@ -274,14 +274,19 @@
         #         overall_style=marks_meaning.get(MarkMeaning.VERBOSITY, None),
         #     )
         # )
         temp = formatter.fmt_message(
             arguments=args,
             varnames=info['variable_names'] if show_varnames else (),
             rich=MarkMeaning.RICH_FORMAT in marks_meaning,
+            expand_rich=(
+                MarkMeaning.RICH_OBJECT in marks_meaning or
+                MarkMeaning.RICHABLE_DATA in marks_meaning or
+                MarkMeaning.TABULAR_DATA in marks_meaning
+            ),
             expand_level=marks_meaning.get(MarkMeaning.EXPAND_OBJECT, 0),
             separator=self._separator_b,
             overall_style=marks_meaning.get(MarkMeaning.VERBOSITY, None),
         )
         
         # PERF: this is compromised design.
         # 8. divider
```

## lk_logger/message_formatter.py

```diff
@@ -1,23 +1,28 @@
 import typing as t
 from dataclasses import dataclass
 from functools import partial
 from io import StringIO
 from math import ceil
+from textwrap import dedent
 from textwrap import indent
 from time import localtime
 from time import strftime as _strftime
 from traceback import format_exception
+from types import GeneratorType
 
 import rich
 # noinspection PyProtectedMember
 from rich._inspect import Inspect
+from rich.box import ROUNDED as BOX_ROUNDED
 from rich.console import RenderableType
-# from rich.padding import Padding
+from rich.markdown import Markdown
+from rich.padding import Padding
 from rich.pretty import pretty_repr
+from rich.table import Table
 from rich.text import Text
 from rich.traceback import Traceback
 
 from .console import console
 
 strftime = lambda t: (t and _strftime('%H:%M:%S', localtime(t))) or ''
 
@@ -27,14 +32,15 @@
     text: str
     mark: str = None
 
 
 class T:
     Level = t.Literal['trace', 'debug', 'info', 'warning', 'error', 'fatal']
     RichText = Text
+    Traceback = Traceback
 
 
 class Color:  # TODO: not used yet (and not ready).
     SEPARATOR = 'bright_black'
     
     # time
     TIME_START = 'green'
@@ -94,15 +100,15 @@
                         # raise ValueError('invalid context', context)
                         length = 80
             else:
                 length = 80
         return self.markup((pattern * length, 'yellow'))
     
     @staticmethod
-    def fmt_exception(e: BaseException, show_locals=False) -> Traceback:
+    def fmt_exception(e: BaseException, show_locals=False) -> T.Traceback:
         trace = Traceback.from_exception(
             type(e), e, e.__traceback__,
             show_locals=show_locals
         )
         return trace
     
     def fmt_funcname(self, funcname: str, fmt_width=False) -> T.RichText:
@@ -145,24 +151,67 @@
         return Text(label, color)
     
     def fmt_message(
         self,
         arguments: t.Iterable[t.Any],
         varnames: t.Tuple[str, ...],
         rich: bool,
+        expand_rich: bool = False,  # expand rich definition
         expand_level: int = 0,
         separator: T.RichText = None,
         overall_style: T.Level = None,
+        _padding: int = 0,
     ) -> T.RichText:
         """
+        the differ of `expand_rich` and `rich`:
+            rich: renders a string like '[red]text[/]' to colored text.
+            expand_rich: renders a union[str, list[list], dict] object to:
+                str  -> markdown object
+                list[list] -> table object
+                dict -> table object. keys are column fields.
+        
         notice the process sequence:
             1. expand
             2. varnames
             3. rich
         """
+        if expand_rich:  # TODO: need a better design
+            assert not rich  # rich and expand_rich are mutually exclusive
+            arguments = tuple(arguments)
+            assert len(arguments) == 1 and isinstance(
+                arguments[0], (str, dict, list, tuple, GeneratorType)
+            )
+            arg = arguments[0]
+            if isinstance(arg, str):
+                out = Markdown(dedent(arg))
+            elif isinstance(arg, dict):
+                table = Table(
+                    *arg.keys(), header_style='yellow', box=BOX_ROUNDED
+                )
+                for row in zip(*arg.values()):
+                    table.add_row(*map(str, row))
+                out = table
+            else:
+                table = None
+                for i, row in enumerate(arg):
+                    if i == 0:
+                        table = Table(
+                            *map(str, row),
+                            header_style='yellow',
+                            box=BOX_ROUNDED
+                        )
+                    else:
+                        table.add_row(*map(str, row))
+                assert table
+                out = table
+            # noinspection PyTypeChecker
+            return Padding(out, (0, 0, 0, _padding)) if _padding else out
+        
+        # ---------------------------------------------------------------------
+        
         if expand_level == 1:
             arguments = map(self._expand_object, arguments)
         elif expand_level == 2:
             arguments = map(self._inspect_object, arguments)
         if varnames:
             arguments = self._mix_arguments_with_varnames(
                 tuple(arguments), varnames
```

## lk_logger/pipeline.py

 * *Ordering differences only*

```diff
@@ -1,90 +1,90 @@
-import typing as t
-from os import name as _os_name
-from os.path import abspath
-from os.path import dirname
-
-from .printer import non_print
-from .printer import std_print
-
-
-class T:
-    PrintFunc = t.Optional[t.Callable]
-    Cache = t.Dict[str, PrintFunc]
-    PipeLines = t.NamedTuple('PipeLines2', (
-        ('abspath', t.Dict[str, PrintFunc]),
-        ('libname', t.Dict[str, PrintFunc]),  # TODO: not used
-    ))
-    ''' e.g.
-        ('abspath': {'/Users/.../python/3.10/lib/python3.10/traceback.py':
-                     <function ...>, ...},
-         'libpath': {'[tornado]': <function bprint at 0x000001D1C1D1B8B0>, ...})
-    '''
-
-
-class Pipeline:
-    _cache: T.Cache
-    _lines: T.PipeLines
-    
-    def __init__(self) -> None:
-        self._cache = {}
-        self._lines = T.PipeLines({}, {})
-    
-    def dump_list(self) -> t.List[str]:
-        return list(self._lines.abspath.keys())
-    
-    def add(
-        self,
-        x: t.Union[str, object],
-        prt: t.Optional[t.Callable] = std_print,
-        scope: bool = False
-    ) -> None:
-        if isinstance(x, str):
-            if x.startswith('['):
-                path = x
-            else:
-                path = _normpath(x)
-        else:
-            # x is a package or a module
-            # dprint(x, x.__file__)
-            path = _normpath(x.__file__)
-            if scope:
-                path = dirname(path)
-        # dprint('add path to pipeline', path)
-        if prt is None:
-            prt = non_print
-        if path.startswith('['):
-            self._lines.libname[path] = prt
-        else:
-            self._lines.abspath[path] = prt
-        self._cache[path] = prt
-    
-    def get(self, path: str) -> T.PrintFunc:
-        """
-        get proper print function for the given path.
-        """
-        # the path is an absolute path.
-        path = _normpath(path)
-        # dprint(path)
-        if path in self._cache:
-            # dprint('path in cache', path, self._cache[path])
-            return self._cache[path]
-        for root, prt in self._lines.abspath.items():
-            if path.startswith(root):
-                self._cache[path] = prt
-                # dprint('use custom print', path)
-                return prt
-        self._cache[path] = None
-        return None
-
-
-_IS_WIN = _os_name == 'nt'
-
-
-def _normpath(path: str) -> str:
-    path = abspath(path)
-    if _IS_WIN:
-        path = path.replace('\\', '/')
-    return path
-
-
-pipeline = Pipeline()
+import typing as t
+from os import name as _os_name
+from os.path import abspath
+from os.path import dirname
+
+from .printer import non_print
+from .printer import std_print
+
+
+class T:
+    PrintFunc = t.Optional[t.Callable]
+    Cache = t.Dict[str, PrintFunc]
+    PipeLines = t.NamedTuple('PipeLines2', (
+        ('abspath', t.Dict[str, PrintFunc]),
+        ('libname', t.Dict[str, PrintFunc]),  # TODO: not used
+    ))
+    ''' e.g.
+        ('abspath': {'/Users/.../python/3.10/lib/python3.10/traceback.py':
+                     <function ...>, ...},
+         'libpath': {'[tornado]': <function bprint at 0x000001D1C1D1B8B0>, ...})
+    '''
+
+
+class Pipeline:
+    _cache: T.Cache
+    _lines: T.PipeLines
+    
+    def __init__(self) -> None:
+        self._cache = {}
+        self._lines = T.PipeLines({}, {})
+    
+    def dump_list(self) -> t.List[str]:
+        return list(self._lines.abspath.keys())
+    
+    def add(
+        self,
+        x: t.Union[str, object],
+        prt: t.Optional[t.Callable] = std_print,
+        scope: bool = False
+    ) -> None:
+        if isinstance(x, str):
+            if x.startswith('['):
+                path = x
+            else:
+                path = _normpath(x)
+        else:
+            # x is a package or a module
+            # dprint(x, x.__file__)
+            path = _normpath(x.__file__)
+            if scope:
+                path = dirname(path)
+        # dprint('add path to pipeline', path)
+        if prt is None:
+            prt = non_print
+        if path.startswith('['):
+            self._lines.libname[path] = prt
+        else:
+            self._lines.abspath[path] = prt
+        self._cache[path] = prt
+    
+    def get(self, path: str) -> T.PrintFunc:
+        """
+        get proper print function for the given path.
+        """
+        # the path is an absolute path.
+        path = _normpath(path)
+        # dprint(path)
+        if path in self._cache:
+            # dprint('path in cache', path, self._cache[path])
+            return self._cache[path]
+        for root, prt in self._lines.abspath.items():
+            if path.startswith(root):
+                self._cache[path] = prt
+                # dprint('use custom print', path)
+                return prt
+        self._cache[path] = None
+        return None
+
+
+_IS_WIN = _os_name == 'nt'
+
+
+def _normpath(path: str) -> str:
+    path = abspath(path)
+    if _IS_WIN:
+        path = path.replace('\\', '/')
+    return path
+
+
+pipeline = Pipeline()
```

## lk_logger/printer.py

 * *Ordering differences only*

```diff
@@ -1,100 +1,100 @@
-import builtins
-import typing as t
-from inspect import currentframe
-from contextlib import contextmanager
-from os import name as os_name
-
-from .console import console
-
-
-class BasePrinter:
-    def __call__(self, *msg: t.Any) -> None:
-        raise NotImplementedError
-
-
-class DebugPrinter(BasePrinter):
-    def __call__(self, *msg: t.Any) -> None:
-        frame = currentframe().f_back
-        filepath = _normpath(frame.f_globals["__file__"])
-        lineno = frame.f_lineno
-        source = '{}:{}'.format(filepath, lineno)
-        std_print(source, '[LKDEBUG]', *msg)
-
-
-class NothingPrinter(BasePrinter):
-    def __call__(self, *msg: t.Any) -> None:
-        pass  # do nothing
-
-
-std_print = t.cast(BasePrinter, builtins.print)
-con_print = console.print
-con_error = console.print_exception
-dbg_print = DebugPrinter()
-non_print = NothingPrinter()
-
-# alias
-bprint = std_print
-dprint = dbg_print
-
-
-# -----------------------------------------------------------------------------
-# group control
-
-class T:
-    Printer = t.Union[BasePrinter, t.Callable[[str], None]]
-    Printers = t.Tuple[Printer, ...]
-
-
-class PrinterManager:
-    _group: t.List[T.Printers]
-    
-    def __init__(self) -> None:
-        # self._group = [(std_print,)]
-        self._group = [()]
-    
-    @property
-    def printers(self) -> T.Printers:
-        return self._group[-1]
-    
-    def add_group(self, printers: T.Printers) -> None:
-        self._group.append(printers)
-        
-    def pop_group(self) -> None:
-        self._group.pop()
-
-
-printer_manager = PrinterManager()
-
-
-@contextmanager
-def parallel_printing(*printers: T.Printer, inherit: bool = True) -> t.Iterator:
-    """
-    params:
-        inherit: if True, will inherit the previous printers.
-            for example:
-                with parallel_printing(p1, p2):
-                    print('aaa')  # p1, p2 called
-                    with parallel_printing(p3):
-                        print('bbb')  # p1, p2, p3 called
-                    with parallel_printing(p4, inherit=False):
-                        print('ccc')  # p4 called
-                        with parallel_printing(p5):
-                            print('ddd')  # p4, p5 called
-    """
-    if inherit:
-        printers = printer_manager.printers + printers
-    printer_manager.add_group(printers)
-    yield
-    printer_manager.pop_group()
-
-
-# -----------------------------------------------------------------------------
-# general
-
-_IS_WIN = os_name == 'nt'
-
-
-def _normpath(path: str) -> str:
-    if _IS_WIN:
-        return path.replace('\\', '/').rstrip('/')
-    return path.rstrip('/')
+import builtins
+import typing as t
+from inspect import currentframe
+from contextlib import contextmanager
+from os import name as os_name
+
+from .console import console
+
+
+class BasePrinter:
+    def __call__(self, *msg: t.Any) -> None:
+        raise NotImplementedError
+
+
+class DebugPrinter(BasePrinter):
+    def __call__(self, *msg: t.Any) -> None:
+        frame = currentframe().f_back
+        filepath = _normpath(frame.f_globals["__file__"])
+        lineno = frame.f_lineno
+        source = '{}:{}'.format(filepath, lineno)
+        std_print(source, '[LKDEBUG]', *msg)
+
+
+class NothingPrinter(BasePrinter):
+    def __call__(self, *msg: t.Any) -> None:
+        pass  # do nothing
+
+
+std_print = t.cast(BasePrinter, builtins.print)
+con_print = console.print
+con_error = console.print_exception
+dbg_print = DebugPrinter()
+non_print = NothingPrinter()
+
+# alias
+bprint = std_print
+dprint = dbg_print
+
+
+# -----------------------------------------------------------------------------
+# group control
+
+class T:
+    Printer = t.Union[BasePrinter, t.Callable[[str], None]]
+    Printers = t.Tuple[Printer, ...]
+
+
+class PrinterManager:
+    _group: t.List[T.Printers]
+    
+    def __init__(self) -> None:
+        # self._group = [(std_print,)]
+        self._group = [()]
+    
+    @property
+    def printers(self) -> T.Printers:
+        return self._group[-1]
+    
+    def add_group(self, printers: T.Printers) -> None:
+        self._group.append(printers)
+        
+    def pop_group(self) -> None:
+        self._group.pop()
+
+
+printer_manager = PrinterManager()
+
+
+@contextmanager
+def parallel_printing(*printers: T.Printer, inherit: bool = True) -> t.Iterator:
+    """
+    params:
+        inherit: if True, will inherit the previous printers.
+            for example:
+                with parallel_printing(p1, p2):
+                    print('aaa')  # p1, p2 called
+                    with parallel_printing(p3):
+                        print('bbb')  # p1, p2, p3 called
+                    with parallel_printing(p4, inherit=False):
+                        print('ccc')  # p4 called
+                        with parallel_printing(p5):
+                            print('ddd')  # p4, p5 called
+    """
+    if inherit:
+        printers = printer_manager.printers + printers
+    printer_manager.add_group(printers)
+    yield
+    printer_manager.pop_group()
+
+
+# -----------------------------------------------------------------------------
+# general
+
+_IS_WIN = os_name == 'nt'
+
+
+def _normpath(path: str) -> str:
+    if _IS_WIN:
+        return path.replace('\\', '/').rstrip('/')
+    return path.rstrip('/')
```

## Comparing `lk_logger-5.7.1.dist-info/RECORD` & `lk_logger-5.7.2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-lk_logger/__init__.py,sha256=U_xd3o1OGBfzqsZ397z3wc-wSGqssnn4SAduPlWyxVw,955
+lk_logger/__init__.py,sha256=U-1ZwuMdW3XFAtS5nSpnZmh4rO97dPgOuSShvcB3jds,955
 lk_logger/cache/__init__.py,sha256=jkWi40WfmTt3Akv3YKjJHI6gxPqzXwpFmdF4bIJ-SUs,34
 lk_logger/cache/cache.py,sha256=b2zusDBHjbAVtoP8CdBedPvkujVjNosUNlsUiCPSJeY,6970
 lk_logger/cache/frame.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 lk_logger/cache/legacy.py,sha256=kuQrFzJGuTd_NQWrO5Vp6b-Da3X73w60Ae2LxVP3Xb8,1875
 lk_logger/cache/util.py,sha256=6qtnnIhdrKTqyP4Elxd1d3OnkTFROzxAGWYz3c4smDk,762
-lk_logger/config.py,sha256=jIB5tc1Eqke8_TGrCiropibesY5dBvyHzur_FtKOYdA,5815
-lk_logger/console.py,sha256=xV0C65Bv4BZ7R7mQgDZNjhmZdV3d0Y5w_n4WP1aAQHE,1267
-lk_logger/control.py,sha256=60G6mzfj7TH6BL07BTzz5ShrzhbUXJpTcZYt2_fvVSE,4988
-lk_logger/frame_info.py,sha256=MFeZoRq8ou5-5m77N40xOO3ADOxNMdWRcn4-EUouQqA,8992
-lk_logger/logger.py,sha256=EMLUj3h6C5d4Vj423GBhB5lvGAdLTt_pA1ebvq2GBD0,13871
-lk_logger/markup.py,sha256=WkIaQIRDwUyYZFY-Jn22qc-Ig7fJyx6V6jYawZcnnYQ,10376
-lk_logger/message_builder.py,sha256=--BtpkikTZXdEbZm1_-dJSxhAiE1E20GWpIIgSm5Nzc,11434
-lk_logger/message_formatter.py,sha256=lpv_rB616EmHLqYaYt7SirNIndvAdbPD9H1ZWrLthbQ,11258
+lk_logger/config.py,sha256=A2773dLIzjvBtvP9ozDzLF7Z3Vie8VfJQBRcg6ZQzRE,5668
+lk_logger/console.py,sha256=TmWt2SC2UO1en0M_tzlQPd2PuI4FoV1PGkeKrnxd6_c,1230
+lk_logger/control.py,sha256=-372tzbaB9cwPkj2YtDwnOA0avDHysRuu-x_SzNvB68,4815
+lk_logger/frame_info.py,sha256=NcKF6CZLRBB_SfEOLsj7SMR6X27w362t6WhBkpmWxBo,8737
+lk_logger/logger.py,sha256=bXDlcv_sc_ra7qulZNjJ25e94UznVX4hZFBoOCZn4SQ,14614
+lk_logger/markup.py,sha256=mahzUkl-8iED1iNEOjsbm_0h2xs5xRew2oRGPZqvYzo,10730
+lk_logger/message_builder.py,sha256=HNQdiio1oYL-z7bKcX8Pv8sa9oH0m_yOlQ_qIcycsMk,11636
+lk_logger/message_formatter.py,sha256=GxFNcHCWxXsHcnF7O_FNjg14etQRw9AHsAuiMXstF3I,13323
 lk_logger/path_helper.py,sha256=LAZOe5XK_51I0YPA6rUuY0_DKtaMtHyz52xcHqRbxY0,4034
-lk_logger/pipeline.py,sha256=V6gWLV_qhb1TNteLqugQ__qWEWPmxYQAj4hVYxX8Yyo,2543
-lk_logger/printer.py,sha256=X9baNbtuLRLK3R43CNbcyvJTA7e6cyXa2b_zDXuNxTQ,2690
+lk_logger/pipeline.py,sha256=dS5_RynnCaxDTM65bxb8YT1fPAyFeH8vzpt8UATmb_o,2453
+lk_logger/printer.py,sha256=O_IFHHKfKdiu-SALeZ2H_maIC0aDwMvM3248ihEUJ68,2590
 lk_logger/scanner/__init__.py,sha256=2b0jy5SdPwiVQSV9kL_3Vd4AkbKrRp7npAUWC3Hbyek,73
 lk_logger/scanner/analyser.py,sha256=y3HuYB2DJ4ixwww4c9o6Jq6mPc2eqz88w5Cf84_Pf6E,6407
 lk_logger/scanner/const.py,sha256=npj77J2VntzHArQOaIUIj9IeRQi9hH33_lo2XYLlg-s,1164
 lk_logger/scanner/exceptions.py,sha256=G1wpgEIzTLLrD6Q_m0qGD85v5KnlPm3CV1ZxgvGCVd8,1780
 lk_logger/scanner/scanner.py,sha256=I9tf-ELQOLgZxWM5YNCEP5FvW5JkmIhfVEdhezXGz4M,9728
 lk_logger/scanner/symbols.py,sha256=FhLqVbYRG-a72ZoVgriP4FKmAhweyeyh02IkiLymT2I,3306
 lk_logger/scanner/text_scanner.py,sha256=84ese30Bh-H1ZVxT0jcNhsTwM1nLDkZOrUO1LSdjV6k,19638
 lk_logger/scanner/typehint.py,sha256=CdX-02JvaI8PkEHgTN279e081njEAfNOHaxPXCQkguc,517
-lk_logger-5.7.1.dist-info/METADATA,sha256=_DiYe02jr9mhg4rCqzwu7eyjsLrNxfuC0Bo3zfmPKxE,4952
-lk_logger-5.7.1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-lk_logger-5.7.1.dist-info/RECORD,,
+lk_logger-5.7.2.dist-info/METADATA,sha256=kU4rA6MBo9-TeAUJaBP1S2MaxQnEw8z_epUXV6wDUf8,10805
+lk_logger-5.7.2.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+lk_logger-5.7.2.dist-info/RECORD,,
```

