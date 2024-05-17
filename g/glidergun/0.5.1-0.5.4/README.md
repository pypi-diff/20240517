# Comparing `tmp/glidergun-0.5.1.tar.gz` & `tmp/glidergun-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glidergun-0.5.1.tar", last modified: Wed Mar 13 11:48:25 2024, max compression
+gzip compressed data, was "glidergun-0.5.4.tar", last modified: Fri May 17 02:15:41 2024, max compression
```

## Comparing `glidergun-0.5.1.tar` & `glidergun-0.5.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-13 11:48:25.238562 glidergun-0.5.1/
--rw-r--r--   0 codespace  (1000) codespace  (1000)     2643 2024-03-13 11:48:25.238562 glidergun-0.5.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1980 2024-03-13 11:19:42.000000 glidergun-0.5.1/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-13 11:48:25.234562 glidergun-0.5.1/glidergun/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      408 2024-03-11 11:44:46.000000 glidergun-0.5.1/glidergun/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    48044 2024-03-13 11:41:38.000000 glidergun-0.5.1/glidergun/grid.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3743 2024-03-13 11:41:35.000000 glidergun-0.5.1/glidergun/ipython.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1663 2024-03-11 11:44:46.000000 glidergun-0.5.1/glidergun/literals.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9981 2024-03-13 11:41:32.000000 glidergun-0.5.1/glidergun/stack.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-13 11:48:25.238562 glidergun-0.5.1/glidergun.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)     2643 2024-03-13 11:48:25.000000 glidergun-0.5.1/glidergun.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      290 2024-03-13 11:48:25.000000 glidergun-0.5.1/glidergun.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-03-13 11:48:25.000000 glidergun-0.5.1/glidergun.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       68 2024-03-13 11:48:25.000000 glidergun-0.5.1/glidergun.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       10 2024-03-13 11:48:25.000000 glidergun-0.5.1/glidergun.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      714 2024-03-13 01:23:47.000000 glidergun-0.5.1/pyproject.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-03-13 11:48:25.238562 glidergun-0.5.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 02:15:41.765731 glidergun-0.5.4/
+-rw-rw-rw-   0        0        0     2832 2024-05-17 02:15:41.764395 glidergun-0.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2148 2024-04-24 03:01:21.000000 glidergun-0.5.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 02:15:41.734629 glidergun-0.5.4/glidergun/
+-rw-rw-rw-   0        0        0      438 2024-05-17 02:12:31.000000 glidergun-0.5.4/glidergun/__init__.py
+-rw-rw-rw-   0        0        0    50020 2024-05-17 02:12:30.000000 glidergun-0.5.4/glidergun/_grid.py
+-rw-rw-rw-   0        0        0     4099 2024-05-17 02:12:37.000000 glidergun-0.5.4/glidergun/_ipython.py
+-rw-rw-rw-   0        0        0     1783 2024-04-24 03:01:21.000000 glidergun-0.5.4/glidergun/_literals.py
+-rw-rw-rw-   0        0        0    10367 2024-05-17 02:12:25.000000 glidergun-0.5.4/glidergun/_stack.py
+drwxrwxrwx   0        0        0        0 2024-05-17 02:15:41.762972 glidergun-0.5.4/glidergun.egg-info/
+-rw-rw-rw-   0        0        0     2832 2024-05-17 02:15:41.000000 glidergun-0.5.4/glidergun.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2024-05-17 02:15:41.000000 glidergun-0.5.4/glidergun.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 02:15:41.000000 glidergun-0.5.4/glidergun.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-05-17 02:15:41.000000 glidergun-0.5.4/glidergun.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-17 02:15:41.000000 glidergun-0.5.4/glidergun.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      746 2024-05-17 02:11:20.000000 glidergun-0.5.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-17 02:15:41.767201 glidergun-0.5.4/setup.cfg
```

### Comparing `glidergun-0.5.1/PKG-INFO` & `glidergun-0.5.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,189 +1,189 @@
-Metadata-Version: 2.1
-Name: glidergun
-Version: 0.5.1
-Summary: Map Algebra with NumPy
-Author-email: Jiro Shirota <jshirota@gmail.com>
-Project-URL: Homepage, https://github.com/jshirota/glidergun
-Project-URL: Bug Tracker, https://github.com/jshirota/glidergun/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Requires-Dist: folium
-Requires-Dist: ipython
-Requires-Dist: matplotlib
-Requires-Dist: numpy
-Requires-Dist: rasterio
-Requires-Dist: scikit-learn
-Requires-Dist: scipy
-Requires-Dist: shapely
-
-# glidergun
-
-```
-pip install glidergun
-```
-
-### Overview
-
-[![Glidergun](https://img.youtube.com/vi/pbVG4bNb96Y/0.jpg)](https://youtu.be/pbVG4bNb96Y)
-
-## creation / io
-
-- grid
-- stack
-- save
-
-## operators
-
-- most overloadable Python operators
-
-## properties
-
-- width
-- height
-- dtype
-- xmin
-- ymin
-- xmax
-- ymax
-- extent
-- mean
-- std
-- min
-- max
-- cell_size
-- bins
-- md5
-
-## local
-
-- local (higher order)
-- is_nan
-- abs
-- sin
-- cos
-- tan
-- arcsin
-- arccos
-- arctan
-- log
-- round
-- gaussian_filter
-- gaussian_gradient_magnitude
-- gaussian_laplace
-- prewitt
-- sobel
-- uniform_filter
-- uniform_filter1d
-
-## focal
-
-- focal (higher order)
-- focal_count
-- focal_mean
-- focal_std
-- focal_var
-- focal_median
-- focal_min
-- focal_max
-- focal_sum
-- focal_ptp
-- focal_percentile
-- focal_quantile
-- focal_entropy
-- focal_hmean
-- focal_pmean
-- focal_kurtosis
-- focal_iqr
-- focal_mode
-- focal_moment
-- focal_skew
-- focal_kstat
-- focal_kstatvar
-- focal_tmean
-- focal_tvar
-- focal_tmin
-- focal_tmax
-- focal_tstd
-- focal_variation
-- focal_median_abs_deviation
-- focal_chisquare
-- focal_ttest_ind
-
-## zonal
-
-- zonal (higher order)
-- zonal_count
-- zonal_mean
-- zonal_std
-- zonal_var
-- zonal_median
-- zonal_min
-- zonal_max
-- zonal_sum
-- zonal_ptp
-- zonal_percentile
-- zonal_quantile
-- zonal_entropy
-- zonal_hmean
-- zonal_pmean
-- zonal_kurtosis
-- zonal_iqr
-- zonal_mode
-- zonal_moment
-- zonal_skew
-- zonal_kstat
-- zonal_kstatvar
-- zonal_tmean
-- zonal_tvar
-- zonal_tmin
-- zonal_tmax
-- zonal_tstd
-- zonal_variation
-- zonal_median_abs_deviation
-
-## interpolation
-
-- interpolate (higher order)
-- interp_linear
-- interp_nearest
-- interp_rbf
-
-## regression / classification
-
-- fit (higher order)
-
-## surface
-
-- aspect
-- slope
-- hillshade
-
-## conversion, etc.
-
-- buffer
-- clip
-- con
-- fill_nan
-- from_polygons
-- mosaic
-- pca
-- percent_clip
-- project
-- randomize
-- reclass
-- replace
-- resample
-- scale
-- set_nan
-- standardize
-- to_points
-- to_polygons
-- to_stack
-
-## ipython
-
-- plot (Matplotlib)
-- map (Folium)
+Metadata-Version: 2.1
+Name: glidergun
+Version: 0.5.4
+Summary: Map Algebra with NumPy
+Author-email: Jiro Shirota <jshirota@gmail.com>
+Project-URL: Homepage, https://github.com/jshirota/glidergun
+Project-URL: Bug Tracker, https://github.com/jshirota/glidergun/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Requires-Dist: folium
+Requires-Dist: ipython
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: rasterio
+Requires-Dist: scikit-learn
+Requires-Dist: scipy
+Requires-Dist: shapely
+
+# glidergun
+
+```
+pip install glidergun
+```
+
+### Overview
+
+[![Glidergun](https://img.youtube.com/vi/pbVG4bNb96Y/0.jpg)](https://youtu.be/pbVG4bNb96Y)
+
+## creation / io
+
+- grid
+- stack
+- save
+
+## operators
+
+- most overloadable Python operators
+
+## properties
+
+- width
+- height
+- dtype
+- xmin
+- ymin
+- xmax
+- ymax
+- extent
+- mean
+- std
+- min
+- max
+- cell_size
+- bins
+- md5
+
+## local
+
+- local (higher order)
+- is_nan
+- abs
+- sin
+- cos
+- tan
+- arcsin
+- arccos
+- arctan
+- log
+- round
+- gaussian_filter
+- gaussian_gradient_magnitude
+- gaussian_laplace
+- prewitt
+- sobel
+- uniform_filter
+- uniform_filter1d
+
+## focal
+
+- focal (higher order)
+- focal_count
+- focal_mean
+- focal_std
+- focal_var
+- focal_median
+- focal_min
+- focal_max
+- focal_sum
+- focal_ptp
+- focal_percentile
+- focal_quantile
+- focal_entropy
+- focal_hmean
+- focal_pmean
+- focal_kurtosis
+- focal_iqr
+- focal_mode
+- focal_moment
+- focal_skew
+- focal_kstat
+- focal_kstatvar
+- focal_tmean
+- focal_tvar
+- focal_tmin
+- focal_tmax
+- focal_tstd
+- focal_variation
+- focal_median_abs_deviation
+- focal_chisquare
+- focal_ttest_ind
+
+## zonal
+
+- zonal (higher order)
+- zonal_count
+- zonal_mean
+- zonal_std
+- zonal_var
+- zonal_median
+- zonal_min
+- zonal_max
+- zonal_sum
+- zonal_ptp
+- zonal_percentile
+- zonal_quantile
+- zonal_entropy
+- zonal_hmean
+- zonal_pmean
+- zonal_kurtosis
+- zonal_iqr
+- zonal_mode
+- zonal_moment
+- zonal_skew
+- zonal_kstat
+- zonal_kstatvar
+- zonal_tmean
+- zonal_tvar
+- zonal_tmin
+- zonal_tmax
+- zonal_tstd
+- zonal_variation
+- zonal_median_abs_deviation
+
+## interpolation
+
+- interpolate (higher order)
+- interp_linear
+- interp_nearest
+- interp_rbf
+
+## regression / classification
+
+- fit (higher order)
+
+## surface
+
+- aspect
+- slope
+- hillshade
+
+## conversion, etc.
+
+- buffer
+- clip
+- con
+- fill_nan
+- from_polygons
+- mosaic
+- pca
+- percent_clip
+- project
+- randomize
+- reclass
+- replace
+- resample
+- scale
+- set_nan
+- standardize
+- to_points
+- to_polygons
+- to_stack
+
+## ipython
+
+- plot (Matplotlib)
+- map (Folium)
```

### Comparing `glidergun-0.5.1/glidergun/grid.py` & `glidergun-0.5.4/glidergun/_grid.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,1561 +1,1574 @@
-import dataclasses
-import hashlib
-import pickle
-import sys
-from dataclasses import dataclass
-from typing import (
-    Any,
-    Callable,
-    Dict,
-    Generic,
-    Iterable,
-    List,
-    NamedTuple,
-    Optional,
-    Protocol,
-    Tuple,
-    TypeVar,
-    Union,
-    cast,
-    overload,
-)
-
-import matplotlib.pyplot as plt
-import numpy as np
-import rasterio
-import scipy as sp
-from numpy import arctan, arctan2, cos, gradient, ndarray, pi, sin, sqrt
-from numpy.lib.stride_tricks import sliding_window_view
-from rasterio import features
-from rasterio.crs import CRS
-from rasterio.drivers import driver_from_extension
-from rasterio.io import MemoryFile
-from rasterio.transform import Affine
-from rasterio.warp import Resampling, calculate_default_transform, reproject
-from scipy.interpolate import (
-    LinearNDInterpolator,
-    NearestNDInterpolator,
-    RBFInterpolator,
-)
-from shapely import Polygon
-from sklearn.decomposition import PCA
-from sklearn.preprocessing import QuantileTransformer, StandardScaler
-
-from glidergun.literals import (
-    ColorMap,
-    DataType,
-    ExtentResolution,
-    InterpolationKernel,
-    ResamplingMethod,
-)
-
-
-class Extent(NamedTuple):
-    xmin: float
-    ymin: float
-    xmax: float
-    ymax: float
-
-    def intersect(self, extent: "Extent"):
-        return Extent(*[f(x) for f, x in zip((max, max, min, min), zip(self, extent))])
-
-    def union(self, extent: "Extent"):
-        return Extent(*[f(x) for f, x in zip((min, min, max, max), zip(self, extent))])
-
-    __and__ = intersect
-    __rand__ = __and__
-    __or__ = union
-    __ror__ = __or__
-
-
-Operand = Union["Grid", float, int]
-
-
-class CellSize(NamedTuple):
-    x: float
-    y: float
-
-    def __mul__(self, n: float):
-        return CellSize(self.x * n, self.y * n)
-
-    def __rmul__(self, n: float):
-        return CellSize(self.x * n, self.y * n)
-
-    def __truediv__(self, n: float):
-        return CellSize(self.x / n, self.y / n)
-
-
-class Point(NamedTuple):
-    x: float
-    y: float
-    value: float
-
-
-class Estimator(Protocol):
-    fit: Callable
-    score: Callable
-    predict: Callable
-
-
-T = TypeVar("T", bound=Estimator)
-
-
-class GridEstimator(Generic[T]):
-    def __init__(self, model: T) -> None:
-        self.model: T = model
-        self._dtype: DataType = "float32"
-
-    def fit(self, dependent_grid: "Grid", *explanatory_grids: "Grid"):
-        head, *tail = self._flatten(*[dependent_grid, *explanatory_grids])
-        self.model = self.model.fit(
-            np.array([g.data.ravel() for g in tail]).transpose(1, 0),
-            head.data.ravel(),
-        )
-        self._dtype = dependent_grid.dtype
-        return self
-
-    def score(self, dependent_grid: "Grid", *explanatory_grids: "Grid") -> float:
-        head, *tail = self._flatten(dependent_grid, *explanatory_grids)
-        return self.model.score(
-            np.array([g.data.ravel() for g in tail]).transpose(1, 0), head.data.ravel()
-        )
-
-    def predict(self, *explanatory_grids: "Grid") -> "Grid":
-        grids = self._flatten(*explanatory_grids)
-        array = self.model.predict(
-            np.array([g.data.ravel() for g in grids]).transpose(1, 0)
-        )
-        grid = grids[0]
-        return grid._create(array.reshape((grid.height, grid.width))).type(self._dtype)
-
-    def _flatten(self, *grids: "Grid"):
-        return [con(g.is_nan(), g.mean, g) for g in standardize(*grids)]
-
-    def save(self, file: str):
-        with open(file, "wb") as f:
-            pickle.dump(self.model, f)
-
-    @classmethod
-    def load(cls, file: str):
-        with open(file, "rb") as f:
-            return GridEstimator(pickle.load(f))
-
-
-class Scaler(Protocol):
-    fit: Callable
-    transform: Callable
-    fit_transform: Callable
-
-
-class StatsResult(NamedTuple):
-    statistic: "Grid"
-    pvalue: "Grid"
-
-
-@dataclass(frozen=True)
-class Grid:
-    data: ndarray
-    crs: CRS
-    transform: Affine
-    _cmap: Union[ColorMap, Any] = "gray"
-
-    def __post_init__(self):
-        self.data.flags.writeable = False
-
-    def __repr__(self):
-        d = 3 if self.dtype.startswith("float") else 0
-        return (
-            f"image: {self.width}x{self.height} {self.dtype} | "
-            + f"range: {self.min:.{d}f}~{self.max:.{d}f} | "
-            + f"mean: {self.mean:.{d}f} | "
-            + f"std: {self.std:.{d}f} | "
-            + f"crs: {self.crs} | "
-            + f"cell: {self.cell_size.x}, {self.cell_size.y}"
-        )
-
-    @property
-    def width(self) -> int:
-        return self.data.shape[1]
-
-    @property
-    def height(self) -> int:
-        return self.data.shape[0]
-
-    @property
-    def dtype(self) -> DataType:
-        return cast(DataType, str(self.data.dtype))
-
-    @property
-    def nodata(self):
-        return _nodata(self.dtype)
-
-    @property
-    def has_nan(self) -> bool:
-        return self._get("_has_nan", lambda: self.is_nan().data.any())
-
-    @property
-    def xmin(self) -> float:
-        return self.transform.c
-
-    @property
-    def ymin(self) -> float:
-        return self.ymax + self.height * self.transform.e
-
-    @property
-    def xmax(self) -> float:
-        return self.xmin + self.width * self.transform.a
-
-    @property
-    def ymax(self) -> float:
-        return self.transform.f
-
-    @property
-    def extent(self) -> Extent:
-        return Extent(self.xmin, self.ymin, self.xmax, self.ymax)
-
-    @property
-    def mean(self) -> float:
-        return self._get("_mean", lambda: np.nanmean(self.data))
-
-    @property
-    def std(self) -> float:
-        return self._get("_std", lambda: np.nanmean(self.data))
-
-    @property
-    def min(self) -> float:
-        return self._get("_min", lambda: np.nanmin(self.data))
-
-    @property
-    def max(self) -> float:
-        return self._get("_max", lambda: np.nanmax(self.data))
-
-    @property
-    def cell_size(self) -> CellSize:
-        return CellSize(self.transform.a, -self.transform.e)
-
-    @property
-    def bins(self) -> Dict[float, int]:
-        def f():
-            unique, counts = zip(np.unique(self.data, return_counts=True))
-            return dict(sorted(zip(map(float, unique[0]), map(int, counts[0]))))
-
-        return self._get("_bins", f)
-
-    @property
-    def md5(self) -> str:
-        return self._get("_md5", lambda: hashlib.md5(self.data.copy(order="C")).hexdigest())  # type: ignore
-
-    def _get(self, name: str, func: Callable):
-        if not hasattr(self, name):
-            object.__setattr__(self, name, func())
-        return self.__getattribute__(name)
-
-    def __add__(self, n: Operand):
-        return self._apply(self, n, np.add)
-
-    __radd__ = __add__
-
-    def __sub__(self, n: Operand):
-        return self._apply(self, n, np.subtract)
-
-    def __rsub__(self, n: Operand):
-        return self._apply(n, self, np.subtract)
-
-    def __mul__(self, n: Operand):
-        return self._apply(self, n, np.multiply)
-
-    __rmul__ = __mul__
-
-    def __pow__(self, n: Operand):
-        return self._apply(self, n, np.power)
-
-    def __rpow__(self, n: Operand):
-        return self._apply(n, self, np.power)
-
-    def __truediv__(self, n: Operand):
-        return self._apply(self, n, np.true_divide)
-
-    def __rtruediv__(self, n: Operand):
-        return self._apply(n, self, np.true_divide)
-
-    def __floordiv__(self, n: Operand):
-        return self._apply(self, n, np.floor_divide)
-
-    def __rfloordiv__(self, n: Operand):
-        return self._apply(n, self, np.floor_divide)
-
-    def __mod__(self, n: Operand):
-        return self._apply(self, n, np.mod)
-
-    def __rmod__(self, n: Operand):
-        return self._apply(n, self, np.mod)
-
-    def __lt__(self, n: Operand):
-        return self._apply(self, n, np.less)
-
-    def __gt__(self, n: Operand):
-        return self._apply(self, n, np.greater)
-
-    __rlt__ = __gt__
-
-    __rgt__ = __lt__
-
-    def __le__(self, n: Operand):
-        return self._apply(self, n, np.less_equal)
-
-    def __ge__(self, n: Operand):
-        return self._apply(self, n, np.greater_equal)
-
-    __rle__ = __ge__
-
-    __rge__ = __le__
-
-    def __eq__(self, n: Operand):
-        return self._apply(self, n, np.equal)
-
-    __req__ = __eq__
-
-    def __ne__(self, n: Operand):
-        return self._apply(self, n, np.not_equal)
-
-    __rne__ = __ne__
-
-    def __and__(self, n: Operand):
-        return self._apply(self, n, np.bitwise_and)
-
-    __rand__ = __and__
-
-    def __or__(self, n: Operand):
-        return self._apply(self, n, np.bitwise_or)
-
-    __ror__ = __or__
-
-    def __xor__(self, n: Operand):
-        return self._apply(self, n, np.bitwise_xor)
-
-    __rxor__ = __xor__
-
-    def __rshift__(self, n: Operand):
-        return self._apply(self, n, np.right_shift)
-
-    def __lshift__(self, n: Operand):
-        return self._apply(self, n, np.left_shift)
-
-    __rrshift__ = __lshift__
-
-    __rlshift__ = __rshift__
-
-    def __neg__(self):
-        return self._create(-1 * self.data)
-
-    def __pos__(self):
-        return self._create(1 * self.data)
-
-    def __invert__(self):
-        return con(self, False, True)
-
-    def _create(self, data: ndarray):
-        return _create(data, self.crs, self.transform)
-
-    def _data(self, n: Operand):
-        if isinstance(n, Grid):
-            return n.data
-        return n
-
-    def _apply(self, left: Operand, right: Operand, op: Callable):
-        if not isinstance(left, Grid) or not isinstance(right, Grid):
-            return self._create(op(self._data(left), self._data(right)))
-
-        if left.cell_size == right.cell_size and left.extent == right.extent:
-            return self._create(op(left.data, right.data))
-
-        l_adjusted, r_adjusted = standardize(left, right)
-
-        return self._create(op(l_adjusted.data, r_adjusted.data))
-
-    def percentile(self, percent: float) -> float:
-        return np.nanpercentile(self.data, percent)  # type: ignore
-
-    def local(self, func: Callable[[ndarray], Any]):
-        return self._create(func(self.data))
-
-    def is_nan(self):
-        return self.local(np.isnan)
-
-    def abs(self):
-        return self.local(np.abs)
-
-    def sin(self):
-        return self.local(np.sin)
-
-    def cos(self):
-        return self.local(np.cos)
-
-    def tan(self):
-        return self.local(np.tan)
-
-    def arcsin(self):
-        return self.local(np.arcsin)
-
-    def arccos(self):
-        return self.local(np.arccos)
-
-    def arctan(self):
-        return self.local(np.arctan)
-
-    def log(self, base: Optional[float] = None):
-        if base is None:
-            return self.local(np.log)
-        return self.local(lambda a: np.log(a) / np.log(base))
-
-    def round(self, decimals: int = 0):
-        return self.local(lambda a: np.round(a, decimals))
-
-    def gaussian_filter(self, sigma: float, **kwargs):
-        return self.local(lambda a: sp.ndimage.gaussian_filter(a, sigma, **kwargs))
-
-    def gaussian_filter1d(self, sigma: float, **kwargs):
-        return self.local(lambda a: sp.ndimage.gaussian_filter1d(a, sigma, **kwargs))
-
-    def gaussian_gradient_magnitude(self, sigma: float, **kwargs):
-        return self.local(
-            lambda a: sp.ndimage.gaussian_gradient_magnitude(a, sigma, **kwargs)
-        )
-
-    def gaussian_laplace(self, sigma: float, **kwargs):
-        return self.local(lambda a: sp.ndimage.gaussian_laplace(a, sigma, **kwargs))
-
-    def prewitt(self, **kwargs):
-        return self.local(lambda a: sp.ndimage.prewitt(a, **kwargs))
-
-    def sobel(self, **kwargs):
-        return self.local(lambda a: sp.ndimage.sobel(a, **kwargs))
-
-    def uniform_filter(self, **kwargs):
-        return self.local(lambda a: sp.ndimage.uniform_filter(a, **kwargs))
-
-    def uniform_filter1d(self, size: float, **kwargs):
-        return self.local(lambda a: sp.ndimage.uniform_filter1d(a, size, **kwargs))
-
-    def focal(
-        self, func: Callable[[ndarray], Any], buffer: int, circle: bool
-    ) -> "Grid":
-        return _batch(lambda g: _focal(func, buffer, circle, *g), buffer, self)[0]
-
-    def focal_count(
-        self,
-        value: Union[float, int],
-        buffer: int = 1,
-        circle: bool = False,
-        **kwargs,
-    ):
-        return self.focal(
-            lambda a: np.count_nonzero(a == value, axis=2, **kwargs), buffer, circle
-        )
-
-    def focal_ptp(self, buffer: int = 1, circle: bool = False, **kwargs):
-        return self.focal(lambda a: np.ptp(a, axis=2, **kwargs), buffer, circle)
-
-    def focal_percentile(
-        self,
-        percentile: float,
-        buffer: int = 1,
-        circle: bool = False,
-        ignore_nan: bool = True,
-        **kwargs,
-    ):
-        f = np.nanpercentile if ignore_nan else np.percentile
-        return self.focal(lambda a: f(a, percentile, axis=2, **kwargs), buffer, circle)
-
-    def focal_quantile(
-        self,
-        probability: float,
-        buffer: int = 1,
-        circle: bool = False,
-        ignore_nan: bool = True,
-        **kwargs,
-    ):
-        f = np.nanquantile if ignore_nan else np.quantile
-        return self.focal(lambda a: f(a, probability, axis=2, **kwargs), buffer, circle)
-
-    def focal_median(
-        self,
-        buffer: int = 1,
-        circle: bool = False,
-        ignore_nan: bool = True,
-        **kwargs,
-    ):
-        f = np.nanmedian if ignore_nan else np.median
-        return self.focal(lambda a: f(a, axis=2, **kwargs), buffer, circle)
-
-    def focal_mean(
-        self,
-        buffer: int = 1,
-        circle: bool = False,
-        ignore_nan: bool = True,
-        **kwargs,
-    ):
-        f = np.nanmean if ignore_nan else np.mean
-        return self.focal(lambda a: f(a, axis=2, **kwargs), buffer, circle)
-
-    def focal_std(
-        self,
-        buffer: int = 1,
-        circle: bool = False,
-        ignore_nan: bool = True,
-        **kwargs,
-    ):
-        f = np.nanstd if ignore_nan else np.std
-        return self.focal(lambda a: f(a, axis=2, **kwargs), buffer, circle)
-
-    def focal_var(
-        self,
-        buffer: int = 1,
-        circle: bool = False,
-        ignore_nan: bool = True,
-        **kwargs,
-    ):
-        f = np.nanvar if ignore_nan else np.var
-        return self.focal(lambda a: f(a, axis=2, **kwargs), buffer, circle)
-
-    def focal_min(
-        self,
-        buffer: int = 1,
-        circle: bool = False,
-        ignore_nan: bool = True,
-        **kwargs,
-    ):
-        f = np.nanmin if ignore_nan else np.min
-        return self.focal(lambda a: f(a, axis=2, **kwargs), buffer, circle)
-
-    def focal_max(
-        self,
-        buffer: int = 1,
-        circle: bool = False,
-        ignore_nan: bool = True,
-        **kwargs,
-    ):
-        f = np.nanmax if ignore_nan else np.max
-        return self.focal(lambda a: f(a, axis=2, **kwargs), buffer, circle)
-
-    def focal_sum(
-        self,
-        buffer: int = 1,
-        circle: bool = False,
-        ignore_nan: bool = True,
-        **kwargs,
-    ):
-        f = np.nansum if ignore_nan else np.sum
-        return self.focal(lambda a: f(a, axis=2, **kwargs), buffer, circle)
-
-    def _kwargs(self, ignore_nan: bool, **kwargs):
-        return {
-            "axis": 2,
-            "nan_policy": "omit" if ignore_nan else "propagate",
-            **kwargs,
-        }
-
-    def focal_entropy(self, buffer: int = 1, circle: bool = False, **kwargs):
-        return self.focal(
-            lambda a: sp.stats.entropy(a, axis=2, **kwargs), buffer, circle
-        )
-
-    def focal_gmean(
-        self, buffer: int = 1, circle: bool = False, ignore_nan: bool = True, **kwargs
-    ):
-        return self.focal(
-            lambda a: sp.stats.gmean(a, **self._kwargs(ignore_nan, **kwargs)),
-            buffer,
-            circle,
-        )
-
-    def focal_hmean(
-        self, buffer: int = 1, circle: bool = False, ignore_nan: bool = True, **kwargs
-    ):
-        return self.focal(
-            lambda a: sp.stats.hmean(a, **self._kwargs(ignore_nan, **kwargs)),
-            buffer,
-            circle,
-        )
-
-    def focal_pmean(
-        self,
-        p: float,
-        buffer: int = 1,
-        circle: bool = False,
-        ignore_nan: bool = True,
-        **kwargs,
-    ):
-        return self.focal(
-            lambda a: sp.stats.pmean(a, p, **self._kwargs(ignore_nan, **kwargs)),
-            buffer,
-            circle,
-        )
-
-    def focal_kurtosis(
-        self, buffer: int = 1, circle: bool = False, ignore_nan: bool = True, **kwargs
-    ):
-        return self.focal(
-            lambda a: sp.stats.kurtosis(a, **self._kwargs(ignore_nan, **kwargs)),
-            buffer,
-            circle,
-        )
-
-    def focal_iqr(
-        self, buffer: int = 1, circle: bool = False, ignore_nan: bool = True, **kwargs
-    ):
-        return self.focal(
-            lambda a: sp.stats.iqr(a, **self._kwargs(ignore_nan, **kwargs)),
-            buffer,
-            circle,
-        )
-
-    def focal_mode(
-        self, buffer: int = 1, circle: bool = False, ignore_nan: bool = True, **kwargs
-    ):
-        return self.focal(
-            lambda a: sp.stats.mode(
-                a, **self._kwargs(ignore_nan, keepdims=True, **kwargs)
-            )[0].transpose(2, 0, 1)[0],
-            buffer,
-            circle,
-        )
-
-    def focal_moment(
-        self, buffer: int = 1, circle: bool = False, ignore_nan: bool = True, **kwargs
-    ):
-        return self.focal(
-            lambda a: sp.stats.moment(a, **self._kwargs(ignore_nan, **kwargs)),
-            buffer,
-            circle,
-        )
-
-    def focal_skew(
-        self, buffer: int = 1, circle: bool = False, ignore_nan: bool = True, **kwargs
-    ):
-        return self.focal(
-            lambda a: sp.stats.skew(a, **self._kwargs(ignore_nan, **kwargs)),
-            buffer,
-            circle,
-        )
-
-    def focal_kstat(
-        self, buffer: int = 1, circle: bool = False, ignore_nan: bool = True, **kwargs
-    ):
-        return self.focal(
-            lambda a: sp.stats.kstat(a, **self._kwargs(ignore_nan, **kwargs)),
-            buffer,
-            circle,
-        )
-
-    def focal_kstatvar(
-        self, buffer: int = 1, circle: bool = False, ignore_nan: bool = True, **kwargs
-    ):
-        return self.focal(
-            lambda a: sp.stats.kstatvar(a, **self._kwargs(ignore_nan, **kwargs)),
-            buffer,
-            circle,
-        )
-
-    def focal_tmean(
-        self, buffer: int = 1, circle: bool = False, ignore_nan: bool = True, **kwargs
-    ):
-        return self.focal(
-            lambda a: sp.stats.tmean(a, **self._kwargs(ignore_nan, **kwargs)),
-            buffer,
-            circle,
-        )
-
-    def focal_tvar(self, buffer: int = 1, circle: bool = False, **kwargs):
-        return self.focal(lambda a: sp.stats.tvar(a, axis=2, **kwargs), buffer, circle)
-
-    def focal_tmin(
-        self, buffer: int = 1, circle: bool = False, ignore_nan: bool = True, **kwargs
-    ):
-        return self.focal(
-            lambda a: sp.stats.tmin(a, **self._kwargs(ignore_nan, **kwargs)),
-            buffer,
-            circle,
-        )
-
-    def focal_tmax(
-        self, buffer: int = 1, circle: bool = False, ignore_nan: bool = True, **kwargs
-    ):
-        return self.focal(
-            lambda a: sp.stats.tmax(a, **self._kwargs(ignore_nan, **kwargs)),
-            buffer,
-            circle,
-        )
-
-    def focal_tstd(self, buffer: int = 1, circle: bool = False, **kwargs):
-        return self.focal(lambda a: sp.stats.tstd(a, axis=2, **kwargs), buffer, circle)
-
-    def focal_variation(
-        self, buffer: int = 1, circle: bool = False, ignore_nan: bool = True, **kwargs
-    ):
-        return self.focal(
-            lambda a: sp.stats.variation(a, **self._kwargs(ignore_nan, **kwargs)),
-            buffer,
-            circle,
-        )
-
-    def focal_median_abs_deviation(
-        self, buffer: int = 1, circle: bool = False, ignore_nan: bool = True, **kwargs
-    ):
-        return self.focal(
-            lambda a: sp.stats.median_abs_deviation(
-                a, **self._kwargs(ignore_nan, **kwargs)
-            ),
-            buffer,
-            circle,
-        )
-
-    def focal_chisquare(
-        self, buffer: int = 1, circle: bool = False, **kwargs
-    ) -> StatsResult:
-        def f(grids):
-            return _focal(
-                lambda a: sp.stats.chisquare(a, axis=2, **kwargs),
-                buffer,
-                circle,
-                *grids,
-            )
-
-        return StatsResult(*_batch(f, buffer, self))
-
-    def focal_ttest_ind(
-        self, other_grid: "Grid", buffer: int = 1, circle: bool = False, **kwargs
-    ) -> StatsResult:
-        def f(grids):
-            return _focal(
-                lambda a: sp.stats.ttest_ind(*a, axis=2, **kwargs),
-                buffer,
-                circle,
-                *grids,
-            )
-
-        return StatsResult(*_batch(f, buffer, self, other_grid))
-
-    def zonal(self, func: Callable[[ndarray], Any], zone_grid: "Grid"):
-        zone_grid = zone_grid.type("int32")
-        result = self
-        for zone in set(zone_grid.data[np.isfinite(zone_grid.data)]):
-            data = self.set_nan(zone_grid != zone).data
-            statistics = func(data[np.isfinite(data)])
-            result = con(zone_grid == zone, statistics, result)  # type: ignore
-        return result
-
-    def zonal_count(self, value: Union[float, int], zone_grid: "Grid", **kwargs):
-        return self.zonal(lambda a: np.count_nonzero(a == value, **kwargs), zone_grid)
-
-    def zonal_ptp(self, zone_grid: "Grid", **kwargs):
-        return self.zonal(lambda a: np.ptp(a, **kwargs), zone_grid)
-
-    def zonal_percentile(self, percentile: float, zone_grid: "Grid", **kwargs):
-        return self.zonal(lambda a: np.percentile(a, percentile, **kwargs), zone_grid)
-
-    def zonal_quantile(self, probability: float, zone_grid: "Grid", **kwargs):
-        return self.zonal(lambda a: np.quantile(a, probability, **kwargs), zone_grid)
-
-    def zonal_median(self, zone_grid: "Grid", **kwargs):
-        return self.zonal(lambda a: np.median(a, **kwargs), zone_grid)
-
-    def zonal_mean(self, zone_grid: "Grid", **kwargs):
-        return self.zonal(lambda a: np.mean(a, **kwargs), zone_grid)
-
-    def zonal_std(self, zone_grid: "Grid", **kwargs):
-        return self.zonal(lambda a: np.std(a, **kwargs), zone_grid)
-
-    def zonal_var(self, zone_grid: "Grid", **kwargs):
-        return self.zonal(lambda a: np.var(a, **kwargs), zone_grid)
-
-    def zonal_min(self, zone_grid: "Grid", **kwargs):
-        return self.zonal(lambda a: np.min(a, **kwargs), zone_grid)
-
-    def zonal_max(self, zone_grid: "Grid", **kwargs):
-        return self.zonal(lambda a: np.max(a, **kwargs), zone_grid)
-
-    def zonal_sum(self, zone_grid: "Grid", **kwargs):
-        return self.zonal(lambda a: np.sum(a, **kwargs), zone_grid)
-
-    def zonal_entropy(self, zone_grid: "Grid", **kwargs):
-        return self.zonal(lambda a: sp.stats.entropy(a, **kwargs), zone_grid)
-
-    def zonal_gmean(self, zone_grid: "Grid", **kwargs):
-        return self.zonal(lambda a: sp.stats.gmean(a, **kwargs), zone_grid)
-
-    def zonal_hmean(self, zone_grid: "Grid", **kwargs):
-        return self.zonal(lambda a: sp.stats.hmean(a, **kwargs), zone_grid)
-
-    def zonal_pmean(self, p: float, zone_grid: "Grid", **kwargs):
-        return self.zonal(lambda a: sp.stats.pmean(a, p, **kwargs), zone_grid)
-
-    def zonal_kurtosis(self, zone_grid: "Grid", **kwargs):
-        return self.zonal(lambda a: sp.stats.kurtosis(a, **kwargs), zone_grid)
-
-    def zonal_iqr(self, zone_grid: "Grid", **kwargs):
-        return self.zonal(lambda a: sp.stats.iqr(a, **kwargs), zone_grid)
-
-    def zonal_mode(self, zone_grid: "Grid", **kwargs):
-        return self.zonal(lambda a: sp.stats.mode(a, **kwargs), zone_grid)
-
-    def zonal_moment(self, zone_grid: "Grid", **kwargs):
-        return self.zonal(lambda a: sp.stats.moment(a, **kwargs), zone_grid)
-
-    def zonal_skew(self, zone_grid: "Grid", **kwargs):
-        return self.zonal(lambda a: sp.stats.skew(a, **kwargs), zone_grid)
-
-    def zonal_kstat(self, zone_grid: "Grid", **kwargs):
-        return self.zonal(lambda a: sp.stats.kstat(a, **kwargs), zone_grid)
-
-    def zonal_kstatvar(self, zone_grid: "Grid", **kwargs):
-        return self.zonal(lambda a: sp.stats.kstatvar(a, **kwargs), zone_grid)
-
-    def zonal_tmean(self, zone_grid: "Grid", **kwargs):
-        return self.zonal(lambda a: sp.stats.tmean(a, **kwargs), zone_grid)
-
-    def zonal_tvar(self, zone_grid: "Grid", **kwargs):
-        return self.zonal(lambda a: sp.stats.tvar(a, **kwargs), zone_grid)
-
-    def zonal_tmin(self, zone_grid: "Grid", **kwargs):
-        return self.zonal(lambda a: sp.stats.tmin(a, **kwargs), zone_grid)
-
-    def zonal_tmax(self, zone_grid: "Grid", **kwargs):
-        return self.zonal(lambda a: sp.stats.tmax(a, **kwargs), zone_grid)
-
-    def zonal_tstd(self, zone_grid: "Grid", **kwargs):
-        return self.zonal(lambda a: sp.stats.tstd(a, **kwargs), zone_grid)
-
-    def zonal_variation(self, zone_grid: "Grid", **kwargs):
-        return self.zonal(lambda a: sp.stats.variation(a, **kwargs), zone_grid)
-
-    def zonal_median_abs_deviation(self, zone_grid: "Grid", **kwargs):
-        return self.zonal(
-            lambda a: sp.stats.median_abs_deviation(a, **kwargs), zone_grid
-        )
-
-    def _reproject(
-        self,
-        transform,
-        crs,
-        width,
-        height,
-        resampling: Union[Resampling, ResamplingMethod],
-    ) -> "Grid":
-        source = self * 1 if self.dtype == "bool" else self
-        destination = np.ones((round(height), round(width))) * np.nan
-        reproject(
-            source=source.data,
-            destination=destination,
-            src_transform=self.transform,
-            src_crs=self.crs,
-            src_nodata=self.nodata,
-            dst_transform=transform,
-            dst_crs=crs,
-            dst_nodata=self.nodata,
-            resampling=(
-                Resampling[resampling] if isinstance(resampling, str) else resampling
-            ),
-        )
-        result = _create(destination, crs, transform)
-        if self.dtype == "bool":
-            return result == 1
-        return con(result == result.nodata, np.nan, result)
-
-    def project(
-        self,
-        epsg: Union[int, CRS],
-        resampling: Union[Resampling, ResamplingMethod] = "nearest",
-    ) -> "Grid":
-        crs = CRS.from_epsg(epsg) if isinstance(epsg, int) else epsg
-        transform, width, height = calculate_default_transform(
-            self.crs, crs, self.width, self.height, *self.extent
-        )
-        return self._reproject(
-            transform,
-            crs,
-            width,
-            height,
-            Resampling[resampling] if isinstance(resampling, str) else resampling,
-        )
-
-    def _resample(
-        self,
-        extent: Tuple[float, float, float, float],
-        cell_size: Tuple[float, float],
-        resampling: Union[Resampling, ResamplingMethod],
-    ) -> "Grid":
-        (xmin, ymin, xmax, ymax) = extent
-        xoff = (xmin - self.xmin) / self.transform.a
-        yoff = (ymax - self.ymax) / self.transform.e
-        scaling_x = cell_size[0] / self.cell_size.x
-        scaling_y = cell_size[1] / self.cell_size.y
-        transform = (
-            self.transform
-            * Affine.translation(xoff, yoff)
-            * Affine.scale(scaling_x, scaling_y)
-        )
-        width = (xmax - xmin) / abs(self.transform.a) / scaling_x
-        height = (ymax - ymin) / abs(self.transform.e) / scaling_y
-        return self._reproject(transform, self.crs, width, height, resampling)
-
-    def clip(self, extent: Tuple[float, float, float, float]):
-        return self._resample(extent, self.cell_size, Resampling.nearest)
-
-    def resample(
-        self,
-        cell_size: Union[Tuple[float, float], float],
-        resampling: Union[Resampling, ResamplingMethod] = "nearest",
-    ):
-        if isinstance(cell_size, (int, float)):
-            cell_size = (cell_size, cell_size)
-        if self.cell_size == cell_size:
-            return self
-        return self._resample(self.extent, cell_size, resampling)
-
-    def buffer(self, value: Union[float, int], count: int):
-        if count < 0:
-            grid = (self != value).buffer(1, -count)
-            return con(grid == 0, value, self.set_nan(self == value))
-        grid = self
-        for _ in range(count):
-            grid = con(grid.focal_count(value, 1, True) > 0, value, grid)
-        return grid
-
-    def randomize(self):
-        return self._create(np.random.rand(self.height, self.width))
-
-    def aspect(self):
-        x, y = gradient(self.data)
-        return self._create(arctan2(-x, y))
-
-    def slope(self):
-        x, y = gradient(self.data)
-        return self._create(pi / 2.0 - arctan(sqrt(x * x + y * y)))
-
-    def hillshade(self, azimuth: float = 315, altitude: float = 45):
-        azimuth = np.deg2rad(azimuth)
-        altitude = np.deg2rad(altitude)
-        aspect = self.aspect().data
-        slope = self.slope().data
-        shaded = sin(altitude) * sin(slope) + cos(altitude) * cos(slope) * cos(
-            azimuth - aspect
-        )
-        return self._create((255 * (shaded + 1) / 2))
-
-    def reclass(self, *mappings: Tuple[float, float, float]):
-        conditions = [
-            (self.data >= min) & (self.data < max) for min, max, _ in mappings
-        ]
-        values = [value for _, _, value in mappings]
-        return self._create(np.select(conditions, values, np.nan))
-
-    def slice(self, count: int, percent_clip: float = 0.1):
-        min = self.percentile(percent_clip)
-        max = self.percentile(100 - percent_clip)
-        interval = (max - min) / count
-        mappings = [
-            (
-                min + (i - 1) * interval if i > 1 else float("-inf"),
-                min + i * interval if i < count else float("inf"),
-                float(i),
-            )
-            for i in range(1, count + 1)
-        ]
-        return self.reclass(*mappings)
-
-    def fill_nan(self, max_exponent: int = 4):
-        if not self.has_nan:
-            return self
-
-        def f(grids):
-            grid = grids[0]
-            n = 0
-            while grid.has_nan and n <= max_exponent:
-                grid = con(grid.is_nan(), grid.focal_mean(2**n, True), grid)
-                n += 1
-            return (grid,)
-
-        return _batch(f, 2**max_exponent, self)[0]
-
-    def replace(
-        self, value: Operand, replacement: Operand, fallback: Optional[Operand] = None
-    ):
-        return con(
-            value if isinstance(value, Grid) else self == value,
-            replacement,
-            self if fallback is None else fallback,
-        )
-
-    def set_nan(self, value: Operand, fallback: Optional[Operand] = None):
-        return self.replace(value, np.nan, fallback)
-
-    def value(self, x: float, y: float) -> float:
-        xoff = (x - self.xmin) / self.transform.a
-        yoff = (y - self.ymax) / self.transform.e
-        if xoff < 0 or xoff >= self.width or yoff < 0 or yoff >= self.height:
-            return float(np.nan)
-        return float(self.data[int(yoff), int(xoff)])
-
-    def data_extent(self):
-        xmin, ymin, xmax, ymax = None, None, None, None
-        for x, y, _ in self.to_points():
-            if not xmin or x < xmin:
-                xmin = x
-            if not ymin or y < ymin:
-                ymin = y
-            if not xmax or x > xmax:
-                xmax = x
-            if not ymax or y > ymax:
-                ymax = y
-        if xmin is None or ymin is None or xmax is None or ymax is None:
-            raise ValueError("None of the cells has a value.")
-        return Extent(
-            xmin - self.cell_size.x / 2,
-            ymin - self.cell_size.y / 2,
-            xmax + self.cell_size.x / 2,
-            ymax + self.cell_size.y / 2,
-        )
-
-    def to_points(self) -> Iterable[Point]:
-        for y, row in enumerate(self.data):
-            for x, value in enumerate(row):
-                if np.isfinite(value):
-                    yield Point(
-                        self.xmin + (x + 0.5) * self.cell_size.x,
-                        self.ymax - (y + 0.5) * self.cell_size.y,
-                        float(value),
-                    )
-
-    def to_polygons(self) -> Iterable[Tuple[Polygon, float]]:
-        for shape, value in features.shapes(
-            self.data, mask=np.isfinite(self.data), transform=self.transform
-        ):
-            if np.isfinite(value):
-                coordinates = shape["coordinates"]
-                yield Polygon(coordinates[0], coordinates[1:]), float(value)
-
-    def from_polygons(
-        self, polygons: Iterable[Tuple[Polygon, float]], all_touched: bool = False
-    ):
-        array = features.rasterize(
-            shapes=polygons,
-            out_shape=self.data.shape,
-            fill=np.nan,  # type: ignore
-            transform=self.transform,
-            all_touched=all_touched,
-            default_value=np.nan,  # type: ignore
-        )
-        return self._create(array)
-
-    def to_stack(self, cmap: Union[ColorMap, Any]):
-        from glidergun.stack import stack
-
-        grid1 = self - self.min
-        grid2 = grid1 / grid1.max
-        arrays = plt.get_cmap(cmap)(grid2.data).transpose(2, 0, 1)[:3]  # type: ignore
-        mask = self.is_nan()
-        r, g, b = [self._create(a * 253 + 1).set_nan(mask) for a in arrays]
-        return stack(r, g, b)
-
-    def scale(self, scaler: Optional[Scaler] = None, **fit_params):
-        if not scaler:
-            scaler = QuantileTransformer(n_quantiles=10)
-        return self.local(lambda a: scaler.fit_transform(a, **fit_params))
-
-    def stretch(self, min_value: float, max_value: float):
-        expected_range = max_value - min_value
-        actual_range = self.max - self.min
-
-        if actual_range == 0:
-            return self
-
-        return (self - self.min) * expected_range / actual_range + min_value
-
-    def cap_range(self, min: Operand, max: Operand, set_nan: bool = False):
-        return self.cap_min(min, set_nan).cap_max(max, set_nan)
-
-    def cap_min(self, value: Operand, set_nan: bool = False):
-        return con(self < value, np.nan if set_nan else value, self)
-
-    def cap_max(self, value: Operand, set_nan: bool = False):
-        return con(self > value, np.nan if set_nan else value, self)
-
-    def percent_clip(self, min_percent: float, max_percent: float):
-        min_value = self.percentile(min_percent)
-        max_value = self.percentile(max_percent)
-
-        if min_value == max_value:
-            return self
-
-        return self.cap_range(min_value, max_value)
-
-    def to_uint8_range(self):
-        if self.dtype == "bool" or self.min > 0 and self.max < 255:
-            return self
-        return self.percent_clip(0.1, 99.9).stretch(1, 254)
-
-    def fit(self, model: T, *explanatory_grids: "Grid") -> GridEstimator[T]:
-        return GridEstimator(model).fit(self, *explanatory_grids)
-
-    def hist(self, **kwargs):
-        return plt.bar(list(self.bins.keys()), list(self.bins.values()), **kwargs)
-
-    def plot(self, cmap: Union[ColorMap, Any]):
-        return dataclasses.replace(self, _cmap=cmap)
-
-    def map(
-        self,
-        cmap: Union[ColorMap, Any] = "gray",
-        opacity: float = 1.0,
-        folium_map=None,
-        width: int = 800,
-        height: int = 600,
-        basemap: Optional[str] = None,
-        attribution: Optional[str] = None,
-        grayscale: bool = True,
-        **kwargs,
-    ):
-        from glidergun.ipython import _map
-
-        return _map(
-            self,
-            cmap,
-            opacity,
-            folium_map,
-            width,
-            height,
-            basemap,
-            attribution,
-            grayscale,
-            **kwargs,
-        )
-
-    def type(self, dtype: DataType):
-        if self.dtype == dtype:
-            return self
-        return self.local(lambda data: np.asanyarray(data, dtype=dtype))
-
-    @overload
-    def save(
-        self, file: str, dtype: Optional[DataType] = None, driver: str = ""
-    ) -> None: ...
-
-    @overload
-    def save(
-        self, file: MemoryFile, dtype: Optional[DataType] = None, driver: str = ""
-    ) -> None: ...
-
-    def save(self, file, dtype: Optional[DataType] = None, driver: str = ""):
-        grid = self * 1 if self.dtype == "bool" else self
-
-        if isinstance(file, str) and (
-            file.lower().endswith(".jpg")
-            or file.lower().endswith(".kml")
-            or file.lower().endswith(".kmz")
-            or file.lower().endswith(".png")
-        ):
-            grid = grid.to_uint8_range()
-            dtype = "uint8"
-        else:
-            grid = grid
-            if dtype is None:
-                dtype = grid.dtype
-
-        nodata = _nodata(dtype)
-
-        if nodata is not None:
-            grid = con(grid.is_nan(), nodata, grid)
-
-        if isinstance(file, str):
-            with rasterio.open(
-                file,
-                "w",
-                driver=driver if driver else driver_from_extension(file),
-                count=1,
-                dtype=dtype,
-                nodata=nodata,
-                **_metadata(self),
-            ) as dataset:
-                dataset.write(grid.data, 1)
-        elif isinstance(file, MemoryFile):
-            with file.open(
-                driver=driver if driver else "GTiff",
-                count=1,
-                dtype=dtype,
-                nodata=nodata,
-                **_metadata(self),
-            ) as dataset:
-                dataset.write(grid.data, 1)
-
-    def save_plot(self, file):
-        self.to_stack(self._cmap).save(file)
-
-
-@overload
-def grid(file: str, index: int = 1) -> Grid:
-    """Creates a new grid from a file path.
-
-    Args:
-        file (str): File path.
-        index (int, optional): Band index.  Defaults to 1.
-
-    Returns:
-        Grid: A new grid.
-    """
-    ...
-
-
-@overload
-def grid(file: MemoryFile, index: int = 1) -> Grid:
-    """Creates a new grid from an in-memory file.
-
-    Args:
-        file (MemoryFile): Rasterio in-memory file.
-        index (int, optional): Band index.  Defaults to 1.
-
-    Returns:
-        Grid: A new grid.
-    """
-    ...
-
-
-def grid(file, index: int = 1) -> Grid:
-    if isinstance(file, str):
-        with rasterio.open(file) as dataset:
-            return _read(dataset, index)
-    elif isinstance(file, MemoryFile):
-        with file.open() as dataset:
-            return _read(dataset, index)
-    raise ValueError()
-
-
-def _create(data: ndarray, crs: CRS, transform: Affine):
-    if data.dtype == "float64":
-        data = np.asanyarray(data, dtype="float32")
-    elif data.dtype == "int64":
-        data = np.asanyarray(data, dtype="int32")
-    elif data.dtype == "uint64":
-        data = np.asanyarray(data, dtype="uint32")
-    return Grid(data, crs, transform)
-
-
-def _read(dataset, index):
-    grid = _create(dataset.read(index), dataset.crs, dataset.transform)
-    return grid if dataset.nodata is None else grid.set_nan(dataset.nodata)
-
-
-def _metadata(grid: Grid):
-    return {
-        "height": grid.height,
-        "width": grid.width,
-        "crs": grid.crs,
-        "transform": grid.transform,
-    }
-
-
-def _mask(buffer: int) -> ndarray:
-    size = 2 * buffer + 1
-    rows = []
-    for y in range(size):
-        row = []
-        for x in range(size):
-            d = ((x - buffer) ** 2 + (y - buffer) ** 2) ** (1 / 2)
-            row.append(d <= buffer)
-        rows.append(row)
-    return np.array(rows)
-
-
-def _pad(data: ndarray, buffer: int):
-    row = np.zeros((buffer, data.shape[1])) * np.nan
-    col = np.zeros((data.shape[0] + 2 * buffer, buffer)) * np.nan
-    return np.hstack([col, np.vstack([row, data, row]), col], dtype="float32")
-
-
-def _focal(func: Callable, buffer: int, circle: bool, *grids: Grid) -> Tuple[Grid, ...]:
-    grids_adjusted = standardize(*grids)
-    size = 2 * buffer + 1
-    mask = _mask(buffer) if circle else np.full((size, size), True)
-
-    if len(grids) == 1:
-        array = sliding_window_view(_pad(grids[0].data, buffer), (size, size))
-        result = func(array[:, :, mask])
-    else:
-        array = np.stack(
-            [
-                sliding_window_view(_pad(g.data, buffer), (size, size))
-                for g in grids_adjusted
-            ]
-        )
-        transposed = np.transpose(array, axes=(1, 2, 0, 3, 4))[:, :, :, mask]
-        result = func(tuple(transposed[:, :, i] for i, _ in enumerate(grids)))
-
-    if isinstance(result, ndarray) and len(result.shape) == 2:
-        return (grids_adjusted[0]._create(np.array(result)),)
-
-    return tuple([grids_adjusted[0]._create(r) for r in result])
-
-
-def _batch(
-    func: Callable[[Tuple[Grid, ...]], Tuple[Grid, ...]], buffer: int, *grids: Grid
-) -> Tuple[Grid, ...]:
-    stride = 8000 // buffer // len(grids)
-    grids1 = standardize(*grids)
-    grid = grids1[0]
-
-    def tile():
-        for x in range(0, grid.width // stride + 1):
-            xmin, xmax = x * stride, min((x + 1) * stride, grid.width)
-            if xmin < xmax:
-                for y in range(0, grid.height // stride + 1):
-                    ymin, ymax = y * stride, min((y + 1) * stride, grid.height)
-                    if ymin < ymax:
-                        yield xmin, ymin, xmax, ymax
-
-    tiles = list(tile())
-    count = len(tiles)
-
-    if count <= 4:
-        return func(tuple(grids1))
-
-    results: List[Grid] = []
-    cell_size = grid.cell_size
-    n = 0
-
-    for xmin, ymin, xmax, ymax in tiles:
-        n += 1
-        sys.stdout.write(f"\rProcessing {n} of {count} tiles...")
-        sys.stdout.flush()
-        grids2 = [
-            g.clip(
-                (
-                    grid.xmin + (xmin - buffer) * cell_size.x,
-                    grid.ymin + (ymin - buffer) * cell_size.y,
-                    grid.xmin + (xmax + buffer) * cell_size.x,
-                    grid.ymin + (ymax + buffer) * cell_size.y,
-                )
-            )
-            for g in grids1
-        ]
-
-        grids3 = func(tuple(grids2))
-
-        grids4 = [
-            g.clip(
-                (
-                    grid.xmin + xmin * cell_size.x,
-                    grid.ymin + ymin * cell_size.y,
-                    grid.xmin + xmax * cell_size.x,
-                    grid.ymin + ymax * cell_size.y,
-                )
-            )
-            for g in grids3
-        ]
-
-        if results:
-            for i, g in enumerate(grids4):
-                results[i] = mosaic(results[i], g)
-        else:
-            results = grids4
-
-    print()
-    return tuple(results)
-
-
-def con(grid: Grid, trueValue: Operand, falseValue: Operand):
-    return grid.local(
-        lambda data: np.where(data, grid._data(trueValue), grid._data(falseValue))
-    )
-
-
-def _aggregate(func: Callable, *grids: Grid) -> Grid:
-    grids_adjusted = standardize(*grids)
-    data = func(np.array([grid.data for grid in grids_adjusted]), axis=0)
-    return grids_adjusted[0]._create(data)
-
-
-def mean(*grids: Grid) -> Grid:
-    return _aggregate(np.mean, *grids)
-
-
-def std(*grids: Grid) -> Grid:
-    return _aggregate(np.std, *grids)
-
-
-def minimum(*grids: Grid) -> Grid:
-    return _aggregate(np.min, *grids)
-
-
-def maximum(*grids: Grid) -> Grid:
-    return _aggregate(np.max, *grids)
-
-
-def load_model(file: str) -> GridEstimator[Any]:
-    return GridEstimator.load(file)
-
-
-def mosaic(*grids: Grid) -> Grid:
-    grids_adjusted = standardize(*grids, extent="union")
-    result = grids_adjusted[0]
-    for grid in grids_adjusted[1:]:
-        result = con(result.is_nan(), grid, result)
-    return result
-
-
-def pca(n_components: int = 1, *grids: Grid) -> Tuple[Grid, ...]:
-    grids_adjusted = [con(g.is_nan(), g.mean, g) for g in standardize(*grids)]
-    arrays = (
-        PCA(n_components=n_components)
-        .fit_transform(
-            np.array(
-                [g.scale(StandardScaler()).data.ravel() for g in grids_adjusted]
-            ).transpose((1, 0))
-        )
-        .transpose((1, 0))
-    )
-    grid = grids_adjusted[0]
-    return tuple(grid._create(a.reshape((grid.height, grid.width))) for a in arrays)
-
-
-def standardize(
-    *grids: Grid,
-    extent: Union[Extent, ExtentResolution] = "intersect",
-    cell_size: Union[Tuple[float, float], float, None] = None,
-) -> Tuple[Grid, ...]:
-    if len(grids) == 1:
-        return tuple(grids)
-
-    crs_set = set(grid.crs for grid in grids)
-
-    if len(crs_set) > 1:
-        raise ValueError("Input grids must have the same CRS.")
-
-    if isinstance(cell_size, (int, float)):
-        cell_size_standardized = (cell_size, cell_size)
-    elif cell_size is None:
-        cell_size_standardized = grids[0].cell_size
-    else:
-        cell_size_standardized = cell_size
-
-    if isinstance(extent, Extent):
-        extent_standardized = extent
-    else:
-        extent_standardized = grids[0].extent
-        for grid in grids:
-            if extent == "intersect":
-                extent_standardized = extent_standardized & grid.extent
-            elif extent == "union":
-                extent_standardized = extent_standardized | grid.extent
-
-    results = []
-
-    for grid in grids:
-        if grid.cell_size != cell_size_standardized:
-            grid = grid.resample(cell_size_standardized)
-        if grid.extent != extent_standardized:
-            grid = grid.clip(extent_standardized)  # type: ignore
-        results.append(grid)
-
-    return tuple(results)
-
-
-def create(
-    extent: Tuple[float, float, float, float],
-    epsg: Union[int, CRS],
-    cell_size: Union[Tuple[float, float], float],
-):
-    cell_size = (
-        CellSize(cell_size, cell_size)
-        if isinstance(cell_size, (int, float))
-        else CellSize(*cell_size)
-    )
-    xmin, ymin, xmax, ymax = extent
-    width = int((xmax - xmin) / cell_size.x)
-    height = int((ymax - ymin) / cell_size.y)
-    xmin = xmax - cell_size.x * width
-    ymax = ymin + cell_size.y * height
-    crs = CRS.from_epsg(epsg) if isinstance(epsg, int) else epsg
-    transform = Affine(cell_size.x, 0, xmin, 0, -cell_size.y, ymax, 0, 0, 1)
-    return Grid(np.zeros((height, width), "uint8"), crs, transform)
-
-
-def interpolate(
-    interpolator_factory: Callable[[ndarray, ndarray], Any],
-    points: Iterable[Tuple[float, float, float]],
-    epsg: Union[int, CRS],
-    cell_size: Union[Tuple[float, float], float],
-):
-    coord_array = []
-    value_array = []
-
-    for p in points:
-        coord_array.append(p[:2])
-        value_array.append(p[-1])
-
-    coords = np.array(coord_array)
-    values = np.array(value_array)
-    x, y = coords.transpose(1, 0)
-    xmin, ymin, xmax, ymax = x.min(), y.min(), x.max(), y.max()
-    extent = Extent(xmin, ymin, xmax, ymax)
-    grid = create(extent, epsg, cell_size)
-    interp = interpolator_factory(coords, values)
-    xs = np.linspace(xmin, xmax, grid.width)
-    ys = np.linspace(ymax, ymin, grid.height)
-    array = np.array([[x0, y0] for x0 in xs for y0 in ys])
-    data = interp(array).reshape((grid.width, grid.height)).transpose(1, 0)
-
-    return grid.local(lambda _: data)
-
-
-def interp_linear(
-    points: Iterable[Tuple[float, float, float]],
-    epsg: Union[int, CRS],
-    cell_size: Union[Tuple[float, float], float],
-    fill_value: float = np.nan,
-    rescale: bool = False,
-):
-    def f(coords, values):
-        return LinearNDInterpolator(coords, values, fill_value, rescale)
-
-    return interpolate(f, points, epsg, cell_size)
-
-
-def interp_nearest(
-    points: Iterable[Tuple[float, float, float]],
-    epsg: Union[int, CRS],
-    cell_size: Union[Tuple[float, float], float],
-    rescale: bool = False,
-    tree_options: Any = None,
-):
-    def f(coords, values):
-        return NearestNDInterpolator(coords, values, rescale, tree_options)
-
-    return interpolate(f, points, epsg, cell_size)
-
-
-def interp_rbf(
-    points: Iterable[Tuple[float, float, float]],
-    epsg: Union[int, CRS],
-    cell_size: Union[Tuple[float, float], float],
-    neighbors: Optional[int] = None,
-    smoothing: float = 0,
-    kernel: InterpolationKernel = "thin_plate_spline",
-    epsilon: float = 1,
-    degree: Optional[int] = None,
-):
-    def f(coords, values):
-        return RBFInterpolator(
-            coords, values, neighbors, smoothing, kernel, epsilon, degree
-        )
-
-    return interpolate(f, points, epsg, cell_size)
-
-
-def _nodata(dtype: str) -> Union[float, int, None]:
-    if dtype == "bool":
-        return None
-    if dtype.startswith("float"):
-        return float(np.finfo(dtype).min)
-    if dtype.startswith("uint"):
-        return np.iinfo(dtype).max
-    return np.iinfo(dtype).min
+import dataclasses
+import hashlib
+import pickle
+import sys
+from dataclasses import dataclass
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Generic,
+    Iterable,
+    List,
+    NamedTuple,
+    Optional,
+    Protocol,
+    Tuple,
+    TypeVar,
+    Union,
+    cast,
+    overload,
+)
+
+import matplotlib.pyplot as plt
+import numpy as np
+import rasterio
+import scipy as sp
+from numpy import arctan, arctan2, cos, gradient, ndarray, pi, sin, sqrt
+from numpy.lib.stride_tricks import sliding_window_view
+from rasterio import features
+from rasterio.crs import CRS
+from rasterio.drivers import driver_from_extension
+from rasterio.io import MemoryFile
+from rasterio.transform import Affine
+from rasterio.warp import Resampling, calculate_default_transform, reproject
+from scipy.interpolate import (
+    LinearNDInterpolator,
+    NearestNDInterpolator,
+    RBFInterpolator,
+)
+from shapely import Polygon
+from sklearn.decomposition import PCA
+from sklearn.preprocessing import QuantileTransformer, StandardScaler
+
+from glidergun._literals import (
+    ColorMap,
+    DataType,
+    ExtentResolution,
+    InterpolationKernel,
+    ResamplingMethod,
+)
+
+
+class Extent(NamedTuple):
+    xmin: float
+    ymin: float
+    xmax: float
+    ymax: float
+
+    def intersect(self, extent: "Extent"):
+        return Extent(*[f(x) for f, x in zip((max, max, min, min), zip(self, extent))])
+
+    def union(self, extent: "Extent"):
+        return Extent(*[f(x) for f, x in zip((min, min, max, max), zip(self, extent))])
+
+    __and__ = intersect
+    __rand__ = __and__
+    __or__ = union
+    __ror__ = __or__
+
+
+Operand = Union["Grid", float, int]
+
+
+class CellSize(NamedTuple):
+    x: float
+    y: float
+
+    def __mul__(self, n: float):
+        return CellSize(self.x * n, self.y * n)
+
+    def __rmul__(self, n: float):
+        return CellSize(self.x * n, self.y * n)
+
+    def __truediv__(self, n: float):
+        return CellSize(self.x / n, self.y / n)
+
+
+class Point(NamedTuple):
+    x: float
+    y: float
+    value: float
+
+
+class Estimator(Protocol):
+    fit: Callable
+    score: Callable
+    predict: Callable
+
+
+T = TypeVar("T", bound=Estimator)
+
+
+class GridEstimator(Generic[T]):
+    def __init__(self, model: T) -> None:
+        self.model: T = model
+        self._dtype: DataType = "float32"
+
+    def fit(self, dependent_grid: "Grid", *explanatory_grids: "Grid"):
+        head, *tail = self._flatten(*[dependent_grid, *explanatory_grids])
+        self.model = self.model.fit(
+            np.array([g.data.ravel() for g in tail]).transpose(1, 0),
+            head.data.ravel(),
+        )
+        self._dtype = dependent_grid.dtype
+        return self
+
+    def score(self, dependent_grid: "Grid", *explanatory_grids: "Grid") -> float:
+        head, *tail = self._flatten(dependent_grid, *explanatory_grids)
+        return self.model.score(
+            np.array([g.data.ravel() for g in tail]).transpose(1, 0), head.data.ravel()
+        )
+
+    def predict(self, *explanatory_grids: "Grid") -> "Grid":
+        grids = self._flatten(*explanatory_grids)
+        array = self.model.predict(
+            np.array([g.data.ravel() for g in grids]).transpose(1, 0)
+        )
+        grid = grids[0]
+        return grid._create(array.reshape((grid.height, grid.width))).type(self._dtype)
+
+    def _flatten(self, *grids: "Grid"):
+        return [con(g.is_nan(), g.mean, g) for g in standardize(*grids)]
+
+    def save(self, file: str):
+        with open(file, "wb") as f:
+            pickle.dump(self.model, f)
+
+    @classmethod
+    def load(cls, file: str):
+        with open(file, "rb") as f:
+            return GridEstimator(pickle.load(f))
+
+
+class Scaler(Protocol):
+    fit: Callable
+    transform: Callable
+    fit_transform: Callable
+
+
+class StatsResult(NamedTuple):
+    statistic: "Grid"
+    pvalue: "Grid"
+
+
+@dataclass(frozen=True)
+class Grid:
+    data: ndarray
+    crs: CRS
+    transform: Affine
+    _cmap: Union[ColorMap, Any] = "gray"
+
+    def __post_init__(self):
+        self.data.flags.writeable = False
+
+    def __repr__(self):
+        d = 3 if self.dtype.startswith("float") else 0
+        return (
+            f"image: {self.width}x{self.height} {self.dtype} | "
+            + f"range: {self.min:.{d}f}~{self.max:.{d}f} | "
+            + f"mean: {self.mean:.{d}f} | "
+            + f"std: {self.std:.{d}f} | "
+            + f"crs: {self.crs} | "
+            + f"cell: {self.cell_size.x}, {self.cell_size.y}"
+        )
+
+    @property
+    def width(self) -> int:
+        return self.data.shape[1]
+
+    @property
+    def height(self) -> int:
+        return self.data.shape[0]
+
+    @property
+    def dtype(self) -> DataType:
+        return cast(DataType, str(self.data.dtype))
+
+    @property
+    def nodata(self):
+        return _nodata(self.dtype)
+
+    @property
+    def has_nan(self) -> bool:
+        return self._get("_has_nan", lambda: self.is_nan().data.any())
+
+    @property
+    def xmin(self) -> float:
+        return self.transform.c
+
+    @property
+    def ymin(self) -> float:
+        return self.ymax + self.height * self.transform.e
+
+    @property
+    def xmax(self) -> float:
+        return self.xmin + self.width * self.transform.a
+
+    @property
+    def ymax(self) -> float:
+        return self.transform.f
+
+    @property
+    def extent(self) -> Extent:
+        return Extent(self.xmin, self.ymin, self.xmax, self.ymax)
+
+    @property
+    def mean(self) -> float:
+        return self._get("_mean", lambda: np.nanmean(self.data))
+
+    @property
+    def std(self) -> float:
+        return self._get("_std", lambda: np.nanmean(self.data))
+
+    @property
+    def min(self) -> float:
+        return self._get("_min", lambda: np.nanmin(self.data))
+
+    @property
+    def max(self) -> float:
+        return self._get("_max", lambda: np.nanmax(self.data))
+
+    @property
+    def cell_size(self) -> CellSize:
+        return CellSize(self.transform.a, -self.transform.e)
+
+    @property
+    def bins(self) -> Dict[float, int]:
+        def f():
+            unique, counts = zip(np.unique(self.data, return_counts=True))
+            return dict(sorted(zip(map(float, unique[0]), map(int, counts[0]))))
+
+        return self._get("_bins", f)
+
+    @property
+    def md5(self) -> str:
+        return self._get("_md5", lambda: hashlib.md5(self.data.copy(order="C")).hexdigest())  # type: ignore
+
+    def _get(self, name: str, func: Callable):
+        if not hasattr(self, name):
+            object.__setattr__(self, name, func())
+        return self.__getattribute__(name)
+
+    def __add__(self, n: Operand):
+        return self._apply(self, n, np.add)
+
+    __radd__ = __add__
+
+    def __sub__(self, n: Operand):
+        return self._apply(self, n, np.subtract)
+
+    def __rsub__(self, n: Operand):
+        return self._apply(n, self, np.subtract)
+
+    def __mul__(self, n: Operand):
+        return self._apply(self, n, np.multiply)
+
+    __rmul__ = __mul__
+
+    def __pow__(self, n: Operand):
+        return self._apply(self, n, np.power)
+
+    def __rpow__(self, n: Operand):
+        return self._apply(n, self, np.power)
+
+    def __truediv__(self, n: Operand):
+        return self._apply(self, n, np.true_divide)
+
+    def __rtruediv__(self, n: Operand):
+        return self._apply(n, self, np.true_divide)
+
+    def __floordiv__(self, n: Operand):
+        return self._apply(self, n, np.floor_divide)
+
+    def __rfloordiv__(self, n: Operand):
+        return self._apply(n, self, np.floor_divide)
+
+    def __mod__(self, n: Operand):
+        return self._apply(self, n, np.mod)
+
+    def __rmod__(self, n: Operand):
+        return self._apply(n, self, np.mod)
+
+    def __lt__(self, n: Operand):
+        return self._apply(self, n, np.less)
+
+    def __gt__(self, n: Operand):
+        return self._apply(self, n, np.greater)
+
+    __rlt__ = __gt__
+
+    __rgt__ = __lt__
+
+    def __le__(self, n: Operand):
+        return self._apply(self, n, np.less_equal)
+
+    def __ge__(self, n: Operand):
+        return self._apply(self, n, np.greater_equal)
+
+    __rle__ = __ge__
+
+    __rge__ = __le__
+
+    def __eq__(self, n: Operand):
+        return self._apply(self, n, np.equal)
+
+    __req__ = __eq__
+
+    def __ne__(self, n: Operand):
+        return self._apply(self, n, np.not_equal)
+
+    __rne__ = __ne__
+
+    def __and__(self, n: Operand):
+        return self._apply(self, n, np.bitwise_and)
+
+    __rand__ = __and__
+
+    def __or__(self, n: Operand):
+        return self._apply(self, n, np.bitwise_or)
+
+    __ror__ = __or__
+
+    def __xor__(self, n: Operand):
+        return self._apply(self, n, np.bitwise_xor)
+
+    __rxor__ = __xor__
+
+    def __rshift__(self, n: Operand):
+        return self._apply(self, n, np.right_shift)
+
+    def __lshift__(self, n: Operand):
+        return self._apply(self, n, np.left_shift)
+
+    __rrshift__ = __lshift__
+
+    __rlshift__ = __rshift__
+
+    def __neg__(self):
+        return self._create(-1 * self.data)
+
+    def __pos__(self):
+        return self._create(1 * self.data)
+
+    def __invert__(self):
+        return con(self, False, True)
+
+    def _create(self, data: ndarray):
+        return _create(data, self.crs, self.transform)
+
+    def _data(self, n: Operand):
+        if isinstance(n, Grid):
+            return n.data
+        return n
+
+    def _apply(self, left: Operand, right: Operand, op: Callable):
+        if not isinstance(left, Grid) or not isinstance(right, Grid):
+            return self._create(op(self._data(left), self._data(right)))
+
+        if left.cell_size == right.cell_size and left.extent == right.extent:
+            return self._create(op(left.data, right.data))
+
+        l_adjusted, r_adjusted = standardize(left, right)
+
+        return self._create(op(l_adjusted.data, r_adjusted.data))
+
+    def percentile(self, percent: float) -> float:
+        return np.nanpercentile(self.data, percent)  # type: ignore
+
+    def local(self, func: Callable[[ndarray], Any]):
+        return self._create(func(self.data))
+
+    def is_nan(self):
+        return self.local(np.isnan)
+
+    def abs(self):
+        return self.local(np.abs)
+
+    def sin(self):
+        return self.local(np.sin)
+
+    def cos(self):
+        return self.local(np.cos)
+
+    def tan(self):
+        return self.local(np.tan)
+
+    def arcsin(self):
+        return self.local(np.arcsin)
+
+    def arccos(self):
+        return self.local(np.arccos)
+
+    def arctan(self):
+        return self.local(np.arctan)
+
+    def log(self, base: Optional[float] = None):
+        if base is None:
+            return self.local(np.log)
+        return self.local(lambda a: np.log(a) / np.log(base))
+
+    def round(self, decimals: int = 0):
+        return self.local(lambda a: np.round(a, decimals))
+
+    def gaussian_filter(self, sigma: float, **kwargs):
+        return self.local(lambda a: sp.ndimage.gaussian_filter(a, sigma, **kwargs))
+
+    def gaussian_filter1d(self, sigma: float, **kwargs):
+        return self.local(lambda a: sp.ndimage.gaussian_filter1d(a, sigma, **kwargs))
+
+    def gaussian_gradient_magnitude(self, sigma: float, **kwargs):
+        return self.local(
+            lambda a: sp.ndimage.gaussian_gradient_magnitude(a, sigma, **kwargs)
+        )
+
+    def gaussian_laplace(self, sigma: float, **kwargs):
+        return self.local(lambda a: sp.ndimage.gaussian_laplace(a, sigma, **kwargs))
+
+    def prewitt(self, **kwargs):
+        return self.local(lambda a: sp.ndimage.prewitt(a, **kwargs))
+
+    def sobel(self, **kwargs):
+        return self.local(lambda a: sp.ndimage.sobel(a, **kwargs))
+
+    def uniform_filter(self, **kwargs):
+        return self.local(lambda a: sp.ndimage.uniform_filter(a, **kwargs))
+
+    def uniform_filter1d(self, size: float, **kwargs):
+        return self.local(lambda a: sp.ndimage.uniform_filter1d(a, size, **kwargs))
+
+    def focal(
+        self, func: Callable[[ndarray], Any], buffer: int, circle: bool
+    ) -> "Grid":
+        return _batch(lambda g: _focal(func, buffer, circle, *g), buffer, self)[0]
+
+    def focal_python(
+        self,
+        func: Callable[[List[float]], float],
+        buffer: int = 1,
+        circle: bool = False,
+        ignore_nan: bool = True,
+    ) -> "Grid":
+        def f(a):
+            values = [n for n in a if n != np.nan] if ignore_nan else list(a)
+            return func(values)
+
+        return self.focal(lambda a: np.apply_along_axis(f, 2, a), buffer, circle)
+
+    def focal_count(
+        self,
+        value: Union[float, int],
+        buffer: int = 1,
+        circle: bool = False,
+        **kwargs,
+    ):
+        return self.focal(
+            lambda a: np.count_nonzero(a == value, axis=2, **kwargs), buffer, circle
+        )
+
+    def focal_ptp(self, buffer: int = 1, circle: bool = False, **kwargs):
+        return self.focal(lambda a: np.ptp(a, axis=2, **kwargs), buffer, circle)
+
+    def focal_percentile(
+        self,
+        percentile: float,
+        buffer: int = 1,
+        circle: bool = False,
+        ignore_nan: bool = True,
+        **kwargs,
+    ):
+        f = np.nanpercentile if ignore_nan else np.percentile
+        return self.focal(lambda a: f(a, percentile, axis=2, **kwargs), buffer, circle)
+
+    def focal_quantile(
+        self,
+        probability: float,
+        buffer: int = 1,
+        circle: bool = False,
+        ignore_nan: bool = True,
+        **kwargs,
+    ):
+        f = np.nanquantile if ignore_nan else np.quantile
+        return self.focal(lambda a: f(a, probability, axis=2, **kwargs), buffer, circle)
+
+    def focal_median(
+        self,
+        buffer: int = 1,
+        circle: bool = False,
+        ignore_nan: bool = True,
+        **kwargs,
+    ):
+        f = np.nanmedian if ignore_nan else np.median
+        return self.focal(lambda a: f(a, axis=2, **kwargs), buffer, circle)
+
+    def focal_mean(
+        self,
+        buffer: int = 1,
+        circle: bool = False,
+        ignore_nan: bool = True,
+        **kwargs,
+    ):
+        f = np.nanmean if ignore_nan else np.mean
+        return self.focal(lambda a: f(a, axis=2, **kwargs), buffer, circle)
+
+    def focal_std(
+        self,
+        buffer: int = 1,
+        circle: bool = False,
+        ignore_nan: bool = True,
+        **kwargs,
+    ):
+        f = np.nanstd if ignore_nan else np.std
+        return self.focal(lambda a: f(a, axis=2, **kwargs), buffer, circle)
+
+    def focal_var(
+        self,
+        buffer: int = 1,
+        circle: bool = False,
+        ignore_nan: bool = True,
+        **kwargs,
+    ):
+        f = np.nanvar if ignore_nan else np.var
+        return self.focal(lambda a: f(a, axis=2, **kwargs), buffer, circle)
+
+    def focal_min(
+        self,
+        buffer: int = 1,
+        circle: bool = False,
+        ignore_nan: bool = True,
+        **kwargs,
+    ):
+        f = np.nanmin if ignore_nan else np.min
+        return self.focal(lambda a: f(a, axis=2, **kwargs), buffer, circle)
+
+    def focal_max(
+        self,
+        buffer: int = 1,
+        circle: bool = False,
+        ignore_nan: bool = True,
+        **kwargs,
+    ):
+        f = np.nanmax if ignore_nan else np.max
+        return self.focal(lambda a: f(a, axis=2, **kwargs), buffer, circle)
+
+    def focal_sum(
+        self,
+        buffer: int = 1,
+        circle: bool = False,
+        ignore_nan: bool = True,
+        **kwargs,
+    ):
+        f = np.nansum if ignore_nan else np.sum
+        return self.focal(lambda a: f(a, axis=2, **kwargs), buffer, circle)
+
+    def _kwargs(self, ignore_nan: bool, **kwargs):
+        return {
+            "axis": 2,
+            "nan_policy": "omit" if ignore_nan else "propagate",
+            **kwargs,
+        }
+
+    def focal_entropy(self, buffer: int = 1, circle: bool = False, **kwargs):
+        return self.focal(
+            lambda a: sp.stats.entropy(a, axis=2, **kwargs), buffer, circle
+        )
+
+    def focal_gmean(
+        self, buffer: int = 1, circle: bool = False, ignore_nan: bool = True, **kwargs
+    ):
+        return self.focal(
+            lambda a: sp.stats.gmean(a, **self._kwargs(ignore_nan, **kwargs)),
+            buffer,
+            circle,
+        )
+
+    def focal_hmean(
+        self, buffer: int = 1, circle: bool = False, ignore_nan: bool = True, **kwargs
+    ):
+        return self.focal(
+            lambda a: sp.stats.hmean(a, **self._kwargs(ignore_nan, **kwargs)),
+            buffer,
+            circle,
+        )
+
+    def focal_pmean(
+        self,
+        p: float,
+        buffer: int = 1,
+        circle: bool = False,
+        ignore_nan: bool = True,
+        **kwargs,
+    ):
+        return self.focal(
+            lambda a: sp.stats.pmean(a, p, **self._kwargs(ignore_nan, **kwargs)),
+            buffer,
+            circle,
+        )
+
+    def focal_kurtosis(
+        self, buffer: int = 1, circle: bool = False, ignore_nan: bool = True, **kwargs
+    ):
+        return self.focal(
+            lambda a: sp.stats.kurtosis(a, **self._kwargs(ignore_nan, **kwargs)),
+            buffer,
+            circle,
+        )
+
+    def focal_iqr(
+        self, buffer: int = 1, circle: bool = False, ignore_nan: bool = True, **kwargs
+    ):
+        return self.focal(
+            lambda a: sp.stats.iqr(a, **self._kwargs(ignore_nan, **kwargs)),
+            buffer,
+            circle,
+        )
+
+    def focal_mode(
+        self, buffer: int = 1, circle: bool = False, ignore_nan: bool = True, **kwargs
+    ):
+        return self.focal(
+            lambda a: sp.stats.mode(
+                a, **self._kwargs(ignore_nan, keepdims=True, **kwargs)
+            )[0].transpose(2, 0, 1)[0],
+            buffer,
+            circle,
+        )
+
+    def focal_moment(
+        self, buffer: int = 1, circle: bool = False, ignore_nan: bool = True, **kwargs
+    ):
+        return self.focal(
+            lambda a: sp.stats.moment(a, **self._kwargs(ignore_nan, **kwargs)),
+            buffer,
+            circle,
+        )
+
+    def focal_skew(
+        self, buffer: int = 1, circle: bool = False, ignore_nan: bool = True, **kwargs
+    ):
+        return self.focal(
+            lambda a: sp.stats.skew(a, **self._kwargs(ignore_nan, **kwargs)),
+            buffer,
+            circle,
+        )
+
+    def focal_kstat(
+        self, buffer: int = 1, circle: bool = False, ignore_nan: bool = True, **kwargs
+    ):
+        return self.focal(
+            lambda a: sp.stats.kstat(a, **self._kwargs(ignore_nan, **kwargs)),
+            buffer,
+            circle,
+        )
+
+    def focal_kstatvar(
+        self, buffer: int = 1, circle: bool = False, ignore_nan: bool = True, **kwargs
+    ):
+        return self.focal(
+            lambda a: sp.stats.kstatvar(a, **self._kwargs(ignore_nan, **kwargs)),
+            buffer,
+            circle,
+        )
+
+    def focal_tmean(
+        self, buffer: int = 1, circle: bool = False, ignore_nan: bool = True, **kwargs
+    ):
+        return self.focal(
+            lambda a: sp.stats.tmean(a, **self._kwargs(ignore_nan, **kwargs)),
+            buffer,
+            circle,
+        )
+
+    def focal_tvar(self, buffer: int = 1, circle: bool = False, **kwargs):
+        return self.focal(lambda a: sp.stats.tvar(a, axis=2, **kwargs), buffer, circle)
+
+    def focal_tmin(
+        self, buffer: int = 1, circle: bool = False, ignore_nan: bool = True, **kwargs
+    ):
+        return self.focal(
+            lambda a: sp.stats.tmin(a, **self._kwargs(ignore_nan, **kwargs)),
+            buffer,
+            circle,
+        )
+
+    def focal_tmax(
+        self, buffer: int = 1, circle: bool = False, ignore_nan: bool = True, **kwargs
+    ):
+        return self.focal(
+            lambda a: sp.stats.tmax(a, **self._kwargs(ignore_nan, **kwargs)),
+            buffer,
+            circle,
+        )
+
+    def focal_tstd(self, buffer: int = 1, circle: bool = False, **kwargs):
+        return self.focal(lambda a: sp.stats.tstd(a, axis=2, **kwargs), buffer, circle)
+
+    def focal_variation(
+        self, buffer: int = 1, circle: bool = False, ignore_nan: bool = True, **kwargs
+    ):
+        return self.focal(
+            lambda a: sp.stats.variation(a, **self._kwargs(ignore_nan, **kwargs)),
+            buffer,
+            circle,
+        )
+
+    def focal_median_abs_deviation(
+        self, buffer: int = 1, circle: bool = False, ignore_nan: bool = True, **kwargs
+    ):
+        return self.focal(
+            lambda a: sp.stats.median_abs_deviation(
+                a, **self._kwargs(ignore_nan, **kwargs)
+            ),
+            buffer,
+            circle,
+        )
+
+    def focal_chisquare(
+        self, buffer: int = 1, circle: bool = False, **kwargs
+    ) -> StatsResult:
+        def f(grids):
+            return _focal(
+                lambda a: sp.stats.chisquare(a, axis=2, **kwargs),
+                buffer,
+                circle,
+                *grids,
+            )
+
+        return StatsResult(*_batch(f, buffer, self))
+
+    def focal_ttest_ind(
+        self, other_grid: "Grid", buffer: int = 1, circle: bool = False, **kwargs
+    ) -> StatsResult:
+        def f(grids):
+            return _focal(
+                lambda a: sp.stats.ttest_ind(*a, axis=2, **kwargs),
+                buffer,
+                circle,
+                *grids,
+            )
+
+        return StatsResult(*_batch(f, buffer, self, other_grid))
+
+    def zonal(self, func: Callable[[ndarray], Any], zone_grid: "Grid"):
+        zone_grid = zone_grid.type("int32")
+        result = self
+        for zone in set(zone_grid.data[np.isfinite(zone_grid.data)]):
+            data = self.set_nan(zone_grid != zone).data
+            statistics = func(data[np.isfinite(data)])
+            result = con(zone_grid == zone, statistics, result)  # type: ignore
+        return result
+
+    def zonal_count(self, value: Union[float, int], zone_grid: "Grid", **kwargs):
+        return self.zonal(lambda a: np.count_nonzero(a == value, **kwargs), zone_grid)
+
+    def zonal_ptp(self, zone_grid: "Grid", **kwargs):
+        return self.zonal(lambda a: np.ptp(a, **kwargs), zone_grid)
+
+    def zonal_percentile(self, percentile: float, zone_grid: "Grid", **kwargs):
+        return self.zonal(lambda a: np.percentile(a, percentile, **kwargs), zone_grid)
+
+    def zonal_quantile(self, probability: float, zone_grid: "Grid", **kwargs):
+        return self.zonal(lambda a: np.quantile(a, probability, **kwargs), zone_grid)
+
+    def zonal_median(self, zone_grid: "Grid", **kwargs):
+        return self.zonal(lambda a: np.median(a, **kwargs), zone_grid)
+
+    def zonal_mean(self, zone_grid: "Grid", **kwargs):
+        return self.zonal(lambda a: np.mean(a, **kwargs), zone_grid)
+
+    def zonal_std(self, zone_grid: "Grid", **kwargs):
+        return self.zonal(lambda a: np.std(a, **kwargs), zone_grid)
+
+    def zonal_var(self, zone_grid: "Grid", **kwargs):
+        return self.zonal(lambda a: np.var(a, **kwargs), zone_grid)
+
+    def zonal_min(self, zone_grid: "Grid", **kwargs):
+        return self.zonal(lambda a: np.min(a, **kwargs), zone_grid)
+
+    def zonal_max(self, zone_grid: "Grid", **kwargs):
+        return self.zonal(lambda a: np.max(a, **kwargs), zone_grid)
+
+    def zonal_sum(self, zone_grid: "Grid", **kwargs):
+        return self.zonal(lambda a: np.sum(a, **kwargs), zone_grid)
+
+    def zonal_entropy(self, zone_grid: "Grid", **kwargs):
+        return self.zonal(lambda a: sp.stats.entropy(a, **kwargs), zone_grid)
+
+    def zonal_gmean(self, zone_grid: "Grid", **kwargs):
+        return self.zonal(lambda a: sp.stats.gmean(a, **kwargs), zone_grid)
+
+    def zonal_hmean(self, zone_grid: "Grid", **kwargs):
+        return self.zonal(lambda a: sp.stats.hmean(a, **kwargs), zone_grid)
+
+    def zonal_pmean(self, p: float, zone_grid: "Grid", **kwargs):
+        return self.zonal(lambda a: sp.stats.pmean(a, p, **kwargs), zone_grid)
+
+    def zonal_kurtosis(self, zone_grid: "Grid", **kwargs):
+        return self.zonal(lambda a: sp.stats.kurtosis(a, **kwargs), zone_grid)
+
+    def zonal_iqr(self, zone_grid: "Grid", **kwargs):
+        return self.zonal(lambda a: sp.stats.iqr(a, **kwargs), zone_grid)
+
+    def zonal_mode(self, zone_grid: "Grid", **kwargs):
+        return self.zonal(lambda a: sp.stats.mode(a, **kwargs), zone_grid)
+
+    def zonal_moment(self, zone_grid: "Grid", **kwargs):
+        return self.zonal(lambda a: sp.stats.moment(a, **kwargs), zone_grid)
+
+    def zonal_skew(self, zone_grid: "Grid", **kwargs):
+        return self.zonal(lambda a: sp.stats.skew(a, **kwargs), zone_grid)
+
+    def zonal_kstat(self, zone_grid: "Grid", **kwargs):
+        return self.zonal(lambda a: sp.stats.kstat(a, **kwargs), zone_grid)
+
+    def zonal_kstatvar(self, zone_grid: "Grid", **kwargs):
+        return self.zonal(lambda a: sp.stats.kstatvar(a, **kwargs), zone_grid)
+
+    def zonal_tmean(self, zone_grid: "Grid", **kwargs):
+        return self.zonal(lambda a: sp.stats.tmean(a, **kwargs), zone_grid)
+
+    def zonal_tvar(self, zone_grid: "Grid", **kwargs):
+        return self.zonal(lambda a: sp.stats.tvar(a, **kwargs), zone_grid)
+
+    def zonal_tmin(self, zone_grid: "Grid", **kwargs):
+        return self.zonal(lambda a: sp.stats.tmin(a, **kwargs), zone_grid)
+
+    def zonal_tmax(self, zone_grid: "Grid", **kwargs):
+        return self.zonal(lambda a: sp.stats.tmax(a, **kwargs), zone_grid)
+
+    def zonal_tstd(self, zone_grid: "Grid", **kwargs):
+        return self.zonal(lambda a: sp.stats.tstd(a, **kwargs), zone_grid)
+
+    def zonal_variation(self, zone_grid: "Grid", **kwargs):
+        return self.zonal(lambda a: sp.stats.variation(a, **kwargs), zone_grid)
+
+    def zonal_median_abs_deviation(self, zone_grid: "Grid", **kwargs):
+        return self.zonal(
+            lambda a: sp.stats.median_abs_deviation(a, **kwargs), zone_grid
+        )
+
+    def _reproject(
+        self,
+        transform,
+        crs,
+        width,
+        height,
+        resampling: Union[Resampling, ResamplingMethod],
+    ) -> "Grid":
+        source = self * 1 if self.dtype == "bool" else self
+        destination = np.ones((round(height), round(width))) * np.nan
+        reproject(
+            source=source.data,
+            destination=destination,
+            src_transform=self.transform,
+            src_crs=self.crs,
+            src_nodata=self.nodata,
+            dst_transform=transform,
+            dst_crs=crs,
+            dst_nodata=self.nodata,
+            resampling=(
+                Resampling[resampling] if isinstance(resampling, str) else resampling
+            ),
+        )
+        result = _create(destination, crs, transform)
+        if self.dtype == "bool":
+            return result == 1
+        return con(result == result.nodata, np.nan, result)
+
+    def project(
+        self,
+        epsg: Union[int, CRS],
+        resampling: Union[Resampling, ResamplingMethod] = "nearest",
+    ) -> "Grid":
+        crs = CRS.from_epsg(epsg) if isinstance(epsg, int) else epsg
+        transform, width, height = calculate_default_transform(
+            self.crs, crs, self.width, self.height, *self.extent
+        )
+        return self._reproject(
+            transform,
+            crs,
+            width,
+            height,
+            Resampling[resampling] if isinstance(resampling, str) else resampling,
+        )
+
+    def _resample(
+        self,
+        extent: Tuple[float, float, float, float],
+        cell_size: Tuple[float, float],
+        resampling: Union[Resampling, ResamplingMethod],
+    ) -> "Grid":
+        (xmin, ymin, xmax, ymax) = extent
+        xoff = (xmin - self.xmin) / self.transform.a
+        yoff = (ymax - self.ymax) / self.transform.e
+        scaling_x = cell_size[0] / self.cell_size.x
+        scaling_y = cell_size[1] / self.cell_size.y
+        transform = (
+            self.transform
+            * Affine.translation(xoff, yoff)
+            * Affine.scale(scaling_x, scaling_y)
+        )
+        width = (xmax - xmin) / abs(self.transform.a) / scaling_x
+        height = (ymax - ymin) / abs(self.transform.e) / scaling_y
+        return self._reproject(transform, self.crs, width, height, resampling)
+
+    def clip(self, extent: Tuple[float, float, float, float]):
+        return self._resample(extent, self.cell_size, Resampling.nearest)
+
+    def resample(
+        self,
+        cell_size: Union[Tuple[float, float], float],
+        resampling: Union[Resampling, ResamplingMethod] = "nearest",
+    ):
+        if isinstance(cell_size, (int, float)):
+            cell_size = (cell_size, cell_size)
+        if self.cell_size == cell_size:
+            return self
+        return self._resample(self.extent, cell_size, resampling)
+
+    def buffer(self, value: Union[float, int], count: int):
+        if count < 0:
+            grid = (self != value).buffer(1, -count)
+            return con(grid == 0, value, self.set_nan(self == value))
+        grid = self
+        for _ in range(count):
+            grid = con(grid.focal_count(value, 1, True) > 0, value, grid)
+        return grid
+
+    def randomize(self):
+        return self._create(np.random.rand(self.height, self.width))
+
+    def aspect(self):
+        x, y = gradient(self.data)
+        return self._create(arctan2(-x, y))
+
+    def slope(self):
+        x, y = gradient(self.data)
+        return self._create(pi / 2.0 - arctan(sqrt(x * x + y * y)))
+
+    def hillshade(self, azimuth: float = 315, altitude: float = 45):
+        azimuth = np.deg2rad(azimuth)
+        altitude = np.deg2rad(altitude)
+        aspect = self.aspect().data
+        slope = self.slope().data
+        shaded = sin(altitude) * sin(slope) + cos(altitude) * cos(slope) * cos(
+            azimuth - aspect
+        )
+        return self._create((255 * (shaded + 1) / 2))
+
+    def reclass(self, *mappings: Tuple[float, float, float]):
+        conditions = [
+            (self.data >= min) & (self.data < max) for min, max, _ in mappings
+        ]
+        values = [value for _, _, value in mappings]
+        return self._create(np.select(conditions, values, np.nan))
+
+    def slice(self, count: int, percent_clip: float = 0.1):
+        min = self.percentile(percent_clip)
+        max = self.percentile(100 - percent_clip)
+        interval = (max - min) / count
+        mappings = [
+            (
+                min + (i - 1) * interval if i > 1 else float("-inf"),
+                min + i * interval if i < count else float("inf"),
+                float(i),
+            )
+            for i in range(1, count + 1)
+        ]
+        return self.reclass(*mappings)
+
+    def fill_nan(self, max_exponent: int = 4):
+        if not self.has_nan:
+            return self
+
+        def f(grids):
+            grid = grids[0]
+            n = 0
+            while grid.has_nan and n <= max_exponent:
+                grid = con(grid.is_nan(), grid.focal_mean(2**n, True), grid)
+                n += 1
+            return (grid,)
+
+        return _batch(f, 2**max_exponent, self)[0]
+
+    def replace(
+        self, value: Operand, replacement: Operand, fallback: Optional[Operand] = None
+    ):
+        return con(
+            value if isinstance(value, Grid) else self == value,
+            replacement,
+            self if fallback is None else fallback,
+        )
+
+    def set_nan(self, value: Operand, fallback: Optional[Operand] = None):
+        return self.replace(value, np.nan, fallback)
+
+    def value(self, x: float, y: float) -> float:
+        xoff = (x - self.xmin) / self.transform.a
+        yoff = (y - self.ymax) / self.transform.e
+        if xoff < 0 or xoff >= self.width or yoff < 0 or yoff >= self.height:
+            return float(np.nan)
+        return float(self.data[int(yoff), int(xoff)])
+
+    def data_extent(self):
+        xmin, ymin, xmax, ymax = None, None, None, None
+        for x, y, _ in self.to_points():
+            if not xmin or x < xmin:
+                xmin = x
+            if not ymin or y < ymin:
+                ymin = y
+            if not xmax or x > xmax:
+                xmax = x
+            if not ymax or y > ymax:
+                ymax = y
+        if xmin is None or ymin is None or xmax is None or ymax is None:
+            raise ValueError("None of the cells has a value.")
+        return Extent(
+            xmin - self.cell_size.x / 2,
+            ymin - self.cell_size.y / 2,
+            xmax + self.cell_size.x / 2,
+            ymax + self.cell_size.y / 2,
+        )
+
+    def to_points(self) -> Iterable[Point]:
+        for y, row in enumerate(self.data):
+            for x, value in enumerate(row):
+                if np.isfinite(value):
+                    yield Point(
+                        self.xmin + (x + 0.5) * self.cell_size.x,
+                        self.ymax - (y + 0.5) * self.cell_size.y,
+                        float(value),
+                    )
+
+    def to_polygons(self) -> Iterable[Tuple[Polygon, float]]:
+        for shape, value in features.shapes(
+            self.data, mask=np.isfinite(self.data), transform=self.transform
+        ):
+            if np.isfinite(value):
+                coordinates = shape["coordinates"]
+                yield Polygon(coordinates[0], coordinates[1:]), float(value)
+
+    def from_polygons(
+        self, polygons: Iterable[Tuple[Polygon, float]], all_touched: bool = False
+    ):
+        array = features.rasterize(
+            shapes=polygons,
+            out_shape=self.data.shape,
+            fill=np.nan,  # type: ignore
+            transform=self.transform,
+            all_touched=all_touched,
+            default_value=np.nan,  # type: ignore
+        )
+        return self._create(array)
+
+    def to_stack(self, cmap: Union[ColorMap, Any]):
+        from glidergun._stack import stack
+
+        grid1 = self - self.min
+        grid2 = grid1 / grid1.max
+        arrays = plt.get_cmap(cmap)(grid2.data).transpose(2, 0, 1)[:3]  # type: ignore
+        mask = self.is_nan()
+        r, g, b = [self._create(a * 253 + 1).set_nan(mask) for a in arrays]
+        return stack(r, g, b)
+
+    def scale(self, scaler: Optional[Scaler] = None, **fit_params):
+        if not scaler:
+            scaler = QuantileTransformer(n_quantiles=10)
+        return self.local(lambda a: scaler.fit_transform(a, **fit_params))
+
+    def stretch(self, min_value: float, max_value: float):
+        expected_range = max_value - min_value
+        actual_range = self.max - self.min
+
+        if actual_range == 0:
+            return self
+
+        return (self - self.min) * expected_range / actual_range + min_value
+
+    def cap_range(self, min: Operand, max: Operand, set_nan: bool = False):
+        return self.cap_min(min, set_nan).cap_max(max, set_nan)
+
+    def cap_min(self, value: Operand, set_nan: bool = False):
+        return con(self < value, np.nan if set_nan else value, self)
+
+    def cap_max(self, value: Operand, set_nan: bool = False):
+        return con(self > value, np.nan if set_nan else value, self)
+
+    def percent_clip(self, min_percent: float, max_percent: float):
+        min_value = self.percentile(min_percent)
+        max_value = self.percentile(max_percent)
+
+        if min_value == max_value:
+            return self
+
+        return self.cap_range(min_value, max_value)
+
+    def to_uint8_range(self):
+        if self.dtype == "bool" or self.min > 0 and self.max < 255:
+            return self
+        return self.percent_clip(0.1, 99.9).stretch(1, 254)
+
+    def fit(self, model: T, *explanatory_grids: "Grid") -> GridEstimator[T]:
+        return GridEstimator(model).fit(self, *explanatory_grids)
+
+    def hist(self, **kwargs):
+        return plt.bar(list(self.bins.keys()), list(self.bins.values()), **kwargs)
+
+    def plot(self, cmap: Union[ColorMap, Any]):
+        return dataclasses.replace(self, _cmap=cmap)
+
+    def map(
+        self,
+        cmap: Union[ColorMap, Any] = "gray",
+        opacity: float = 1.0,
+        folium_map=None,
+        width: int = 800,
+        height: int = 600,
+        basemap: Optional[str] = None,
+        attribution: Optional[str] = None,
+        grayscale: bool = True,
+        **kwargs,
+    ):
+        from glidergun._ipython import _map
+
+        return _map(
+            self,
+            cmap,
+            opacity,
+            folium_map,
+            width,
+            height,
+            basemap,
+            attribution,
+            grayscale,
+            **kwargs,
+        )
+
+    def type(self, dtype: DataType):
+        if self.dtype == dtype:
+            return self
+        return self.local(lambda data: np.asanyarray(data, dtype=dtype))
+
+    @overload
+    def save(
+        self, file: str, dtype: Optional[DataType] = None, driver: str = ""
+    ) -> None: ...
+
+    @overload
+    def save(
+        self, file: MemoryFile, dtype: Optional[DataType] = None, driver: str = ""
+    ) -> None: ...
+
+    def save(self, file, dtype: Optional[DataType] = None, driver: str = ""):
+        grid = self * 1 if self.dtype == "bool" else self
+
+        if isinstance(file, str) and (
+            file.lower().endswith(".jpg")
+            or file.lower().endswith(".kml")
+            or file.lower().endswith(".kmz")
+            or file.lower().endswith(".png")
+        ):
+            grid = grid.to_uint8_range()
+            dtype = "uint8"
+        else:
+            grid = grid
+            if dtype is None:
+                dtype = grid.dtype
+
+        nodata = _nodata(dtype)
+
+        if nodata is not None:
+            grid = con(grid.is_nan(), nodata, grid)
+
+        if isinstance(file, str):
+            with rasterio.open(
+                file,
+                "w",
+                driver=driver if driver else driver_from_extension(file),
+                count=1,
+                dtype=dtype,
+                nodata=nodata,
+                **_metadata(self),
+            ) as dataset:
+                dataset.write(grid.data, 1)
+        elif isinstance(file, MemoryFile):
+            with file.open(
+                driver=driver if driver else "GTiff",
+                count=1,
+                dtype=dtype,
+                nodata=nodata,
+                **_metadata(self),
+            ) as dataset:
+                dataset.write(grid.data, 1)
+
+    def save_plot(self, file):
+        self.to_stack(self._cmap).save(file)
+
+
+@overload
+def grid(file: str, index: int = 1) -> Grid:
+    """Creates a new grid from a file path.
+
+    Args:
+        file (str): File path.
+        index (int, optional): Band index.  Defaults to 1.
+
+    Returns:
+        Grid: A new grid.
+    """
+    ...
+
+
+@overload
+def grid(file: MemoryFile, index: int = 1) -> Grid:
+    """Creates a new grid from an in-memory file.
+
+    Args:
+        file (MemoryFile): Rasterio in-memory file.
+        index (int, optional): Band index.  Defaults to 1.
+
+    Returns:
+        Grid: A new grid.
+    """
+    ...
+
+
+def grid(file, index: int = 1) -> Grid:
+    if isinstance(file, str):
+        with rasterio.open(file) as dataset:
+            return _read(dataset, index)
+    elif isinstance(file, MemoryFile):
+        with file.open() as dataset:
+            return _read(dataset, index)
+    raise ValueError()
+
+
+def _create(data: ndarray, crs: CRS, transform: Affine):
+    if data.dtype == "float64":
+        data = np.asanyarray(data, dtype="float32")
+    elif data.dtype == "int64":
+        data = np.asanyarray(data, dtype="int32")
+    elif data.dtype == "uint64":
+        data = np.asanyarray(data, dtype="uint32")
+    return Grid(data, crs, transform)
+
+
+def _read(dataset, index):
+    grid = _create(dataset.read(index), dataset.crs, dataset.transform)
+    return grid if dataset.nodata is None else grid.set_nan(dataset.nodata)
+
+
+def _metadata(grid: Grid):
+    return {
+        "height": grid.height,
+        "width": grid.width,
+        "crs": grid.crs,
+        "transform": grid.transform,
+    }
+
+
+def _mask(buffer: int) -> ndarray:
+    size = 2 * buffer + 1
+    rows = []
+    for y in range(size):
+        row = []
+        for x in range(size):
+            d = ((x - buffer) ** 2 + (y - buffer) ** 2) ** (1 / 2)
+            row.append(d <= buffer)
+        rows.append(row)
+    return np.array(rows)
+
+
+def _pad(data: ndarray, buffer: int):
+    row = np.zeros((buffer, data.shape[1])) * np.nan
+    col = np.zeros((data.shape[0] + 2 * buffer, buffer)) * np.nan
+    return np.hstack([col, np.vstack([row, data, row]), col], dtype="float32")
+
+
+def _focal(func: Callable, buffer: int, circle: bool, *grids: Grid) -> Tuple[Grid, ...]:
+    grids_adjusted = standardize(*grids)
+    size = 2 * buffer + 1
+    mask = _mask(buffer) if circle else np.full((size, size), True)
+
+    if len(grids) == 1:
+        array = sliding_window_view(_pad(grids[0].data, buffer), (size, size))
+        result = func(array[:, :, mask])
+    else:
+        array = np.stack(
+            [
+                sliding_window_view(_pad(g.data, buffer), (size, size))
+                for g in grids_adjusted
+            ]
+        )
+        transposed = np.transpose(array, axes=(1, 2, 0, 3, 4))[:, :, :, mask]
+        result = func(tuple(transposed[:, :, i] for i, _ in enumerate(grids)))
+
+    if isinstance(result, ndarray) and len(result.shape) == 2:
+        return (grids_adjusted[0]._create(np.array(result)),)
+
+    return tuple([grids_adjusted[0]._create(r) for r in result])
+
+
+def _batch(
+    func: Callable[[Tuple[Grid, ...]], Tuple[Grid, ...]], buffer: int, *grids: Grid
+) -> Tuple[Grid, ...]:
+    stride = 8000 // buffer // len(grids)
+    grids1 = standardize(*grids)
+    grid = grids1[0]
+
+    def tile():
+        for x in range(0, grid.width // stride + 1):
+            xmin, xmax = x * stride, min((x + 1) * stride, grid.width)
+            if xmin < xmax:
+                for y in range(0, grid.height // stride + 1):
+                    ymin, ymax = y * stride, min((y + 1) * stride, grid.height)
+                    if ymin < ymax:
+                        yield xmin, ymin, xmax, ymax
+
+    tiles = list(tile())
+    count = len(tiles)
+
+    if count <= 4:
+        return func(tuple(grids1))
+
+    results: List[Grid] = []
+    cell_size = grid.cell_size
+    n = 0
+
+    for xmin, ymin, xmax, ymax in tiles:
+        n += 1
+        sys.stdout.write(f"\rProcessing {n} of {count} tiles...")
+        sys.stdout.flush()
+        grids2 = [
+            g.clip(
+                (
+                    grid.xmin + (xmin - buffer) * cell_size.x,
+                    grid.ymin + (ymin - buffer) * cell_size.y,
+                    grid.xmin + (xmax + buffer) * cell_size.x,
+                    grid.ymin + (ymax + buffer) * cell_size.y,
+                )
+            )
+            for g in grids1
+        ]
+
+        grids3 = func(tuple(grids2))
+
+        grids4 = [
+            g.clip(
+                (
+                    grid.xmin + xmin * cell_size.x,
+                    grid.ymin + ymin * cell_size.y,
+                    grid.xmin + xmax * cell_size.x,
+                    grid.ymin + ymax * cell_size.y,
+                )
+            )
+            for g in grids3
+        ]
+
+        if results:
+            for i, g in enumerate(grids4):
+                results[i] = mosaic(results[i], g)
+        else:
+            results = grids4
+
+    print()
+    return tuple(results)
+
+
+def con(grid: Grid, trueValue: Operand, falseValue: Operand):
+    return grid.local(
+        lambda data: np.where(data, grid._data(trueValue), grid._data(falseValue))
+    )
+
+
+def _aggregate(func: Callable, *grids: Grid) -> Grid:
+    grids_adjusted = standardize(*grids)
+    data = func(np.array([grid.data for grid in grids_adjusted]), axis=0)
+    return grids_adjusted[0]._create(data)
+
+
+def mean(*grids: Grid) -> Grid:
+    return _aggregate(np.mean, *grids)
+
+
+def std(*grids: Grid) -> Grid:
+    return _aggregate(np.std, *grids)
+
+
+def minimum(*grids: Grid) -> Grid:
+    return _aggregate(np.min, *grids)
+
+
+def maximum(*grids: Grid) -> Grid:
+    return _aggregate(np.max, *grids)
+
+
+def load_model(file: str) -> GridEstimator[Any]:
+    return GridEstimator.load(file)
+
+
+def mosaic(*grids: Grid) -> Grid:
+    grids_adjusted = standardize(*grids, extent="union")
+    result = grids_adjusted[0]
+    for grid in grids_adjusted[1:]:
+        result = con(result.is_nan(), grid, result)
+    return result
+
+
+def pca(n_components: int = 1, *grids: Grid) -> Tuple[Grid, ...]:
+    grids_adjusted = [con(g.is_nan(), g.mean, g) for g in standardize(*grids)]
+    arrays = (
+        PCA(n_components=n_components)
+        .fit_transform(
+            np.array(
+                [g.scale(StandardScaler()).data.ravel() for g in grids_adjusted]
+            ).transpose((1, 0))
+        )
+        .transpose((1, 0))
+    )
+    grid = grids_adjusted[0]
+    return tuple(grid._create(a.reshape((grid.height, grid.width))) for a in arrays)
+
+
+def standardize(
+    *grids: Grid,
+    extent: Union[Extent, ExtentResolution] = "intersect",
+    cell_size: Union[Tuple[float, float], float, None] = None,
+) -> Tuple[Grid, ...]:
+    if len(grids) == 1:
+        return tuple(grids)
+
+    crs_set = set(grid.crs for grid in grids)
+
+    if len(crs_set) > 1:
+        raise ValueError("Input grids must have the same CRS.")
+
+    if isinstance(cell_size, (int, float)):
+        cell_size_standardized = (cell_size, cell_size)
+    elif cell_size is None:
+        cell_size_standardized = grids[0].cell_size
+    else:
+        cell_size_standardized = cell_size
+
+    if isinstance(extent, Extent):
+        extent_standardized = extent
+    else:
+        extent_standardized = grids[0].extent
+        for grid in grids:
+            if extent == "intersect":
+                extent_standardized = extent_standardized & grid.extent
+            elif extent == "union":
+                extent_standardized = extent_standardized | grid.extent
+
+    results = []
+
+    for grid in grids:
+        if grid.cell_size != cell_size_standardized:
+            grid = grid.resample(cell_size_standardized)
+        if grid.extent != extent_standardized:
+            grid = grid.clip(extent_standardized)  # type: ignore
+        results.append(grid)
+
+    return tuple(results)
+
+
+def create(
+    extent: Tuple[float, float, float, float],
+    epsg: Union[int, CRS],
+    cell_size: Union[Tuple[float, float], float],
+):
+    cell_size = (
+        CellSize(cell_size, cell_size)
+        if isinstance(cell_size, (int, float))
+        else CellSize(*cell_size)
+    )
+    xmin, ymin, xmax, ymax = extent
+    width = int((xmax - xmin) / cell_size.x)
+    height = int((ymax - ymin) / cell_size.y)
+    xmin = xmax - cell_size.x * width
+    ymax = ymin + cell_size.y * height
+    crs = CRS.from_epsg(epsg) if isinstance(epsg, int) else epsg
+    transform = Affine(cell_size.x, 0, xmin, 0, -cell_size.y, ymax, 0, 0, 1)
+    return Grid(np.zeros((height, width), "uint8"), crs, transform)
+
+
+def interpolate(
+    interpolator_factory: Callable[[ndarray, ndarray], Any],
+    points: Iterable[Tuple[float, float, float]],
+    epsg: Union[int, CRS],
+    cell_size: Union[Tuple[float, float], float],
+):
+    coord_array = []
+    value_array = []
+
+    for p in points:
+        coord_array.append(p[:2])
+        value_array.append(p[-1])
+
+    coords = np.array(coord_array)
+    values = np.array(value_array)
+    x, y = coords.transpose(1, 0)
+    xmin, ymin, xmax, ymax = x.min(), y.min(), x.max(), y.max()
+    extent = Extent(xmin, ymin, xmax, ymax)
+    grid = create(extent, epsg, cell_size)
+    interp = interpolator_factory(coords, values)
+    xs = np.linspace(xmin, xmax, grid.width)
+    ys = np.linspace(ymax, ymin, grid.height)
+    array = np.array([[x0, y0] for x0 in xs for y0 in ys])
+    data = interp(array).reshape((grid.width, grid.height)).transpose(1, 0)
+
+    return grid.local(lambda _: data)
+
+
+def interp_linear(
+    points: Iterable[Tuple[float, float, float]],
+    epsg: Union[int, CRS],
+    cell_size: Union[Tuple[float, float], float],
+    fill_value: float = np.nan,
+    rescale: bool = False,
+):
+    def f(coords, values):
+        return LinearNDInterpolator(coords, values, fill_value, rescale)
+
+    return interpolate(f, points, epsg, cell_size)
+
+
+def interp_nearest(
+    points: Iterable[Tuple[float, float, float]],
+    epsg: Union[int, CRS],
+    cell_size: Union[Tuple[float, float], float],
+    rescale: bool = False,
+    tree_options: Any = None,
+):
+    def f(coords, values):
+        return NearestNDInterpolator(coords, values, rescale, tree_options)
+
+    return interpolate(f, points, epsg, cell_size)
+
+
+def interp_rbf(
+    points: Iterable[Tuple[float, float, float]],
+    epsg: Union[int, CRS],
+    cell_size: Union[Tuple[float, float], float],
+    neighbors: Optional[int] = None,
+    smoothing: float = 0,
+    kernel: InterpolationKernel = "thin_plate_spline",
+    epsilon: float = 1,
+    degree: Optional[int] = None,
+):
+    def f(coords, values):
+        return RBFInterpolator(
+            coords, values, neighbors, smoothing, kernel, epsilon, degree
+        )
+
+    return interpolate(f, points, epsg, cell_size)
+
+
+def _nodata(dtype: str) -> Union[float, int, None]:
+    if dtype == "bool":
+        return None
+    if dtype.startswith("float"):
+        return float(np.finfo(dtype).min)
+    if dtype.startswith("uint"):
+        return np.iinfo(dtype).max
+    return np.iinfo(dtype).min
```

### Comparing `glidergun-0.5.1/glidergun/ipython.py` & `glidergun-0.5.4/glidergun/_ipython.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,122 +1,130 @@
-from base64 import b64encode
-from io import BytesIO
-from typing import Optional, Union
-
-import IPython
-import matplotlib.pyplot as plt
-import numpy as np
-
-from glidergun.grid import Grid
-from glidergun.stack import Stack
-
-
-def _thumbnail(obj: Union[Grid, Stack], color, figsize=None):
-    with BytesIO() as buffer:
-        figure = plt.figure(figsize=figsize, frameon=False)
-        axes = figure.add_axes((0, 0, 1, 1))
-        axes.axis("off")
-
-        n = 2000 / max(obj.width, obj.height)
-
-        if n < 1:
-            obj = obj.resample(obj.cell_size / n)
-
-        obj = obj.to_uint8_range()
-
-        if isinstance(obj, Grid):
-            plt.imshow(obj.data, cmap=color)
-
-        elif isinstance(obj, Stack):
-            rgb = [obj.grids[i - 1].data for i in (color if color else (1, 2, 3))]
-            alpha = np.where(np.isfinite(rgb[0] + rgb[1] + rgb[2]), 255, 0)
-            plt.imshow(np.dstack([*[np.asanyarray(g, "uint8") for g in rgb], alpha]))
-
-        plt.savefig(buffer, bbox_inches="tight", pad_inches=0)
-        plt.close(figure)
-        image = b64encode(buffer.getvalue()).decode()
-        return f"data:image/png;base64, {image}"
-
-
-def _map(
-    obj: Union[Grid, Stack],
-    color,
-    opacity: float,
-    folium_map,
-    width: int,
-    height: int,
-    basemap: Optional[str],
-    attribution: Optional[str],
-    grayscale: bool = True,
-    **kwargs,
-):
-    import folium
-    import jinja2
-
-    obj = obj.project(4326)
-    figure = folium.Figure(width=str(width), height=height)
-    bounds = [[obj.ymin, obj.xmin], [obj.ymax, obj.xmax]]
-
-    if folium_map is None:
-        if basemap:
-            tile_layer = folium.TileLayer(basemap, attr=attribution)
-        else:
-            tile_layer = folium.TileLayer(
-                tiles="https://server.arcgisonline.com/ArcGIS/rest/services/World_Imagery/MapServer/tile/{z}/{y}/{x}",
-                attr="&copy; Esri",
-            )
-
-        options = {"zoom_control": False, **kwargs}
-        folium_map = folium.Map(tiles=tile_layer, **options).add_to(figure)
-        folium_map.fit_bounds(bounds)
-
-        if grayscale:
-            macro = folium.MacroElement().add_to(folium_map)
-            macro._template = jinja2.Template(
-                f"""
-                {{% macro script(this, kwargs) %}}
-                tile_layer_{tile_layer._id}.getContainer()
-                    .setAttribute("style", "filter: grayscale(100%); -webkit-filter: grayscale(100%);")
-                {{% endmacro %}}
-            """
-            )
-
-    folium.raster_layers.ImageOverlay(  # type: ignore
-        image=_thumbnail(obj, color, (20, 20)),
-        bounds=bounds,
-        opacity=opacity,
-    ).add_to(folium_map)
-
-    return folium_map
-
-
-ipython = IPython.get_ipython()  # type: ignore
-
-if ipython:
-
-    def html(obj: Union[Grid, Stack]):
-        description = str(obj).replace("|", "<br />")
-        if isinstance(obj, Grid):
-            thumbnail = _thumbnail(obj, obj._cmap)
-            extent = obj.extent
-        elif isinstance(obj, Stack):
-            thumbnail = _thumbnail(obj, obj._rgb)
-            extent = obj.extent
-        return f'<div>{description}</div><img src="{thumbnail}" /><div>{extent}</div>'
-
-    formatter = ipython.display_formatter.formatters["text/html"]  # type: ignore
-    formatter.for_type(Grid, html)
-    formatter.for_type(Stack, html)
-    formatter.for_type(
-        tuple,
-        lambda items: (
-            f"""
-            <table>
-                <tr style="text-align: left">
-                    {"".join(f"<td>{html(item)}</td>" for item in items)}
-                </tr>
-            </table>
-        """
-            if all(isinstance(item, Grid) or isinstance(item, Stack) for item in items)
-            else f"{items}"
-        ),
-    )
+from base64 import b64encode
+from io import BytesIO
+from typing import Optional, Union
+
+import IPython
+import matplotlib.pyplot as plt
+import numpy as np
+
+from glidergun._grid import Grid
+from glidergun._stack import Stack
+
+
+def _thumbnail(obj: Union[Grid, Stack], color, figsize=None):
+    with BytesIO() as buffer:
+        figure = plt.figure(figsize=figsize, frameon=False)
+        axes = figure.add_axes((0, 0, 1, 1))
+        axes.axis("off")
+
+        n = 2000 / max(obj.width, obj.height)
+
+        if n < 1:
+            obj = obj.resample(obj.cell_size / n)
+
+        obj = obj.to_uint8_range()
+
+        if isinstance(obj, Grid):
+            plt.imshow(obj.data, cmap=color)
+
+        elif isinstance(obj, Stack):
+            rgb = [
+                obj.grids[i - 1].data for i in (color if color else (1, 2, 3))]
+            alpha = np.where(np.isfinite(rgb[0] + rgb[1] + rgb[2]), 255, 0)
+            plt.imshow(
+                np.dstack([*[np.asanyarray(g, "uint8") for g in rgb], alpha]))
+
+        plt.savefig(buffer, bbox_inches="tight", pad_inches=0)
+        plt.close(figure)
+        image = b64encode(buffer.getvalue()).decode()
+        return f"data:image/png;base64, {image}"
+
+
+def _map(
+    obj: Union[Grid, Stack],
+    color,
+    opacity: float,
+    folium_map,
+    width: int,
+    height: int,
+    basemap: Optional[str],
+    attribution: Optional[str],
+    grayscale: bool = True,
+    **kwargs,
+):
+    import folium
+    import jinja2
+
+    obj = obj.project(4326)
+    obj_4326 = obj.clip((obj.xmin, max(obj.ymin, -80),
+                        obj.xmax, min(obj.ymax, 80)))
+    obj_3857 = obj_4326.project(3857)
+
+    figure = folium.Figure(width=str(width), height=height)
+    bounds = [[obj_4326.ymin, obj_4326.xmin],
+              [obj_4326.ymax, obj_4326.xmax]]
+
+    if folium_map is None:
+        if basemap:
+            tile_layer = folium.TileLayer(basemap, attr=attribution)
+        else:
+            tile_layer = folium.TileLayer(
+                tiles="https://server.arcgisonline.com/ArcGIS/rest/services/World_Imagery/MapServer/tile/{z}/{y}/{x}",
+                attr="&copy; Esri",
+            )
+
+        options = {"zoom_control": False, **kwargs}
+        folium_map = folium.Map(tiles=tile_layer, **options).add_to(figure)
+        folium_map.fit_bounds(bounds)
+
+        if grayscale:
+            macro = folium.MacroElement().add_to(folium_map)
+            macro._template = jinja2.Template(
+                f"""
+                {{% macro script(this, kwargs) %}}
+                tile_layer_{tile_layer._id}.getContainer()
+                    .setAttribute("style", "filter: grayscale(100%); -webkit-filter: grayscale(100%);")
+                {{% endmacro %}}
+            """
+            )
+
+    folium.raster_layers.ImageOverlay(  # type: ignore
+        image=_thumbnail(obj_3857, color, (20, 20)),
+        bounds=bounds,
+        opacity=opacity,
+    ).add_to(folium_map)
+
+    return folium_map
+
+
+ipython = IPython.get_ipython()  # type: ignore
+
+if ipython:
+
+    def html(obj: Union[Grid, Stack]):
+        description = str(obj).replace("|", "<br />")
+        if isinstance(obj, Grid):
+            thumbnail = _thumbnail(obj, obj._cmap)
+            extent = obj.extent
+        elif isinstance(obj, Stack):
+            thumbnail = _thumbnail(obj, obj._rgb)
+            extent = obj.extent
+        return f'<div>{description}</div><img src="{thumbnail}" /><div>{extent}</div>'
+
+    # type: ignore
+    formatter = ipython.display_formatter.formatters["text/html"]
+    formatter.for_type(Grid, html)
+    formatter.for_type(Stack, html)
+    formatter.for_type(
+        tuple,
+        lambda items: (
+            f"""
+            <table>
+                <tr style="text-align: left">
+                    {"".join(f"<td>{html(item)}</td>" for item in items)}
+                </tr>
+            </table>
+        """
+            if all(isinstance(item, Grid) or isinstance(item, Stack) for item in items)
+            else f"{items}"
+        ),
+    )
```

### Comparing `glidergun-0.5.1/glidergun/stack.py` & `glidergun-0.5.4/glidergun/_stack.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,383 +1,383 @@
-import dataclasses
-from dataclasses import dataclass
-from typing import Callable, List, Optional, Tuple, Union, overload
-
-import rasterio
-from rasterio.crs import CRS
-from rasterio.drivers import driver_from_extension
-from rasterio.io import MemoryFile
-from rasterio.warp import Resampling
-
-from glidergun.grid import (
-    CellSize,
-    Extent,
-    Grid,
-    Scaler,
-    _metadata,
-    _nodata,
-    _read,
-    con,
-    pca,
-    standardize,
-)
-from glidergun.literals import DataType
-
-Operand = Union["Stack", Grid, float, int]
-
-
-@dataclass(frozen=True)
-class Stack:
-    grids: Tuple[Grid, ...]
-    _rgb: Tuple[int, int, int] = (1, 2, 3)
-
-    def __repr__(self):
-        g = self.grids[0]
-        return (
-            f"image: {g.width}x{g.height} {g.dtype} | "
-            + f"crs: {g.crs} | "
-            + f"cell: {g.cell_size.x}, {g.cell_size.y} | "
-            + f"count: {len(self.grids)} | "
-            + f"rgb: {self._rgb}"
-        )
-
-    @property
-    def crs(self) -> CRS:
-        return self.grids[0].crs
-
-    @property
-    def width(self) -> int:
-        return self.grids[0].width
-
-    @property
-    def height(self) -> int:
-        return self.grids[0].height
-
-    @property
-    def dtype(self) -> DataType:
-        return self.grids[0].dtype
-
-    @property
-    def xmin(self) -> float:
-        return self.grids[0].xmin
-
-    @property
-    def ymin(self) -> float:
-        return self.grids[0].ymin
-
-    @property
-    def xmax(self) -> float:
-        return self.grids[0].xmax
-
-    @property
-    def ymax(self) -> float:
-        return self.grids[0].ymax
-
-    @property
-    def cell_size(self) -> CellSize:
-        return self.grids[0].cell_size
-
-    @property
-    def extent(self) -> Extent:
-        return self.grids[0].extent
-
-    @property
-    def md5s(self) -> Tuple[str, ...]:
-        return tuple(g.md5 for g in self.grids)
-
-    def __add__(self, n: Operand):
-        return self._apply(n, lambda g, n: g.__add__(n))
-
-    __radd__ = __add__
-
-    def __sub__(self, n: Operand):
-        return self._apply(n, lambda g, n: g.__sub__(n))
-
-    def __rsub__(self, n: Operand):
-        return self._apply(n, lambda g, n: g.__rsub__(n))
-
-    def __mul__(self, n: Operand):
-        return self._apply(n, lambda g, n: g.__mul__(n))
-
-    __rmul__ = __mul__
-
-    def __pow__(self, n: Operand):
-        return self._apply(n, lambda g, n: g.__pow__(n))
-
-    def __rpow__(self, n: Operand):
-        return self._apply(n, lambda g, n: g.__rpow__(n))
-
-    def __truediv__(self, n: Operand):
-        return self._apply(n, lambda g, n: g.__truediv__(n))
-
-    def __rtruediv__(self, n: Operand):
-        return self._apply(n, lambda g, n: g.__rtruediv__(n))
-
-    def __floordiv__(self, n: Operand):
-        return self._apply(n, lambda g, n: g.__floordiv__(n))
-
-    def __rfloordiv__(self, n: Operand):
-        return self._apply(n, lambda g, n: g.__rfloordiv__(n))
-
-    def __mod__(self, n: Operand):
-        return self._apply(n, lambda g, n: g.__mod__(n))
-
-    def __rmod__(self, n: Operand):
-        return self._apply(n, lambda g, n: g.__rmod__(n))
-
-    def __lt__(self, n: Operand):
-        return self._apply(n, lambda g, n: g.__lt__(n))
-
-    def __gt__(self, n: Operand):
-        return self._apply(n, lambda g, n: g.__gt__(n))
-
-    __rlt__ = __gt__
-
-    __rgt__ = __lt__
-
-    def __le__(self, n: Operand):
-        return self._apply(n, lambda g, n: g.__le__(n))
-
-    def __ge__(self, n: Operand):
-        return self._apply(n, lambda g, n: g.__ge__(n))
-
-    __rle__ = __ge__
-
-    __rge__ = __le__
-
-    def __eq__(self, n: Operand):
-        return self._apply(n, lambda g, n: g.__eq__(n))
-
-    __req__ = __eq__
-
-    def __ne__(self, n: Operand):
-        return self._apply(n, lambda g, n: g.__ne__(n))
-
-    __rne__ = __ne__
-
-    def __and__(self, n: Operand):
-        return self._apply(n, lambda g, n: g.__and__(n))
-
-    __rand__ = __and__
-
-    def __or__(self, n: Operand):
-        return self._apply(n, lambda g, n: g.__or__(n))
-
-    __ror__ = __or__
-
-    def __xor__(self, n: Operand):
-        return self._apply(n, lambda g, n: g.__xor__(n))
-
-    __rxor__ = __xor__
-
-    def __rshift__(self, n: Operand):
-        return self._apply(n, lambda g, n: g.__rshift__(n))
-
-    def __lshift__(self, n: Operand):
-        return self._apply(n, lambda g, n: g.__lshift__(n))
-
-    __rrshift__ = __lshift__
-
-    __rlshift__ = __rshift__
-
-    def __neg__(self):
-        return self.each(lambda g: g.__neg__())
-
-    def __pos__(self):
-        return self.each(lambda g: g.__pos__())
-
-    def __invert__(self):
-        return self.each(lambda g: g.__invert__())
-
-    def _apply(self, n: Operand, op: Callable):
-        if isinstance(n, Stack):
-            return self.zip_with(n, lambda g1, g2: op(g1, g2))
-        return self.each(lambda g: op(g, n))
-
-    def scale(self, scaler: Optional[Scaler] = None, **fit_params):
-        return self.each(lambda g: g.scale(scaler, **fit_params))
-
-    def percent_clip(self, min_percent: float, max_percent: float):
-        return self.each(lambda g: g.percent_clip(min_percent, max_percent))
-
-    def to_uint8_range(self):
-        return self.each(lambda g: g.to_uint8_range())
-
-    def plot(self, r: int, g: int, b: int):
-        return dataclasses.replace(self, _rgb=(r, g, b))
-
-    def map(
-        self,
-        r: int,
-        g: int,
-        b: int,
-        opacity: float = 1.0,
-        folium_map=None,
-        width: int = 800,
-        height: int = 600,
-        basemap: Optional[str] = None,
-        attribution: Optional[str] = None,
-        grayscale: bool = True,
-        **kwargs,
-    ):
-        from glidergun.ipython import _map
-
-        return _map(
-            self,
-            (r, g, b),
-            opacity,
-            folium_map,
-            width,
-            height,
-            basemap,
-            attribution,
-            grayscale,
-            **kwargs,
-        )
-
-    def each(self, func: Callable[[Grid], Grid]):
-        return stack(*map(func, self.grids))
-
-    def clip(self, extent: Tuple[float, float, float, float]):
-        return self.each(lambda g: g.clip(extent))
-
-    def extract_bands(self, *bands: int):
-        return stack(*(self.grids[i - 1] for i in bands))
-
-    def pca(self, n_components: int = 3):
-        return stack(*pca(n_components, *self.grids))
-
-    def project(
-        self, epsg: Union[int, CRS], resampling: Resampling = Resampling.nearest
-    ):
-        return self.each(lambda g: g.project(epsg, resampling))
-
-    def resample(
-        self,
-        cell_size: Union[Tuple[float, float], float],
-        resampling: Resampling = Resampling.nearest,
-    ):
-        return self.each(lambda g: g.resample(cell_size, resampling))
-
-    def zip_with(self, other_stack: "Stack", func: Callable[[Grid, Grid], Grid]):
-        grids = []
-        for grid1, grid2 in zip(self.grids, other_stack.grids):
-            grid1, grid2 = standardize(grid1, grid2)
-            grids.append(func(grid1, grid2))
-        return stack(*grids)
-
-    def values(self, x: float, y: float):
-        return tuple(grid.value(x, y) for grid in self.grids)
-
-    def type(self, dtype: DataType):
-        return self.each(lambda g: g.type(dtype))
-
-    @overload
-    def save(
-        self, file: str, dtype: Optional[DataType] = None, driver: str = ""
-    ) -> None: ...
-
-    @overload
-    def save(
-        self, file: MemoryFile, dtype: Optional[DataType] = None, driver: str = ""
-    ) -> None: ...
-
-    def save(self, file, dtype: Optional[DataType] = None, driver: str = ""):
-        if isinstance(file, str) and (
-            file.lower().endswith(".jpg")
-            or file.lower().endswith(".kml")
-            or file.lower().endswith(".kmz")
-            or file.lower().endswith(".png")
-        ):
-            grids = self.to_uint8_range().grids
-            dtype = "uint8"
-        else:
-            grids = self.grids
-            if dtype is None:
-                dtype = self.dtype
-
-        nodata = _nodata(dtype)
-
-        if nodata is not None:
-            grids = tuple(con(g.is_nan(), nodata, g) for g in grids)
-
-        if isinstance(file, str):
-            with rasterio.open(
-                file,
-                "w",
-                driver=driver if driver else driver_from_extension(file),
-                count=len(grids),
-                dtype=dtype,
-                nodata=nodata,
-                **_metadata(self.grids[0]),
-            ) as dataset:
-                for index, grid in enumerate(grids):
-                    dataset.write(grid.data, index + 1)
-        elif isinstance(file, MemoryFile):
-            with file.open(
-                driver=driver if driver else "GTiff",
-                count=len(grids),
-                dtype=dtype,
-                nodata=nodata,
-                **_metadata(self.grids[0]),
-            ) as dataset:
-                for index, grid in enumerate(grids):
-                    dataset.write(grid.data, index + 1)
-
-    def save_plot(self, file):
-        self.extract_bands(*self._rgb).save(file)
-
-
-@overload
-def stack(*grids: str) -> Stack:
-    """Creates a new stack from file paths.
-
-    Args:
-        grids (str): File paths.
-
-    Returns:
-        Stack: A new stack.
-    """
-    ...
-
-
-@overload
-def stack(*grids: MemoryFile) -> Stack:
-    """Creates a new stack from in-memory files.
-
-    Args:
-        grids (str): Rasterio in-memory files.
-
-    Returns:
-        Stack: A new stack.
-    """
-    ...
-
-
-@overload
-def stack(*grids: Grid) -> Stack:
-    """Creates a new stack from grids.
-
-    Args:
-        grids (str): Grids.
-
-    Returns:
-        Stack: A new stack.
-    """
-    ...
-
-
-def stack(*grids) -> Stack:
-    bands: List[Grid] = []
-
-    for grid in grids:
-        if isinstance(grid, Grid):
-            bands.append(grid)
-        else:
-            with (
-                rasterio.open(grid) if isinstance(grid, str) else grid.open()
-            ) as dataset:
-                for index in dataset.indexes:
-                    band = _read(dataset, index)
-                    bands.append(band)
-
-    return Stack(standardize(*bands))
+import dataclasses
+from dataclasses import dataclass
+from typing import Callable, List, Optional, Tuple, Union, overload
+
+import rasterio
+from rasterio.crs import CRS
+from rasterio.drivers import driver_from_extension
+from rasterio.io import MemoryFile
+from rasterio.warp import Resampling
+
+from glidergun._grid import (
+    CellSize,
+    Extent,
+    Grid,
+    Scaler,
+    _metadata,
+    _nodata,
+    _read,
+    con,
+    pca,
+    standardize,
+)
+from glidergun._literals import DataType
+
+Operand = Union["Stack", Grid, float, int]
+
+
+@dataclass(frozen=True)
+class Stack:
+    grids: Tuple[Grid, ...]
+    _rgb: Tuple[int, int, int] = (1, 2, 3)
+
+    def __repr__(self):
+        g = self.grids[0]
+        return (
+            f"image: {g.width}x{g.height} {g.dtype} | "
+            + f"crs: {g.crs} | "
+            + f"cell: {g.cell_size.x}, {g.cell_size.y} | "
+            + f"count: {len(self.grids)} | "
+            + f"rgb: {self._rgb}"
+        )
+
+    @property
+    def crs(self) -> CRS:
+        return self.grids[0].crs
+
+    @property
+    def width(self) -> int:
+        return self.grids[0].width
+
+    @property
+    def height(self) -> int:
+        return self.grids[0].height
+
+    @property
+    def dtype(self) -> DataType:
+        return self.grids[0].dtype
+
+    @property
+    def xmin(self) -> float:
+        return self.grids[0].xmin
+
+    @property
+    def ymin(self) -> float:
+        return self.grids[0].ymin
+
+    @property
+    def xmax(self) -> float:
+        return self.grids[0].xmax
+
+    @property
+    def ymax(self) -> float:
+        return self.grids[0].ymax
+
+    @property
+    def cell_size(self) -> CellSize:
+        return self.grids[0].cell_size
+
+    @property
+    def extent(self) -> Extent:
+        return self.grids[0].extent
+
+    @property
+    def md5s(self) -> Tuple[str, ...]:
+        return tuple(g.md5 for g in self.grids)
+
+    def __add__(self, n: Operand):
+        return self._apply(n, lambda g, n: g.__add__(n))
+
+    __radd__ = __add__
+
+    def __sub__(self, n: Operand):
+        return self._apply(n, lambda g, n: g.__sub__(n))
+
+    def __rsub__(self, n: Operand):
+        return self._apply(n, lambda g, n: g.__rsub__(n))
+
+    def __mul__(self, n: Operand):
+        return self._apply(n, lambda g, n: g.__mul__(n))
+
+    __rmul__ = __mul__
+
+    def __pow__(self, n: Operand):
+        return self._apply(n, lambda g, n: g.__pow__(n))
+
+    def __rpow__(self, n: Operand):
+        return self._apply(n, lambda g, n: g.__rpow__(n))
+
+    def __truediv__(self, n: Operand):
+        return self._apply(n, lambda g, n: g.__truediv__(n))
+
+    def __rtruediv__(self, n: Operand):
+        return self._apply(n, lambda g, n: g.__rtruediv__(n))
+
+    def __floordiv__(self, n: Operand):
+        return self._apply(n, lambda g, n: g.__floordiv__(n))
+
+    def __rfloordiv__(self, n: Operand):
+        return self._apply(n, lambda g, n: g.__rfloordiv__(n))
+
+    def __mod__(self, n: Operand):
+        return self._apply(n, lambda g, n: g.__mod__(n))
+
+    def __rmod__(self, n: Operand):
+        return self._apply(n, lambda g, n: g.__rmod__(n))
+
+    def __lt__(self, n: Operand):
+        return self._apply(n, lambda g, n: g.__lt__(n))
+
+    def __gt__(self, n: Operand):
+        return self._apply(n, lambda g, n: g.__gt__(n))
+
+    __rlt__ = __gt__
+
+    __rgt__ = __lt__
+
+    def __le__(self, n: Operand):
+        return self._apply(n, lambda g, n: g.__le__(n))
+
+    def __ge__(self, n: Operand):
+        return self._apply(n, lambda g, n: g.__ge__(n))
+
+    __rle__ = __ge__
+
+    __rge__ = __le__
+
+    def __eq__(self, n: Operand):
+        return self._apply(n, lambda g, n: g.__eq__(n))
+
+    __req__ = __eq__
+
+    def __ne__(self, n: Operand):
+        return self._apply(n, lambda g, n: g.__ne__(n))
+
+    __rne__ = __ne__
+
+    def __and__(self, n: Operand):
+        return self._apply(n, lambda g, n: g.__and__(n))
+
+    __rand__ = __and__
+
+    def __or__(self, n: Operand):
+        return self._apply(n, lambda g, n: g.__or__(n))
+
+    __ror__ = __or__
+
+    def __xor__(self, n: Operand):
+        return self._apply(n, lambda g, n: g.__xor__(n))
+
+    __rxor__ = __xor__
+
+    def __rshift__(self, n: Operand):
+        return self._apply(n, lambda g, n: g.__rshift__(n))
+
+    def __lshift__(self, n: Operand):
+        return self._apply(n, lambda g, n: g.__lshift__(n))
+
+    __rrshift__ = __lshift__
+
+    __rlshift__ = __rshift__
+
+    def __neg__(self):
+        return self.each(lambda g: g.__neg__())
+
+    def __pos__(self):
+        return self.each(lambda g: g.__pos__())
+
+    def __invert__(self):
+        return self.each(lambda g: g.__invert__())
+
+    def _apply(self, n: Operand, op: Callable):
+        if isinstance(n, Stack):
+            return self.zip_with(n, lambda g1, g2: op(g1, g2))
+        return self.each(lambda g: op(g, n))
+
+    def scale(self, scaler: Optional[Scaler] = None, **fit_params):
+        return self.each(lambda g: g.scale(scaler, **fit_params))
+
+    def percent_clip(self, min_percent: float, max_percent: float):
+        return self.each(lambda g: g.percent_clip(min_percent, max_percent))
+
+    def to_uint8_range(self):
+        return self.each(lambda g: g.to_uint8_range())
+
+    def plot(self, r: int, g: int, b: int):
+        return dataclasses.replace(self, _rgb=(r, g, b))
+
+    def map(
+        self,
+        r: int,
+        g: int,
+        b: int,
+        opacity: float = 1.0,
+        folium_map=None,
+        width: int = 800,
+        height: int = 600,
+        basemap: Optional[str] = None,
+        attribution: Optional[str] = None,
+        grayscale: bool = True,
+        **kwargs,
+    ):
+        from glidergun._ipython import _map
+
+        return _map(
+            self,
+            (r, g, b),
+            opacity,
+            folium_map,
+            width,
+            height,
+            basemap,
+            attribution,
+            grayscale,
+            **kwargs,
+        )
+
+    def each(self, func: Callable[[Grid], Grid]):
+        return stack(*map(func, self.grids))
+
+    def clip(self, extent: Tuple[float, float, float, float]):
+        return self.each(lambda g: g.clip(extent))
+
+    def extract_bands(self, *bands: int):
+        return stack(*(self.grids[i - 1] for i in bands))
+
+    def pca(self, n_components: int = 3):
+        return stack(*pca(n_components, *self.grids))
+
+    def project(
+        self, epsg: Union[int, CRS], resampling: Resampling = Resampling.nearest
+    ):
+        return self.each(lambda g: g.project(epsg, resampling))
+
+    def resample(
+        self,
+        cell_size: Union[Tuple[float, float], float],
+        resampling: Resampling = Resampling.nearest,
+    ):
+        return self.each(lambda g: g.resample(cell_size, resampling))
+
+    def zip_with(self, other_stack: "Stack", func: Callable[[Grid, Grid], Grid]):
+        grids = []
+        for grid1, grid2 in zip(self.grids, other_stack.grids):
+            grid1, grid2 = standardize(grid1, grid2)
+            grids.append(func(grid1, grid2))
+        return stack(*grids)
+
+    def values(self, x: float, y: float):
+        return tuple(grid.value(x, y) for grid in self.grids)
+
+    def type(self, dtype: DataType):
+        return self.each(lambda g: g.type(dtype))
+
+    @overload
+    def save(
+        self, file: str, dtype: Optional[DataType] = None, driver: str = ""
+    ) -> None: ...
+
+    @overload
+    def save(
+        self, file: MemoryFile, dtype: Optional[DataType] = None, driver: str = ""
+    ) -> None: ...
+
+    def save(self, file, dtype: Optional[DataType] = None, driver: str = ""):
+        if isinstance(file, str) and (
+            file.lower().endswith(".jpg")
+            or file.lower().endswith(".kml")
+            or file.lower().endswith(".kmz")
+            or file.lower().endswith(".png")
+        ):
+            grids = self.to_uint8_range().grids
+            dtype = "uint8"
+        else:
+            grids = self.grids
+            if dtype is None:
+                dtype = self.dtype
+
+        nodata = _nodata(dtype)
+
+        if nodata is not None:
+            grids = tuple(con(g.is_nan(), nodata, g) for g in grids)
+
+        if isinstance(file, str):
+            with rasterio.open(
+                file,
+                "w",
+                driver=driver if driver else driver_from_extension(file),
+                count=len(grids),
+                dtype=dtype,
+                nodata=nodata,
+                **_metadata(self.grids[0]),
+            ) as dataset:
+                for index, grid in enumerate(grids):
+                    dataset.write(grid.data, index + 1)
+        elif isinstance(file, MemoryFile):
+            with file.open(
+                driver=driver if driver else "GTiff",
+                count=len(grids),
+                dtype=dtype,
+                nodata=nodata,
+                **_metadata(self.grids[0]),
+            ) as dataset:
+                for index, grid in enumerate(grids):
+                    dataset.write(grid.data, index + 1)
+
+    def save_plot(self, file):
+        self.extract_bands(*self._rgb).save(file)
+
+
+@overload
+def stack(*grids: str) -> Stack:
+    """Creates a new stack from file paths.
+
+    Args:
+        grids (str): File paths.
+
+    Returns:
+        Stack: A new stack.
+    """
+    ...
+
+
+@overload
+def stack(*grids: MemoryFile) -> Stack:
+    """Creates a new stack from in-memory files.
+
+    Args:
+        grids (str): Rasterio in-memory files.
+
+    Returns:
+        Stack: A new stack.
+    """
+    ...
+
+
+@overload
+def stack(*grids: Grid) -> Stack:
+    """Creates a new stack from grids.
+
+    Args:
+        grids (str): Grids.
+
+    Returns:
+        Stack: A new stack.
+    """
+    ...
+
+
+def stack(*grids) -> Stack:
+    bands: List[Grid] = []
+
+    for grid in grids:
+        if isinstance(grid, Grid):
+            bands.append(grid)
+        else:
+            with (
+                rasterio.open(grid) if isinstance(grid, str) else grid.open()
+            ) as dataset:
+                for index in dataset.indexes:
+                    band = _read(dataset, index)
+                    bands.append(band)
+
+    return Stack(standardize(*bands))
```

### Comparing `glidergun-0.5.1/glidergun.egg-info/PKG-INFO` & `glidergun-0.5.4/glidergun.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,189 +1,189 @@
-Metadata-Version: 2.1
-Name: glidergun
-Version: 0.5.1
-Summary: Map Algebra with NumPy
-Author-email: Jiro Shirota <jshirota@gmail.com>
-Project-URL: Homepage, https://github.com/jshirota/glidergun
-Project-URL: Bug Tracker, https://github.com/jshirota/glidergun/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Requires-Dist: folium
-Requires-Dist: ipython
-Requires-Dist: matplotlib
-Requires-Dist: numpy
-Requires-Dist: rasterio
-Requires-Dist: scikit-learn
-Requires-Dist: scipy
-Requires-Dist: shapely
-
-# glidergun
-
-```
-pip install glidergun
-```
-
-### Overview
-
-[![Glidergun](https://img.youtube.com/vi/pbVG4bNb96Y/0.jpg)](https://youtu.be/pbVG4bNb96Y)
-
-## creation / io
-
-- grid
-- stack
-- save
-
-## operators
-
-- most overloadable Python operators
-
-## properties
-
-- width
-- height
-- dtype
-- xmin
-- ymin
-- xmax
-- ymax
-- extent
-- mean
-- std
-- min
-- max
-- cell_size
-- bins
-- md5
-
-## local
-
-- local (higher order)
-- is_nan
-- abs
-- sin
-- cos
-- tan
-- arcsin
-- arccos
-- arctan
-- log
-- round
-- gaussian_filter
-- gaussian_gradient_magnitude
-- gaussian_laplace
-- prewitt
-- sobel
-- uniform_filter
-- uniform_filter1d
-
-## focal
-
-- focal (higher order)
-- focal_count
-- focal_mean
-- focal_std
-- focal_var
-- focal_median
-- focal_min
-- focal_max
-- focal_sum
-- focal_ptp
-- focal_percentile
-- focal_quantile
-- focal_entropy
-- focal_hmean
-- focal_pmean
-- focal_kurtosis
-- focal_iqr
-- focal_mode
-- focal_moment
-- focal_skew
-- focal_kstat
-- focal_kstatvar
-- focal_tmean
-- focal_tvar
-- focal_tmin
-- focal_tmax
-- focal_tstd
-- focal_variation
-- focal_median_abs_deviation
-- focal_chisquare
-- focal_ttest_ind
-
-## zonal
-
-- zonal (higher order)
-- zonal_count
-- zonal_mean
-- zonal_std
-- zonal_var
-- zonal_median
-- zonal_min
-- zonal_max
-- zonal_sum
-- zonal_ptp
-- zonal_percentile
-- zonal_quantile
-- zonal_entropy
-- zonal_hmean
-- zonal_pmean
-- zonal_kurtosis
-- zonal_iqr
-- zonal_mode
-- zonal_moment
-- zonal_skew
-- zonal_kstat
-- zonal_kstatvar
-- zonal_tmean
-- zonal_tvar
-- zonal_tmin
-- zonal_tmax
-- zonal_tstd
-- zonal_variation
-- zonal_median_abs_deviation
-
-## interpolation
-
-- interpolate (higher order)
-- interp_linear
-- interp_nearest
-- interp_rbf
-
-## regression / classification
-
-- fit (higher order)
-
-## surface
-
-- aspect
-- slope
-- hillshade
-
-## conversion, etc.
-
-- buffer
-- clip
-- con
-- fill_nan
-- from_polygons
-- mosaic
-- pca
-- percent_clip
-- project
-- randomize
-- reclass
-- replace
-- resample
-- scale
-- set_nan
-- standardize
-- to_points
-- to_polygons
-- to_stack
-
-## ipython
-
-- plot (Matplotlib)
-- map (Folium)
+Metadata-Version: 2.1
+Name: glidergun
+Version: 0.5.4
+Summary: Map Algebra with NumPy
+Author-email: Jiro Shirota <jshirota@gmail.com>
+Project-URL: Homepage, https://github.com/jshirota/glidergun
+Project-URL: Bug Tracker, https://github.com/jshirota/glidergun/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Requires-Dist: folium
+Requires-Dist: ipython
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: rasterio
+Requires-Dist: scikit-learn
+Requires-Dist: scipy
+Requires-Dist: shapely
+
+# glidergun
+
+```
+pip install glidergun
+```
+
+### Overview
+
+[![Glidergun](https://img.youtube.com/vi/pbVG4bNb96Y/0.jpg)](https://youtu.be/pbVG4bNb96Y)
+
+## creation / io
+
+- grid
+- stack
+- save
+
+## operators
+
+- most overloadable Python operators
+
+## properties
+
+- width
+- height
+- dtype
+- xmin
+- ymin
+- xmax
+- ymax
+- extent
+- mean
+- std
+- min
+- max
+- cell_size
+- bins
+- md5
+
+## local
+
+- local (higher order)
+- is_nan
+- abs
+- sin
+- cos
+- tan
+- arcsin
+- arccos
+- arctan
+- log
+- round
+- gaussian_filter
+- gaussian_gradient_magnitude
+- gaussian_laplace
+- prewitt
+- sobel
+- uniform_filter
+- uniform_filter1d
+
+## focal
+
+- focal (higher order)
+- focal_count
+- focal_mean
+- focal_std
+- focal_var
+- focal_median
+- focal_min
+- focal_max
+- focal_sum
+- focal_ptp
+- focal_percentile
+- focal_quantile
+- focal_entropy
+- focal_hmean
+- focal_pmean
+- focal_kurtosis
+- focal_iqr
+- focal_mode
+- focal_moment
+- focal_skew
+- focal_kstat
+- focal_kstatvar
+- focal_tmean
+- focal_tvar
+- focal_tmin
+- focal_tmax
+- focal_tstd
+- focal_variation
+- focal_median_abs_deviation
+- focal_chisquare
+- focal_ttest_ind
+
+## zonal
+
+- zonal (higher order)
+- zonal_count
+- zonal_mean
+- zonal_std
+- zonal_var
+- zonal_median
+- zonal_min
+- zonal_max
+- zonal_sum
+- zonal_ptp
+- zonal_percentile
+- zonal_quantile
+- zonal_entropy
+- zonal_hmean
+- zonal_pmean
+- zonal_kurtosis
+- zonal_iqr
+- zonal_mode
+- zonal_moment
+- zonal_skew
+- zonal_kstat
+- zonal_kstatvar
+- zonal_tmean
+- zonal_tvar
+- zonal_tmin
+- zonal_tmax
+- zonal_tstd
+- zonal_variation
+- zonal_median_abs_deviation
+
+## interpolation
+
+- interpolate (higher order)
+- interp_linear
+- interp_nearest
+- interp_rbf
+
+## regression / classification
+
+- fit (higher order)
+
+## surface
+
+- aspect
+- slope
+- hillshade
+
+## conversion, etc.
+
+- buffer
+- clip
+- con
+- fill_nan
+- from_polygons
+- mosaic
+- pca
+- percent_clip
+- project
+- randomize
+- reclass
+- replace
+- resample
+- scale
+- set_nan
+- standardize
+- to_points
+- to_polygons
+- to_stack
+
+## ipython
+
+- plot (Matplotlib)
+- map (Folium)
```

### Comparing `glidergun-0.5.1/pyproject.toml` & `glidergun-0.5.4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "glidergun"
-version = "0.5.1"
-authors = [
-  { name="Jiro Shirota", email="jshirota@gmail.com" },
-]
-description = "Map Algebra with NumPy"
-readme = "README.md"
-requires-python = ">=3.8"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-dependencies = [
-    "folium",
-    "ipython",
-    "matplotlib",
-    "numpy",
-    "rasterio",
-    "scikit-learn",
-    "scipy",
-    "shapely",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/jshirota/glidergun"
-"Bug Tracker" = "https://github.com/jshirota/glidergun/issues"
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "glidergun"
+version = "0.5.4"
+authors = [
+  { name="Jiro Shirota", email="jshirota@gmail.com" },
+]
+description = "Map Algebra with NumPy"
+readme = "README.md"
+requires-python = ">=3.8"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+dependencies = [
+    "folium",
+    "ipython",
+    "matplotlib",
+    "numpy",
+    "rasterio",
+    "scikit-learn",
+    "scipy",
+    "shapely",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/jshirota/glidergun"
+"Bug Tracker" = "https://github.com/jshirota/glidergun/issues"
```

