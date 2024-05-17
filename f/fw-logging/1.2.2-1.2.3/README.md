# Comparing `tmp/fw_logging-1.2.2-py3-none-any.whl.zip` & `tmp/fw_logging-1.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 9021 bytes, number of entries: 6
--rw-r--r--  2.0 unx    17832 b- defN 80-Jan-01 00:00 fw_logging.py
--rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_logging-1.2.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     2500 b- defN 80-Jan-01 00:00 fw_logging-1.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_logging-1.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 80-Jan-01 00:00 fw_logging-1.2.2.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      475 b- defN 16-Jan-01 00:00 fw_logging-1.2.2.dist-info/RECORD
-6 files, 22023 bytes uncompressed, 8163 bytes compressed:  62.9%
+Zip file size: 9008 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    17879 b- defN 80-Jan-01 00:00 fw_logging.py
+-rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_logging-1.2.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2550 b- defN 80-Jan-01 00:00 fw_logging-1.2.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_logging-1.2.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 80-Jan-01 00:00 fw_logging-1.2.3.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      475 b- defN 16-Jan-01 00:00 fw_logging-1.2.3.dist-info/RECORD
+6 files, 22120 bytes uncompressed, 8150 bytes compressed:  63.2%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: fw_logging.py
 Comment: 
 
-Filename: fw_logging-1.2.2.dist-info/LICENSE
+Filename: fw_logging-1.2.3.dist-info/LICENSE
 Comment: 
 
-Filename: fw_logging-1.2.2.dist-info/METADATA
+Filename: fw_logging-1.2.3.dist-info/METADATA
 Comment: 
 
-Filename: fw_logging-1.2.2.dist-info/WHEEL
+Filename: fw_logging-1.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: fw_logging-1.2.2.dist-info/entry_points.txt
+Filename: fw_logging-1.2.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: fw_logging-1.2.2.dist-info/RECORD
+Filename: fw_logging-1.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fw_logging.py

```diff
@@ -11,15 +11,16 @@
 import re
 import sys
 import typing as t
 from datetime import datetime
 
 from dateutil.parser import parse as parse_dt
 from devtools.ansi import sformat
-from pydantic import BaseSettings, Field
+from pydantic import Field
+from pydantic_settings import BaseSettings, SettingsConfigDict
 from pygments import highlight
 from pygments.formatters import get_formatter_by_name
 from pygments.lexers import get_lexer_by_name
 from striprtf.striprtf import rtf_to_text
 
 __all__ = ["setup_logging", "get_log_config", "Filter", "add_log_level"]
 
@@ -111,37 +112,35 @@
         },
     }
 
 
 class LogConfig(BaseSettings):
     """Logging config."""
 
-    class Config:
-        """Enable envvars with prefix `FW_LOG_`."""
+    # settings config
+    model_config = SettingsConfigDict(env_prefix="FW_LOG_")
 
-        env_prefix = "FW_LOG_"
-
-    level: str = Field("INFO", regex=r"DEBUG|INFO|WARNING|ERROR|CRITICAL")
-    handler: str = Field("stdout", regex=r"stdout|stderr|file")
-    formatter: str = Field("text", regex=r"text|json")
+    level: str = Field("INFO", pattern=r"DEBUG|INFO|WARNING|ERROR|CRITICAL")
+    handler: str = Field("stdout", pattern=r"stdout|stderr|file")
+    formatter: str = Field("text", pattern=r"text|json")
     loggers: t.Dict[str, t.Optional[str]] = {}
     filters: t.Dict[str, t.Dict[str, str]] = {}
 
     # options for the file handler
     filename: pathlib.Path = pathlib.Path("log.txt")
     max_bytes: int = 10 << 20  # 10 MB
     backup_count: int = 10
 
     # options for the text formatter
     fmt: str = "{asctime}.{msecs:03.0f} {levelname} {caller} {message}"
     datefmt: str = "%Y-%m-%dT%H:%M:%S"
-    color: t.Optional[bool]
+    color: t.Optional[bool] = None
 
     # options for the json formatter
-    json_tag: t.Optional[str]
+    json_tag: t.Optional[str] = None
 
 
 class Filter(logging.Filter):
     """Log exclusion filter allowing temporary filtering as a context manager."""
 
     def __init__(self, *, name: str = "", msg: str = "", add_all: bool = True) -> None:
         """Add exclusion filter to all handlers attached to the root logger.
@@ -334,35 +333,39 @@
         lvl = sformat(lvl, lvl_clr[lvl])
     # get msg, indent multiline (ie. trace)
     msg = record.get("msg") or ""
     msg = re.sub(rf"^{time_re}", "", msg, flags=re.I | re.X)
     # colorize python traces
     if color and "Traceback (most recent call last)" in msg:
         msg = highlight(msg, tb_lexer, term_formatter).rstrip()
-    # colorize slow mongo queries
-    if color and "Slow query\n" in msg:
-        msg, attrs = msg.split("\n", maxsplit=1)
-        attr_line = attrs.replace("\n", " ")
-        ms = int(re.sub(r'.*"durationMillis": (\d+).*', r"\1", attr_line))
-        clr = "green" if ms < 500 else "yellow" if ms < 10000 else "red"
-        msg = sformat(msg, "bold", clr)
-        msg = f"{msg}\n{highlight(attrs, json_lexer, term_formatter)}".rstrip()
-        # Highlight the durationMillis value
-        msg = re.sub(f"({str(ms)})", sformat(str(ms), clr), msg)
-    msg = msg.replace("\n", "\n  ")  # multiline -> indent
+    # format and colorize mongo attr jsons
+    if mongo_attr := record.get("mongo_attr"):
+        pretty = json.dumps(mongo_attr, indent=2)
+        compact = json.dumps(mongo_attr, separators=(",", ":"))
+        attr = pretty if "Slow query" in msg else compact
+        if color:
+            attr = highlight(attr, json_lexer, term_formatter)
+        if color and "Slow query" in msg:
+            ms = int(re.sub(r'.*"durationMillis":(\d+).*', r"\1", compact))
+            clr = "green" if ms < 500 else "yellow" if ms < 10000 else "red"
+            attr = re.sub(str(ms), sformat(str(ms), "bold", clr), attr)
+        attr = attr.rstrip()
+        join = "\n" if "\n" in attr else " "
+        msg += f"{join}{attr}"
+    # multiline -> indent
+    msg = msg.replace("\n", "\n  ")
     # put together the output parts
     parts = []
     parts.append(f"{time:>23.23}")
     parts.append(lvl)
     if pod:
         # TODO globally track pods and pad to max len
         # TODO add colors (keep or strip+re-color stern)
         parts.append(pod)
-    caller = record.get("caller")
-    if caller:
+    if caller := record.get("caller"):
         parts.append(sformat(caller, "blue") if color else caller)
     parts.append(msg)
     return " ".join(parts)
 
 
 ansi_re = r"(\x9B|\x1B\[)[0-?]*[ -\/]*[@-~]"
 pod_re = rf"""
@@ -447,26 +450,23 @@
     msg = f"({action}) {msg}" if action else msg
     # perimeter heartbeat: suffix stats
     stats = record.get("stats")
     msg = f"{msg} {stats}" if stats else msg
     # fw-logging:exc / flywheel-common:exc_info
     exc = record.get("exc") or record.get("exc_info")
     msg = f"{msg}\n{exc}" if exc else msg
-    # long queries in json format, mongodb 4.4 by default logs in json
-    if msg == "Slow query" and record.get("attr"):
-        exc = json.dumps(record["attr"], indent=2)
-        msg = f"{msg}\n{exc}"
     # engine:err - usually a single line
     if record.get("err"):
         msg = f"{msg}: {record['err']}"
     return dict(
         time=time,
         lvl=lvl,
         caller=caller,
         msg=msg,
+        mongo_attr=record.get("attr"),
     )
 
 
 def add_log_level(name: str, num: int) -> None:
     """Add a custom log level to the logging module.
 
     * add `name.upper()` attribute to the logging module with value num.
```

## Comparing `fw_logging-1.2.2.dist-info/LICENSE` & `fw_logging-1.2.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fw_logging-1.2.2.dist-info/METADATA` & `fw_logging-1.2.3.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fw-logging
-Version: 1.2.2
+Version: 1.2.3
 Summary: Logging helper library.
 Home-page: https://gitlab.com/flywheel-io/tools/lib/fw-logging
 License: MIT
 Keywords: Flywheel,helper,logging
 Author: Flywheel
 Author-email: support@flywheel.io
 Requires-Python: >=3.8,<4.0
@@ -12,15 +12,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: devtools (>=0,<1)
-Requires-Dist: pydantic (>=1.6.1,<2.0.0)
+Requires-Dist: pydantic (>=2.1.1,<3.0.0)
+Requires-Dist: pydantic-settings (>=2.0.2,<3.0.0)
 Requires-Dist: pygments (>=2.13.0,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: striprtf (>=0,<1)
 Project-URL: Repository, https://gitlab.com/flywheel-io/tools/lib/fw-logging
 Description-Content-Type: text/markdown
 
 # fw-logging
```

