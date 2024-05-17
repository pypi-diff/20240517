# Comparing `tmp/nanodjango-0.5.0.tar.gz` & `tmp/nanodjango-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanodjango-0.5.0.tar", last modified: Tue May 14 19:19:15 2024, max compression
+gzip compressed data, was "nanodjango-0.6.0.tar", last modified: Fri May 17 12:34:11 2024, max compression
```

## Comparing `nanodjango-0.5.0.tar` & `nanodjango-0.6.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:19:15.504042 nanodjango-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-05-14 19:19:15.500042 nanodjango-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-14 19:19:10.000000 nanodjango-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:19:15.496042 nanodjango-0.5.0/nanodjango/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8488 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/app_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:19:15.500042 nanodjango-0.5.0/nanodjango/convert/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/convert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:19:15.500042 nanodjango-0.5.0/nanodjango/convert/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/convert/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/convert/contrib/django_ninja.py
--rw-r--r--   0 runner    (1001) docker     (127)    23877 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/convert/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/convert/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    10410 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/convert/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/convert/reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/convert/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:19:15.500042 nanodjango-0.5.0/nanodjango/django_glue/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/django_glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/django_glue/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/django_glue/db.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:19:15.500042 nanodjango-0.5.0/nanodjango.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-05-14 19:19:15.000000 nanodjango-0.5.0/nanodjango.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-14 19:19:15.000000 nanodjango-0.5.0/nanodjango.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:19:15.000000 nanodjango-0.5.0/nanodjango.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-14 19:19:15.000000 nanodjango-0.5.0/nanodjango.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-14 19:19:15.000000 nanodjango-0.5.0/nanodjango.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 19:19:15.000000 nanodjango-0.5.0/nanodjango.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-14 19:19:10.000000 nanodjango-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 19:19:15.504042 nanodjango-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:19:15.500042 nanodjango-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-14 19:19:10.000000 nanodjango-0.5.0/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-14 19:19:10.000000 nanodjango-0.5.0/tests/test_run_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-14 19:19:10.000000 nanodjango-0.5.0/tests/test_run_runserver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:34:11.740775 nanodjango-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-05-17 12:34:11.740775 nanodjango-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-05-17 12:34:06.000000 nanodjango-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:34:11.736775 nanodjango-0.6.0/nanodjango/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-17 12:34:06.000000 nanodjango-0.6.0/nanodjango/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-17 12:34:06.000000 nanodjango-0.6.0/nanodjango/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9402 2024-05-17 12:34:06.000000 nanodjango-0.6.0/nanodjango/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-17 12:34:06.000000 nanodjango-0.6.0/nanodjango/app_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-17 12:34:06.000000 nanodjango-0.6.0/nanodjango/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-17 12:34:06.000000 nanodjango-0.6.0/nanodjango/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:34:11.740775 nanodjango-0.6.0/nanodjango/convert/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-17 12:34:06.000000 nanodjango-0.6.0/nanodjango/convert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:34:11.740775 nanodjango-0.6.0/nanodjango/convert/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-17 12:34:06.000000 nanodjango-0.6.0/nanodjango/convert/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-17 12:34:06.000000 nanodjango-0.6.0/nanodjango/convert/contrib/django_ninja.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23877 2024-05-17 12:34:06.000000 nanodjango-0.6.0/nanodjango/convert/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-05-17 12:34:06.000000 nanodjango-0.6.0/nanodjango/convert/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10410 2024-05-17 12:34:06.000000 nanodjango-0.6.0/nanodjango/convert/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-17 12:34:06.000000 nanodjango-0.6.0/nanodjango/convert/reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-05-17 12:34:06.000000 nanodjango-0.6.0/nanodjango/convert/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:34:11.740775 nanodjango-0.6.0/nanodjango/django_glue/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:34:06.000000 nanodjango-0.6.0/nanodjango/django_glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-17 12:34:06.000000 nanodjango-0.6.0/nanodjango/django_glue/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-17 12:34:06.000000 nanodjango-0.6.0/nanodjango/django_glue/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-17 12:34:06.000000 nanodjango-0.6.0/nanodjango/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-17 12:34:06.000000 nanodjango-0.6.0/nanodjango/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-17 12:34:06.000000 nanodjango-0.6.0/nanodjango/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-17 12:34:06.000000 nanodjango-0.6.0/nanodjango/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-17 12:34:06.000000 nanodjango-0.6.0/nanodjango/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:34:11.740775 nanodjango-0.6.0/nanodjango.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-05-17 12:34:11.000000 nanodjango-0.6.0/nanodjango.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-17 12:34:11.000000 nanodjango-0.6.0/nanodjango.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 12:34:11.000000 nanodjango-0.6.0/nanodjango.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-17 12:34:11.000000 nanodjango-0.6.0/nanodjango.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-17 12:34:11.000000 nanodjango-0.6.0/nanodjango.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 12:34:11.000000 nanodjango-0.6.0/nanodjango.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-17 12:34:06.000000 nanodjango-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 12:34:11.740775 nanodjango-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:34:11.740775 nanodjango-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-17 12:34:06.000000 nanodjango-0.6.0/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-17 12:34:06.000000 nanodjango-0.6.0/tests/test_run_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-17 12:34:06.000000 nanodjango-0.6.0/tests/test_run_runserver.py
```

### Comparing `nanodjango-0.5.0/PKG-INFO` & `nanodjango-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanodjango
-Version: 0.5.0
+Version: 0.6.0
 Summary: Run Django models and views from a single file, and convert it to a full project.
 Author-email: Richard Terry <code@radiac.net>
 Project-URL: Homepage, https://radiac.net/projects/nanodjango/
 Project-URL: Documentation, https://nanodjango.readthedocs.io/en/latest/
 Project-URL: Changelog, https://nanodjango.readthedocs.io/en/latest/changelog.html
 Project-URL: Repository, https://github.com/radiac/nanodjango
 Project-URL: Issues, https://github.com/radiac/nanodjango/issues
@@ -68,33 +68,32 @@
     CountLog.objects.create()
     return f"<p>Number of page loads: {CountLog.objects.count()}</p>"
 ```
 
 Save that as ``counter.py``, then set up your database and run it locally with:
 
 ```sh
-nanodjango run counter.py makemigrations counter
-nanodjango run counter.py migrate
-nanodjango run counter.py createsuperuser
-nanodjango run counter.py
+nanodjango start counter.py
 ```
 
 It will create your database in a ``db.sqlite3`` file next to your ``counter.py``, with
-the appropriate migrations in ``migrations/``.
+the appropriate migrations in ``migrations/``. Alternatively you could run each of these
+commands manually with the ``run`` command, eg
+``nanodjango run counter.py runserver 0:8000``
 
 Run it in production using WSGI:
 
 ```sh
 gunicorn -w 4 counter:app
 ```
 
 or automatically convert it to a full Django project:
 
 ```sh
-nanodjango counter.py convert /path/to/project --name=myproject
+nanodjango convert counter.py /path/to/project --name=myproject
 ```
 
 and with a [couple of extra
 lines](https://nanodjango.readthedocs.io/en/latest/management.html#run-script), run the
 development server as a standalone script using ``python``, or use ``pipx run`` to run
 it and automatically install dependencies to a temporary virtual environment:
```

### Comparing `nanodjango-0.5.0/README.md` & `nanodjango-0.6.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -45,33 +45,32 @@
     CountLog.objects.create()
     return f"<p>Number of page loads: {CountLog.objects.count()}</p>"
 ```
 
 Save that as ``counter.py``, then set up your database and run it locally with:
 
 ```sh
-nanodjango run counter.py makemigrations counter
-nanodjango run counter.py migrate
-nanodjango run counter.py createsuperuser
-nanodjango run counter.py
+nanodjango start counter.py
 ```
 
 It will create your database in a ``db.sqlite3`` file next to your ``counter.py``, with
-the appropriate migrations in ``migrations/``.
+the appropriate migrations in ``migrations/``. Alternatively you could run each of these
+commands manually with the ``run`` command, eg
+``nanodjango run counter.py runserver 0:8000``
 
 Run it in production using WSGI:
 
 ```sh
 gunicorn -w 4 counter:app
 ```
 
 or automatically convert it to a full Django project:
 
 ```sh
-nanodjango counter.py convert /path/to/project --name=myproject
+nanodjango convert counter.py /path/to/project --name=myproject
 ```
 
 and with a [couple of extra
 lines](https://nanodjango.readthedocs.io/en/latest/management.html#run-script), run the
 development server as a standalone script using ``python``, or use ``pipx run`` to run
 it and automatically install dependencies to a temporary virtual environment:
```

### Comparing `nanodjango-0.5.0/nanodjango/app.py` & `nanodjango-0.6.0/nanodjango/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,26 +6,33 @@
 from pathlib import Path
 from types import ModuleType
 from typing import TYPE_CHECKING, Any, Callable
 
 from django import setup
 from django import urls as django_urls
 from django.contrib import admin
+from django.contrib.auth import get_user_model
+from django.db.models import Model
 from django.views import View
 
 from . import app_meta
 from .exceptions import ConfigurationError, UsageError
 from .urls import urlpatterns
 from .views import string_view
 
 
 if TYPE_CHECKING:
     from pathlib import Path
 
-    from django.db.models import Model
+
+def exec_manage(*args):
+    from django.core.management import execute_from_command_line
+
+    args = ["nanodjango"] + list(args)
+    execute_from_command_line(args)
 
 
 class Django:
     """
     The main Django app
     """
 
@@ -106,32 +113,14 @@
 
         patch_db(self.app_name)
         prepare_apps(self.app_name, self.app_module)
 
         # Ready for Django's standard setup
         setup()
 
-    def _prepare(self):
-        """
-        Perform any final setup for this project after it has been imported:
-
-        * register the admin site
-        """
-        admin_url = self.settings.ADMIN_URL
-        if admin_url or self.has_admin:
-            if admin_url is None:
-                admin_url = "admin/"
-            if not isinstance(admin_url, str) or not admin_url.endswith("/"):
-                raise ConfigurationError(
-                    "settings.ADMIN_URL must be a string path ending in /"
-                )
-            urlpatterns.append(
-                django_urls.path(admin_url.removeprefix("/"), admin.site.urls)
-            )
-
     def route(self, pattern: str, *, re=False, include=None):
         """
         Decorator to add a view to the urls
 
         The pattern should use the Django path syntax - see
         https://docs.djangoproject.com/en/dev/ref/urls/#path
 
@@ -215,46 +204,87 @@
         if model is None:
             # Called with arguments, @admin(attr=val)
             return wrap
 
         # Called without arguments, @admin - call wrapped immediately
         return wrap(model)
 
-    def run(self, args: list[str] | tuple[str] | None = None):
+    def _prepare(self):
         """
-        Run a Django management command, passing all arguments
+        Perform any final setup for this project after it has been imported:
 
-        Defaults to:
-            runserver 0:8000
+        * detect if it has been run directly; if so, register it as an app
+        * register the admin site
         """
+
         # Check if this is being called from click commands or directly
         if self.app_name not in sys.modules:
             # Hasn't been run through the ``nanodjango`` command
             if (
                 "__main__" not in sys.modules
                 or getattr(sys.modules["__main__"], self._instance_name) != self
             ):
                 # Doesn't look like it was run directly either
                 raise UsageError("App module not initialised")
 
             # Run directly, so register app module so Django won't try to load it again
             sys.modules[self.app_name] = sys.modules["__main__"]
 
+        # Register the admin site
+        admin_url = self.settings.ADMIN_URL
+        if admin_url or self.has_admin:
+            if admin_url is None:
+                admin_url = "admin/"
+            if not isinstance(admin_url, str) or not admin_url.endswith("/"):
+                raise ConfigurationError(
+                    "settings.ADMIN_URL must be a string path ending in /"
+                )
+            urlpatterns.append(
+                django_urls.path(admin_url.removeprefix("/"), admin.site.urls)
+            )
+
+    def run(self, args: list[str] | tuple[str] | None = None):
+        """
+        Run a Django management command, passing all arguments
+
+        Defaults to:
+            runserver 0:8000
+        """
         # Be helpful and check sys.argv for args. This will almost certainly be because
         # it's running directly.
         if args is None:
             args = sys.argv[1:]
 
         self._prepare()
-        from django.core.management import execute_from_command_line
+        if args:
+            exec_manage(*args)
+        else:
+            exec_manage("runserver", "0:8000")
+
+    def start(self, host: str | None = None):
+        """
+        Perform app setup commands and run the server
+        """
+        # Be helpful and check sys.argv for the host
+        if host is None:
+            print(sys.argv)
+            if len(sys.argv) > 2:
+                raise UsageError("Usage: start [HOST]")
+            elif len(sys.argv) == 2:
+                host = sys.argv[1]
+        if not host:
+            host = "0:8000"
 
-        if not args:
-            args = ["runserver", "0:8000"]
-        args = ["nanodjango"] + list(args)
-        execute_from_command_line(args)
+        self._prepare()
+        exec_manage("makemigrations", self.app_name)
+        exec_manage("migrate")
+        User = get_user_model()
+        if User.objects.count() == 0:
+            exec_manage("createsuperuser")
+        exec_manage("runserver", host)
 
     def convert(self, path: Path, name: str):
         from .convert import Converter
 
         if path.exists():
             raise UsageError("Upgrade path is not empty - path cannot exist")
         path.mkdir()
```

### Comparing `nanodjango-0.5.0/nanodjango/app_meta.py` & `nanodjango-0.6.0/nanodjango/app_meta.py`

 * *Files identical despite different names*

### Comparing `nanodjango-0.5.0/nanodjango/commands.py` & `nanodjango-0.6.0/nanodjango/commands.py`

 * *Files 12% similar despite different names*

```diff
@@ -64,19 +64,41 @@
     pass
 
 
 @cli.command()
 @click.argument("app", type=str, required=True, callback=load_app)
 @click.argument("args", type=str, required=False, nargs=-1)
 def run(app: Django, args: tuple[str]):
+    """
+    Run a management command.
+
+    If no command is specified, it will run runserver 0:8000
+    """
     app.run(args)
 
 
 @cli.command()
 @click.argument("app", type=str, required=True, callback=load_app)
+@click.argument("host", type=str, required=False, default="")
+def start(app: Django, host: str):
+    """
+    Start the app on the specified IP and port
+
+    This will perform a series of setup commands:
+
+        makemigrations <app>
+        migrate
+        createsuperuser
+        runserver HOST
+    """
+    app.start(host)
+
+
+@cli.command()
+@click.argument("app", type=str, required=True, callback=load_app)
 @click.argument("path", type=click.Path(), required=True)
 @click.option("--name", "-n", default="project", help="The project name")
 @click.option(
     "--delete",
     "can_delete",
     is_flag=True,
     default=False,
```

### Comparing `nanodjango-0.5.0/nanodjango/convert/contrib/django_ninja.py` & `nanodjango-0.6.0/nanodjango/convert/contrib/django_ninja.py`

 * *Files identical despite different names*

### Comparing `nanodjango-0.5.0/nanodjango/convert/converter.py` & `nanodjango-0.6.0/nanodjango/convert/converter.py`

 * *Files identical despite different names*

### Comparing `nanodjango-0.5.0/nanodjango/convert/objects.py` & `nanodjango-0.6.0/nanodjango/convert/objects.py`

 * *Files identical despite different names*

### Comparing `nanodjango-0.5.0/nanodjango/convert/plugin.py` & `nanodjango-0.6.0/nanodjango/convert/plugin.py`

 * *Files identical despite different names*

### Comparing `nanodjango-0.5.0/nanodjango/convert/reference.py` & `nanodjango-0.6.0/nanodjango/convert/reference.py`

 * *Files identical despite different names*

### Comparing `nanodjango-0.5.0/nanodjango/convert/utils.py` & `nanodjango-0.6.0/nanodjango/convert/utils.py`

 * *Files identical despite different names*

### Comparing `nanodjango-0.5.0/nanodjango/django_glue/apps.py` & `nanodjango-0.6.0/nanodjango/django_glue/apps.py`

 * *Files identical despite different names*

### Comparing `nanodjango-0.5.0/nanodjango/django_glue/db.py` & `nanodjango-0.6.0/nanodjango/django_glue/db.py`

 * *Files identical despite different names*

### Comparing `nanodjango-0.5.0/nanodjango/settings.py` & `nanodjango-0.6.0/nanodjango/settings.py`

 * *Files identical despite different names*

### Comparing `nanodjango-0.5.0/nanodjango.egg-info/PKG-INFO` & `nanodjango-0.6.0/nanodjango.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanodjango
-Version: 0.5.0
+Version: 0.6.0
 Summary: Run Django models and views from a single file, and convert it to a full project.
 Author-email: Richard Terry <code@radiac.net>
 Project-URL: Homepage, https://radiac.net/projects/nanodjango/
 Project-URL: Documentation, https://nanodjango.readthedocs.io/en/latest/
 Project-URL: Changelog, https://nanodjango.readthedocs.io/en/latest/changelog.html
 Project-URL: Repository, https://github.com/radiac/nanodjango
 Project-URL: Issues, https://github.com/radiac/nanodjango/issues
@@ -68,33 +68,32 @@
     CountLog.objects.create()
     return f"<p>Number of page loads: {CountLog.objects.count()}</p>"
 ```
 
 Save that as ``counter.py``, then set up your database and run it locally with:
 
 ```sh
-nanodjango run counter.py makemigrations counter
-nanodjango run counter.py migrate
-nanodjango run counter.py createsuperuser
-nanodjango run counter.py
+nanodjango start counter.py
 ```
 
 It will create your database in a ``db.sqlite3`` file next to your ``counter.py``, with
-the appropriate migrations in ``migrations/``.
+the appropriate migrations in ``migrations/``. Alternatively you could run each of these
+commands manually with the ``run`` command, eg
+``nanodjango run counter.py runserver 0:8000``
 
 Run it in production using WSGI:
 
 ```sh
 gunicorn -w 4 counter:app
 ```
 
 or automatically convert it to a full Django project:
 
 ```sh
-nanodjango counter.py convert /path/to/project --name=myproject
+nanodjango convert counter.py /path/to/project --name=myproject
 ```
 
 and with a [couple of extra
 lines](https://nanodjango.readthedocs.io/en/latest/management.html#run-script), run the
 development server as a standalone script using ``python``, or use ``pipx run`` to run
 it and automatically install dependencies to a temporary virtual environment:
```

### Comparing `nanodjango-0.5.0/nanodjango.egg-info/SOURCES.txt` & `nanodjango-0.6.0/nanodjango.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nanodjango-0.5.0/pyproject.toml` & `nanodjango-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nanodjango-0.5.0/tests/test_convert.py` & `nanodjango-0.6.0/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `nanodjango-0.5.0/tests/test_run_check.py` & `nanodjango-0.6.0/tests/test_run_check.py`

 * *Files identical despite different names*

### Comparing `nanodjango-0.5.0/tests/test_run_runserver.py` & `nanodjango-0.6.0/tests/test_run_runserver.py`

 * *Files identical despite different names*

