# Comparing `tmp/musc-0.1.0.tar.gz` & `tmp/musc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musc-0.1.0.tar", last modified: Fri Apr 19 03:08:53 2024, max compression
+gzip compressed data, was "musc-0.1.1.tar", last modified: Fri May 17 08:46:25 2024, max compression
```

## Comparing `musc-0.1.0.tar` & `musc-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0        8 2024-04-02 06:41:46.000000 musc-0.1.0/README.md
--rw-r--r--   0        0        0      125 2024-04-02 06:41:46.000000 musc-0.1.0/musc/__init__.py
--rw-r--r--   0        0        0     1637 2024-04-02 06:41:46.000000 musc-0.1.0/musc/adaptors/drift_detectors/a.py
--rw-r--r--   0        0        0     2963 2024-04-02 06:41:46.000000 musc-0.1.0/musc/adaptors/drift_detectors/river/a.py
--rw-r--r--   0        0        0     2103 2024-04-02 06:41:46.000000 musc-0.1.0/musc/adaptors/drift_detectors/river/with_kdp/__init__.py
--rw-r--r--   0        0        0     4139 2024-04-02 06:41:46.000000 musc-0.1.0/musc/adaptors/models.py
--rw-r--r--   0        0        0     2070 2024-04-02 06:41:46.000000 musc-0.1.0/musc/commons.py
--rw-r--r--   0        0        0     3123 2024-04-02 06:41:46.000000 musc-0.1.0/musc/evaluator/a.py
--rw-r--r--   0        0        0     8188 2024-04-02 06:41:46.000000 musc-0.1.0/musc/evaluator/a2.py
--rw-r--r--   0        0        0     1288 2024-04-02 06:41:46.000000 musc-0.1.0/musc/evaluator/active_count.py
--rw-r--r--   0        0        0     3205 2024-04-02 06:41:46.000000 musc-0.1.0/musc/evaluator/high_level.py
--rw-r--r--   0        0        0     1195 2024-04-02 06:41:46.000000 musc-0.1.0/musc/high_level/__init__.py
--rw-r--r--   0        0        0       53 2024-04-02 06:41:46.000000 musc-0.1.0/musc/high_level/drift_detectors/__init__.py
--rw-r--r--   0        0        0      150 2024-04-02 06:41:46.000000 musc-0.1.0/musc/high_level/drift_detectors/river/__init__.py
--rw-r--r--   0        0        0    12350 2024-04-02 06:41:46.000000 musc-0.1.0/musc/hpo/a.py
--rw-r--r--   0        0        0     7120 2024-04-02 06:41:46.000000 musc-0.1.0/musc/hpo/distr/a.py
--rw-r--r--   0        0        0     2223 2024-04-02 06:41:46.000000 musc-0.1.0/musc/hpo/distr/high_level.py
--rw-r--r--   0        0        0    26682 2024-04-02 06:41:46.000000 musc-0.1.0/musc/hpo/high_level/a.py
--rw-r--r--   0        0        0     2362 2024-04-02 06:41:46.000000 musc-0.1.0/musc/hpo/high_level/helper.py
--rw-r--r--   0        0        0      378 2024-04-02 06:41:46.000000 musc-0.1.0/musc/hpo/res_pool/base.py
--rw-r--r--   0        0        0     2730 2024-04-02 06:41:46.000000 musc-0.1.0/musc/hpo/res_pool/global_.py
--rw-r--r--   0        0        0     1079 2024-04-02 06:41:46.000000 musc-0.1.0/musc/hpo/res_pool/torch_device.py
--rw-r--r--   0        0        0     2312 2024-04-02 06:41:46.000000 musc-0.1.0/musc/service/a.py
--rw-r--r--   0        0        0     4384 2024-04-02 06:41:46.000000 musc-0.1.0/musc/service/concepts/a.py
--rw-r--r--   0        0        0     5591 2024-04-02 06:41:46.000000 musc-0.1.0/musc/service/concepts/high_level/a.py
--rw-r--r--   0        0        0      666 2024-04-02 06:41:46.000000 musc-0.1.0/musc/service/concepts/high_level/no_clone.py
--rw-r--r--   0        0        0      283 2024-04-02 06:41:46.000000 musc-0.1.0/musc/service/errors.py
--rw-r--r--   0        0        0     3900 2024-04-02 06:41:46.000000 musc-0.1.0/musc/service/high_level.py
--rw-r--r--   0        0        0     1549 2024-04-02 06:41:46.000000 musc-0.1.0/musc/service/impl/data_history/base.py
--rw-r--r--   0        0        0     4418 2024-04-02 06:41:46.000000 musc-0.1.0/musc/service/impl/data_history/in_memory.py
--rw-r--r--   0        0        0     5582 2024-04-02 06:41:46.000000 musc-0.1.0/musc/service/impl/dd_process/a.py
--rw-r--r--   0        0        0     6651 2024-04-02 06:41:46.000000 musc-0.1.0/musc/service/impl/dd_process/dh_walker.py
--rw-r--r--   0        0        0     1203 2024-04-02 06:41:46.000000 musc-0.1.0/musc/service/impl/dd_process/stats.py
--rw-r--r--   0        0        0     3468 2024-04-02 06:41:46.000000 musc-0.1.0/musc/service/impl/model_wrapper.py
--rw-r--r--   0        0        0      532 2024-04-19 03:08:53.747504 musc-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 musc-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7933 2024-05-17 08:43:39.000000 musc-0.1.1/README.md
+-rw-r--r--   0        0        0      125 2024-05-17 08:43:39.000000 musc-0.1.1/musc/__init__.py
+-rw-r--r--   0        0        0     1643 2024-05-17 08:43:39.000000 musc-0.1.1/musc/adaptors/drift_detectors/a.py
+-rw-r--r--   0        0        0     4810 2024-05-17 08:43:39.000000 musc-0.1.1/musc/adaptors/drift_detectors/river/a.py
+-rw-r--r--   0        0        0     2103 2024-05-17 08:43:39.000000 musc-0.1.1/musc/adaptors/drift_detectors/river/with_kdp/__init__.py
+-rw-r--r--   0        0        0     4129 2024-05-17 08:43:39.000000 musc-0.1.1/musc/adaptors/models.py
+-rw-r--r--   0        0        0     2070 2024-05-17 08:43:39.000000 musc-0.1.1/musc/commons.py
+-rw-r--r--   0        0        0     3122 2024-05-17 08:43:39.000000 musc-0.1.1/musc/eval/a.py
+-rw-r--r--   0        0        0     8188 2024-05-17 08:43:39.000000 musc-0.1.1/musc/eval/a2.py
+-rw-r--r--   0        0        0     1288 2024-05-17 08:43:39.000000 musc-0.1.1/musc/eval/active_count.py
+-rw-r--r--   0        0        0     3211 2024-05-17 08:43:39.000000 musc-0.1.1/musc/eval/high_level.py
+-rw-r--r--   0        0        0     1274 2024-05-17 08:43:39.000000 musc-0.1.1/musc/high_level/__init__.py
+-rw-r--r--   0        0        0       53 2024-05-17 08:43:39.000000 musc-0.1.1/musc/high_level/drift_detectors/__init__.py
+-rw-r--r--   0        0        0      150 2024-05-17 08:43:39.000000 musc-0.1.1/musc/high_level/drift_detectors/river/__init__.py
+-rw-r--r--   0        0        0    12350 2024-05-17 08:43:39.000000 musc-0.1.1/musc/hpo/a.py
+-rw-r--r--   0        0        0     7120 2024-05-17 08:43:39.000000 musc-0.1.1/musc/hpo/distr/a.py
+-rw-r--r--   0        0        0     2223 2024-05-17 08:43:39.000000 musc-0.1.1/musc/hpo/distr/high_level.py
+-rw-r--r--   0        0        0    26685 2024-05-17 08:43:39.000000 musc-0.1.1/musc/hpo/high_level/a.py
+-rw-r--r--   0        0        0     2362 2024-05-17 08:43:39.000000 musc-0.1.1/musc/hpo/high_level/helper.py
+-rw-r--r--   0        0        0      378 2024-05-17 08:43:39.000000 musc-0.1.1/musc/hpo/res_pool/base.py
+-rw-r--r--   0        0        0     2730 2024-05-17 08:43:39.000000 musc-0.1.1/musc/hpo/res_pool/global_.py
+-rw-r--r--   0        0        0     1079 2024-05-17 08:43:39.000000 musc-0.1.1/musc/hpo/res_pool/torch_device.py
+-rw-r--r--   0        0        0     2307 2024-05-17 08:43:39.000000 musc-0.1.1/musc/service/a.py
+-rw-r--r--   0        0        0     4535 2024-05-17 08:43:39.000000 musc-0.1.1/musc/service/concepts/a.py
+-rw-r--r--   0        0        0     6100 2024-05-17 08:43:39.000000 musc-0.1.1/musc/service/concepts/high_level/a.py
+-rw-r--r--   0        0        0      666 2024-05-17 08:43:39.000000 musc-0.1.1/musc/service/concepts/high_level/no_clone.py
+-rw-r--r--   0        0        0      283 2024-05-17 08:43:39.000000 musc-0.1.1/musc/service/errors.py
+-rw-r--r--   0        0        0     3900 2024-05-17 08:43:39.000000 musc-0.1.1/musc/service/high_level.py
+-rw-r--r--   0        0        0     1549 2024-05-17 08:43:39.000000 musc-0.1.1/musc/service/impl/data_history/base.py
+-rw-r--r--   0        0        0     4413 2024-05-17 08:43:39.000000 musc-0.1.1/musc/service/impl/data_history/in_memory.py
+-rw-r--r--   0        0        0     5577 2024-05-17 08:43:39.000000 musc-0.1.1/musc/service/impl/dd_process/a.py
+-rw-r--r--   0        0        0     6646 2024-05-17 08:43:39.000000 musc-0.1.1/musc/service/impl/dd_process/dh_walker.py
+-rw-r--r--   0        0        0     1203 2024-05-17 08:43:39.000000 musc-0.1.1/musc/service/impl/dd_process/stats.py
+-rw-r--r--   0        0        0     3468 2024-05-17 08:43:39.000000 musc-0.1.1/musc/service/impl/model_wrapper.py
+-rw-r--r--   0        0        0      593 2024-05-17 08:46:25.870789 musc-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     8316 1970-01-01 00:00:00.000000 musc-0.1.1/PKG-INFO
```

### Comparing `musc-0.1.0/musc/adaptors/drift_detectors/a.py` & `musc-0.1.1/musc/adaptors/drift_detectors/a.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 import random
 from typing import Any
 
 from musc.service.concepts.a import BaseDriftDetectorWithNcl, DriftDetected
 
 
-class DriftDetectorNone(BaseDriftDetectorWithNcl):
+class DriftDetectorBlank(BaseDriftDetectorWithNcl):
 
     def step(self, x: Any, y: Any, y_pred: Any) -> DriftDetected | None:
         del x, y, y_pred
         return None
 
-    def clone_without_state(self) -> DriftDetectorNone:
-        return DriftDetectorNone()
+    def clone_without_state(self) -> DriftDetectorBlank:
+        return DriftDetectorBlank()
 
 
 class DriftDetectorPeriodicallyUpdate(BaseDriftDetectorWithNcl):
 
     def __init__(
         self,
         period: int,
@@ -33,22 +33,22 @@
 
     def step(self, x: Any, y: Any, y_pred: Any) -> DriftDetected | None:
         del x, y, y_pred
         self._cnt += 1
         if self._cnt % self._period == 0:
             if self._probability is not None and random.random() >= self._probability:
                 return None
-            if self._ncl <= -1:
+            elif self._ncl <= -1:
                 return DriftDetected(self._cnt)
             else:
                 return DriftDetected(min(self._ncl, self._cnt))
         else:
             return None
 
     def clone_without_state(self) -> DriftDetectorPeriodicallyUpdate:
         return DriftDetectorPeriodicallyUpdate(self._period, self._ncl, self._probability)
 
 
 __all__ = [
-    'DriftDetectorNone',
+    'DriftDetectorBlank',
     'DriftDetectorPeriodicallyUpdate',
 ]
```

### Comparing `musc-0.1.0/musc/adaptors/drift_detectors/river/a.py` & `musc-0.1.1/musc/adaptors/drift_detectors/river/a.py`

 * *Files 21% similar despite different names*

```diff
@@ -32,46 +32,97 @@
         self._drift_detector.update(y != y_pred)
         return DriftDetected(None) if self._drift_detector.drift_detected else None
 
     def clone_without_state(self) -> DriftDetectorByRiverBinary:
         return DriftDetectorByRiverBinary(self._drift_detector.clone())
 
 
-class DriftDetectorByRiverWithNcl(BaseDriftDetectorWithNcl):
+class DriftDetectorByRiverWithManualNcl(BaseDriftDetectorWithNcl):
+
+    def __init__(self, drift_detector: DriftDetector, metric: Metric, ncl: int) -> None:
+        self._drift_detector = drift_detector
+        self._metric = metric
+        self._ncl = ncl
+        self._cnt = 0
+
+    def step(self, x: Any, y: Any, y_pred: Any) -> DriftDetected | None:
+        del x
+        self._cnt += 1
+        self._drift_detector.update(self._metric(y=y, y_pred=y_pred))
+        if self._drift_detector.drift_detected:
+            if self._ncl <= -1:
+                return DriftDetected(self._cnt)
+            else:
+                return DriftDetected(min(self._ncl, self._cnt))
+        else:
+            return None
+
+    def clone_without_state(self) -> DriftDetectorByRiverWithManualNcl:
+        return DriftDetectorByRiverWithManualNcl(
+            self._drift_detector.clone(),
+            self._metric,
+            self._ncl,
+        )
+
+
+class DriftDetectorByRiverBinaryWithManualNcl(BaseDriftDetectorWithNcl):
+
+    def __init__(self, drift_detector: BinaryDriftDetector, ncl: int) -> None:
+        self._drift_detector = drift_detector
+        self._ncl = ncl
+        self._cnt = 0
+
+    def step(self, x: Any, y: Any, y_pred: Any) -> DriftDetected | None:
+        del x
+        self._cnt += 1
+        self._drift_detector.update(y != y_pred)
+        if self._drift_detector.drift_detected:
+            if self._ncl <= -1:
+                return DriftDetected(self._cnt)
+            else:
+                return DriftDetected(min(self._ncl, self._cnt))
+        else:
+            return None
+
+    def clone_without_state(self) -> DriftDetectorByRiverBinaryWithManualNcl:
+        return DriftDetectorByRiverBinaryWithManualNcl(self._drift_detector.clone(), self._ncl)
+
+
+class DriftDetectorByRiverWithAutoNcl(BaseDriftDetectorWithNcl):
 
     def __init__(self, drift_detector: DriftDetector, metric: Metric) -> None:
         assert hasattr(drift_detector, 'new_concept_length')
         self._drift_detector = drift_detector
         self._metric = metric
 
     def step(self, x: Any, y: Any, y_pred: Any) -> DriftDetected | None:
         del x
         self._drift_detector.update(self._metric(y=y, y_pred=y_pred))
         ncl = self._drift_detector.new_concept_length  # type: ignore
         return DriftDetected(ncl) if ncl is not None else None
 
-    def clone_without_state(self) -> DriftDetectorByRiverWithNcl:
-        return DriftDetectorByRiverWithNcl(self._drift_detector.clone(), self._metric)
+    def clone_without_state(self) -> DriftDetectorByRiverWithAutoNcl:
+        return DriftDetectorByRiverWithAutoNcl(self._drift_detector.clone(), self._metric)
 
 
-class DriftDetectorByRiverBinaryWithNcl(BaseDriftDetectorWithNcl):
+class DriftDetectorByRiverBinaryWithAutoNcl(BaseDriftDetectorWithNcl):
 
     def __init__(self, drift_detector: BinaryDriftDetector) -> None:
         assert hasattr(drift_detector, 'new_concept_length')
         self._drift_detector = drift_detector
 
     def step(self, x: Any, y: Any, y_pred: Any) -> DriftDetected | None:
         del x
         self._drift_detector.update(y != y_pred)
         ncl = self._drift_detector.new_concept_length  # type: ignore
         return DriftDetected(ncl) if ncl is not None else None
 
-    def clone_without_state(self) -> DriftDetectorByRiverBinaryWithNcl:
-        return DriftDetectorByRiverBinaryWithNcl(self._drift_detector.clone())
+    def clone_without_state(self) -> DriftDetectorByRiverBinaryWithAutoNcl:
+        return DriftDetectorByRiverBinaryWithAutoNcl(self._drift_detector.clone())
 
 
 __all__ = [
     'DriftDetectorByRiver',
     'DriftDetectorByRiverBinary',
-    'DriftDetectorByRiverWithNcl',
-    'DriftDetectorByRiverBinaryWithNcl',
+    'DriftDetectorByRiverWithAutoNcl',
+    'DriftDetectorByRiverBinaryWithAutoNcl',
 ]
```

### Comparing `musc-0.1.0/musc/adaptors/drift_detectors/river/with_kdp/__init__.py` & `musc-0.1.1/musc/adaptors/drift_detectors/river/with_kdp/__init__.py`

 * *Files identical despite different names*

### Comparing `musc-0.1.0/musc/adaptors/models.py` & `musc-0.1.1/musc/adaptors/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
     class ModelScikitLearn(BaseModel):
 
         def __init__(self, model: Any) -> None:
             self._model = model
 
         def predict(self, x: np.ndarray) -> np.ndarray:
-            return self._model.predict(np.array([x]))[0]
+            return self._model.predict([x])[0]
 
         def inner(self) -> Any:
             return self._model
 
         def preprocess_x(self, x: Any) -> np.ndarray:
             # See https://numpy.org/doc/stable/reference/arrays.scalars.html#built-in-scalar-types
             # "The default data type in NumPy is float_."
```

### Comparing `musc-0.1.0/musc/commons.py` & `musc-0.1.1/musc/commons.py`

 * *Files identical despite different names*

### Comparing `musc-0.1.0/musc/evaluator/a.py` & `musc-0.1.1/musc/eval/a.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import operator
 from collections.abc import Iterable
 from multiprocessing.pool import ThreadPool
 from threading import Lock
 from typing import Any
 
-from musc.evaluator.active_count import ActiveCount
+from musc.eval.active_count import ActiveCount
 from musc.service.a import Service
 from musc.service.concepts.a import BaseModel, UpdateStrategy
 from musc.service.impl.dd_process.stats import Stats
 
 
 class Evaluator:
 
@@ -33,16 +33,16 @@
         with self._service._model._model_lock.gen_rlock():
             return self._service._model._model
 
     def evaluate(
         self,
         x_arr: Iterable[Any],
         y_arr: Iterable[Any],
-        t_x_arr: Iterable[Any],
-        t_y_arr: Iterable[Any],
+        t_x_arr: Iterable[float],
+        t_y_arr: Iterable[float],
     ) -> tuple[list[Any], Stats]:
         with self._evaluated[1]:
             if self._evaluated[0]:
                 raise RuntimeError
             self._evaluated[0] = True
         events = []
         for i, (x, t_x) in enumerate(zip(x_arr, t_x_arr)):
```

### Comparing `musc-0.1.0/musc/evaluator/a2.py` & `musc-0.1.1/musc/eval/a2.py`

 * *Files identical despite different names*

### Comparing `musc-0.1.0/musc/evaluator/active_count.py` & `musc-0.1.1/musc/eval/active_count.py`

 * *Files identical despite different names*

### Comparing `musc-0.1.0/musc/evaluator/high_level.py` & `musc-0.1.1/musc/eval/high_level.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collections.abc import Iterable, Sequence
 from typing import Any, Literal, overload
 
-from musc.evaluator.a import Evaluator as EvaluatorLowLevel
-from musc.evaluator.a2 import Evaluator2 as EvaluatorLowLevel2
+from musc.eval.a import Evaluator as EvaluatorLowLevel
+from musc.eval.a2 import Evaluator2 as EvaluatorLowLevel2
 from musc.service.concepts.a import Metric, UpdateStrategy
 from musc.service.concepts.high_level.a import apply_model_adaptors
 from musc.service.impl.dd_process.stats import Stats
 
 
 class Evaluator:
 
@@ -27,47 +27,47 @@
                 raise ValueError
 
     @overload
     def evaluate(
         self,
         x_arr: Iterable[Any],
         y_arr: Iterable[Any],
-        t_x_arr: Iterable[Any],
-        t_y_arr: Iterable[Any],
+        t_x_arr: Iterable[float],
+        t_y_arr: Iterable[float],
     ) -> tuple[list[Any], Stats]:
         pass
 
     @overload
     def evaluate(
         self,
         x_arr: Iterable[Any],
         y_arr: Iterable[Any],
-        t_x_arr: Iterable[Any],
-        t_y_arr: Iterable[Any],
+        t_x_arr: Iterable[float],
+        t_y_arr: Iterable[float],
         metric: Metric,
     ) -> tuple[float, Stats]:
         pass
 
     @overload
     def evaluate(
         self,
         x_arr: Iterable[Any],
         y_arr: Iterable[Any],
-        t_x_arr: Iterable[Any],
-        t_y_arr: Iterable[Any],
+        t_x_arr: Iterable[float],
+        t_y_arr: Iterable[float],
         metric: Sequence[Metric],
     ) -> tuple[list[float], Stats]:
         pass
 
     def evaluate(
         self,
         x_arr: Iterable[Any],
         y_arr: Iterable[Any],
-        t_x_arr: Iterable[Any],
-        t_y_arr: Iterable[Any],
+        t_x_arr: Iterable[float],
+        t_y_arr: Iterable[float],
         metric: Metric | Sequence[Metric] | None = None,
     ) -> tuple[float | list[float] | list[Any], Stats]:
 
         x_arr_, y_arr_, t_x_arr_, t_y_arr_ = list(x_arr), list(y_arr), list(t_x_arr), list(t_y_arr)
         del x_arr, y_arr, t_x_arr, t_y_arr
         if not len(x_arr_) == len(y_arr_) == len(t_x_arr_) == len(t_y_arr_) != 0:
             raise ValueError
```

### Comparing `musc-0.1.0/musc/high_level/__init__.py` & `musc-0.1.1/musc/high_level/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-from musc.evaluator.high_level import Evaluator
+from musc.eval.high_level import Evaluator
 from musc.hpo.distr.high_level import SingleValue, into_distr
 from musc.hpo.high_level.a import UpdateStrategySearch
-from musc.service.concepts.a import BaseModel, Metric
+from musc.service.concepts.a import BaseDriftDetector, BaseModel, DriftDetected, Metric
 from musc.service.concepts.high_level.a import (
     UpdateStrategyByDriftDetection,
     UpdateStrategyByPeriodicallyUpdate,
-    UpdateStrategyNone,
+    UpdateStrategyBlank,
 )
 from musc.service.high_level import Service, run_service_http
 
 from . import drift_detectors
 
 __all__ = [
+    'BaseDriftDetector',
     'BaseModel',
+    'DriftDetected',
     'Evaluator',
     'Metric',
     'Service',
     'SingleValue',
     'UpdateStrategyByDriftDetection',
     'UpdateStrategyByPeriodicallyUpdate',
-    'UpdateStrategyNone',
+    'UpdateStrategyBlank',
     'UpdateStrategySearch',
     'drift_detectors',
     'into_distr',
     'run_service_http',
 ]
 
 try:
```

### Comparing `musc-0.1.0/musc/hpo/a.py` & `musc-0.1.1/musc/hpo/a.py`

 * *Files identical despite different names*

### Comparing `musc-0.1.0/musc/hpo/distr/a.py` & `musc-0.1.1/musc/hpo/distr/a.py`

 * *Files identical despite different names*

### Comparing `musc-0.1.0/musc/hpo/distr/high_level.py` & `musc-0.1.1/musc/hpo/distr/high_level.py`

 * *Files identical despite different names*

### Comparing `musc-0.1.0/musc/hpo/high_level/a.py` & `musc-0.1.1/musc/hpo/high_level/a.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from queue import Queue
 from threading import Thread
 from typing import Any, Generic, Literal, TypeVar
 
 import pandas as pd
 
 from musc.commons import safe_save
-from musc.evaluator.high_level import Evaluator
+from musc.eval.high_level import Evaluator
 from musc.hpo.a import ExhaustiveSearch, RandomizedSearch, Sample
 from musc.hpo.distr.a import BaseDistribution
 from musc.hpo.distr.high_level import into_distr
 from musc.hpo.high_level.helper import ModelCloneHelper
 from musc.hpo.res_pool.base import BaseResourcePool
 from musc.hpo.res_pool.global_ import GlobalResourcePool
 from musc.service.concepts.a import BaseModel, Metric, UpdateStrategy
@@ -35,16 +35,16 @@
 
     def __init__(
         self,
         distr: BaseDistribution[UpdateStrategy],
         model: BaseModel,
         x_arr: Iterable[Any],
         y_arr: Iterable[Any],
-        t_x_arr: Iterable[Any],
-        t_y_arr: Iterable[Any],
+        t_x_arr: Iterable[float],
+        t_y_arr: Iterable[float],
         metric: list[Metric],
         score_fn: Callable[[list[float], Stats], S],
         greater_score_fn: Callable[[S, S], bool] | None,
         weak_greater_score_fn: Callable[[S, S], bool] | None,
         eval_retry: int,
         top_k_kept: int,
         exhaustive: bool,
@@ -182,16 +182,16 @@
 
     def __init__(
         self,
         search_space: Any,
         model: Any,
         x_arr: Iterable[Any],
         y_arr: Iterable[Any],
-        t_x_arr: Iterable[Any],
-        t_y_arr: Iterable[Any],
+        t_x_arr: Iterable[float],
+        t_y_arr: Iterable[float],
         metric: Metric | Sequence[Metric | Literal['time', 'n_updates', 'n_samples']],
         optim_mode: Literal['min', 'max'] | Sequence[Literal['min', 'max']] | None,
         *,
         weight_fn: Callable[..., Any] | None = None,
         top_k_kept: int = 0,
         exhaustive: bool = False,
         n_jobs: int | None = None,
```

### Comparing `musc-0.1.0/musc/hpo/high_level/helper.py` & `musc-0.1.1/musc/hpo/high_level/helper.py`

 * *Files identical despite different names*

### Comparing `musc-0.1.0/musc/hpo/res_pool/global_.py` & `musc-0.1.1/musc/hpo/res_pool/global_.py`

 * *Files identical despite different names*

### Comparing `musc-0.1.0/musc/hpo/res_pool/torch_device.py` & `musc-0.1.1/musc/hpo/res_pool/torch_device.py`

 * *Files identical despite different names*

### Comparing `musc-0.1.0/musc/service/a.py` & `musc-0.1.1/musc/service/a.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from collections.abc import Callable
 from typing import Generic, TypeVar
 
-from musc.evaluator.active_count import BaseActiveCount, NullActiveCount
+from musc.eval.active_count import BaseActiveCount, NullActiveCount
 from musc.service.concepts.a import BaseModel, UpdateStrategy
 from musc.service.impl.model_wrapper import ModelWrapper
 from musc.service.impl.data_history.base import BaseDataHistory
 from musc.service.impl.data_history.in_memory import DataHistoryInMemory
 from musc.service.impl.dd_process.a import DriftDetectorProcess
 from musc.service.impl.dd_process.stats import Stats
```

### Comparing `musc-0.1.0/musc/service/concepts/a.py` & `musc-0.1.1/musc/service/concepts/a.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,24 +76,29 @@
 
 class BaseDriftDetector(Generic[X, Y, YP], ABC):
 
     @abstractmethod
     def step(self, x: X, y: Y, y_pred: YP) -> DriftDetected | None:
         pass
 
-    @abstractmethod
+    def reset(self) -> None:
+        raise NotImplementedError
+
     def clone_without_state(self) -> BaseDriftDetector[X, Y, YP]:
-        pass
+        cloned = deepcopy(self)
+        cloned.reset()
+        return cloned
 
 
 class BaseDriftDetectorWithNcl(Generic[X, Y, YP], BaseDriftDetector[X, Y, YP]):
 
-    @abstractmethod
     def clone_without_state(self) -> BaseDriftDetectorWithNcl[X, Y, YP]:
-        pass
+        cloned = deepcopy(self)
+        cloned.reset()
+        return cloned
 
 
 class Metric(Generic[Y, YP]):
 
     @overload
     def __init__(self, callable: Callable[[Y, YP], Any], pred_first: Literal[False]) -> None:
         pass
@@ -107,15 +112,15 @@
         self._pred_first = pred_first
         try:
             from torch import Tensor
             self._torch_tensor_class = Tensor
         except ImportError:
             self._torch_tensor_class = None
 
-    def __call__(self, *, y: Y, y_pred: YP) -> int | float:
+    def __call__(self, *, y: Y, y_pred: YP) -> float:
         if self._pred_first:
             metric_value = self._callable(y_pred, y)
         else:
             metric_value = self._callable(y, y_pred)
         if (
             self._torch_tensor_class is not None
             and isinstance(metric_value, self._torch_tensor_class)
```

### Comparing `musc-0.1.0/musc/service/concepts/high_level/a.py` & `musc-0.1.1/musc/service/concepts/high_level/a.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
 
 from collections.abc import Callable
 from typing import Any, Generic, TypeVar
 
 from river.base import BinaryDriftDetector, DriftDetector
 
-from musc.adaptors.drift_detectors.a import DriftDetectorNone, DriftDetectorPeriodicallyUpdate
+from musc.adaptors.drift_detectors.a import DriftDetectorBlank, DriftDetectorPeriodicallyUpdate
 from musc.adaptors.drift_detectors.river.a import (
     DriftDetectorByRiver,
     DriftDetectorByRiverBinary,
-    DriftDetectorByRiverBinaryWithNcl,
-    DriftDetectorByRiverWithNcl,
+    DriftDetectorByRiverBinaryWithAutoNcl,
+    DriftDetectorByRiverBinaryWithManualNcl,
+    DriftDetectorByRiverWithAutoNcl,
+    DriftDetectorByRiverWithManualNcl,
 )
 from musc.adaptors.drift_detectors.river.with_kdp import ADWIN, PageHinkley, kswin_distr_prelude
 from musc.hpo.distr.a import BaseDistribution
 from musc.hpo.distr.high_level import into_distr
 from musc.service.concepts.a import BaseModel, Metric, UpdateStrategy
 
 
@@ -63,21 +65,21 @@
             self.drift_detector,
             self.updator,
             self.data_amount_required,
             self.use_ncl,
         ).__repr__()
 
 
-class UpdateStrategyNone(UpdateStrategySubclass):
+class UpdateStrategyBlank(UpdateStrategySubclass):
 
     def __init__(self) -> None:
-        super().__init__(DriftDetectorNone(), updator_no_op, 0, False)
+        super().__init__(DriftDetectorBlank(), updator_no_op, 0, False)
 
-    def clone_without_state(self) -> UpdateStrategyNone:
-        return UpdateStrategyNone()
+    def clone_without_state(self) -> UpdateStrategyBlank:
+        return UpdateStrategyBlank()
 
 
 class UpdateStrategyByPeriodicallyUpdate(UpdateStrategySubclass):
 
     def __init__(
         self,
         period: int,
@@ -98,33 +100,42 @@
 
     def __init__(
         self,
         drift_detector: BinaryDriftDetector | DriftDetector,
         updator: Callable[[Any, list[Any], list[Any]], None],
         data_amount_required: int,
         metric: Metric | None = None,
-        use_ncl: bool | None = None,
+        use_ncl: bool | int | None = None,
     ) -> None:
         if isinstance(drift_detector, BinaryDriftDetector):
-            if not hasattr(drift_detector, 'new_concept_length'):
+            if type(use_ncl) is int:
+                drift_detector_ = DriftDetectorByRiverBinaryWithManualNcl(drift_detector, use_ncl)
+            elif not hasattr(drift_detector, 'new_concept_length'):
                 drift_detector_ = DriftDetectorByRiverBinary(drift_detector)
             else:
-                drift_detector_ = DriftDetectorByRiverBinaryWithNcl(drift_detector)
+                drift_detector_ = DriftDetectorByRiverBinaryWithAutoNcl(drift_detector)
         elif isinstance(drift_detector, DriftDetector):
             if metric is None:
                 raise TypeError
-            if not hasattr(drift_detector, 'new_concept_length'):
+            if type(use_ncl) is int:
+                drift_detector_ = DriftDetectorByRiverWithManualNcl(drift_detector, metric, use_ncl)
+            elif not hasattr(drift_detector, 'new_concept_length'):
                 drift_detector_ = DriftDetectorByRiver(drift_detector, metric)
             else:
-                drift_detector_ = DriftDetectorByRiverWithNcl(drift_detector, metric)
+                drift_detector_ = DriftDetectorByRiverWithAutoNcl(drift_detector, metric)
         else:
             raise TypeError
         drift_detector_ = drift_detector_.clone_without_state()
         updator_ = UpdatorWrapper(updator)
-        use_ncl = use_ncl if use_ncl is not None else hasattr(drift_detector, 'new_concept_length')
+        if type(use_ncl) is int:
+            use_ncl = True
+        elif type(use_ncl) is bool:
+            use_ncl = use_ncl
+        else:
+            use_ncl = hasattr(drift_detector, 'new_concept_length')
         super().__init__(drift_detector_, updator_, data_amount_required, use_ncl)
 
     @staticmethod
     def kwargs_distr_prelude() -> dict[str, BaseDistribution[Any]]:
         return {
             'drift_detector': into_distr([
                 {'type': ADWIN},
@@ -171,12 +182,12 @@
 
 def updator_no_op(model: BaseModel, x_arr: list[Any], y_arr: list[Any]) -> None:
     del model, x_arr, y_arr
 
 
 __all__ = [
     'ModelGuard',
-    'UpdateStrategyNone',
+    'UpdateStrategyBlank',
     'UpdateStrategyByPeriodicallyUpdate',
     'UpdateStrategyByDriftDetection',
     'apply_model_adaptors',
 ]
```

### Comparing `musc-0.1.0/musc/service/concepts/high_level/no_clone.py` & `musc-0.1.1/musc/service/concepts/high_level/no_clone.py`

 * *Files identical despite different names*

### Comparing `musc-0.1.0/musc/service/high_level.py` & `musc-0.1.1/musc/service/high_level.py`

 * *Files identical despite different names*

### Comparing `musc-0.1.0/musc/service/impl/data_history/base.py` & `musc-0.1.1/musc/service/impl/data_history/base.py`

 * *Files identical despite different names*

### Comparing `musc-0.1.0/musc/service/impl/data_history/in_memory.py` & `musc-0.1.1/musc/service/impl/data_history/in_memory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import typing
 from typing import Generic, TypeVar
 
 from readerwriterlock.rwlock import RWLockFair
 
-from musc.evaluator.active_count import BaseActiveCount
+from musc.eval.active_count import BaseActiveCount
 from musc.service.errors import ServiceErrorByDuplicatedId, ServiceErrorFromModelPrediction
 from musc.service.impl.data_history.base import (
     BaseDataHistory,
     BaseDataHistoryListener,
     DataHistoryItem,
     DataHistoryItemYNone,
 )
```

### Comparing `musc-0.1.0/musc/service/impl/dd_process/a.py` & `musc-0.1.1/musc/service/impl/dd_process/a.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import time
 import typing
 from collections.abc import Callable
 from dataclasses import dataclass
 from threading import Thread
 from typing import Generic, TypeVar
 
-from musc.evaluator.active_count import BaseActiveCount
+from musc.eval.active_count import BaseActiveCount
 from musc.service.concepts.a import UpdateStrategy
 from musc.service.impl.model_wrapper import ModelWrapper
 from musc.service.impl.data_history.base import BaseDataHistory
 from musc.service.impl.dd_process.dh_walker import DataHistoryWalker, Never
 from musc.service.impl.dd_process.stats import ModelUpdateRecord, Stats, StatsWithLock
```

### Comparing `musc-0.1.0/musc/service/impl/dd_process/dh_walker.py` & `musc-0.1.1/musc/service/impl/dd_process/dh_walker.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import queue
 import typing
 from queue import Queue
 from threading import Lock
 from typing import Generic, Literal, TypeVar, overload
 
-from musc.evaluator.active_count import BaseActiveCount, NullActiveCount
+from musc.eval.active_count import BaseActiveCount, NullActiveCount
 from musc.service.impl.model_wrapper import ModelPredictionProcess, ModelWrapper, Prediction
 from musc.service.impl.data_history.base import (
     BaseDataHistory,
     BaseDataHistoryListener,
     DataHistoryItemYNone,
 )
```

### Comparing `musc-0.1.0/musc/service/impl/dd_process/stats.py` & `musc-0.1.1/musc/service/impl/dd_process/stats.py`

 * *Files identical despite different names*

### Comparing `musc-0.1.0/musc/service/impl/model_wrapper.py` & `musc-0.1.1/musc/service/impl/model_wrapper.py`

 * *Files identical despite different names*

### Comparing `musc-0.1.0/pyproject.toml` & `musc-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "musc"
-version = "0.1.0"
-description = ""
+version = "0.1.1"
+description = "A library to construct concept drift adaptive model services."
 authors = [
     { name = "YANG Qi", email = "y3tothe6@outlook.com" },
 ]
 dependencies = [
     "flask>=3.0.0",
     "gevent>=23.9.1",
     "joblib>=1.3.2",
```

