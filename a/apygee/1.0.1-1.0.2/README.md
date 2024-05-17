# Comparing `tmp/apygee-1.0.1.tar.gz` & `tmp/apygee-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apygee-1.0.1.tar", max compression
+gzip compressed data, was "apygee-1.0.2.tar", max compression
```

## Comparing `apygee-1.0.1.tar` & `apygee-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1060 2024-05-15 20:02:54.236495 apygee-1.0.1/LICENSE.md
--rw-r--r--   0        0        0     1072 2024-05-15 20:02:54.240495 apygee-1.0.1/README.md
--rw-r--r--   0        0        0      555 2024-05-15 20:02:54.240495 apygee-1.0.1/apygee/__init__.py
--rw-r--r--   0        0        0     4014 2024-05-15 20:02:54.240495 apygee-1.0.1/apygee/constants.py
--rw-r--r--   0        0        0    10159 2024-05-15 20:02:54.240495 apygee-1.0.1/apygee/kepler.py
--rw-r--r--   0        0        0     2863 2024-05-15 20:02:54.240495 apygee-1.0.1/apygee/nb.py
--rw-r--r--   0        0        0    37115 2024-05-15 20:02:54.240495 apygee-1.0.1/apygee/orbit.py
--rw-r--r--   0        0        0    19124 2024-05-15 20:02:54.240495 apygee-1.0.1/apygee/plot.py
--rw-r--r--   0        0        0     6234 2024-05-15 20:02:54.240495 apygee-1.0.1/apygee/utils.py
--rw-r--r--   0        0        0      716 2024-05-15 20:02:54.244495 apygee-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1598 1970-01-01 00:00:00.000000 apygee-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-05-17 17:20:32.270526 apygee-1.0.2/LICENSE.md
+-rw-r--r--   0        0        0    10812 2024-05-17 17:20:32.270526 apygee-1.0.2/README.md
+-rw-r--r--   0        0        0      555 2024-05-17 17:20:32.270526 apygee-1.0.2/apygee/__init__.py
+-rw-r--r--   0        0        0     4014 2024-05-17 17:20:32.270526 apygee-1.0.2/apygee/constants.py
+-rw-r--r--   0        0        0    10159 2024-05-17 17:20:32.270526 apygee-1.0.2/apygee/kepler.py
+-rw-r--r--   0        0        0     2863 2024-05-17 17:20:32.270526 apygee-1.0.2/apygee/nb.py
+-rw-r--r--   0        0        0    37115 2024-05-17 17:20:32.270526 apygee-1.0.2/apygee/orbit.py
+-rw-r--r--   0        0        0    19714 2024-05-17 17:20:32.270526 apygee-1.0.2/apygee/plot.py
+-rw-r--r--   0        0        0     6262 2024-05-17 17:20:32.270526 apygee-1.0.2/apygee/utils.py
+-rw-r--r--   0        0        0      734 2024-05-17 17:20:32.278525 apygee-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    11377 1970-01-01 00:00:00.000000 apygee-1.0.2/PKG-INFO
```

### Comparing `apygee-1.0.1/LICENSE.md` & `apygee-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `apygee-1.0.1/apygee/__init__.py` & `apygee-1.0.2/apygee/__init__.py`

 * *Files identical despite different names*

### Comparing `apygee-1.0.1/apygee/constants.py` & `apygee-1.0.2/apygee/constants.py`

 * *Files identical despite different names*

### Comparing `apygee-1.0.1/apygee/kepler.py` & `apygee-1.0.2/apygee/kepler.py`

 * *Files identical despite different names*

### Comparing `apygee-1.0.1/apygee/nb.py` & `apygee-1.0.2/apygee/nb.py`

 * *Files identical despite different names*

### Comparing `apygee-1.0.1/apygee/orbit.py` & `apygee-1.0.2/apygee/orbit.py`

 * *Files identical despite different names*

### Comparing `apygee-1.0.1/apygee/plot.py` & `apygee-1.0.2/apygee/plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from matplotlib.colors import to_rgba
+from typing import Unpack, TypedDict
 from numpy.typing import ArrayLike
 
 import matplotlib.pyplot as plt
 import numpy as np
 
+from matplotlib.colors import to_rgba
 from mpl_toolkits.mplot3d.art3d import Patch3D
 from matplotlib.patches import Arc, FancyArrowPatch
 from matplotlib.transforms import Bbox, IdentityTransform, TransformedBbox
 from mpl_toolkits.mplot3d.proj3d import proj_transform
 
 from apygee.utils import mix_colors, omit
 
@@ -30,30 +31,48 @@
         ax = fig.gca()
     else:
         ax = fig.add_subplot(projection="3d")
 
     return ax
 
 
-def plot_vector(*args, ax=None, **kwargs):
+class VectorKwargs(TypedDict):
+    origin: ArrayLike
+    text: str | dict
+    color: str
+    plot_components: bool
+    arrow_kwargs: dict
+    text_kwargs: dict
+
+
+def plot_vector(v: ArrayLike, ax=None, **kwargs: Unpack[VectorKwargs]):
     ax = ax or plt.gca()
 
     if ax.name == "3d":
-        plot_vector_3d(*args, ax=ax, **kwargs)
+        plot_vector_3d(v, ax=ax, **kwargs)
     else:
-        plot_vector_2d(*args, ax=ax, **kwargs)
+        plot_vector_2d(v, ax=ax, **kwargs)
 
 
-def plot_angle(*args, ax=None, **kwargs):
+class AngleKwargs(TypedDict):
+    origin: ArrayLike
+    text: str
+    radius: float
+    unit: str
+    angle_kwargs: dict
+    text_kwargs: dict
+
+
+def plot_angle(v1: ArrayLike, v2: ArrayLike, ax=None, **kwargs: Unpack[AngleKwargs]):
     ax = ax or plt.gca()
 
     if ax.name == "3d":
-        plot_angle_3d(*args, ax=ax, **kwargs)
+        plot_angle_3d(v1, v2, ax=ax, **kwargs)
     else:
-        plot_angle_2d(*args, ax=ax, **kwargs)
+        plot_angle_2d(v1, v2, ax=ax, **kwargs)
 
 
 def plot_vector_2d(
     v: ArrayLike,
     origin=[0, 0],
     text: str | dict = None,
     ax=None,
@@ -68,15 +87,19 @@
 
     _color = plot_dummy_line(np.stack([origin, origin + v]).T, ax=ax)
     if color is None:
         color = _color
 
     arrow_kwargs = {**arrow_kwargs}
     zorder = arrow_kwargs.pop("zorder", None)
-    arrowprops = {"width": 1.5, "headwidth": 9, "headlength": 9, **arrow_kwargs}
+
+    if "arrowstyle" in arrow_kwargs:
+        arrowprops = {**arrow_kwargs}
+    else:
+        arrowprops = {"width": 1.5, "headwidth": 9, "headlength": 9, **arrow_kwargs}
 
     if plot_components:
         ax.annotate(
             "",
             xy=origin + [v[0], 0],
             xytext=origin,
             xycoords="data",
@@ -108,15 +131,15 @@
 
     # Plot main vector after to ensure it's on top
     ax.annotate(
         "",
         xy=origin + v,
         xytext=origin,
         xycoords="data",
-        arrowprops={**arrowprops, "color": color},
+        arrowprops={"color": color, **arrowprops},
         zorder=zorder,
     )
 
     if text is None:
         return
 
     bg = ax.get_facecolor()
@@ -167,14 +190,15 @@
     plot_components=False,
     arrow_kwargs={},
     text_kwargs={},
 ) -> None:
     origin = np.asarray(origin).ravel()[:3]
     v = np.asarray(v).ravel()[:3]
     ax = ax or get_3d_axes()
+    ax.computed_zorder = False
 
     _color = plot_dummy_line(np.stack([origin, origin + v]).T, ax=ax)
     if color is None:
         color = _color
 
     vtext = text if text is None or isinstance(text, str) else text.get("v")
 
@@ -233,16 +257,16 @@
     if radius is None:
         [vn1, vn2] = [np.linalg.norm(v) for v in [v1, v2]]
         vnmin = min(vn1, vn2)
         radius = 0.3 * vnmin
 
     _angle = AngleAnnotation(
         origin,
-        v1,
-        v2,
+        origin + v1,
+        origin + v2,
         ax=ax,
         size=2 * radius,
         unit=unit,
         text=text,
         textposition="inside",
         text_kwargs=text_kwargs,
         angle_kwargs=angle_kwargs,
@@ -260,27 +284,28 @@
     angle_kwargs={},
     text_kwargs={},
 ) -> None:
     origin = np.asarray(origin).ravel()[:3]
     v1 = np.asarray(v1).ravel()[:3]
     v2 = np.asarray(v2).ravel()[:3]
     ax = ax or get_3d_axes()
+    ax.computed_zorder = False
 
     if radius is None:
         [vn1, vn2] = [np.linalg.norm(v) for v in [v1, v2]]
         vnmin = min(vn1, vn2)
         radius = vnmin
 
     v = v1 - v2
     pts = np.apply_along_axis(
         lambda x: v2 + v * x, 1, np.linspace(0, 1, num=100)[None, :].repeat(3, 0).T
     )
     phis = np.arctan2(pts[:, 1], pts[:, 0])
     thetas = np.arccos(pts[:, 2] / np.linalg.norm(pts, axis=-1))
-    arc = np.stack(
+    arc = origin + np.stack(
         [
             radius * np.sin(thetas) * np.cos(phis),
             radius * np.sin(thetas) * np.sin(phis),
             radius * np.cos(thetas),
         ],
         axis=-1,
     )
```

### Comparing `apygee-1.0.1/apygee/utils.py` & `apygee-1.0.2/apygee/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,17 @@
     b = np.asarray(b, dtype=np.float64)
     return np.sum(a * b, axis=-1)
 
 
 def angle_between(a: ArrayLike, b: ArrayLike) -> float:
     a = np.asarray(a, dtype=np.float64)
     b = np.asarray(b, dtype=np.float64)
-    return np.arccos(np.clip(np.dot(a, b) / (np.linalg.norm(a) * np.linalg.norm(b)), -1, 1))
+    return np.round(
+        np.arccos(np.clip(np.dot(a, b) / (np.linalg.norm(a) * np.linalg.norm(b)), -1, 1)), 15
+    )
 
 
 def mix_colors(
     color1: str | tuple[float],
     color2: str | tuple[float],
     fraction: float = 0.5,
 ) -> str:
```

### Comparing `apygee-1.0.1/pyproject.toml` & `apygee-1.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "apygee"
-version = "1.0.1"
+version = "1.0.2"
 description = "A package for creating, manipulating and visualizing Kepler orbits"
 authors = ["Jelmar Gerritsen <jelmargerritsen@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 matplotlib = "^3.8.3"
 numpy = "^1.26.4"
 plotly = "^5.20.0"
 ipywidgets = "^8.1.2"
+pandas = "^2.2.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.0"
 ipykernel = "^6.29.2"
 ruff = "^0.3.2"
 ipympl = "^0.9.3"
```

