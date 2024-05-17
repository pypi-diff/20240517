# Comparing `tmp/django-exception-logger-0.1.3.tar.gz` & `tmp/django-exception-logger-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-exception-logger-0.1.3.tar", last modified: Fri May 17 14:46:57 2024, max compression
+gzip compressed data, was "django-exception-logger-0.1.4.tar", last modified: Fri May 17 15:44:28 2024, max compression
```

## Comparing `django-exception-logger-0.1.3.tar` & `django-exception-logger-0.1.4.tar`

### file list

```diff
@@ -1,38 +1,45 @@
-drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 14:46:57.488410 django-exception-logger-0.1.3/
--rwxrwxrwx   0 titov     (1000) titov     (1000)     1065 2024-05-17 09:26:59.000000 django-exception-logger-0.1.3/LICENSE
--rwxrwxrwx   0 titov     (1000) titov     (1000)      341 2024-05-17 14:18:21.000000 django-exception-logger-0.1.3/MANIFEST.in
--rwxrwxrwx   0 titov     (1000) titov     (1000)     1679 2024-05-17 14:46:57.479411 django-exception-logger-0.1.3/PKG-INFO
--rwxrwxrwx   0 titov     (1000) titov     (1000)     1351 2024-05-17 12:38:32.000000 django-exception-logger-0.1.3/README.md
-drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 14:46:56.944409 django-exception-logger-0.1.3/django_exception_logger.egg-info/
--rwxrwxrwx   0 titov     (1000) titov     (1000)     1679 2024-05-17 14:46:56.000000 django-exception-logger-0.1.3/django_exception_logger.egg-info/PKG-INFO
--rwxrwxrwx   0 titov     (1000) titov     (1000)     1035 2024-05-17 14:46:56.000000 django-exception-logger-0.1.3/django_exception_logger.egg-info/SOURCES.txt
--rwxrwxrwx   0 titov     (1000) titov     (1000)        1 2024-05-17 14:46:56.000000 django-exception-logger-0.1.3/django_exception_logger.egg-info/dependency_links.txt
--rwxrwxrwx   0 titov     (1000) titov     (1000)       12 2024-05-17 14:46:56.000000 django-exception-logger-0.1.3/django_exception_logger.egg-info/requires.txt
--rwxrwxrwx   0 titov     (1000) titov     (1000)       17 2024-05-17 14:46:56.000000 django-exception-logger-0.1.3/django_exception_logger.egg-info/top_level.txt
-drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 14:46:57.049565 django-exception-logger-0.1.3/exception_logger/
--rwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-06 12:59:31.000000 django-exception-logger-0.1.3/exception_logger/__init__.py
-drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 14:46:57.141933 django-exception-logger-0.1.3/exception_logger/admin/
--rwxrwxrwx   0 titov     (1000) titov     (1000)      193 2024-05-06 12:59:31.000000 django-exception-logger-0.1.3/exception_logger/admin/__init__.py
--rwxrwxrwx   0 titov     (1000) titov     (1000)     1764 2024-05-17 09:33:45.000000 django-exception-logger-0.1.3/exception_logger/admin/celery_exception.py
--rwxrwxrwx   0 titov     (1000) titov     (1000)     2028 2024-05-17 12:38:32.000000 django-exception-logger-0.1.3/exception_logger/admin/exception.py
--rwxrwxrwx   0 titov     (1000) titov     (1000)      741 2024-05-17 12:38:32.000000 django-exception-logger-0.1.3/exception_logger/admin/request_time.py
--rwxrwxrwx   0 titov     (1000) titov     (1000)      253 2024-05-17 09:33:45.000000 django-exception-logger-0.1.3/exception_logger/apps.py
--rwxrwxrwx   0 titov     (1000) titov     (1000)      391 2024-05-06 12:59:31.000000 django-exception-logger-0.1.3/exception_logger/forms.py
-drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 14:46:57.212536 django-exception-logger-0.1.3/exception_logger/middlewares/
--rwxrwxrwx   0 titov     (1000) titov     (1000)      106 2024-05-06 12:59:31.000000 django-exception-logger-0.1.3/exception_logger/middlewares/__init__.py
--rwxrwxrwx   0 titov     (1000) titov     (1000)     1235 2024-05-06 12:59:31.000000 django-exception-logger-0.1.3/exception_logger/middlewares/exception_logger.py
--rwxrwxrwx   0 titov     (1000) titov     (1000)      620 2024-05-06 12:59:31.000000 django-exception-logger-0.1.3/exception_logger/middlewares/request_time.py
-drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 14:46:57.278745 django-exception-logger-0.1.3/exception_logger/migrations/
--rwxrwxrwx   0 titov     (1000) titov     (1000)     6640 2024-05-17 09:46:17.000000 django-exception-logger-0.1.3/exception_logger/migrations/0001_initial.py
--rwxrwxrwx   0 titov     (1000) titov     (1000)      381 2024-05-06 12:59:31.000000 django-exception-logger-0.1.3/exception_logger/migrations/0002_alter_exceptionmodel_exception.py
--rwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-06 12:59:31.000000 django-exception-logger-0.1.3/exception_logger/migrations/__init__.py
-drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 14:46:57.431801 django-exception-logger-0.1.3/exception_logger/models/
--rwxrwxrwx   0 titov     (1000) titov     (1000)      235 2024-05-06 12:59:31.000000 django-exception-logger-0.1.3/exception_logger/models/__init__.py
--rwxrwxrwx   0 titov     (1000) titov     (1000)     2366 2024-05-17 09:44:15.000000 django-exception-logger-0.1.3/exception_logger/models/celery_exception.py
--rwxrwxrwx   0 titov     (1000) titov     (1000)      215 2024-05-06 12:59:31.000000 django-exception-logger-0.1.3/exception_logger/models/enums.py
--rwxrwxrwx   0 titov     (1000) titov     (1000)     2791 2024-05-17 09:44:15.000000 django-exception-logger-0.1.3/exception_logger/models/exception.py
--rwxrwxrwx   0 titov     (1000) titov     (1000)     1702 2024-05-17 09:46:43.000000 django-exception-logger-0.1.3/exception_logger/models/request_time.py
--rwxrwxrwx   0 titov     (1000) titov     (1000)     1457 2024-05-06 12:59:31.000000 django-exception-logger-0.1.3/exception_logger/signals.py
--rwxrwxrwx   0 titov     (1000) titov     (1000)      387 2024-05-17 14:41:04.000000 django-exception-logger-0.1.3/exception_logger/utils.py
--rwxrwxrwx   0 titov     (1000) titov     (1000)       38 2024-05-17 14:46:57.489429 django-exception-logger-0.1.3/setup.cfg
--rwxrwxrwx   0 titov     (1000) titov     (1000)      636 2024-05-17 14:46:14.000000 django-exception-logger-0.1.3/setup.py
+drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 15:44:28.474914 django-exception-logger-0.1.4/
+-rwxrwxrwx   0 titov     (1000) titov     (1000)     1065 2024-05-17 09:26:59.000000 django-exception-logger-0.1.4/LICENSE
+-rwxrwxrwx   0 titov     (1000) titov     (1000)      341 2024-05-17 14:18:21.000000 django-exception-logger-0.1.4/MANIFEST.in
+-rwxrwxrwx   0 titov     (1000) titov     (1000)     1679 2024-05-17 15:44:28.471814 django-exception-logger-0.1.4/PKG-INFO
+-rwxrwxrwx   0 titov     (1000) titov     (1000)     1351 2024-05-17 12:38:32.000000 django-exception-logger-0.1.4/README.md
+drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 15:44:27.906764 django-exception-logger-0.1.4/django_exception_logger.egg-info/
+-rwxrwxrwx   0 titov     (1000) titov     (1000)     1679 2024-05-17 15:44:27.000000 django-exception-logger-0.1.4/django_exception_logger.egg-info/PKG-INFO
+-rwxrwxrwx   0 titov     (1000) titov     (1000)     1133 2024-05-17 15:44:27.000000 django-exception-logger-0.1.4/django_exception_logger.egg-info/SOURCES.txt
+-rwxrwxrwx   0 titov     (1000) titov     (1000)        1 2024-05-17 15:44:27.000000 django-exception-logger-0.1.4/django_exception_logger.egg-info/dependency_links.txt
+-rwxrwxrwx   0 titov     (1000) titov     (1000)       12 2024-05-17 15:44:27.000000 django-exception-logger-0.1.4/django_exception_logger.egg-info/requires.txt
+-rwxrwxrwx   0 titov     (1000) titov     (1000)       17 2024-05-17 15:44:27.000000 django-exception-logger-0.1.4/django_exception_logger.egg-info/top_level.txt
+drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 15:44:28.034467 django-exception-logger-0.1.4/exception_logger/
+-rwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-06 12:59:31.000000 django-exception-logger-0.1.4/exception_logger/__init__.py
+drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 15:44:28.193388 django-exception-logger-0.1.4/exception_logger/admin/
+-rwxrwxrwx   0 titov     (1000) titov     (1000)      193 2024-05-06 12:59:31.000000 django-exception-logger-0.1.4/exception_logger/admin/__init__.py
+-rwxrwxrwx   0 titov     (1000) titov     (1000)     1764 2024-05-17 09:33:45.000000 django-exception-logger-0.1.4/exception_logger/admin/celery_exception.py
+-rwxrwxrwx   0 titov     (1000) titov     (1000)     2028 2024-05-17 12:38:32.000000 django-exception-logger-0.1.4/exception_logger/admin/exception.py
+-rwxrwxrwx   0 titov     (1000) titov     (1000)      799 2024-05-17 15:37:01.000000 django-exception-logger-0.1.4/exception_logger/admin/request_time.py
+-rwxrwxrwx   0 titov     (1000) titov     (1000)      311 2024-05-17 15:39:16.000000 django-exception-logger-0.1.4/exception_logger/apps.py
+-rwxrwxrwx   0 titov     (1000) titov     (1000)      391 2024-05-06 12:59:31.000000 django-exception-logger-0.1.4/exception_logger/forms.py
+drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 15:44:27.751535 django-exception-logger-0.1.4/exception_logger/locale/
+drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 15:44:27.747532 django-exception-logger-0.1.4/exception_logger/locale/en/
+drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 15:44:28.209392 django-exception-logger-0.1.4/exception_logger/locale/en/LC_MESSAGES/
+-rwxrwxrwx   0 titov     (1000) titov     (1000)      380 2024-05-17 15:40:37.000000 django-exception-logger-0.1.4/exception_logger/locale/en/LC_MESSAGES/django.mo
+drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 15:44:27.752537 django-exception-logger-0.1.4/exception_logger/locale/ru/
+drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 15:44:28.229312 django-exception-logger-0.1.4/exception_logger/locale/ru/LC_MESSAGES/
+-rwxrwxrwx   0 titov     (1000) titov     (1000)     1325 2024-05-17 15:40:37.000000 django-exception-logger-0.1.4/exception_logger/locale/ru/LC_MESSAGES/django.mo
+drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 15:44:28.274776 django-exception-logger-0.1.4/exception_logger/middlewares/
+-rwxrwxrwx   0 titov     (1000) titov     (1000)      106 2024-05-06 12:59:31.000000 django-exception-logger-0.1.4/exception_logger/middlewares/__init__.py
+-rwxrwxrwx   0 titov     (1000) titov     (1000)     1235 2024-05-06 12:59:31.000000 django-exception-logger-0.1.4/exception_logger/middlewares/exception_logger.py
+-rwxrwxrwx   0 titov     (1000) titov     (1000)      620 2024-05-06 12:59:31.000000 django-exception-logger-0.1.4/exception_logger/middlewares/request_time.py
+drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 15:44:28.341598 django-exception-logger-0.1.4/exception_logger/migrations/
+-rwxrwxrwx   0 titov     (1000) titov     (1000)     9468 2024-05-17 15:12:08.000000 django-exception-logger-0.1.4/exception_logger/migrations/0001_initial.py
+-rwxrwxrwx   0 titov     (1000) titov     (1000)      381 2024-05-06 12:59:31.000000 django-exception-logger-0.1.4/exception_logger/migrations/0002_alter_exceptionmodel_exception.py
+-rwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-06 12:59:31.000000 django-exception-logger-0.1.4/exception_logger/migrations/__init__.py
+drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 15:44:28.451216 django-exception-logger-0.1.4/exception_logger/models/
+-rwxrwxrwx   0 titov     (1000) titov     (1000)      235 2024-05-06 12:59:31.000000 django-exception-logger-0.1.4/exception_logger/models/__init__.py
+-rwxrwxrwx   0 titov     (1000) titov     (1000)     2452 2024-05-17 15:12:07.000000 django-exception-logger-0.1.4/exception_logger/models/celery_exception.py
+-rwxrwxrwx   0 titov     (1000) titov     (1000)      215 2024-05-06 12:59:31.000000 django-exception-logger-0.1.4/exception_logger/models/enums.py
+-rwxrwxrwx   0 titov     (1000) titov     (1000)     2880 2024-05-17 15:12:07.000000 django-exception-logger-0.1.4/exception_logger/models/exception.py
+-rwxrwxrwx   0 titov     (1000) titov     (1000)     1779 2024-05-17 15:12:07.000000 django-exception-logger-0.1.4/exception_logger/models/request_time.py
+-rwxrwxrwx   0 titov     (1000) titov     (1000)     1457 2024-05-06 12:59:31.000000 django-exception-logger-0.1.4/exception_logger/signals.py
+-rwxrwxrwx   0 titov     (1000) titov     (1000)      387 2024-05-17 14:41:04.000000 django-exception-logger-0.1.4/exception_logger/utils.py
+-rwxrwxrwx   0 titov     (1000) titov     (1000)       38 2024-05-17 15:44:28.475911 django-exception-logger-0.1.4/setup.cfg
+-rwxrwxrwx   0 titov     (1000) titov     (1000)      668 2024-05-17 15:44:24.000000 django-exception-logger-0.1.4/setup.py
```

### Comparing `django-exception-logger-0.1.3/LICENSE` & `django-exception-logger-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-exception-logger-0.1.3/PKG-INFO` & `django-exception-logger-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-exception-logger
-Version: 0.1.3
+Version: 0.1.4
 Summary: Adds error logging to the admin panel
 Home-page: https://github.com/Leonid-T/django-exception-logger/
 Author: Titov Leonid
 Author-email: titov281@yandex.ru
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `django-exception-logger-0.1.3/README.md` & `django-exception-logger-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `django-exception-logger-0.1.3/django_exception_logger.egg-info/PKG-INFO` & `django-exception-logger-0.1.4/django_exception_logger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-exception-logger
-Version: 0.1.3
+Version: 0.1.4
 Summary: Adds error logging to the admin panel
 Home-page: https://github.com/Leonid-T/django-exception-logger/
 Author: Titov Leonid
 Author-email: titov281@yandex.ru
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `django-exception-logger-0.1.3/django_exception_logger.egg-info/SOURCES.txt` & `django-exception-logger-0.1.4/django_exception_logger.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 exception_logger/forms.py
 exception_logger/signals.py
 exception_logger/utils.py
 exception_logger/admin/__init__.py
 exception_logger/admin/celery_exception.py
 exception_logger/admin/exception.py
 exception_logger/admin/request_time.py
+exception_logger/locale/en/LC_MESSAGES/django.mo
+exception_logger/locale/ru/LC_MESSAGES/django.mo
 exception_logger/middlewares/__init__.py
 exception_logger/middlewares/exception_logger.py
 exception_logger/middlewares/request_time.py
 exception_logger/migrations/0001_initial.py
 exception_logger/migrations/0002_alter_exceptionmodel_exception.py
 exception_logger/migrations/__init__.py
 exception_logger/models/__init__.py
```

### Comparing `django-exception-logger-0.1.3/exception_logger/admin/celery_exception.py` & `django-exception-logger-0.1.4/exception_logger/admin/celery_exception.py`

 * *Files identical despite different names*

### Comparing `django-exception-logger-0.1.3/exception_logger/admin/exception.py` & `django-exception-logger-0.1.4/exception_logger/admin/exception.py`

 * *Files identical despite different names*

### Comparing `django-exception-logger-0.1.3/exception_logger/admin/request_time.py` & `django-exception-logger-0.1.4/exception_logger/admin/request_time.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from django.contrib import admin
+from django.utils.translation import gettext_lazy as _
 
 
 class RequestTimeAdmin(admin.ModelAdmin):
     fields = ("method", "path", "average_with_delta_error", "quantity")
     list_display = ("method", "path", "average_with_delta_error", "quantity")
     list_display_links = ("method", "path")
     list_filter = ("method",)
     search_fields = ("path", "method")
     ordering = ("-average_time", "-quantity")
 
-    @admin.display(description="Время запроса, сек")
+    @admin.display(description=(_("Request time") + ", " + _("sec")))
     def average_with_delta_error(self, obj):
         return f"{round(obj.average_time, 6)} ± {round(obj.error_delta, 6)}"
 
     def has_add_permission(self, request):
         return False
 
     def has_change_permission(self, request, obj=None):
```

### Comparing `django-exception-logger-0.1.3/exception_logger/middlewares/exception_logger.py` & `django-exception-logger-0.1.4/exception_logger/middlewares/exception_logger.py`

 * *Files identical despite different names*

### Comparing `django-exception-logger-0.1.3/exception_logger/middlewares/request_time.py` & `django-exception-logger-0.1.4/exception_logger/middlewares/request_time.py`

 * *Files identical despite different names*

### Comparing `django-exception-logger-0.1.3/exception_logger/models/celery_exception.py` & `django-exception-logger-0.1.4/exception_logger/models/celery_exception.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     TextField,
     JSONField,
     PositiveIntegerField,
     ForeignKey,
     CASCADE,
     UniqueConstraint,
 )
+from django.utils.translation import gettext_lazy as _
 
 
 class CeleryExceptionManager(Manager):
     @staticmethod
     def save_exception(*, task, exception, traceback, args, kwargs):
         unique_data = {"task": task, "exception": exception}
 
@@ -26,28 +27,28 @@
 
         CeleryExceptionDataModel.objects.create(
             exception=exception_model, args=args, kwargs=kwargs
         )
 
 
 class CeleryExceptionModel(Model):
-    task = CharField("Task", max_length=512)
+    task = CharField(_("Task"), max_length=512)
 
     exception = TextField()
     traceback = TextField()
 
-    count = PositiveIntegerField("Quantity", default=1)
-    last_throw = DateTimeField("Last throw", auto_now=True)
-    first_throw = DateTimeField("First throw", auto_now_add=True)
+    count = PositiveIntegerField(_("Quantity"), default=1)
+    last_throw = DateTimeField(_("Last throw"), auto_now=True)
+    first_throw = DateTimeField(_("First throw"), auto_now_add=True)
 
     objects = CeleryExceptionManager()
 
     class Meta:
-        verbose_name = "Celery Exception"
-        verbose_name_plural = "Celery Exceptions"
+        verbose_name = _("Celery Exception")
+        verbose_name_plural = _("Celery Exceptions")
         constraints = (
             UniqueConstraint(fields=("task", "exception"), name="exception_task"),
         )
 
     def __str__(self):
         return ""
 
@@ -62,26 +63,26 @@
 
 class CeleryExceptionDataModel(Model):
     exception = ForeignKey(CeleryExceptionModel, on_delete=CASCADE)
 
     args = JSONField("args", default=list)
     kwargs = JSONField("kwargs", default=dict)
 
-    datetime = DateTimeField("Date", auto_now_add=True)
+    datetime = DateTimeField(_("Date"), auto_now_add=True)
 
     class Meta:
-        verbose_name = "Throw data"
+        verbose_name = _("Throw data")
         verbose_name_plural = verbose_name
 
     def __str__(self):
         return str(self.pk or "-")
 
 
 class NoLogCeleryException(Model):
     exception = CharField(max_length=256)
 
     class Meta:
-        verbose_name = "No log Celery Exception"
-        verbose_name_plural = "No log Celery Exceptions"
+        verbose_name = _("No log Celery Exception")
+        verbose_name_plural = _("No log Celery Exceptions")
 
     def __str__(self):
         return self.exception
```

### Comparing `django-exception-logger-0.1.3/exception_logger/models/exception.py` & `django-exception-logger-0.1.4/exception_logger/models/exception.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     TextField,
     JSONField,
     PositiveIntegerField,
     ForeignKey,
     CASCADE,
     UniqueConstraint,
 )
+from django.utils.translation import gettext_lazy as _
 
 from .enums import Method
 
 
 class ExceptionManager(Manager):
     @staticmethod
     def save_exception(
@@ -45,29 +46,29 @@
             headers=headers,
             cookies=cookies,
             base_url=base_url,
         )
 
 
 class ExceptionModel(Model):
-    method = CharField("Request method", max_length=8, choices=Method.choices)
-    path = CharField("Request path", max_length=512)
+    method = CharField(_("Request method"), max_length=8, choices=Method.choices)
+    path = CharField(_("Request path"), max_length=512)
 
     exception = TextField()
     traceback = TextField()
 
-    count = PositiveIntegerField("Quantity", default=1)
-    last_throw = DateTimeField("Last throw", auto_now=True)
-    first_throw = DateTimeField("Fast throw", auto_now_add=True)
+    count = PositiveIntegerField(_("Quantity"), default=1)
+    last_throw = DateTimeField(_("Last throw"), auto_now=True)
+    first_throw = DateTimeField(_("First throw"), auto_now_add=True)
 
     objects = ExceptionManager()
 
     class Meta:
-        verbose_name = "Exception"
-        verbose_name_plural = "Exceptions"
+        verbose_name = _("Exception")
+        verbose_name_plural = _("Exceptions")
         constraints = (
             UniqueConstraint(
                 fields=("method", "path", "exception"), name="exception_path"
             ),
         )
 
     def __str__(self):
@@ -87,26 +88,26 @@
 
     base_url = CharField(max_length=128)
     data = JSONField("Body", default=dict)
     query_params = JSONField("Query params", default=dict)
     headers = JSONField("Headers", default=dict)
     cookies = JSONField("Cookies", default=dict)
 
-    datetime = DateTimeField("Date", auto_now_add=True)
+    datetime = DateTimeField(_("Date"), auto_now_add=True)
 
     class Meta:
-        verbose_name = "Throw data"
+        verbose_name = _("Throw data")
         verbose_name_plural = verbose_name
 
     def __str__(self):
         return str(self.pk or "-")
 
 
 class NoLogException(Model):
     exception = CharField(max_length=256)
 
     class Meta:
-        verbose_name = "No log Exception"
-        verbose_name_plural = "No log Exceptions"
+        verbose_name = _("No log Exception")
+        verbose_name_plural = _("No log Exceptions")
 
     def __str__(self):
         return self.exception
```

### Comparing `django-exception-logger-0.1.3/exception_logger/models/request_time.py` & `django-exception-logger-0.1.4/exception_logger/models/request_time.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,15 @@
     Model,
     FloatField,
     CharField,
     Manager,
     PositiveIntegerField,
     UniqueConstraint,
 )
+from django.utils.translation import gettext_lazy as _
 
 from .enums import Method
 
 
 class RequestTimeManager(Manager):
     def update_request_time(self, *, method, path, time_delta):
         try:
@@ -32,26 +33,26 @@
 
         request_time.save()
 
 
 class RequestTime(Model):
     Method = Method
 
-    method = CharField("Request method", max_length=8, choices=Method.choices)
-    path = CharField("Request path", max_length=512)
+    method = CharField(_("Request method"), max_length=8, choices=Method.choices)
+    path = CharField(_("Request path"), max_length=512)
 
-    average_time = FloatField("Average request time", default=0)
-    dispersion = FloatField("Dispersion", default=0)
-    quantity = PositiveIntegerField("Quantity", default=0)
+    average_time = FloatField(_("Average request time"), default=0)
+    dispersion = FloatField(_("Dispersion"), default=0)
+    quantity = PositiveIntegerField(_("Quantity"), default=0)
 
     objects = RequestTimeManager()
 
     class Meta:
-        verbose_name = "Request time"
-        verbose_name_plural = "Request times"
+        verbose_name = _("Request time")
+        verbose_name_plural = _("Request times")
         constraints = (
             UniqueConstraint(fields=("method", "path"), name="request_path"),
         )
 
     def __str__(self):
         return ""
```

### Comparing `django-exception-logger-0.1.3/exception_logger/signals.py` & `django-exception-logger-0.1.4/exception_logger/signals.py`

 * *Files identical despite different names*

### Comparing `django-exception-logger-0.1.3/setup.py` & `django-exception-logger-0.1.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 README = open(os.path.join(here, "README.md")).read()
 
 
 setup(
     name="django-exception-logger",
-    version="0.1.3",
+    version="0.1.4",
     packages=find_packages(exclude=["tests*"]),
+    include_package_data=True,
     description="Adds error logging to the admin panel",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Titov Leonid",
     author_email="titov281@yandex.ru",
     url="https://github.com/Leonid-T/django-exception-logger/",
     license="MIT",
```

