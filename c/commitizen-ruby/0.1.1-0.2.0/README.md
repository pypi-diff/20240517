# Comparing `tmp/commitizen_ruby-0.1.1.tar.gz` & `tmp/commitizen_ruby-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commitizen_ruby-0.1.1.tar", max compression
+gzip compressed data, was "commitizen_ruby-0.2.0.tar", max compression
```

## Comparing `commitizen_ruby-0.1.1.tar` & `commitizen_ruby-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1129 2024-05-14 16:35:27.959321 commitizen_ruby-0.1.1/LICENSE
--rw-r--r--   0        0        0     1649 2024-05-14 17:44:54.113173 commitizen_ruby-0.1.1/README.md
--rw-r--r--   0        0        0      952 2024-05-14 18:01:52.784973 commitizen_ruby-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-14 16:32:35.598176 commitizen_ruby-0.1.1/src/commitizen_ruby/__init__.py
--rw-r--r--   0        0        0     1628 2024-05-14 18:01:05.829702 commitizen_ruby-0.1.1/src/commitizen_ruby/ruby_version_provider.py
--rw-r--r--   0        0        0     2063 1970-01-01 00:00:00.000000 commitizen_ruby-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1129 2024-05-14 16:35:27.959321 commitizen_ruby-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1649 2024-05-14 17:44:54.113173 commitizen_ruby-0.2.0/README.md
+-rw-r--r--   0        0        0      952 2024-05-17 13:48:24.694720 commitizen_ruby-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-14 16:32:35.598176 commitizen_ruby-0.2.0/src/commitizen_ruby/__init__.py
+-rw-r--r--   0        0        0     1629 2024-05-17 13:46:20.556605 commitizen_ruby-0.2.0/src/commitizen_ruby/ruby_version_provider.py
+-rw-r--r--   0        0        0     2063 1970-01-01 00:00:00.000000 commitizen_ruby-0.2.0/PKG-INFO
```

### Comparing `commitizen_ruby-0.1.1/LICENSE` & `commitizen_ruby-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `commitizen_ruby-0.1.1/README.md` & `commitizen_ruby-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `commitizen_ruby-0.1.1/src/commitizen_ruby/ruby_version_provider.py` & `commitizen_ruby-0.2.0/src/commitizen_ruby/ruby_version_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
         if 'commitizen_ruby' in config._settings:
             self.config = always_merger.merge(self.config, config._settings['commitizen_ruby'])
 
         if self.config['file']:
             self.file = Path(self.config['file'])
         else:
-            for file in Path().glob("lib/*/version.rb"):
+            for file in Path().glob("lib/**/version.rb"):
                 self.file = file
                 break
 
         if self.file == None:
             raise InvalidConfigurationError(f"Can't determine version file and no file path is set in config.")
```

### Comparing `commitizen_ruby-0.1.1/PKG-INFO` & `commitizen_ruby-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commitizen-ruby
-Version: 0.1.1
+Version: 0.2.0
 Summary: Commitizen version provider for Ruby gems/projects.
 Author: Karsten Silkenbäumer
 Author-email: 993392+kassi@users.noreply.github.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: deepmerge (>=1.1.1,<2.0.0)
```

