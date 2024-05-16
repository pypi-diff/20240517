# Comparing `tmp/nadl-1.2.0.tar.gz` & `tmp/nadl-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nadl-1.2.0.tar", last modified: Tue May 14 05:07:44 2024, max compression
+gzip compressed data, was "nadl-1.3.0.tar", last modified: Thu May 16 22:59:49 2024, max compression
```

## Comparing `nadl-1.2.0.tar` & `nadl-1.3.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     2243 2024-05-14 05:07:44.948155 nadl-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.2.0/readme.org
--rw-r--r--   0        0        0     1687 2024-05-14 05:06:30.746531 nadl-1.2.0/src/nadl/__init__.py
--rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.2.0/src/nadl/blocks.py
--rw-r--r--   0        0        0     5343 2024-05-14 05:05:57.551156 nadl-1.2.0/src/nadl/data.py
--rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.2.0/src/nadl/images.py
--rw-r--r--   0        0        0     3170 2024-04-22 06:27:49.753850 nadl-1.2.0/src/nadl/keys.py
--rw-r--r--   0        0        0     4348 2024-05-14 05:03:33.511530 nadl-1.2.0/src/nadl/loops.py
--rw-r--r--   0        0        0     1828 2024-04-19 19:57:58.670986 nadl-1.2.0/src/nadl/metrics.py
--rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.2.0/src/nadl/nets.py
--rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.2.0/src/nadl/preprocessing.py
--rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.2.0/src/nadl/py.typed
--rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.2.0/src/nadl/transformers.py
--rw-r--r--   0        0        0     1964 2024-04-22 04:28:48.528308 nadl-1.2.0/src/nadl/utils.py
--rw-r--r--   0        0        0     1328 1970-01-01 00:00:00.000000 nadl-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2275 2024-05-16 22:59:49.513755 nadl-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.3.0/readme.org
+-rw-r--r--   0        0        0     1784 2024-05-16 22:59:08.461595 nadl-1.3.0/src/nadl/__init__.py
+-rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.3.0/src/nadl/blocks.py
+-rw-r--r--   0        0        0     5343 2024-05-14 05:05:57.551156 nadl-1.3.0/src/nadl/data.py
+-rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.3.0/src/nadl/images.py
+-rw-r--r--   0        0        0     3170 2024-04-22 06:27:49.753850 nadl-1.3.0/src/nadl/keys.py
+-rw-r--r--   0        0        0     3986 2024-05-14 05:17:02.160133 nadl-1.3.0/src/nadl/loops.py
+-rw-r--r--   0        0        0     1828 2024-04-19 19:57:58.670986 nadl-1.3.0/src/nadl/metrics.py
+-rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.3.0/src/nadl/nets.py
+-rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.3.0/src/nadl/preprocessing.py
+-rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.3.0/src/nadl/py.typed
+-rw-r--r--   0        0        0     3884 2024-05-15 03:21:02.151713 nadl-1.3.0/src/nadl/states.py
+-rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.3.0/src/nadl/transformers.py
+-rw-r--r--   0        0        0     2363 2024-05-14 05:16:59.307787 nadl-1.3.0/src/nadl/utils.py
+-rw-r--r--   0        0        0     1368 1970-01-01 00:00:00.000000 nadl-1.3.0/PKG-INFO
```

### Comparing `nadl-1.2.0/pyproject.toml` & `nadl-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,18 @@
     "numpy>=1.26.4",
     "rich>=13.7.1",
     "jaxtyping>=0.2.28",
     "optax>=0.2.2",
     "equinox>=0.11.4",
     "beartype>=0.18.5",
     "scikit-image>=0.23.2",
+    "orbax-checkpoint>=0.5.11",
 ]
 requires-python = ">=3.12"
-version = "1.2.0"
+version = "1.3.0"
 
 [project.readme]
 content-type = "text/plain"
 file = "readme.org"
 
 [project.license]
 text = "GPLv3"
```

### Comparing `nadl-1.2.0/readme.org` & `nadl-1.3.0/readme.org`

 * *Files identical despite different names*

### Comparing `nadl-1.2.0/src/nadl/__init__.py` & `nadl-1.3.0/src/nadl/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,32 +36,34 @@
 """
 
 from .data import DState, IdxDataloader, es_loop
 from .keys import Keys, new_key
 from .loops import PG
 from .metrics import dice_coef, iou_coef
 from .preprocessing import (
-  SCALER,
-  identity_scaler,
-  min_max_scaler,
-  normalizer,
-  select_scaler,
-  standard_scaler,
+    SCALER,
+    identity_scaler,
+    min_max_scaler,
+    normalizer,
+    select_scaler,
+    standard_scaler,
 )
+from .states import BaseTrainState, state_fn
 from .utils import (
-  classit,
-  rle,
-  rle_array,
+    classit,
+    rle,
+    rle_array,
 )
 
-__version__ = "1.2.0"
+__version__ = "1.3.0"
 
 __all__ = [
   "PG",
   "SCALER",
+  "BaseTrainState",
   "DState",
   "IdxDataloader",
   "Keys",
   "classit",
   "dice_coef",
   "es_loop",
   "identity_scaler",
@@ -69,8 +71,9 @@
   "min_max_scaler",
   "new_key",
   "normalizer",
   "rle",
   "rle_array",
   "select_scaler",
   "standard_scaler",
+  "state_fn",
 ]
```

### Comparing `nadl-1.2.0/src/nadl/blocks.py` & `nadl-1.3.0/src/nadl/blocks.py`

 * *Files identical despite different names*

### Comparing `nadl-1.2.0/src/nadl/data.py` & `nadl-1.3.0/src/nadl/data.py`

 * *Files identical despite different names*

### Comparing `nadl-1.2.0/src/nadl/images.py` & `nadl-1.3.0/src/nadl/images.py`

 * *Files identical despite different names*

### Comparing `nadl-1.2.0/src/nadl/keys.py` & `nadl-1.3.0/src/nadl/keys.py`

 * *Files identical despite different names*

### Comparing `nadl-1.2.0/src/nadl/loops.py` & `nadl-1.3.0/src/nadl/loops.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 license  : GPL-3.0+
 
 Train Eval Loops
 """
 
 from collections.abc import Hashable, Mapping
 
-import jax
 from equinox import Module
 
 from types import TracebackType
 from typing import Any, Self
 
 from rich.console import Console
 from rich.progress import (
@@ -51,14 +50,16 @@
   TaskID,
   TextColumn,
   TimeElapsedColumn,
   TimeRemainingColumn,
 )
 from rich.theme import Theme
 
+from .utils import pformat
+
 DEF_LIGHT_THEME = Theme({
   "bar.back": "#50616D",
   "bar.complete": "#D3CBAF",
   "bar.finished": "#b49b7f",
 })
 
 
@@ -137,28 +138,20 @@
     exc_type: type[BaseException] | None,
     exc_val: BaseException | None,
     exc_tb: TracebackType | None,
   ) -> None:
     """Exit."""
     self.pg.__exit__(exc_type, exc_val, exc_tb)
 
-  @staticmethod
-  def pformat(xs: Mapping[str, float | int | str | None]) -> str:
-    """Pretty format progress results."""
-    with (console := Console()).capture() as capture:
-      nxs = jax.tree.map(lambda x: float(f"{x:.4f}") if isinstance(x, float) else x, xs)
-      console.print(nxs, soft_wrap=True, justify="left", no_wrap=True, width=40)
-    return capture.get()
-
   def update_res(
     self, name: str, updates: Mapping[str, float | int | str | None]
   ) -> None:
     """Update res."""
     if name in self.tasks:
-      self.pg.update(self.tasks[name], res=self.pformat(updates))
+      self.pg.update(self.tasks[name], res=pformat(updates))
 
 
 def test() -> None:
   """Test progress."""
   import time  # noqa: PLC0415
 
   pg = PG.init_progress()
```

### Comparing `nadl-1.2.0/src/nadl/metrics.py` & `nadl-1.3.0/src/nadl/metrics.py`

 * *Files identical despite different names*

### Comparing `nadl-1.2.0/src/nadl/nets.py` & `nadl-1.3.0/src/nadl/nets.py`

 * *Files identical despite different names*

### Comparing `nadl-1.2.0/src/nadl/preprocessing.py` & `nadl-1.3.0/src/nadl/preprocessing.py`

 * *Files identical despite different names*

### Comparing `nadl-1.2.0/src/nadl/transformers.py` & `nadl-1.3.0/src/nadl/transformers.py`

 * *Files identical despite different names*

### Comparing `nadl-1.2.0/src/nadl/utils.py` & `nadl-1.3.0/src/nadl/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,17 +31,19 @@
 filename : utils.py
 project  : nadl
 license  : GPL-3.0+
 
 Utils
 """
 
+from collections.abc import Mapping
 from typing import Literal
 import jax
 import jax.numpy as jnp
+from rich.console import Console
 
 
 def rle_array(x: jax.Array, shift: int = 1) -> jax.Array:
   """Run length encoding array."""
   x = x.flatten()
   x = jnp.pad(x, (1, 1), mode="constant")
   x = jnp.argwhere(x[1:] != x[:-1]).flatten() + shift
@@ -65,7 +67,15 @@
     case "softmax":
       x = jax.nn.softmax(x)
       return jnp.argmax(x, axis=-1, keepdims=True)
     case "threshold":
       return x > threshold
     case _:
       raise ValueError(f"Unknown method {method}")
+
+
+def pformat(xs: Mapping[str, float | int | str | None]) -> str:
+  """Pretty format."""
+  with (console := Console()).capture() as capture:
+    nxs = jax.tree.map(lambda x: float(f"{x:.4f}") if isinstance(x, float) else x, xs)
+    console.print(nxs, soft_wrap=True, justify="left", no_wrap=True, width=40)
+  return capture.get()
```

### Comparing `nadl-1.2.0/PKG-INFO` & `nadl-1.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: nadl
-Version: 1.2.0
+Version: 1.3.0
 Summary: Nasy's Deep Learning Toolkit
 Author-Email: Nasy <nasyxx+python@gmail.com>, Nasy <nasyxx+dl@gmail.com>, Nasy <nasyxx+git@gmail.com>
 License: GPLv3
 Requires-Python: >=3.12
 Requires-Dist: jax>=0.4.28
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: rich>=13.7.1
 Requires-Dist: jaxtyping>=0.2.28
 Requires-Dist: optax>=0.2.2
 Requires-Dist: equinox>=0.11.4
 Requires-Dist: beartype>=0.18.5
 Requires-Dist: scikit-image>=0.23.2
+Requires-Dist: orbax-checkpoint>=0.5.11
 Requires-Dist: mkdocs-material>=9.5.22; extra == "doc"
 Requires-Dist: mkdocs>=1.6.0; extra == "doc"
 Requires-Dist: mike>=2.1.1; extra == "doc"
 Requires-Dist: mkdocstrings[python]>=0.25.1; extra == "doc"
 Provides-Extra: doc
 Description-Content-Type: text/plain
```

