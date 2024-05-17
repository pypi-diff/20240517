# Comparing `tmp/canvas-0.1.6.tar.gz` & `tmp/canvas-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canvas-0.1.6.tar", max compression
+gzip compressed data, was "canvas-0.1.7.tar", max compression
```

## Comparing `canvas-0.1.6.tar` & `canvas-0.1.7.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0     2821 2024-05-14 19:42:35.023965 canvas-0.1.6/README.md
--rw-r--r--   0        0        0        0 2024-02-22 21:15:33.529941 canvas-0.1.6/canvas_cli/__init__.py
--rw-r--r--   0        0        0        0 2024-02-22 21:15:33.530030 canvas-0.1.6/canvas_cli/apps/__init__.py
--rw-r--r--   0        0        0      105 2024-05-11 15:50:29.885352 canvas-0.1.6/canvas_cli/apps/auth/__init__.py
--rw-r--r--   0        0        0     4528 2024-05-14 19:42:35.024117 canvas-0.1.6/canvas_cli/apps/auth/tests.py
--rw-r--r--   0        0        0     5434 2024-05-14 19:52:30.122404 canvas-0.1.6/canvas_cli/apps/auth/utils.py
--rw-r--r--   0        0        0       64 2024-02-22 21:15:33.530476 canvas-0.1.6/canvas_cli/apps/logs/__init__.py
--rw-r--r--   0        0        0     1825 2024-05-11 15:50:29.885926 canvas-0.1.6/canvas_cli/apps/logs/logs.py
--rw-r--r--   0        0        0      190 2024-05-11 15:50:29.886101 canvas-0.1.6/canvas_cli/apps/plugin/__init__.py
--rw-r--r--   0        0        0     9360 2024-05-11 15:50:29.886407 canvas-0.1.6/canvas_cli/apps/plugin/plugin.py
--rw-r--r--   0        0        0     1035 2024-02-22 21:15:33.530903 canvas-0.1.6/canvas_cli/apps/plugin/tests.py
--rw-r--r--   0        0        0      959 2024-02-22 21:15:33.530977 canvas-0.1.6/canvas_cli/conftest.py
--rw-r--r--   0        0        0     2527 2024-05-11 15:50:29.886582 canvas-0.1.6/canvas_cli/main.py
--rw-r--r--   0        0        0      124 2024-05-14 19:42:35.025394 canvas-0.1.6/canvas_cli/templates/plugins/default/cookiecutter.json
--rw-r--r--   0        0        0      787 2024-05-14 22:06:23.722577 canvas-0.1.6/canvas_cli/templates/plugins/default/{{ cookiecutter.__project_slug }}/CANVAS_MANIFEST.json
--rw-r--r--   0        0        0      347 2024-05-14 19:42:35.025623 canvas-0.1.6/canvas_cli/templates/plugins/default/{{ cookiecutter.__project_slug }}/README.md
--rw-r--r--   0        0        0        0 2024-05-14 19:42:35.025694 canvas-0.1.6/canvas_cli/templates/plugins/default/{{ cookiecutter.__project_slug }}/protocols/__init__.py
--rw-r--r--   0        0        0     2202 2024-05-14 19:42:35.025930 canvas-0.1.6/canvas_cli/templates/plugins/default/{{ cookiecutter.__project_slug }}/protocols/my_protocol.py
--rw-r--r--   0        0        0      285 2024-02-22 21:15:33.531711 canvas-0.1.6/canvas_cli/tests.py
--rw-r--r--   0        0        0        0 2024-02-22 21:15:33.531785 canvas-0.1.6/canvas_cli/utils/__init__.py
--rw-r--r--   0        0        0      102 2024-02-22 21:15:33.531882 canvas-0.1.6/canvas_cli/utils/context/__init__.py
--rw-r--r--   0        0        0     5714 2024-05-11 15:50:29.887529 canvas-0.1.6/canvas_cli/utils/context/context.py
--rw-r--r--   0        0        0     4211 2024-02-22 21:15:33.532069 canvas-0.1.6/canvas_cli/utils/context/tests.py
--rw-r--r--   0        0        0       88 2024-02-22 21:15:33.532161 canvas-0.1.6/canvas_cli/utils/print/__init__.py
--rw-r--r--   0        0        0     1829 2024-02-22 21:15:33.532221 canvas-0.1.6/canvas_cli/utils/print/print.py
--rw-r--r--   0        0        0     2376 2024-02-22 21:15:33.532285 canvas-0.1.6/canvas_cli/utils/print/tests.py
--rw-r--r--   0        0        0       81 2024-02-22 21:15:33.532384 canvas-0.1.6/canvas_cli/utils/urls/__init__.py
--rw-r--r--   0        0        0      407 2024-02-22 21:15:33.532447 canvas-0.1.6/canvas_cli/utils/urls/tests.py
--rw-r--r--   0        0        0      798 2024-02-22 21:15:33.532511 canvas-0.1.6/canvas_cli/utils/urls/urls.py
--rw-r--r--   0        0        0      113 2024-05-11 15:50:29.887707 canvas-0.1.6/canvas_cli/utils/validators/__init__.py
--rw-r--r--   0        0        0     3117 2024-05-11 15:50:29.887855 canvas-0.1.6/canvas_cli/utils/validators/manifest_schema.py
--rw-r--r--   0        0        0     1206 2024-05-11 15:50:29.888019 canvas-0.1.6/canvas_cli/utils/validators/tests.py
--rw-r--r--   0        0        0     1614 2024-05-11 15:50:29.888512 canvas-0.1.6/canvas_cli/utils/validators/validators.py
--rw-r--r--   0        0        0        0 2024-02-22 21:15:33.532827 canvas-0.1.6/canvas_sdk/__init__.py
--rw-r--r--   0        0        0     1116 2024-05-11 15:50:29.888698 canvas-0.1.6/canvas_sdk/commands/__init__.py
--rw-r--r--   0        0        0     4141 2024-05-11 15:50:29.888840 canvas-0.1.6/canvas_sdk/commands/base.py
--rw-r--r--   0        0        0     1636 2024-05-11 15:50:29.889167 canvas-0.1.6/canvas_sdk/commands/commands/assess.py
--rw-r--r--   0        0        0     1382 2024-05-11 15:50:29.889477 canvas-0.1.6/canvas_sdk/commands/commands/diagnose.py
--rw-r--r--   0        0        0     1527 2024-05-11 15:50:29.889617 canvas-0.1.6/canvas_sdk/commands/commands/goal.py
--rw-r--r--   0        0        0      366 2024-05-11 15:50:29.889835 canvas-0.1.6/canvas_sdk/commands/commands/history_present_illness.py
--rw-r--r--   0        0        0      937 2024-05-11 15:50:29.890041 canvas-0.1.6/canvas_sdk/commands/commands/medication_statement.py
--rw-r--r--   0        0        0      350 2024-05-11 15:50:29.890231 canvas-0.1.6/canvas_sdk/commands/commands/plan.py
--rw-r--r--   0        0        0     1574 2024-05-11 15:50:29.890317 canvas-0.1.6/canvas_sdk/commands/commands/prescribe.py
--rw-r--r--   0        0        0      553 2024-05-11 15:50:29.890518 canvas-0.1.6/canvas_sdk/commands/commands/questionnaire.py
--rw-r--r--   0        0        0     1252 2024-05-11 15:50:29.890728 canvas-0.1.6/canvas_sdk/commands/commands/reason_for_visit.py
--rw-r--r--   0        0        0      627 2024-05-11 15:50:29.890933 canvas-0.1.6/canvas_sdk/commands/commands/stop_medication.py
--rw-r--r--   0        0        0     1499 2024-05-11 15:50:29.891031 canvas-0.1.6/canvas_sdk/commands/commands/update_goal.py
--rw-r--r--   0        0        0      176 2024-03-15 16:24:46.654687 canvas-0.1.6/canvas_sdk/commands/constants.py
--rw-r--r--   0        0        0     6287 2024-05-11 15:50:29.891189 canvas-0.1.6/canvas_sdk/commands/tests/test_utils.py
--rw-r--r--   0        0        0    13863 2024-05-11 15:50:29.891357 canvas-0.1.6/canvas_sdk/commands/tests/tests.py
--rw-r--r--   0        0        0        0 2024-02-22 21:15:33.533678 canvas-0.1.6/canvas_sdk/data/__init__.py
--rw-r--r--   0        0        0       62 2024-05-11 15:50:29.891476 canvas-0.1.6/canvas_sdk/effects/__init__.py
--rw-r--r--   0        0        0     1013 2024-05-11 15:50:29.891757 canvas-0.1.6/canvas_sdk/effects/banner_alert/banner_alert.py
--rw-r--r--   0        0        0      436 2024-05-11 15:50:29.891977 canvas-0.1.6/canvas_sdk/effects/banner_alert/constants.py
--rw-r--r--   0        0        0      688 2024-05-11 15:50:29.892062 canvas-0.1.6/canvas_sdk/effects/base.py
--rw-r--r--   0        0        0       74 2024-05-11 15:50:29.892176 canvas-0.1.6/canvas_sdk/events/__init__.py
--rw-r--r--   0        0        0       51 2024-05-11 15:50:29.892351 canvas-0.1.6/canvas_sdk/protocols/__init__.py
--rw-r--r--   0        0        0      260 2024-05-14 19:42:35.026075 canvas-0.1.6/canvas_sdk/protocols/base.py
--rw-r--r--   0        0        0        0 2024-02-22 21:15:33.533969 canvas-0.1.6/canvas_sdk/tests/__init__.py
--rw-r--r--   0        0        0       60 2024-05-14 19:42:35.026185 canvas-0.1.6/canvas_sdk/utils/__init__.py
--rw-r--r--   0        0        0     2159 2024-05-14 19:42:35.026264 canvas-0.1.6/canvas_sdk/utils/http.py
--rw-r--r--   0        0        0     1931 2024-05-14 19:42:35.026342 canvas-0.1.6/canvas_sdk/utils/tests.py
--rw-r--r--   0        0        0        0 2024-02-22 21:15:33.534137 canvas-0.1.6/canvas_sdk/views/__init__.py
--rw-r--r--   0        0        0     2210 2024-05-14 22:07:08.711950 canvas-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3776 1970-01-01 00:00:00.000000 canvas-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     2821 2024-05-14 19:42:35.023965 canvas-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2024-02-22 21:15:33.529941 canvas-0.1.7/canvas_cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-22 21:15:33.530030 canvas-0.1.7/canvas_cli/apps/__init__.py
+-rw-r--r--   0        0        0      105 2024-05-11 15:50:29.885352 canvas-0.1.7/canvas_cli/apps/auth/__init__.py
+-rw-r--r--   0        0        0     4528 2024-05-14 19:42:35.024117 canvas-0.1.7/canvas_cli/apps/auth/tests.py
+-rw-r--r--   0        0        0     5434 2024-05-14 19:52:30.122404 canvas-0.1.7/canvas_cli/apps/auth/utils.py
+-rw-r--r--   0        0        0       64 2024-02-22 21:15:33.530476 canvas-0.1.7/canvas_cli/apps/logs/__init__.py
+-rw-r--r--   0        0        0     1825 2024-05-11 15:50:29.885926 canvas-0.1.7/canvas_cli/apps/logs/logs.py
+-rw-r--r--   0        0        0      190 2024-05-11 15:50:29.886101 canvas-0.1.7/canvas_cli/apps/plugin/__init__.py
+-rw-r--r--   0        0        0     9360 2024-05-11 15:50:29.886407 canvas-0.1.7/canvas_cli/apps/plugin/plugin.py
+-rw-r--r--   0        0        0     1035 2024-02-22 21:15:33.530903 canvas-0.1.7/canvas_cli/apps/plugin/tests.py
+-rw-r--r--   0        0        0      959 2024-02-22 21:15:33.530977 canvas-0.1.7/canvas_cli/conftest.py
+-rw-r--r--   0        0        0     2527 2024-05-11 15:50:29.886582 canvas-0.1.7/canvas_cli/main.py
+-rw-r--r--   0        0        0      124 2024-05-14 19:42:35.025394 canvas-0.1.7/canvas_cli/templates/plugins/default/cookiecutter.json
+-rw-r--r--   0        0        0      787 2024-05-14 22:06:23.722577 canvas-0.1.7/canvas_cli/templates/plugins/default/{{ cookiecutter.__project_slug }}/CANVAS_MANIFEST.json
+-rw-r--r--   0        0        0      347 2024-05-14 19:42:35.025623 canvas-0.1.7/canvas_cli/templates/plugins/default/{{ cookiecutter.__project_slug }}/README.md
+-rw-r--r--   0        0        0        0 2024-05-14 19:42:35.025694 canvas-0.1.7/canvas_cli/templates/plugins/default/{{ cookiecutter.__project_slug }}/protocols/__init__.py
+-rw-r--r--   0        0        0     2189 2024-05-17 18:02:41.931419 canvas-0.1.7/canvas_cli/templates/plugins/default/{{ cookiecutter.__project_slug }}/protocols/my_protocol.py
+-rw-r--r--   0        0        0      285 2024-02-22 21:15:33.531711 canvas-0.1.7/canvas_cli/tests.py
+-rw-r--r--   0        0        0        0 2024-02-22 21:15:33.531785 canvas-0.1.7/canvas_cli/utils/__init__.py
+-rw-r--r--   0        0        0      102 2024-02-22 21:15:33.531882 canvas-0.1.7/canvas_cli/utils/context/__init__.py
+-rw-r--r--   0        0        0     5714 2024-05-11 15:50:29.887529 canvas-0.1.7/canvas_cli/utils/context/context.py
+-rw-r--r--   0        0        0     4211 2024-02-22 21:15:33.532069 canvas-0.1.7/canvas_cli/utils/context/tests.py
+-rw-r--r--   0        0        0       88 2024-02-22 21:15:33.532161 canvas-0.1.7/canvas_cli/utils/print/__init__.py
+-rw-r--r--   0        0        0     1829 2024-02-22 21:15:33.532221 canvas-0.1.7/canvas_cli/utils/print/print.py
+-rw-r--r--   0        0        0     2376 2024-02-22 21:15:33.532285 canvas-0.1.7/canvas_cli/utils/print/tests.py
+-rw-r--r--   0        0        0       81 2024-02-22 21:15:33.532384 canvas-0.1.7/canvas_cli/utils/urls/__init__.py
+-rw-r--r--   0        0        0      407 2024-02-22 21:15:33.532447 canvas-0.1.7/canvas_cli/utils/urls/tests.py
+-rw-r--r--   0        0        0      798 2024-02-22 21:15:33.532511 canvas-0.1.7/canvas_cli/utils/urls/urls.py
+-rw-r--r--   0        0        0      113 2024-05-11 15:50:29.887707 canvas-0.1.7/canvas_cli/utils/validators/__init__.py
+-rw-r--r--   0        0        0     3117 2024-05-11 15:50:29.887855 canvas-0.1.7/canvas_cli/utils/validators/manifest_schema.py
+-rw-r--r--   0        0        0     1206 2024-05-11 15:50:29.888019 canvas-0.1.7/canvas_cli/utils/validators/tests.py
+-rw-r--r--   0        0        0     1614 2024-05-11 15:50:29.888512 canvas-0.1.7/canvas_cli/utils/validators/validators.py
+-rw-r--r--   0        0        0        0 2024-02-22 21:15:33.532827 canvas-0.1.7/canvas_sdk/__init__.py
+-rw-r--r--   0        0        0     1116 2024-05-11 15:50:29.888698 canvas-0.1.7/canvas_sdk/commands/__init__.py
+-rw-r--r--   0        0        0     4141 2024-05-11 15:50:29.888840 canvas-0.1.7/canvas_sdk/commands/base.py
+-rw-r--r--   0        0        0     1636 2024-05-11 15:50:29.889167 canvas-0.1.7/canvas_sdk/commands/commands/assess.py
+-rw-r--r--   0        0        0     1382 2024-05-11 15:50:29.889477 canvas-0.1.7/canvas_sdk/commands/commands/diagnose.py
+-rw-r--r--   0        0        0     1527 2024-05-11 15:50:29.889617 canvas-0.1.7/canvas_sdk/commands/commands/goal.py
+-rw-r--r--   0        0        0      366 2024-05-11 15:50:29.889835 canvas-0.1.7/canvas_sdk/commands/commands/history_present_illness.py
+-rw-r--r--   0        0        0      937 2024-05-11 15:50:29.890041 canvas-0.1.7/canvas_sdk/commands/commands/medication_statement.py
+-rw-r--r--   0        0        0      350 2024-05-11 15:50:29.890231 canvas-0.1.7/canvas_sdk/commands/commands/plan.py
+-rw-r--r--   0        0        0     1574 2024-05-11 15:50:29.890317 canvas-0.1.7/canvas_sdk/commands/commands/prescribe.py
+-rw-r--r--   0        0        0      553 2024-05-11 15:50:29.890518 canvas-0.1.7/canvas_sdk/commands/commands/questionnaire.py
+-rw-r--r--   0        0        0     1252 2024-05-11 15:50:29.890728 canvas-0.1.7/canvas_sdk/commands/commands/reason_for_visit.py
+-rw-r--r--   0        0        0      627 2024-05-11 15:50:29.890933 canvas-0.1.7/canvas_sdk/commands/commands/stop_medication.py
+-rw-r--r--   0        0        0     1499 2024-05-11 15:50:29.891031 canvas-0.1.7/canvas_sdk/commands/commands/update_goal.py
+-rw-r--r--   0        0        0      176 2024-03-15 16:24:46.654687 canvas-0.1.7/canvas_sdk/commands/constants.py
+-rw-r--r--   0        0        0     6287 2024-05-11 15:50:29.891189 canvas-0.1.7/canvas_sdk/commands/tests/test_utils.py
+-rw-r--r--   0        0        0    13863 2024-05-11 15:50:29.891357 canvas-0.1.7/canvas_sdk/commands/tests/tests.py
+-rw-r--r--   0        0        0        0 2024-02-22 21:15:33.533678 canvas-0.1.7/canvas_sdk/data/__init__.py
+-rw-r--r--   0        0        0       62 2024-05-11 15:50:29.891476 canvas-0.1.7/canvas_sdk/effects/__init__.py
+-rw-r--r--   0        0        0     1013 2024-05-11 15:50:29.891757 canvas-0.1.7/canvas_sdk/effects/banner_alert/banner_alert.py
+-rw-r--r--   0        0        0      436 2024-05-11 15:50:29.891977 canvas-0.1.7/canvas_sdk/effects/banner_alert/constants.py
+-rw-r--r--   0        0        0      688 2024-05-11 15:50:29.892062 canvas-0.1.7/canvas_sdk/effects/base.py
+-rw-r--r--   0        0        0       74 2024-05-11 15:50:29.892176 canvas-0.1.7/canvas_sdk/events/__init__.py
+-rw-r--r--   0        0        0       51 2024-05-11 15:50:29.892351 canvas-0.1.7/canvas_sdk/protocols/__init__.py
+-rw-r--r--   0        0        0      260 2024-05-14 19:42:35.026075 canvas-0.1.7/canvas_sdk/protocols/base.py
+-rw-r--r--   0        0        0        0 2024-02-22 21:15:33.533969 canvas-0.1.7/canvas_sdk/tests/__init__.py
+-rw-r--r--   0        0        0       60 2024-05-14 19:42:35.026185 canvas-0.1.7/canvas_sdk/utils/__init__.py
+-rw-r--r--   0        0        0     2159 2024-05-14 19:42:35.026264 canvas-0.1.7/canvas_sdk/utils/http.py
+-rw-r--r--   0        0        0     1931 2024-05-14 19:42:35.026342 canvas-0.1.7/canvas_sdk/utils/tests.py
+-rw-r--r--   0        0        0        0 2024-02-22 21:15:33.534137 canvas-0.1.7/canvas_sdk/views/__init__.py
+-rw-r--r--   0        0        0     2210 2024-05-17 18:47:24.751145 canvas-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3776 1970-01-01 00:00:00.000000 canvas-0.1.7/PKG-INFO
```

### Comparing `canvas-0.1.6/README.md` & `canvas-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_cli/apps/auth/tests.py` & `canvas-0.1.7/canvas_cli/apps/auth/tests.py`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_cli/apps/auth/utils.py` & `canvas-0.1.7/canvas_cli/apps/auth/utils.py`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_cli/apps/logs/logs.py` & `canvas-0.1.7/canvas_cli/apps/logs/logs.py`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_cli/apps/plugin/plugin.py` & `canvas-0.1.7/canvas_cli/apps/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_cli/apps/plugin/tests.py` & `canvas-0.1.7/canvas_cli/apps/plugin/tests.py`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_cli/conftest.py` & `canvas-0.1.7/canvas_cli/conftest.py`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_cli/main.py` & `canvas-0.1.7/canvas_cli/main.py`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_cli/templates/plugins/default/{{ cookiecutter.__project_slug }}/CANVAS_MANIFEST.json` & `canvas-0.1.7/canvas_cli/templates/plugins/default/{{ cookiecutter.__project_slug }}/CANVAS_MANIFEST.json`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_cli/templates/plugins/default/{{ cookiecutter.__project_slug }}/protocols/my_protocol.py` & `canvas-0.1.7/canvas_cli/templates/plugins/default/{{ cookiecutter.__project_slug }}/protocols/my_protocol.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,9 +47,9 @@
         payload = {
             "note": {"uuid": self.context["note"]["uuid"]},
             "data": {"narrative": self.NARRATIVE_STRING},
         }
 
         # Return zero, one, or many effects.
         # Example:
-        # return [Effect(type=EffectType.ADD_PLAN_COMMAND, payload=json.dumps(payload))]
+        # return [Effect(type=EffectType.LOG, payload=json.dumps(payload))]
         return []
```

### Comparing `canvas-0.1.6/canvas_cli/utils/context/context.py` & `canvas-0.1.7/canvas_cli/utils/context/context.py`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_cli/utils/context/tests.py` & `canvas-0.1.7/canvas_cli/utils/context/tests.py`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_cli/utils/print/print.py` & `canvas-0.1.7/canvas_cli/utils/print/print.py`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_cli/utils/print/tests.py` & `canvas-0.1.7/canvas_cli/utils/print/tests.py`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_cli/utils/urls/urls.py` & `canvas-0.1.7/canvas_cli/utils/urls/urls.py`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_cli/utils/validators/manifest_schema.py` & `canvas-0.1.7/canvas_cli/utils/validators/manifest_schema.py`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_cli/utils/validators/tests.py` & `canvas-0.1.7/canvas_cli/utils/validators/tests.py`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_cli/utils/validators/validators.py` & `canvas-0.1.7/canvas_cli/utils/validators/validators.py`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_sdk/commands/__init__.py` & `canvas-0.1.7/canvas_sdk/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_sdk/commands/base.py` & `canvas-0.1.7/canvas_sdk/commands/base.py`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_sdk/commands/commands/assess.py` & `canvas-0.1.7/canvas_sdk/commands/commands/assess.py`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_sdk/commands/commands/diagnose.py` & `canvas-0.1.7/canvas_sdk/commands/commands/diagnose.py`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_sdk/commands/commands/goal.py` & `canvas-0.1.7/canvas_sdk/commands/commands/goal.py`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_sdk/commands/commands/medication_statement.py` & `canvas-0.1.7/canvas_sdk/commands/commands/medication_statement.py`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_sdk/commands/commands/prescribe.py` & `canvas-0.1.7/canvas_sdk/commands/commands/prescribe.py`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_sdk/commands/commands/questionnaire.py` & `canvas-0.1.7/canvas_sdk/commands/commands/questionnaire.py`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_sdk/commands/commands/reason_for_visit.py` & `canvas-0.1.7/canvas_sdk/commands/commands/reason_for_visit.py`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_sdk/commands/commands/stop_medication.py` & `canvas-0.1.7/canvas_sdk/commands/commands/stop_medication.py`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_sdk/commands/commands/update_goal.py` & `canvas-0.1.7/canvas_sdk/commands/commands/update_goal.py`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_sdk/commands/tests/test_utils.py` & `canvas-0.1.7/canvas_sdk/commands/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_sdk/commands/tests/tests.py` & `canvas-0.1.7/canvas_sdk/commands/tests/tests.py`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_sdk/effects/banner_alert/banner_alert.py` & `canvas-0.1.7/canvas_sdk/effects/banner_alert/banner_alert.py`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_sdk/effects/base.py` & `canvas-0.1.7/canvas_sdk/effects/base.py`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_sdk/utils/http.py` & `canvas-0.1.7/canvas_sdk/utils/http.py`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/canvas_sdk/utils/tests.py` & `canvas-0.1.7/canvas_sdk/utils/tests.py`

 * *Files identical despite different names*

### Comparing `canvas-0.1.6/pyproject.toml` & `canvas-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 [tool.poetry]
 authors = ["Canvas Team <engineering@canvasmedical.com>"]
 description = "SDK to customize event-driven actions in your Canvas instance"
 license = "MIT"
 name = "canvas"
 packages = [{include = "canvas_cli"}, {include = "canvas_sdk"}]
 readme = "README.md"
-version = "0.1.6"
+version = "0.1.7"
 
 [tool.poetry.dependencies]
 cookiecutter = "*"
 grpcio = "^1.60.1"
 ipython = "^8.21.0"
 jsonschema = "^4.21.1"
 keyring = "*"
```

### Comparing `canvas-0.1.6/PKG-INFO` & `canvas-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canvas
-Version: 0.1.6
+Version: 0.1.7
 Summary: SDK to customize event-driven actions in your Canvas instance
 License: MIT
 Author: Canvas Team
 Author-email: engineering@canvasmedical.com
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

