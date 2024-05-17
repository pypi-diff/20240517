# Comparing `tmp/wagtail-footnotes-0.8.1.tar.gz` & `tmp/wagtail-footnotes-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-footnotes-0.8.1.tar", last modified: Fri Jun 24 11:02:36 2022, max compression
+gzip compressed data, was "wagtail-footnotes-0.9.0.tar", last modified: Fri Oct 14 15:42:21 2022, max compression
```

## Comparing `wagtail-footnotes-0.8.1.tar` & `wagtail-footnotes-0.9.0.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2022-06-24 11:02:36.299810 wagtail-footnotes-0.8.1/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1264 2022-06-23 16:15:42.000000 wagtail-footnotes-0.8.1/CHANGELOG.md
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1070 2022-06-23 15:42:52.000000 wagtail-footnotes-0.8.1/LICENCE.txt
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      133 2022-06-23 15:42:52.000000 wagtail-footnotes-0.8.1/MANIFEST.in
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2187 2022-06-24 11:02:36.299810 wagtail-footnotes-0.8.1/PKG-INFO
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1824 2022-06-23 15:42:52.000000 wagtail-footnotes-0.8.1/README.md
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      579 2022-06-24 11:02:36.299810 wagtail-footnotes-0.8.1/setup.cfg
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      133 2022-06-23 16:15:42.000000 wagtail-footnotes-0.8.1/setup.py
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2022-06-24 11:02:36.299810 wagtail-footnotes-0.8.1/wagtail_footnotes/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)        0 2022-06-23 15:42:52.000000 wagtail-footnotes-0.8.1/wagtail_footnotes/__init__.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2723 2022-06-23 16:15:42.000000 wagtail-footnotes-0.8.1/wagtail_footnotes/blocks.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      254 2022-06-23 15:42:52.000000 wagtail-footnotes-0.8.1/wagtail_footnotes/fields.py
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2022-06-24 11:02:36.299810 wagtail-footnotes-0.8.1/wagtail_footnotes/migrations/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1621 2022-06-23 16:15:42.000000 wagtail-footnotes-0.8.1/wagtail_footnotes/migrations/0001_initial.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      779 2022-06-23 16:15:42.000000 wagtail-footnotes-0.8.1/wagtail_footnotes/migrations/0002_alter_footnote_unique_together.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)        0 2022-06-23 15:42:52.000000 wagtail-footnotes-0.8.1/wagtail_footnotes/migrations/__init__.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1265 2022-06-23 16:15:42.000000 wagtail-footnotes-0.8.1/wagtail_footnotes/models.py
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2022-06-24 11:02:36.299810 wagtail-footnotes-0.8.1/wagtail_footnotes/static/
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2022-06-24 11:02:36.299810 wagtail-footnotes-0.8.1/wagtail_footnotes/static/footnotes/
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2022-06-24 11:02:36.299810 wagtail-footnotes-0.8.1/wagtail_footnotes/static/footnotes/js/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3459 2022-06-23 15:42:52.000000 wagtail-footnotes-0.8.1/wagtail_footnotes/static/footnotes/js/footnotes.js
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2022-06-24 11:02:36.299810 wagtail-footnotes-0.8.1/wagtail_footnotes/templates/
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2022-06-24 11:02:36.299810 wagtail-footnotes-0.8.1/wagtail_footnotes/templates/wagtail_footnotes/
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2022-06-24 11:02:36.299810 wagtail-footnotes-0.8.1/wagtail_footnotes/templates/wagtail_footnotes/admin/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2122 2022-06-23 15:42:52.000000 wagtail-footnotes-0.8.1/wagtail_footnotes/templates/wagtail_footnotes/admin/footnotes_modal.html
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2022-06-24 11:02:36.299810 wagtail-footnotes-0.8.1/wagtail_footnotes/templates/wagtail_footnotes/includes/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      557 2022-06-23 15:42:52.000000 wagtail-footnotes-0.8.1/wagtail_footnotes/templates/wagtail_footnotes/includes/footnotes.html
--rw-rw-r--   0 kevin     (1000) kevin     (1000)       62 2022-06-23 15:42:52.000000 wagtail-footnotes-0.8.1/wagtail_footnotes/tests.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      284 2022-06-23 15:42:52.000000 wagtail-footnotes-0.8.1/wagtail_footnotes/urls.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2080 2022-06-23 16:15:42.000000 wagtail-footnotes-0.8.1/wagtail_footnotes/wagtail_hooks.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      833 2022-06-23 15:42:52.000000 wagtail-footnotes-0.8.1/wagtail_footnotes/widgets.py
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2022-06-24 11:02:36.299810 wagtail-footnotes-0.8.1/wagtail_footnotes.egg-info/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2187 2022-06-24 11:02:36.000000 wagtail-footnotes-0.8.1/wagtail_footnotes.egg-info/PKG-INFO
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      848 2022-06-24 11:02:36.000000 wagtail-footnotes-0.8.1/wagtail_footnotes.egg-info/SOURCES.txt
--rw-rw-r--   0 kevin     (1000) kevin     (1000)        1 2022-06-24 11:02:36.000000 wagtail-footnotes-0.8.1/wagtail_footnotes.egg-info/dependency_links.txt
--rw-rw-r--   0 kevin     (1000) kevin     (1000)       19 2022-06-24 11:02:36.000000 wagtail-footnotes-0.8.1/wagtail_footnotes.egg-info/requires.txt
--rw-rw-r--   0 kevin     (1000) kevin     (1000)       18 2022-06-24 11:02:36.000000 wagtail-footnotes-0.8.1/wagtail_footnotes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 15:42:21.745227 wagtail-footnotes-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1425 2022-10-14 15:42:17.000000 wagtail-footnotes-0.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-10-14 15:42:17.000000 wagtail-footnotes-0.9.0/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      133 2022-10-14 15:42:17.000000 wagtail-footnotes-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2622 2022-10-14 15:42:21.745227 wagtail-footnotes-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1824 2022-10-14 15:42:17.000000 wagtail-footnotes-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      579 2022-10-14 15:42:21.745227 wagtail-footnotes-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      133 2022-10-14 15:42:17.000000 wagtail-footnotes-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 15:42:21.745227 wagtail-footnotes-0.9.0/wagtail_footnotes/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-14 15:42:17.000000 wagtail-footnotes-0.9.0/wagtail_footnotes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2723 2022-10-14 15:42:17.000000 wagtail-footnotes-0.9.0/wagtail_footnotes/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (121)      254 2022-10-14 15:42:17.000000 wagtail-footnotes-0.9.0/wagtail_footnotes/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 15:42:21.745227 wagtail-footnotes-0.9.0/wagtail_footnotes/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)     1621 2022-10-14 15:42:17.000000 wagtail-footnotes-0.9.0/wagtail_footnotes/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)      779 2022-10-14 15:42:17.000000 wagtail-footnotes-0.9.0/wagtail_footnotes/migrations/0002_alter_footnote_unique_together.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-14 15:42:17.000000 wagtail-footnotes-0.9.0/wagtail_footnotes/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1265 2022-10-14 15:42:17.000000 wagtail-footnotes-0.9.0/wagtail_footnotes/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 15:42:21.745227 wagtail-footnotes-0.9.0/wagtail_footnotes/static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 15:42:21.745227 wagtail-footnotes-0.9.0/wagtail_footnotes/static/footnotes/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 15:42:21.745227 wagtail-footnotes-0.9.0/wagtail_footnotes/static/footnotes/js/
+-rw-r--r--   0 runner    (1001) docker     (121)     3484 2022-10-14 15:42:17.000000 wagtail-footnotes-0.9.0/wagtail_footnotes/static/footnotes/js/footnotes.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3447 2022-10-14 15:42:17.000000 wagtail-footnotes-0.9.0/wagtail_footnotes/static/footnotes/js/footnotes_legacy.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 15:42:21.745227 wagtail-footnotes-0.9.0/wagtail_footnotes/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 15:42:21.745227 wagtail-footnotes-0.9.0/wagtail_footnotes/templates/wagtail_footnotes/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 15:42:21.745227 wagtail-footnotes-0.9.0/wagtail_footnotes/templates/wagtail_footnotes/admin/
+-rw-r--r--   0 runner    (1001) docker     (121)     2360 2022-10-14 15:42:17.000000 wagtail-footnotes-0.9.0/wagtail_footnotes/templates/wagtail_footnotes/admin/footnotes_modal.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2122 2022-10-14 15:42:17.000000 wagtail-footnotes-0.9.0/wagtail_footnotes/templates/wagtail_footnotes/admin/footnotes_modal_legacy.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 15:42:21.745227 wagtail-footnotes-0.9.0/wagtail_footnotes/templates/wagtail_footnotes/includes/
+-rw-r--r--   0 runner    (1001) docker     (121)      557 2022-10-14 15:42:17.000000 wagtail-footnotes-0.9.0/wagtail_footnotes/templates/wagtail_footnotes/includes/footnotes.html
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-10-14 15:42:17.000000 wagtail-footnotes-0.9.0/wagtail_footnotes/tests.py
+-rw-r--r--   0 runner    (1001) docker     (121)      454 2022-10-14 15:42:17.000000 wagtail-footnotes-0.9.0/wagtail_footnotes/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2267 2022-10-14 15:42:17.000000 wagtail-footnotes-0.9.0/wagtail_footnotes/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (121)      833 2022-10-14 15:42:17.000000 wagtail-footnotes-0.9.0/wagtail_footnotes/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 15:42:21.745227 wagtail-footnotes-0.9.0/wagtail_footnotes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2622 2022-10-14 15:42:20.000000 wagtail-footnotes-0.9.0/wagtail_footnotes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      986 2022-10-14 15:42:21.000000 wagtail-footnotes-0.9.0/wagtail_footnotes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-14 15:42:20.000000 wagtail-footnotes-0.9.0/wagtail_footnotes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2022-10-14 15:42:20.000000 wagtail-footnotes-0.9.0/wagtail_footnotes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-10-14 15:42:20.000000 wagtail-footnotes-0.9.0/wagtail_footnotes.egg-info/top_level.txt
```

### Comparing `wagtail-footnotes-0.8.1/CHANGELOG.md` & `wagtail-footnotes-0.9.0/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Wagtail Footnotes Changelog
 
+## 0.9.0
+
+- Add support for Wagtail 4.0
+- Add GitHub Action to publish to PyPI on release by @zerolab in https://github.com/torchbox/wagtail-footnotes/pull/45
+
 ## 0.8.0
 
  - Add support for Wagtail 3.0 and drop support for all Wagtail versions
    before 2.15
  - Dropped support for all Django versions
    before 3.2
  - Removed support for Python 3.6
@@ -43,8 +48,8 @@
 
 ## 0.2.0
 
 - Moved templates to `wagtail_footnotes/templates/wagtail_footnotes/*`
 
 ## 0.1.0
 
-- Initial release of the Wagtail Footnotes package
+- Initial release of the Wagtail Footnotes package
```

### Comparing `wagtail-footnotes-0.8.1/LICENCE.txt` & `wagtail-footnotes-0.9.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `wagtail-footnotes-0.8.1/PKG-INFO` & `wagtail-footnotes-0.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,68 +1,66 @@
 Metadata-Version: 2.1
 Name: wagtail-footnotes
-Version: 0.8.1
+Version: 0.9.0
 Summary: Add footnotes to rich text in your Wagtail pages
 Home-page: https://github.com/torchbox/wagtail-footnotes
 Author: Cameron Lamb
 Author-email: cameron.lamb@torchbox.com
 License: UNKNOWN
+Description: # Wagtail Footnotes
+        
+        Add footnotes functionality to your Wagtail project.
+        
+        ## Usage
+         - Add the app to `INSTALLED_APPS`:
+           ```python
+           INSTALLED_APPS = [
+               ...
+               "wagtail_footnotes",
+               ...
+           ]
+           ```
+         - Add the footnotes `urls.py` to your project's `urls.py`:
+           ```python
+           from wagtail_footnotes import urls as footnotes_urls
+           urlpatterns = [
+               ...
+               path("footnotes/", include(footnotes_urls)),
+               ...
+           ]
+           ```
+           Note: The URL has to be defined as above as it is currently hardcoded in the Javascript.
+         - Update your page models to show the footnotes field:
+           ```python
+           class InformationPage(BasePage):
+                ...
+                content_panels = [
+                    ...
+                    InlinePanel("footnotes", label="Footnotes"),
+                ]
+           ```
+         - Update your `RichTextBlock`s 
+            - Add `"footnotes"` to the `features` arg for each `RichTextBlock` that you want to have this functionality
+            - You will also need to change any `RichTextBlock`s to `wagtail_footnotes.blocks.RichTextBlockWithFootnotes`
+         - Update your page templates to include `{% include "wagtail_footnotes/includes/footnotes.html" %}`
+         - Make and run migrations:
+           ```
+           ./manage.py makemigrations
+           ./manage.py migrate
+           ```
+        
+        ## Settings
+        
+         - `WAGTAIL_FOOTNOTES_TEXT_FEATURES`
+           - Default: `["bold", "italic", "link"]`
+           - Use this to update a list of Rich Text features allowed in the footnote text.
+        
+        ## Common issues
+         - I click on the `Fn` button in the editor and it stops working
+            - This is likely because the URL in the JS does not match the URL of the footnotes view. Check the URL in `wagtail_footnotes/static/footnotes/js/footnotes.js` matches the URL you set.
+         - `NoneType` error when rendering page.
+            - Make sure you are rendering the field in the template using `{% include_block page.field_name %}`
+        
 Keywords: wagtail,django
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-
-# Wagtail Footnotes
-
-Add footnotes functionality to your Wagtail project.
-
-## Usage
- - Add the app to `INSTALLED_APPS`:
-   ```python
-   INSTALLED_APPS = [
-       ...
-       "wagtail_footnotes",
-       ...
-   ]
-   ```
- - Add the footnotes `urls.py` to your project's `urls.py`:
-   ```python
-   from wagtail_footnotes import urls as footnotes_urls
-   urlpatterns = [
-       ...
-       path("footnotes/", include(footnotes_urls)),
-       ...
-   ]
-   ```
-   Note: The URL has to be defined as above as it is currently hardcoded in the Javascript.
- - Update your page models to show the footnotes field:
-   ```python
-   class InformationPage(BasePage):
-        ...
-        content_panels = [
-            ...
-            InlinePanel("footnotes", label="Footnotes"),
-        ]
-   ```
- - Update your `RichTextBlock`s 
-    - Add `"footnotes"` to the `features` arg for each `RichTextBlock` that you want to have this functionality
-    - You will also need to change any `RichTextBlock`s to `wagtail_footnotes.blocks.RichTextBlockWithFootnotes`
- - Update your page templates to include `{% include "wagtail_footnotes/includes/footnotes.html" %}`
- - Make and run migrations:
-   ```
-   ./manage.py makemigrations
-   ./manage.py migrate
-   ```
-
-## Settings
-
- - `WAGTAIL_FOOTNOTES_TEXT_FEATURES`
-   - Default: `["bold", "italic", "link"]`
-   - Use this to update a list of Rich Text features allowed in the footnote text.
-
-## Common issues
- - I click on the `Fn` button in the editor and it stops working
-    - This is likely because the URL in the JS does not match the URL of the footnotes view. Check the URL in `wagtail_footnotes/static/footnotes/js/footnotes.js` matches the URL you set.
- - `NoneType` error when rendering page.
-    - Make sure you are rendering the field in the template using `{% include_block page.field_name %}`
-
-
```

### Comparing `wagtail-footnotes-0.8.1/README.md` & `wagtail-footnotes-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-footnotes-0.8.1/setup.cfg` & `wagtail-footnotes-0.9.0/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = wagtail-footnotes
 author = Cameron Lamb
 author_email = cameron.lamb@torchbox.com
 description = Add footnotes to rich text in your Wagtail pages
-version = 0.8.1
+version = 0.9.0
 url = https://github.com/torchbox/wagtail-footnotes
 keywords = 
 	wagtail
 	django
 long_description = file:README.md
 long_description_content_type = text/markdown
 license_files = 
@@ -17,13 +17,13 @@
 python_requires = >= 3.7
 setup_requires = 
 	setuptools >= 40.6
 	pip >= 10
 include_package_data = true
 packages = find:
 install_requires = 
-	wagtail>=2.15, <4.0
+	wagtail>=2.15, <5.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `wagtail-footnotes-0.8.1/wagtail_footnotes/blocks.py` & `wagtail-footnotes-0.9.0/wagtail_footnotes/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-footnotes-0.8.1/wagtail_footnotes/migrations/0001_initial.py` & `wagtail-footnotes-0.9.0/wagtail_footnotes/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-footnotes-0.8.1/wagtail_footnotes/migrations/0002_alter_footnote_unique_together.py` & `wagtail-footnotes-0.9.0/wagtail_footnotes/migrations/0002_alter_footnote_unique_together.py`

 * *Files identical despite different names*

### Comparing `wagtail-footnotes-0.8.1/wagtail_footnotes/models.py` & `wagtail-footnotes-0.9.0/wagtail_footnotes/models.py`

 * *Files identical despite different names*

### Comparing `wagtail-footnotes-0.8.1/wagtail_footnotes/static/footnotes/js/footnotes.js` & `wagtail-footnotes-0.9.0/wagtail_footnotes/static/footnotes/js/footnotes_legacy.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: ASCII text*

 * *Files 0% similar despite different names*

```diff
@@ -94,124 +94,123 @@
 000005d0: 2020 2020 2020 2020 2076 6172 2075 7569           var uui
 000005e0: 6420 3d20 2428 2769 6e70 7574 5b69 642a  d = $('input[id*
 000005f0: 3d22 2d75 7569 6422 5d27 2c20 7661 6c75  ="-uuid"]', valu
 00000600: 6529 5b30 5d2e 7661 6c75 653b 0a20 2020  e)[0].value;.   
 00000610: 2020 2020 2020 2076 6172 2072 6f77 203d         var row =
 00000620: 2024 280a 2020 2020 2020 2020 2020 2020   $(.            
 00000630: 223c 7472 2064 6174 612d 7575 6964 3d22  "<tr data-uuid="
-00000640: 202b 0a20 2020 2020 2020 2020 2020 2020   +.             
-00000650: 2075 7569 6420 2b0a 2020 2020 2020 2020   uuid +.        
-00000660: 2020 2020 2020 223e 3c74 643e 2220 2b0a        "><td>" +.
-00000670: 2020 2020 2020 2020 2020 2020 2020 7465                te
-00000680: 7874 202b 0a20 2020 2020 2020 2020 2020  xt +.           
-00000690: 2020 2022 3c2f 7464 3e3c 7464 3e22 202b     "</td><td>" +
-000006a0: 0a20 2020 2020 2020 2020 2020 2020 2075  .              u
-000006b0: 7569 642e 7375 6273 7472 696e 6728 302c  uid.substring(0,
-000006c0: 2036 2920 2b0a 2020 2020 2020 2020 2020   6) +.          
-000006d0: 2020 2020 223c 2f74 643e 3c2f 7472 3e22      "</td></tr>"
-000006e0: 0a20 2020 2020 2020 2020 2029 2e63 7373  .          ).css
-000006f0: 287b 2063 7572 736f 723a 2022 706f 696e  ({ cursor: "poin
-00000700: 7465 7222 207d 293b 0a20 2020 2020 2020  ter" });.       
-00000710: 2020 2074 6162 6c65 2e61 7070 656e 6428     table.append(
-00000720: 726f 7729 3b0a 0a20 2020 2020 2020 2020  row);..         
-00000730: 2072 6f77 2e6f 6e28 2263 6c69 636b 222c   row.on("click",
-00000740: 2066 756e 6374 696f 6e20 2865 7665 6e74   function (event
-00000750: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
-00000760: 636f 6e73 7420 666f 6f74 6e6f 7465 5555  const footnoteUU
-00000770: 4944 203d 2065 7665 6e74 2e74 6172 6765  ID = event.targe
-00000780: 742e 7061 7265 6e74 456c 656d 656e 742e  t.parentElement.
-00000790: 6461 7461 7365 745b 2275 7569 6422 5d3b  dataset["uuid"];
-000007a0: 0a0a 2020 2020 2020 2020 2020 2020 2f2f  ..            //
-000007b0: 2055 7365 7320 7468 6520 4472 6166 742e   Uses the Draft.
-000007c0: 6a73 2041 5049 2074 6f20 6372 6561 7465  js API to create
-000007d0: 2061 206e 6577 2065 6e74 6974 7920 7769   a new entity wi
-000007e0: 7468 2074 6865 2072 6967 6874 2064 6174  th the right dat
-000007f0: 612e 0a20 2020 2020 2020 2020 2020 2063  a..            c
-00000800: 6f6e 7374 2063 6f6e 7465 6e74 5769 7468  onst contentWith
-00000810: 456e 7469 7479 203d 2063 6f6e 7465 6e74  Entity = content
-00000820: 2e63 7265 6174 6545 6e74 6974 7928 0a20  .createEntity(. 
-00000830: 2020 2020 2020 2020 2020 2020 2065 6e74               ent
-00000840: 6974 7954 7970 652e 7479 7065 2c0a 2020  ityType.type,.  
-00000850: 2020 2020 2020 2020 2020 2020 2249 4d4d              "IMM
-00000860: 5554 4142 4c45 222c 0a20 2020 2020 2020  UTABLE",.       
-00000870: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-00000880: 2020 2020 2020 2020 2066 6f6f 746e 6f74           footnot
-00000890: 653a 2066 6f6f 746e 6f74 6555 5549 442c  e: footnoteUUID,
-000008a0: 0a20 2020 2020 2020 2020 2020 2020 207d  .              }
-000008b0: 0a20 2020 2020 2020 2020 2020 2029 3b0a  .            );.
-000008c0: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
-000008d0: 7420 656e 7469 7479 4b65 7920 3d20 636f  t entityKey = co
-000008e0: 6e74 656e 7457 6974 6845 6e74 6974 792e  ntentWithEntity.
-000008f0: 6765 744c 6173 7443 7265 6174 6564 456e  getLastCreatedEn
-00000900: 7469 7479 4b65 7928 293b 0a0a 2020 2020  tityKey();..    
-00000910: 2020 2020 2020 2020 2f2f 2057 6520 616c          // We al
-00000920: 736f 2061 6464 2073 6f6d 6520 7465 7874  so add some text
-00000930: 2066 6f72 2074 6865 2065 6e74 6974 7920   for the entity 
-00000940: 746f 2062 6520 6163 7469 7661 7465 6420  to be activated 
-00000950: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
-00000960: 636f 6e73 7420 7368 6f72 744b 6579 203d  const shortKey =
-00000970: 2066 6f6f 746e 6f74 6555 5549 442e 7375   footnoteUUID.su
-00000980: 6273 7472 696e 6728 302c 2036 293b 0a20  bstring(0, 6);. 
-00000990: 2020 2020 2020 2020 2020 2063 6f6e 7374             const
-000009a0: 2074 6578 7420 3d20 605b 247b 7368 6f72   text = `[${shor
-000009b0: 744b 6579 7d5d 603b 0a0a 2020 2020 2020  tKey}]`;..      
-000009c0: 2020 2020 2020 636f 6e73 7420 6e65 7743        const newC
-000009d0: 6f6e 7465 6e74 203d 204d 6f64 6966 6965  ontent = Modifie
-000009e0: 722e 7265 706c 6163 6554 6578 7428 0a20  r.replaceText(. 
-000009f0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00000a00: 7465 6e74 2c0a 2020 2020 2020 2020 2020  tent,.          
-00000a10: 2020 2020 7365 6c65 6374 696f 6e2c 0a20      selection,. 
-00000a20: 2020 2020 2020 2020 2020 2020 2074 6578               tex
-00000a30: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
-00000a40: 206e 756c 6c2c 0a20 2020 2020 2020 2020   null,.         
-00000a50: 2020 2020 2065 6e74 6974 794b 6579 0a20       entityKey. 
-00000a60: 2020 2020 2020 2020 2020 2029 3b0a 2020             );.  
-00000a70: 2020 2020 2020 2020 2020 636f 6e73 7420            const 
-00000a80: 6e65 7874 5374 6174 6520 3d20 4564 6974  nextState = Edit
-00000a90: 6f72 5374 6174 652e 7075 7368 280a 2020  orState.push(.  
-00000aa0: 2020 2020 2020 2020 2020 2020 6564 6974              edit
-00000ab0: 6f72 5374 6174 652c 0a20 2020 2020 2020  orState,.       
-00000ac0: 2020 2020 2020 206e 6577 436f 6e74 656e         newConten
-00000ad0: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
-00000ae0: 2022 696e 7365 7274 2d63 6861 7261 6374   "insert-charact
-00000af0: 6572 7322 0a20 2020 2020 2020 2020 2020  ers".           
-00000b00: 2029 3b0a 0a20 2020 2020 2020 2020 2020   );..           
-00000b10: 206f 6e43 6f6d 706c 6574 6528 6e65 7874   onComplete(next
-00000b20: 5374 6174 6529 3b0a 0a20 2020 2020 2020  State);..       
-00000b30: 2020 2020 2024 2822 2366 6f6f 746e 6f74       $("#footnot
-00000b40: 6573 2d6d 6f64 616c 2229 2e6d 6f64 616c  es-modal").modal
-00000b50: 2822 6869 6465 2229 3b0a 2020 2020 2020  ("hide");.      
-00000b60: 2020 2020 7d29 3b0a 2020 2020 2020 2020      });.        
-00000b70: 7d29 3b0a 0a20 2020 2020 2020 2024 2822  });..        $("
-00000b80: 2366 6f6f 746e 6f74 6573 2d6d 6f64 616c  #footnotes-modal
-00000b90: 2229 2e6d 6f64 616c 2822 7368 6f77 2229  ").modal("show")
-00000ba0: 3b0a 2020 2020 2020 7d2c 0a20 2020 2020  ;.      },.     
-00000bb0: 2064 6174 6154 7970 653a 2022 6874 6d6c   dataType: "html
-00000bc0: 222c 0a20 2020 207d 293b 0a20 207d 0a0a  ",.    });.  }..
-00000bd0: 2020 6f6e 436c 6f73 6528 6529 207b 0a20    onClose(e) {. 
-00000be0: 2020 2063 6f6e 7374 207b 206f 6e43 6c6f     const { onClo
-00000bf0: 7365 207d 203d 2074 6869 732e 7072 6f70  se } = this.prop
-00000c00: 733b 0a20 2020 2065 2e70 7265 7665 6e74  s;.    e.prevent
-00000c10: 4465 6661 756c 7428 293b 0a20 2020 206f  Default();.    o
-00000c20: 6e43 6c6f 7365 2829 3b0a 2020 7d0a 0a20  nClose();.  }.. 
-00000c30: 2072 656e 6465 7228 2920 7b0a 2020 2020   render() {.    
-00000c40: 7265 7475 726e 206e 756c 6c3b 0a20 207d  return null;.  }
-00000c50: 0a7d 0a0a 636f 6e73 7420 466f 6f74 6e6f  .}..const Footno
-00000c60: 7465 203d 2028 7072 6f70 7329 203d 3e20  te = (props) => 
-00000c70: 7b0a 2020 636f 6e73 7420 7b20 656e 7469  {.  const { enti
-00000c80: 7479 4b65 792c 2063 6f6e 7465 6e74 5374  tyKey, contentSt
-00000c90: 6174 6520 7d20 3d20 7072 6f70 733b 0a20  ate } = props;. 
-00000ca0: 2063 6f6e 7374 2064 6174 6120 3d20 636f   const data = co
-00000cb0: 6e74 656e 7453 7461 7465 2e67 6574 456e  ntentState.getEn
-00000cc0: 7469 7479 2865 6e74 6974 794b 6579 292e  tity(entityKey).
-00000cd0: 6765 7444 6174 6128 293b 0a20 2072 6574  getData();.  ret
-00000ce0: 7572 6e20 5265 6163 742e 6372 6561 7465  urn React.create
-00000cf0: 456c 656d 656e 7428 2273 7570 222c 207b  Element("sup", {
-00000d00: 7d2c 2070 726f 7073 2e63 6869 6c64 7265  }, props.childre
-00000d10: 6e29 3b0a 7d3b 0a0a 7769 6e64 6f77 2e64  n);.};..window.d
-00000d20: 7261 6674 6169 6c2e 7265 6769 7374 6572  raftail.register
-00000d30: 506c 7567 696e 287b 0a20 2074 7970 653a  Plugin({.  type:
-00000d40: 2022 464f 4f54 4e4f 5445 5322 2c0a 2020   "FOOTNOTES",.  
-00000d50: 736f 7572 6365 3a20 466f 6f74 6e6f 7465  source: Footnote
-00000d60: 536f 7572 6365 2c0a 2020 6465 636f 7261  Source,.  decora
-00000d70: 746f 723a 2046 6f6f 746e 6f74 652c 0a7d  tor: Footnote,.}
-00000d80: 293b 0a                                  );.
+00000640: 202b 0a20 2020 2020 2020 2020 2020 2075   +.            u
+00000650: 7569 6420 2b0a 2020 2020 2020 2020 2020  uid +.          
+00000660: 2020 223e 3c74 643e 2220 2b0a 2020 2020    "><td>" +.    
+00000670: 2020 2020 2020 2020 7465 7874 202b 0a20          text +. 
+00000680: 2020 2020 2020 2020 2020 2022 3c2f 7464             "</td
+00000690: 3e3c 7464 3e22 202b 0a20 2020 2020 2020  ><td>" +.       
+000006a0: 2020 2020 2075 7569 642e 7375 6273 7472       uuid.substr
+000006b0: 696e 6728 302c 2036 2920 2b0a 2020 2020  ing(0, 6) +.    
+000006c0: 2020 2020 2020 2020 223c 2f74 643e 3c2f          "</td></
+000006d0: 7472 3e22 0a20 2020 2020 2020 2020 2029  tr>".          )
+000006e0: 2e63 7373 287b 2063 7572 736f 723a 2022  .css({ cursor: "
+000006f0: 706f 696e 7465 7222 207d 293b 0a20 2020  pointer" });.   
+00000700: 2020 2020 2020 2074 6162 6c65 2e61 7070         table.app
+00000710: 656e 6428 726f 7729 3b0a 0a20 2020 2020  end(row);..     
+00000720: 2020 2020 2072 6f77 2e6f 6e28 2263 6c69       row.on("cli
+00000730: 636b 222c 2066 756e 6374 696f 6e20 2865  ck", function (e
+00000740: 7665 6e74 2920 7b0a 2020 2020 2020 2020  vent) {.        
+00000750: 2020 2020 636f 6e73 7420 666f 6f74 6e6f      const footno
+00000760: 7465 5555 4944 203d 2065 7665 6e74 2e74  teUUID = event.t
+00000770: 6172 6765 742e 7061 7265 6e74 456c 656d  arget.parentElem
+00000780: 656e 742e 6461 7461 7365 745b 2275 7569  ent.dataset["uui
+00000790: 6422 5d3b 0a0a 2020 2020 2020 2020 2020  d"];..          
+000007a0: 2020 2f2f 2055 7365 7320 7468 6520 4472    // Uses the Dr
+000007b0: 6166 742e 6a73 2041 5049 2074 6f20 6372  aft.js API to cr
+000007c0: 6561 7465 2061 206e 6577 2065 6e74 6974  eate a new entit
+000007d0: 7920 7769 7468 2074 6865 2072 6967 6874  y with the right
+000007e0: 2064 6174 612e 0a20 2020 2020 2020 2020   data..         
+000007f0: 2020 2063 6f6e 7374 2063 6f6e 7465 6e74     const content
+00000800: 5769 7468 456e 7469 7479 203d 2063 6f6e  WithEntity = con
+00000810: 7465 6e74 2e63 7265 6174 6545 6e74 6974  tent.createEntit
+00000820: 7928 0a20 2020 2020 2020 2020 2020 2020  y(.             
+00000830: 2065 6e74 6974 7954 7970 652e 7479 7065   entityType.type
+00000840: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000850: 2249 4d4d 5554 4142 4c45 222c 0a20 2020  "IMMUTABLE",.   
+00000860: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
+00000870: 2020 2020 2020 2020 2020 2020 2066 6f6f               foo
+00000880: 746e 6f74 653a 2066 6f6f 746e 6f74 6555  tnote: footnoteU
+00000890: 5549 442c 0a20 2020 2020 2020 2020 2020  UID,.           
+000008a0: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
+000008b0: 2029 3b0a 2020 2020 2020 2020 2020 2020   );.            
+000008c0: 636f 6e73 7420 656e 7469 7479 4b65 7920  const entityKey 
+000008d0: 3d20 636f 6e74 656e 7457 6974 6845 6e74  = contentWithEnt
+000008e0: 6974 792e 6765 744c 6173 7443 7265 6174  ity.getLastCreat
+000008f0: 6564 456e 7469 7479 4b65 7928 293b 0a0a  edEntityKey();..
+00000900: 2020 2020 2020 2020 2020 2020 2f2f 2057              // W
+00000910: 6520 616c 736f 2061 6464 2073 6f6d 6520  e also add some 
+00000920: 7465 7874 2066 6f72 2074 6865 2065 6e74  text for the ent
+00000930: 6974 7920 746f 2062 6520 6163 7469 7661  ity to be activa
+00000940: 7465 6420 6f6e 2e0a 2020 2020 2020 2020  ted on..        
+00000950: 2020 2020 636f 6e73 7420 7368 6f72 744b      const shortK
+00000960: 6579 203d 2066 6f6f 746e 6f74 6555 5549  ey = footnoteUUI
+00000970: 442e 7375 6273 7472 696e 6728 302c 2036  D.substring(0, 6
+00000980: 293b 0a20 2020 2020 2020 2020 2020 2063  );.            c
+00000990: 6f6e 7374 2074 6578 7420 3d20 605b 247b  onst text = `[${
+000009a0: 7368 6f72 744b 6579 7d5d 603b 0a0a 2020  shortKey}]`;..  
+000009b0: 2020 2020 2020 2020 2020 636f 6e73 7420            const 
+000009c0: 6e65 7743 6f6e 7465 6e74 203d 204d 6f64  newContent = Mod
+000009d0: 6966 6965 722e 7265 706c 6163 6554 6578  ifier.replaceTex
+000009e0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+000009f0: 2063 6f6e 7465 6e74 2c0a 2020 2020 2020   content,.      
+00000a00: 2020 2020 2020 2020 7365 6c65 6374 696f          selectio
+00000a10: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
+00000a20: 2074 6578 742c 0a20 2020 2020 2020 2020   text,.         
+00000a30: 2020 2020 206e 756c 6c2c 0a20 2020 2020       null,.     
+00000a40: 2020 2020 2020 2020 2065 6e74 6974 794b           entityK
+00000a50: 6579 0a20 2020 2020 2020 2020 2020 2029  ey.            )
+00000a60: 3b0a 2020 2020 2020 2020 2020 2020 636f  ;.            co
+00000a70: 6e73 7420 6e65 7874 5374 6174 6520 3d20  nst nextState = 
+00000a80: 4564 6974 6f72 5374 6174 652e 7075 7368  EditorState.push
+00000a90: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00000aa0: 6564 6974 6f72 5374 6174 652c 0a20 2020  editorState,.   
+00000ab0: 2020 2020 2020 2020 2020 206e 6577 436f             newCo
+00000ac0: 6e74 656e 742c 0a20 2020 2020 2020 2020  ntent,.         
+00000ad0: 2020 2020 2022 696e 7365 7274 2d63 6861       "insert-cha
+00000ae0: 7261 6374 6572 7322 0a20 2020 2020 2020  racters".       
+00000af0: 2020 2020 2029 3b0a 0a20 2020 2020 2020       );..       
+00000b00: 2020 2020 206f 6e43 6f6d 706c 6574 6528       onComplete(
+00000b10: 6e65 7874 5374 6174 6529 3b0a 0a20 2020  nextState);..   
+00000b20: 2020 2020 2020 2020 2024 2822 2366 6f6f           $("#foo
+00000b30: 746e 6f74 6573 2d6d 6f64 616c 2229 2e6d  tnotes-modal").m
+00000b40: 6f64 616c 2822 6869 6465 2229 3b0a 2020  odal("hide");.  
+00000b50: 2020 2020 2020 2020 7d29 3b0a 2020 2020          });.    
+00000b60: 2020 2020 7d29 3b0a 0a20 2020 2020 2020      });..       
+00000b70: 2024 2822 2366 6f6f 746e 6f74 6573 2d6d   $("#footnotes-m
+00000b80: 6f64 616c 2229 2e6d 6f64 616c 2822 7368  odal").modal("sh
+00000b90: 6f77 2229 3b0a 2020 2020 2020 7d2c 0a20  ow");.      },. 
+00000ba0: 2020 2020 2064 6174 6154 7970 653a 2022       dataType: "
+00000bb0: 6874 6d6c 222c 0a20 2020 207d 293b 0a20  html",.    });. 
+00000bc0: 207d 0a0a 2020 6f6e 436c 6f73 6528 6529   }..  onClose(e)
+00000bd0: 207b 0a20 2020 2063 6f6e 7374 207b 206f   {.    const { o
+00000be0: 6e43 6c6f 7365 207d 203d 2074 6869 732e  nClose } = this.
+00000bf0: 7072 6f70 733b 0a20 2020 2065 2e70 7265  props;.    e.pre
+00000c00: 7665 6e74 4465 6661 756c 7428 293b 0a20  ventDefault();. 
+00000c10: 2020 206f 6e43 6c6f 7365 2829 3b0a 2020     onClose();.  
+00000c20: 7d0a 0a20 2072 656e 6465 7228 2920 7b0a  }..  render() {.
+00000c30: 2020 2020 7265 7475 726e 206e 756c 6c3b      return null;
+00000c40: 0a20 207d 0a7d 0a0a 636f 6e73 7420 466f  .  }.}..const Fo
+00000c50: 6f74 6e6f 7465 203d 2028 7072 6f70 7329  otnote = (props)
+00000c60: 203d 3e20 7b0a 2020 636f 6e73 7420 7b20   => {.  const { 
+00000c70: 656e 7469 7479 4b65 792c 2063 6f6e 7465  entityKey, conte
+00000c80: 6e74 5374 6174 6520 7d20 3d20 7072 6f70  ntState } = prop
+00000c90: 733b 0a20 2063 6f6e 7374 2064 6174 6120  s;.  const data 
+00000ca0: 3d20 636f 6e74 656e 7453 7461 7465 2e67  = contentState.g
+00000cb0: 6574 456e 7469 7479 2865 6e74 6974 794b  etEntity(entityK
+00000cc0: 6579 292e 6765 7444 6174 6128 293b 0a20  ey).getData();. 
+00000cd0: 2072 6574 7572 6e20 5265 6163 742e 6372   return React.cr
+00000ce0: 6561 7465 456c 656d 656e 7428 2273 7570  eateElement("sup
+00000cf0: 222c 207b 7d2c 2070 726f 7073 2e63 6869  ", {}, props.chi
+00000d00: 6c64 7265 6e29 3b0a 7d3b 0a0a 7769 6e64  ldren);.};..wind
+00000d10: 6f77 2e64 7261 6674 6169 6c2e 7265 6769  ow.draftail.regi
+00000d20: 7374 6572 506c 7567 696e 287b 0a20 2074  sterPlugin({.  t
+00000d30: 7970 653a 2022 464f 4f54 4e4f 5445 5322  ype: "FOOTNOTES"
+00000d40: 2c0a 2020 736f 7572 6365 3a20 466f 6f74  ,.  source: Foot
+00000d50: 6e6f 7465 536f 7572 6365 2c0a 2020 6465  noteSource,.  de
+00000d60: 636f 7261 746f 723a 2046 6f6f 746e 6f74  corator: Footnot
+00000d70: 652c 0a7d 293b 0a                        e,.});.
```

### Comparing `wagtail-footnotes-0.8.1/wagtail_footnotes/templates/wagtail_footnotes/admin/footnotes_modal.html` & `wagtail-footnotes-0.9.0/wagtail_footnotes/templates/wagtail_footnotes/admin/footnotes_modal_legacy.html`

 * *Files identical despite different names*

### Comparing `wagtail-footnotes-0.8.1/wagtail_footnotes/templates/wagtail_footnotes/includes/footnotes.html` & `wagtail-footnotes-0.9.0/wagtail_footnotes/templates/wagtail_footnotes/includes/footnotes.html`

 * *Files identical despite different names*

### Comparing `wagtail-footnotes-0.8.1/wagtail_footnotes/wagtail_hooks.py` & `wagtail-footnotes-0.9.0/wagtail_footnotes/wagtail_hooks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import wagtail.admin.rich_text.editors.draftail.features as draftail_features
 from django.templatetags.static import static
 from django.utils.html import format_html_join
 from draftjs_exporter.dom import DOM
+from wagtail import VERSION as WAGTAIL_VERSION
 from wagtail.admin.rich_text.converters.html_to_contentstate import \
     InlineEntityElementHandler
 
 try:
     from wagtail import hooks
 except ImportError:
     # Wagtail<3.0
@@ -20,20 +21,25 @@
     `<footnotes id="">short-id</footnotes>` tag.
     """
     feature_name = "footnotes"
     type_ = "FOOTNOTES"
 
     control = {"type": type_, "label": "Fn", "description": "Footnotes"}
 
+    if WAGTAIL_VERSION >= (4, 0):
+        footnotes_js = "footnotes/js/footnotes.js"
+    else:
+        footnotes_js = "footnotes/js/footnotes_legacy.js"
+
     features.register_editor_plugin(
         "draftail",
         feature_name,
         draftail_features.EntityFeature(
             control,
-            js = ['wagtailadmin/js/draftail.js', 'footnotes/js/footnotes.js']
+            js = ['wagtailadmin/js/draftail.js', footnotes_js],
         ),
     )
 
     features.register_converter_rule(
         "contentstate",
         feature_name,
         {
```

### Comparing `wagtail-footnotes-0.8.1/wagtail_footnotes/widgets.py` & `wagtail-footnotes-0.9.0/wagtail_footnotes/widgets.py`

 * *Files identical despite different names*

### Comparing `wagtail-footnotes-0.8.1/wagtail_footnotes.egg-info/PKG-INFO` & `wagtail-footnotes-0.9.0/wagtail_footnotes.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,68 +1,66 @@
 Metadata-Version: 2.1
 Name: wagtail-footnotes
-Version: 0.8.1
+Version: 0.9.0
 Summary: Add footnotes to rich text in your Wagtail pages
 Home-page: https://github.com/torchbox/wagtail-footnotes
 Author: Cameron Lamb
 Author-email: cameron.lamb@torchbox.com
 License: UNKNOWN
+Description: # Wagtail Footnotes
+        
+        Add footnotes functionality to your Wagtail project.
+        
+        ## Usage
+         - Add the app to `INSTALLED_APPS`:
+           ```python
+           INSTALLED_APPS = [
+               ...
+               "wagtail_footnotes",
+               ...
+           ]
+           ```
+         - Add the footnotes `urls.py` to your project's `urls.py`:
+           ```python
+           from wagtail_footnotes import urls as footnotes_urls
+           urlpatterns = [
+               ...
+               path("footnotes/", include(footnotes_urls)),
+               ...
+           ]
+           ```
+           Note: The URL has to be defined as above as it is currently hardcoded in the Javascript.
+         - Update your page models to show the footnotes field:
+           ```python
+           class InformationPage(BasePage):
+                ...
+                content_panels = [
+                    ...
+                    InlinePanel("footnotes", label="Footnotes"),
+                ]
+           ```
+         - Update your `RichTextBlock`s 
+            - Add `"footnotes"` to the `features` arg for each `RichTextBlock` that you want to have this functionality
+            - You will also need to change any `RichTextBlock`s to `wagtail_footnotes.blocks.RichTextBlockWithFootnotes`
+         - Update your page templates to include `{% include "wagtail_footnotes/includes/footnotes.html" %}`
+         - Make and run migrations:
+           ```
+           ./manage.py makemigrations
+           ./manage.py migrate
+           ```
+        
+        ## Settings
+        
+         - `WAGTAIL_FOOTNOTES_TEXT_FEATURES`
+           - Default: `["bold", "italic", "link"]`
+           - Use this to update a list of Rich Text features allowed in the footnote text.
+        
+        ## Common issues
+         - I click on the `Fn` button in the editor and it stops working
+            - This is likely because the URL in the JS does not match the URL of the footnotes view. Check the URL in `wagtail_footnotes/static/footnotes/js/footnotes.js` matches the URL you set.
+         - `NoneType` error when rendering page.
+            - Make sure you are rendering the field in the template using `{% include_block page.field_name %}`
+        
 Keywords: wagtail,django
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-
-# Wagtail Footnotes
-
-Add footnotes functionality to your Wagtail project.
-
-## Usage
- - Add the app to `INSTALLED_APPS`:
-   ```python
-   INSTALLED_APPS = [
-       ...
-       "wagtail_footnotes",
-       ...
-   ]
-   ```
- - Add the footnotes `urls.py` to your project's `urls.py`:
-   ```python
-   from wagtail_footnotes import urls as footnotes_urls
-   urlpatterns = [
-       ...
-       path("footnotes/", include(footnotes_urls)),
-       ...
-   ]
-   ```
-   Note: The URL has to be defined as above as it is currently hardcoded in the Javascript.
- - Update your page models to show the footnotes field:
-   ```python
-   class InformationPage(BasePage):
-        ...
-        content_panels = [
-            ...
-            InlinePanel("footnotes", label="Footnotes"),
-        ]
-   ```
- - Update your `RichTextBlock`s 
-    - Add `"footnotes"` to the `features` arg for each `RichTextBlock` that you want to have this functionality
-    - You will also need to change any `RichTextBlock`s to `wagtail_footnotes.blocks.RichTextBlockWithFootnotes`
- - Update your page templates to include `{% include "wagtail_footnotes/includes/footnotes.html" %}`
- - Make and run migrations:
-   ```
-   ./manage.py makemigrations
-   ./manage.py migrate
-   ```
-
-## Settings
-
- - `WAGTAIL_FOOTNOTES_TEXT_FEATURES`
-   - Default: `["bold", "italic", "link"]`
-   - Use this to update a list of Rich Text features allowed in the footnote text.
-
-## Common issues
- - I click on the `Fn` button in the editor and it stops working
-    - This is likely because the URL in the JS does not match the URL of the footnotes view. Check the URL in `wagtail_footnotes/static/footnotes/js/footnotes.js` matches the URL you set.
- - `NoneType` error when rendering page.
-    - Make sure you are rendering the field in the template using `{% include_block page.field_name %}`
-
-
```

### Comparing `wagtail-footnotes-0.8.1/wagtail_footnotes.egg-info/SOURCES.txt` & `wagtail-footnotes-0.9.0/wagtail_footnotes.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -17,9 +17,11 @@
 wagtail_footnotes.egg-info/dependency_links.txt
 wagtail_footnotes.egg-info/requires.txt
 wagtail_footnotes.egg-info/top_level.txt
 wagtail_footnotes/migrations/0001_initial.py
 wagtail_footnotes/migrations/0002_alter_footnote_unique_together.py
 wagtail_footnotes/migrations/__init__.py
 wagtail_footnotes/static/footnotes/js/footnotes.js
+wagtail_footnotes/static/footnotes/js/footnotes_legacy.js
 wagtail_footnotes/templates/wagtail_footnotes/admin/footnotes_modal.html
+wagtail_footnotes/templates/wagtail_footnotes/admin/footnotes_modal_legacy.html
 wagtail_footnotes/templates/wagtail_footnotes/includes/footnotes.html
```

