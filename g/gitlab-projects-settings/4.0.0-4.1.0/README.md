# Comparing `tmp/gitlab_projects_settings-4.0.0.tar.gz` & `tmp/gitlab_projects_settings-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab_projects_settings-4.0.0.tar", last modified: Wed May 15 00:04:27 2024, max compression
+gzip compressed data, was "gitlab_projects_settings-4.1.0.tar", last modified: Fri May 17 02:44:43 2024, max compression
```

## Comparing `gitlab_projects_settings-4.0.0.tar` & `gitlab_projects_settings-4.1.0.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:27.672427 gitlab_projects_settings-4.0.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:27.661428 gitlab_projects_settings-4.0.0/.chglog/
--rwxrwxrwx   0 root         (0) root         (0)      649 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/.chglog/CHANGELOG.tpl.md
--rw-rw-rw-   0 root         (0) root         (0)      759 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/.chglog/changelog.sh
--rwxrwxrwx   0 root         (0) root         (0)      703 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/.chglog/config.yml
--rw-rw-rw-   0 root         (0) root         (0)      137 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)    11981 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/.markdownlint.json
--rw-rw-rw-   0 root         (0) root         (0)     1505 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/.style.yapf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:27.662428 gitlab_projects_settings-4.0.0/.vscode/
--rw-rw-rw-   0 root         (0) root         (0)      675 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/.vscode/extensions.json
--rw-rw-rw-   0 root         (0) root         (0)     1252 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/.vscode/settings.json
--rw-rw-rw-   0 root         (0) root         (0)     5064 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7311 2024-05-15 00:04:27.671427 gitlab_projects_settings-4.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5664 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:27.671427 gitlab_projects_settings-4.0.0/gitlab_projects_settings.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7311 2024-05-15 00:04:27.000000 gitlab_projects_settings-4.0.0/gitlab_projects_settings.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1054 2024-05-15 00:04:27.000000 gitlab_projects_settings-4.0.0/gitlab_projects_settings.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 00:04:27.000000 gitlab_projects_settings-4.0.0/gitlab_projects_settings.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2024-05-15 00:04:27.000000 gitlab_projects_settings-4.0.0/gitlab_projects_settings.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-05-15 00:04:27.000000 gitlab_projects_settings-4.0.0/gitlab_projects_settings.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-05-15 00:04:27.000000 gitlab_projects_settings-4.0.0/gitlab_projects_settings.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      425 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/mypy.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:27.665428 gitlab_projects_settings-4.0.0/requirements/
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/requirements/build.txt
--rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/requirements/deploy.txt
--rw-rw-rw-   0 root         (0) root         (0)       75 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/requirements/quality.txt
--rw-rw-rw-   0 root         (0) root         (0)       78 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/requirements/runtime.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 00:04:27.672427 gitlab_projects_settings-4.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2868 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:27.665428 gitlab_projects_settings-4.0.0/src/
--rw-rw-rw-   0 root         (0) root         (0)      143 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      115 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:27.666427 gitlab_projects_settings-4.0.0/src/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16950 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/cli/entrypoint.py
--rwxrwxrwx   0 root         (0) root         (0)     8980 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/cli/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:27.667427 gitlab_projects_settings-4.0.0/src/features/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/features/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14733 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/features/gitlab.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:27.668428 gitlab_projects_settings-4.0.0/src/package/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      754 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/package/bundle.py
--rw-rw-rw-   0 root         (0) root         (0)     3810 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/package/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     6845 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/package/updates.py
--rw-rw-rw-   0 root         (0) root         (0)     1607 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/package/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:27.669427 gitlab_projects_settings-4.0.0/src/prints/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/prints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2549 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/prints/boxes.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/prints/colors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:27.669427 gitlab_projects_settings-4.0.0/src/system/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/system/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1788 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/system/platform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:04:27.670427 gitlab_projects_settings-4.0.0/src/types/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11270 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/types/gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)      728 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/types/namespaces.py
--rw-rw-rw-   0 root         (0) root         (0)     3849 2024-05-15 00:04:23.000000 gitlab_projects_settings-4.0.0/src/types/strings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:43.090166 gitlab_projects_settings-4.1.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:43.080166 gitlab_projects_settings-4.1.0/.chglog/
+-rwxrwxrwx   0 root         (0) root         (0)      649 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/.chglog/CHANGELOG.tpl.md
+-rw-rw-rw-   0 root         (0) root         (0)      759 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/.chglog/changelog.sh
+-rwxrwxrwx   0 root         (0) root         (0)      703 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/.chglog/config.yml
+-rw-rw-rw-   0 root         (0) root         (0)      137 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)    11981 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/.markdownlint.json
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/.style.yapf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:43.080166 gitlab_projects_settings-4.1.0/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      675 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/.vscode/extensions.json
+-rw-rw-rw-   0 root         (0) root         (0)     1252 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/.vscode/settings.json
+-rw-rw-rw-   0 root         (0) root         (0)     5380 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7748 2024-05-17 02:44:43.090166 gitlab_projects_settings-4.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6067 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:43.089166 gitlab_projects_settings-4.1.0/gitlab_projects_settings.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7748 2024-05-17 02:44:43.000000 gitlab_projects_settings-4.1.0/gitlab_projects_settings.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1075 2024-05-17 02:44:43.000000 gitlab_projects_settings-4.1.0/gitlab_projects_settings.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 02:44:43.000000 gitlab_projects_settings-4.1.0/gitlab_projects_settings.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2024-05-17 02:44:43.000000 gitlab_projects_settings-4.1.0/gitlab_projects_settings.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       97 2024-05-17 02:44:43.000000 gitlab_projects_settings-4.1.0/gitlab_projects_settings.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-17 02:44:43.000000 gitlab_projects_settings-4.1.0/gitlab_projects_settings.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      425 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/mypy.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:43.083166 gitlab_projects_settings-4.1.0/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/requirements/build.txt
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/requirements/deploy.txt
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/requirements/quality.txt
+-rw-rw-rw-   0 root         (0) root         (0)       97 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/requirements/runtime.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 02:44:43.090166 gitlab_projects_settings-4.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2868 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:43.084167 gitlab_projects_settings-4.1.0/src/
+-rw-rw-rw-   0 root         (0) root         (0)      143 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      115 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:43.085167 gitlab_projects_settings-4.1.0/src/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18062 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/cli/entrypoint.py
+-rwxrwxrwx   0 root         (0) root         (0)     9111 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/cli/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:43.085167 gitlab_projects_settings-4.1.0/src/features/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/features/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14811 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/features/gitlab.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:43.086166 gitlab_projects_settings-4.1.0/src/package/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/package/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      754 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/package/bundle.py
+-rw-rw-rw-   0 root         (0) root         (0)     3810 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/package/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     6845 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/package/updates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1607 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/package/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:43.087166 gitlab_projects_settings-4.1.0/src/prints/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/prints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2549 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/prints/boxes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/prints/colors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1565 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/prints/themes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:43.088167 gitlab_projects_settings-4.1.0/src/system/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/system/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1788 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/system/platform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:43.089166 gitlab_projects_settings-4.1.0/src/types/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11789 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/types/gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)      728 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/types/namespaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     3849 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/types/strings.py
```

### Comparing `gitlab_projects_settings-4.0.0/.chglog/CHANGELOG.tpl.md` & `gitlab_projects_settings-4.1.0/.chglog/CHANGELOG.tpl.md`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.0.0/.chglog/changelog.sh` & `gitlab_projects_settings-4.1.0/.chglog/changelog.sh`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.0.0/.chglog/config.yml` & `gitlab_projects_settings-4.1.0/.chglog/config.yml`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.0.0/.gitlab-ci.yml` & `gitlab_projects_settings-4.1.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.0.0/.style.yapf` & `gitlab_projects_settings-4.1.0/.style.yapf`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.0.0/.vscode/extensions.json` & `gitlab_projects_settings-4.1.0/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.0.0/.vscode/settings.json` & `gitlab_projects_settings-4.1.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.0.0/CHANGELOG.md` & `gitlab_projects_settings-4.1.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,18 @@
 
+<a name="4.1.0"></a>
+## [4.1.0](https://gitlab.com/AdrianDC/gitlab-projects-settings/compare/4.0.0...4.1.0) (2024-05-17)
+
+### Features
+
+* **entrypoint:** implement prompt confirmation upon deletions
+* **gitlab:** isolate 'ProtectionLevels' enumeration
+* **requirements:** prepare 'questionary' library integration
+
+
 <a name="4.0.0"></a>
 ## [4.0.0](https://gitlab.com/AdrianDC/gitlab-projects-settings/compare/3.0.0...4.0.0) (2024-05-15)
 
 ### Bug Fixes
 
 * **entrypoint:** refactor to return no error upon final actions
 * **entrypoint:** avoid missing 'namespace_id' in 'User' responses
```

### Comparing `gitlab_projects_settings-4.0.0/LICENSE` & `gitlab_projects_settings-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.0.0/PKG-INFO` & `gitlab_projects_settings-4.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-projects-settings
-Version: 4.0.0
+Version: 4.1.0
 Summary: Configure GitLab groups and projects settings automatically
 Home-page: https://gitlab.com/AdrianDC/gitlab-projects-settings
 Author: Adrian DC
 Author-email: radian.dc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://gitlab.com/AdrianDC/gitlab-projects-settings/-/issues
 Project-URL: Changelog, https://gitlab.com/AdrianDC/gitlab-projects-settings/blob/main/CHANGELOG.md
@@ -26,14 +26,15 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Requires-Python: >=3, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: colored>=1.4.2
 Requires-Dist: python-gitlab>=4.4.0
+Requires-Dist: questionary>=2.0.1
 Requires-Dist: setuptools>=45.1.0
 Requires-Dist: update_checker>=0.18.0
 
 # gitlab-projects-settings
 
 <!-- markdownlint-disable no-inline-html -->
 
@@ -65,15 +66,15 @@
 ```yaml
 usage: gitlab-projects-settings [-h] [--version] [--update-check] [--settings] [--set GROUP KEY VAL] [-t TOKEN]
                                 [--dry-run] [--exclude-group] [--exclude-subgroups] [--exclude-projects]
                                 [--available-features] [--reset-features [KEEP_FEATURES]]
                                 [--disable-features FEATURES] [--enable-features FEATURES] [--reset-members]
                                 [--set-avatar FILE] [--set-description TEXT] [--update-description]
                                 [--run-housekeeping] [--archive-project | --unarchive-project] [--delete-group]
-                                [--delete-project] [--protect-branches] [--protect-tags LEVEL] [--]
+                                [--delete-project] [--protect-branches] [--protect-tags [LEVEL]] [--]
                                 [gitlab] [path]
 
 gitlab-projects-settings: Configure GitLab groups and projects settings automatically
 
 internal arguments:
   -h, --help                        # Show this help message
   --version                         # Show the current version
@@ -107,15 +108,15 @@
   --archive-project                 # Archive project or projects in GitLab groups
   --unarchive-project               # Unarchive project or projects in GitLab groups
   --delete-group                    # Delete group or groups in GitLab groups
   --delete-project                  # Delete project or projects in GitLab groups
 
 repository settings arguments:
   --protect-branches                # Protect branches with default master/main, develop and staging
-  --protect-tags LEVEL              # Protect tags at level [no-one,admins,maintainers,developers]
+  --protect-tags [LEVEL]            # Protect tags at level [no-one,admins,maintainers,developers] (default: no-one)
 
 positional arguments:
   --                                # Positional arguments separator (recommended)
   gitlab                            # GitLab URL (default: https://gitlab.com)
   path                              # GitLab group, user namespace or project path
 ```
 
@@ -134,18 +135,28 @@
 
 ```bash
 gitlab-projects-settings --settings
 ```
 
 ---
 
+## Environment available configurations
+
+`gitlab-projects-settings` uses `colored` for colors outputs and `questionary` for interactive menus.
+
+If colors of both outputs types do not match the terminal's theme,  
+an environment variable `NO_COLOR=1` can be defined to disable colors.
+
+---
+
 ## Dependencies
 
 - [colored](https://pypi.org/project/colored/): Terminal colors and styles
 - [python-gitlab](https://pypi.org/project/python-gitlab/): A python wrapper for the GitLab API
+- [questionary](https://pypi.org/project/questionary/): Interactive terminal user interfaces
 - [setuptools](https://pypi.org/project/setuptools/): Build and manage Python packages
 - [update-checker](https://pypi.org/project/update-checker/): Check for package updates on PyPI
 
 ---
 
 ## References
```

### Comparing `gitlab_projects_settings-4.0.0/README.md` & `gitlab_projects_settings-4.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 ```yaml
 usage: gitlab-projects-settings [-h] [--version] [--update-check] [--settings] [--set GROUP KEY VAL] [-t TOKEN]
                                 [--dry-run] [--exclude-group] [--exclude-subgroups] [--exclude-projects]
                                 [--available-features] [--reset-features [KEEP_FEATURES]]
                                 [--disable-features FEATURES] [--enable-features FEATURES] [--reset-members]
                                 [--set-avatar FILE] [--set-description TEXT] [--update-description]
                                 [--run-housekeeping] [--archive-project | --unarchive-project] [--delete-group]
-                                [--delete-project] [--protect-branches] [--protect-tags LEVEL] [--]
+                                [--delete-project] [--protect-branches] [--protect-tags [LEVEL]] [--]
                                 [gitlab] [path]
 
 gitlab-projects-settings: Configure GitLab groups and projects settings automatically
 
 internal arguments:
   -h, --help                        # Show this help message
   --version                         # Show the current version
@@ -72,15 +72,15 @@
   --archive-project                 # Archive project or projects in GitLab groups
   --unarchive-project               # Unarchive project or projects in GitLab groups
   --delete-group                    # Delete group or groups in GitLab groups
   --delete-project                  # Delete project or projects in GitLab groups
 
 repository settings arguments:
   --protect-branches                # Protect branches with default master/main, develop and staging
-  --protect-tags LEVEL              # Protect tags at level [no-one,admins,maintainers,developers]
+  --protect-tags [LEVEL]            # Protect tags at level [no-one,admins,maintainers,developers] (default: no-one)
 
 positional arguments:
   --                                # Positional arguments separator (recommended)
   gitlab                            # GitLab URL (default: https://gitlab.com)
   path                              # GitLab group, user namespace or project path
 ```
 
@@ -99,18 +99,28 @@
 
 ```bash
 gitlab-projects-settings --settings
 ```
 
 ---
 
+## Environment available configurations
+
+`gitlab-projects-settings` uses `colored` for colors outputs and `questionary` for interactive menus.
+
+If colors of both outputs types do not match the terminal's theme,  
+an environment variable `NO_COLOR=1` can be defined to disable colors.
+
+---
+
 ## Dependencies
 
 - [colored](https://pypi.org/project/colored/): Terminal colors and styles
 - [python-gitlab](https://pypi.org/project/python-gitlab/): A python wrapper for the GitLab API
+- [questionary](https://pypi.org/project/questionary/): Interactive terminal user interfaces
 - [setuptools](https://pypi.org/project/setuptools/): Build and manage Python packages
 - [update-checker](https://pypi.org/project/update-checker/): Check for package updates on PyPI
 
 ---
 
 ## References
```

### Comparing `gitlab_projects_settings-4.0.0/gitlab_projects_settings.egg-info/PKG-INFO` & `gitlab_projects_settings-4.1.0/gitlab_projects_settings.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-projects-settings
-Version: 4.0.0
+Version: 4.1.0
 Summary: Configure GitLab groups and projects settings automatically
 Home-page: https://gitlab.com/AdrianDC/gitlab-projects-settings
 Author: Adrian DC
 Author-email: radian.dc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://gitlab.com/AdrianDC/gitlab-projects-settings/-/issues
 Project-URL: Changelog, https://gitlab.com/AdrianDC/gitlab-projects-settings/blob/main/CHANGELOG.md
@@ -26,14 +26,15 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Requires-Python: >=3, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: colored>=1.4.2
 Requires-Dist: python-gitlab>=4.4.0
+Requires-Dist: questionary>=2.0.1
 Requires-Dist: setuptools>=45.1.0
 Requires-Dist: update_checker>=0.18.0
 
 # gitlab-projects-settings
 
 <!-- markdownlint-disable no-inline-html -->
 
@@ -65,15 +66,15 @@
 ```yaml
 usage: gitlab-projects-settings [-h] [--version] [--update-check] [--settings] [--set GROUP KEY VAL] [-t TOKEN]
                                 [--dry-run] [--exclude-group] [--exclude-subgroups] [--exclude-projects]
                                 [--available-features] [--reset-features [KEEP_FEATURES]]
                                 [--disable-features FEATURES] [--enable-features FEATURES] [--reset-members]
                                 [--set-avatar FILE] [--set-description TEXT] [--update-description]
                                 [--run-housekeeping] [--archive-project | --unarchive-project] [--delete-group]
-                                [--delete-project] [--protect-branches] [--protect-tags LEVEL] [--]
+                                [--delete-project] [--protect-branches] [--protect-tags [LEVEL]] [--]
                                 [gitlab] [path]
 
 gitlab-projects-settings: Configure GitLab groups and projects settings automatically
 
 internal arguments:
   -h, --help                        # Show this help message
   --version                         # Show the current version
@@ -107,15 +108,15 @@
   --archive-project                 # Archive project or projects in GitLab groups
   --unarchive-project               # Unarchive project or projects in GitLab groups
   --delete-group                    # Delete group or groups in GitLab groups
   --delete-project                  # Delete project or projects in GitLab groups
 
 repository settings arguments:
   --protect-branches                # Protect branches with default master/main, develop and staging
-  --protect-tags LEVEL              # Protect tags at level [no-one,admins,maintainers,developers]
+  --protect-tags [LEVEL]            # Protect tags at level [no-one,admins,maintainers,developers] (default: no-one)
 
 positional arguments:
   --                                # Positional arguments separator (recommended)
   gitlab                            # GitLab URL (default: https://gitlab.com)
   path                              # GitLab group, user namespace or project path
 ```
 
@@ -134,18 +135,28 @@
 
 ```bash
 gitlab-projects-settings --settings
 ```
 
 ---
 
+## Environment available configurations
+
+`gitlab-projects-settings` uses `colored` for colors outputs and `questionary` for interactive menus.
+
+If colors of both outputs types do not match the terminal's theme,  
+an environment variable `NO_COLOR=1` can be defined to disable colors.
+
+---
+
 ## Dependencies
 
 - [colored](https://pypi.org/project/colored/): Terminal colors and styles
 - [python-gitlab](https://pypi.org/project/python-gitlab/): A python wrapper for the GitLab API
+- [questionary](https://pypi.org/project/questionary/): Interactive terminal user interfaces
 - [setuptools](https://pypi.org/project/setuptools/): Build and manage Python packages
 - [update-checker](https://pypi.org/project/update-checker/): Check for package updates on PyPI
 
 ---
 
 ## References
```

### Comparing `gitlab_projects_settings-4.0.0/gitlab_projects_settings.egg-info/SOURCES.txt` & `gitlab_projects_settings-4.1.0/gitlab_projects_settings.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -33,13 +33,14 @@
 src/package/bundle.py
 src/package/settings.py
 src/package/updates.py
 src/package/version.py
 src/prints/__init__.py
 src/prints/boxes.py
 src/prints/colors.py
+src/prints/themes.py
 src/system/__init__.py
 src/system/platform.py
 src/types/__init__.py
 src/types/gitlab.py
 src/types/namespaces.py
 src/types/strings.py
```

### Comparing `gitlab_projects_settings-4.0.0/setup.py` & `gitlab_projects_settings-4.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.0.0/src/cli/entrypoint.py` & `gitlab_projects_settings-4.1.0/src/cli/entrypoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,20 @@
 # Modules libraries
 from gitlab.exceptions import GitlabGetError
 from gitlab.v4.objects import (
     Group as GitLabGroup,
     Project as GitLabProject,
     User as GitLabUser,
 )
+import questionary
 
 # Components
 from ..features.gitlab import GitLabFeature
 from ..prints.colors import Colors
+from ..prints.themes import Themes
 from ..system.platform import Platform
 from ..types.namespaces import Namespaces
 
 # Entrypoint class, pylint: disable=too-few-public-methods
 class Entrypoint:
 
     # Enumerations
@@ -169,14 +171,38 @@
                     )
                     if result in [Entrypoint.Result.FINALIZE, Entrypoint.Result.ERROR]:
                         return result
 
         # Result
         return Entrypoint.Result.SUCCESS
 
+    # Confirm
+    @staticmethod
+    def confirm(description: str, text: str = '') -> bool:
+
+        # Header
+        print(
+            f'{Colors.BOLD}   - Delete {description}: Confirm "'
+            f'{Colors.RED}{text}'
+            f'{Colors.BOLD}" deletion:'
+            f'{Colors.RESET}', end='')
+        Platform.flush()
+
+        # Get user configuration
+        answer: bool = questionary.confirm(
+            message='',
+            default=False,
+            qmark='',
+            style=Themes.confirmation_style(),
+            auto_enter=True,
+        ).ask()
+
+        # Result
+        return answer
+
     # Group
     @staticmethod
     def group(
         options: Namespace,
         gitlab: GitLabFeature,
         criteria: str,
         subgroup: bool = False,
@@ -201,16 +227,23 @@
         group_type = 'subgroup' if subgroup else 'group'
         print(f'{Colors.BOLD} - GitLab {group_type}: '
               f'{Colors.YELLOW_LIGHT}{group.full_path} '
               f'{Colors.CYAN}({group.description})'
               f'{Colors.RESET}')
         Platform.flush()
 
-        # Delete group
+        # Delete group after validation
         if options.delete_group:
+            if not Entrypoint.confirm(
+                    group_type,
+                    group.full_path,
+            ):
+                return Entrypoint.Result.SUCCESS
+
+            # Delete group
             gitlab.group_delete(criteria)
             print(f'{Colors.BOLD}   - Delete {group_type}: '
                   f'{Colors.GREEN}Success'
                   f'{Colors.RESET}')
             print(' ')
             Platform.flush()
             return Entrypoint.Result.SUCCESS if subgroup else Entrypoint.Result.FINALIZE
@@ -285,16 +318,23 @@
         # Show project details
         print(f'{Colors.BOLD} - GitLab project: '
               f'{Colors.YELLOW_LIGHT}{project.path_with_namespace} '
               f'{Colors.CYAN}({project.description})'
               f'{Colors.RESET}')
         Platform.flush()
 
-        # Delete project
+        # Delete project after validation
         if options.delete_project:
+            if not Entrypoint.confirm(
+                    'project',
+                    project.path_with_namespace,
+            ):
+                return Entrypoint.Result.SUCCESS
+
+            # Delete project
             gitlab.project_delete(criteria)
             print(f'{Colors.BOLD}   - Delete project: '
                   f'{Colors.GREEN}Success'
                   f'{Colors.RESET}')
             print(' ')
             Platform.flush()
             return Entrypoint.Result.SUCCESS
```

### Comparing `gitlab_projects_settings-4.0.0/src/cli/main.py` & `gitlab_projects_settings-4.1.0/src/cli/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # Components
 from ..package.bundle import Bundle
 from ..package.settings import Settings
 from ..package.updates import Updates
 from ..package.version import Version
 from ..prints.colors import Colors
 from ..system.platform import Platform
+from ..types.gitlab import ProtectionLevels
 from .entrypoint import Entrypoint
 
 # Main, pylint: disable=too-many-statements
 def main() -> None:
 
     # Variables
     group: _ArgumentGroup
@@ -212,15 +213,18 @@
         help='Protect branches with default master/main, develop and staging',
     )
     group.add_argument(
         '--protect-tags',
         dest='protect_tags',
         action='store',
         metavar='LEVEL',
-        help='Protect tags at level [no-one,admins,maintainers,developers]',
+        nargs='?',
+        const=ProtectionLevels.default(),
+        help=f'Protect tags at level [{",".join(ProtectionLevels.names())}]'
+        ' (default: %(const)s)',
     )
 
     # Arguments positional definitions
     group = parser.add_argument_group('positional arguments')
     group.add_argument(
         '--',
         dest='double_dash',
@@ -228,15 +232,15 @@
         help='Positional arguments separator (recommended)',
     )
     group.add_argument(
         dest='gitlab',
         action='store',
         nargs='?',
         default='https://gitlab.com',
-        help='GitLab URL (default: https://gitlab.com)',
+        help='GitLab URL (default: %(default)s)',
     )
     group.add_argument(
         dest='path',
         action='store',
         nargs='?',
         help='GitLab group, user namespace or project path',
     )
```

### Comparing `gitlab_projects_settings-4.0.0/src/features/gitlab.py` & `gitlab_projects_settings-4.1.0/src/features/gitlab.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Modules libraries
 from gitlab import Gitlab
 from gitlab.exceptions import GitlabDeleteError, GitlabGetError, GitlabListError
 from gitlab.v4.objects import Group, Namespace, Project, User
 
 # Components
-from ..types.gitlab import AccessLevels, ProjectFeatures
+from ..types.gitlab import AccessLevels, ProjectFeatures, ProtectionLevels
 
 # GitLabFeature class, pylint: disable=too-many-public-methods
 class GitLabFeature:
 
     # Constants
     TIMEOUT_DELETION: int = 300
 
@@ -345,21 +345,21 @@
         try:
             assert project.tags.list(get_all=True)
         except (AssertionError, GitlabListError):
             return result
 
         # Prepare access level
         access_level: int
-        if protect_level == 'no-one':
+        if protect_level == ProtectionLevels.NO_ONE:
             access_level = 0
-        elif protect_level == 'admins':
+        elif protect_level == ProtectionLevels.ADMINS:
             access_level = 60
-        elif protect_level == 'maintainers':
+        elif protect_level == ProtectionLevels.MAINTAINERS:
             access_level = 40
-        elif protect_level == 'developers':
+        elif protect_level == ProtectionLevels.DEVELOPERS:
             access_level = 30
         else:
             raise SyntaxError(f'Unknown protection level: {access_level}')
 
         # Acquire protected tags
         protectedtags = [
             protectedtag.name for protectedtag in project.protectedtags.list(get_all=True)
```

### Comparing `gitlab_projects_settings-4.0.0/src/package/bundle.py` & `gitlab_projects_settings-4.1.0/src/package/bundle.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.0.0/src/package/settings.py` & `gitlab_projects_settings-4.1.0/src/package/settings.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.0.0/src/package/updates.py` & `gitlab_projects_settings-4.1.0/src/package/updates.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.0.0/src/package/version.py` & `gitlab_projects_settings-4.1.0/src/package/version.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.0.0/src/prints/boxes.py` & `gitlab_projects_settings-4.1.0/src/prints/boxes.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.0.0/src/prints/colors.py` & `gitlab_projects_settings-4.1.0/src/prints/colors.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.0.0/src/system/platform.py` & `gitlab_projects_settings-4.1.0/src/system/platform.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.0.0/src/types/gitlab.py` & `gitlab_projects_settings-4.1.0/src/types/gitlab.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,36 @@
 
 # AccessLevels class, pylint: disable=too-few-public-methods
 class AccessLevels:
     DISABLED: str = 'disabled'
     PRIVATE: str = 'private'
     ENABLED: str = 'enabled'
 
+# ProtectionLevels class
+class ProtectionLevels:
+    NO_ONE: str = 'no-one'
+    ADMINS: str = 'admins'
+    MAINTAINERS: str = 'maintainers'
+    DEVELOPERS: str = 'developers'
+
+    # Default
+    @staticmethod
+    def default() -> str:
+        return ProtectionLevels.NO_ONE
+
+    # Names
+    @staticmethod
+    def names() -> List[str]:
+        return [
+            ProtectionLevels.NO_ONE,
+            ProtectionLevels.ADMINS,
+            ProtectionLevels.MAINTAINERS,
+            ProtectionLevels.DEVELOPERS,
+        ]
+
 # Visibility class, pylint: disable=too-few-public-methods
 class Visibility:
     PRIVATE: str = 'private'
     INTERNAL: str = 'internal'
     PUBLIC: str = 'public'
 
 # ProjectFeatureLevel class, pylint: disable=too-few-public-methods
```

### Comparing `gitlab_projects_settings-4.0.0/src/types/namespaces.py` & `gitlab_projects_settings-4.1.0/src/types/namespaces.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.0.0/src/types/strings.py` & `gitlab_projects_settings-4.1.0/src/types/strings.py`

 * *Files identical despite different names*

