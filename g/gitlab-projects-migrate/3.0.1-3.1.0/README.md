# Comparing `tmp/gitlab_projects_migrate-3.0.1.tar.gz` & `tmp/gitlab_projects_migrate-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab_projects_migrate-3.0.1.tar", last modified: Wed May 15 16:26:53 2024, max compression
+gzip compressed data, was "gitlab_projects_migrate-3.1.0.tar", last modified: Fri May 17 02:44:47 2024, max compression
```

## Comparing `gitlab_projects_migrate-3.0.1.tar` & `gitlab_projects_migrate-3.1.0.tar`

### file list

```diff
@@ -1,58 +1,60 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:26:53.946177 gitlab_projects_migrate-3.0.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:26:53.937177 gitlab_projects_migrate-3.0.1/.chglog/
--rwxrwxrwx   0 root         (0) root         (0)      649 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/.chglog/CHANGELOG.tpl.md
--rw-rw-rw-   0 root         (0) root         (0)      759 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/.chglog/changelog.sh
--rwxrwxrwx   0 root         (0) root         (0)      702 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/.chglog/config.yml
--rw-rw-rw-   0 root         (0) root         (0)      137 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)    11965 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/.markdownlint.json
--rw-rw-rw-   0 root         (0) root         (0)     1505 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/.style.yapf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:26:53.938177 gitlab_projects_migrate-3.0.1/.vscode/
--rw-rw-rw-   0 root         (0) root         (0)      675 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/.vscode/extensions.json
--rw-rw-rw-   0 root         (0) root         (0)     1252 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/.vscode/settings.json
--rw-rw-rw-   0 root         (0) root         (0)     4164 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6640 2024-05-15 16:26:53.946177 gitlab_projects_migrate-3.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4991 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:26:53.946177 gitlab_projects_migrate-3.0.1/gitlab_projects_migrate.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6640 2024-05-15 16:26:53.000000 gitlab_projects_migrate-3.0.1/gitlab_projects_migrate.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1028 2024-05-15 16:26:53.000000 gitlab_projects_migrate-3.0.1/gitlab_projects_migrate.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 16:26:53.000000 gitlab_projects_migrate-3.0.1/gitlab_projects_migrate.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       82 2024-05-15 16:26:53.000000 gitlab_projects_migrate-3.0.1/gitlab_projects_migrate.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-05-15 16:26:53.000000 gitlab_projects_migrate-3.0.1/gitlab_projects_migrate.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2024-05-15 16:26:53.000000 gitlab_projects_migrate-3.0.1/gitlab_projects_migrate.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      425 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/mypy.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:26:53.940177 gitlab_projects_migrate-3.0.1/requirements/
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/requirements/build.txt
--rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/requirements/deploy.txt
--rw-rw-rw-   0 root         (0) root         (0)       75 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/requirements/quality.txt
--rw-rw-rw-   0 root         (0) root         (0)       78 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/requirements/runtime.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 16:26:53.947177 gitlab_projects_migrate-3.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2875 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:26:53.941177 gitlab_projects_migrate-3.0.1/src/
--rw-rw-rw-   0 root         (0) root         (0)      142 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/src/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      114 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/src/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:26:53.942177 gitlab_projects_migrate-3.0.1/src/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/src/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    26927 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/src/cli/entrypoint.py
--rwxrwxrwx   0 root         (0) root         (0)     7821 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/src/cli/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:26:53.942177 gitlab_projects_migrate-3.0.1/src/features/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/src/features/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12338 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/src/features/gitlab.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:26:53.944177 gitlab_projects_migrate-3.0.1/src/package/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/src/package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      875 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/src/package/bundle.py
--rw-rw-rw-   0 root         (0) root         (0)     3810 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/src/package/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     6845 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/src/package/updates.py
--rw-rw-rw-   0 root         (0) root         (0)     1607 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/src/package/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:26:53.944177 gitlab_projects_migrate-3.0.1/src/prints/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/src/prints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2549 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/src/prints/boxes.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/src/prints/colors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:26:53.945177 gitlab_projects_migrate-3.0.1/src/system/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/src/system/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1788 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/src/system/platform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:26:53.945177 gitlab_projects_migrate-3.0.1/src/types/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/src/types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1704 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/src/types/namespaces.py
--rw-rw-rw-   0 root         (0) root         (0)     3849 2024-05-15 16:26:50.000000 gitlab_projects_migrate-3.0.1/src/types/strings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:47.018808 gitlab_projects_migrate-3.1.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:47.008808 gitlab_projects_migrate-3.1.0/.chglog/
+-rwxrwxrwx   0 root         (0) root         (0)      649 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/.chglog/CHANGELOG.tpl.md
+-rw-rw-rw-   0 root         (0) root         (0)      759 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/.chglog/changelog.sh
+-rwxrwxrwx   0 root         (0) root         (0)      702 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/.chglog/config.yml
+-rw-rw-rw-   0 root         (0) root         (0)      137 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)    11965 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/.markdownlint.json
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/.style.yapf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:47.009808 gitlab_projects_migrate-3.1.0/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      675 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/.vscode/extensions.json
+-rw-rw-rw-   0 root         (0) root         (0)     1252 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/.vscode/settings.json
+-rw-rw-rw-   0 root         (0) root         (0)     4720 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7248 2024-05-17 02:44:47.018808 gitlab_projects_migrate-3.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5565 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:47.017808 gitlab_projects_migrate-3.1.0/gitlab_projects_migrate.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7248 2024-05-17 02:44:46.000000 gitlab_projects_migrate-3.1.0/gitlab_projects_migrate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1068 2024-05-17 02:44:47.000000 gitlab_projects_migrate-3.1.0/gitlab_projects_migrate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 02:44:46.000000 gitlab_projects_migrate-3.1.0/gitlab_projects_migrate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2024-05-17 02:44:46.000000 gitlab_projects_migrate-3.1.0/gitlab_projects_migrate.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       97 2024-05-17 02:44:46.000000 gitlab_projects_migrate-3.1.0/gitlab_projects_migrate.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2024-05-17 02:44:46.000000 gitlab_projects_migrate-3.1.0/gitlab_projects_migrate.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      425 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/mypy.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:47.011808 gitlab_projects_migrate-3.1.0/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/requirements/build.txt
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/requirements/deploy.txt
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/requirements/quality.txt
+-rw-rw-rw-   0 root         (0) root         (0)       97 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/requirements/runtime.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 02:44:47.018808 gitlab_projects_migrate-3.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2875 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:47.011808 gitlab_projects_migrate-3.1.0/src/
+-rw-rw-rw-   0 root         (0) root         (0)      142 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      114 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:47.012808 gitlab_projects_migrate-3.1.0/src/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    29592 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/cli/entrypoint.py
+-rwxrwxrwx   0 root         (0) root         (0)     8605 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/cli/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:47.013808 gitlab_projects_migrate-3.1.0/src/features/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/features/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12565 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/features/gitlab.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:47.014808 gitlab_projects_migrate-3.1.0/src/package/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/package/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      875 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/package/bundle.py
+-rw-rw-rw-   0 root         (0) root         (0)     3810 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/package/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     6845 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/package/updates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1607 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/package/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:47.015808 gitlab_projects_migrate-3.1.0/src/prints/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/prints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2549 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/prints/boxes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/prints/colors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1565 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/prints/themes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:47.016808 gitlab_projects_migrate-3.1.0/src/system/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/system/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1788 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/system/platform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:47.017808 gitlab_projects_migrate-3.1.0/src/types/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/types/namespaces.py
+-rw-rw-rw-   0 root         (0) root         (0)      709 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/types/paths.py
+-rw-rw-rw-   0 root         (0) root         (0)     3849 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/types/strings.py
```

### Comparing `gitlab_projects_migrate-3.0.1/.chglog/CHANGELOG.tpl.md` & `gitlab_projects_migrate-3.1.0/.chglog/CHANGELOG.tpl.md`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.0.1/.chglog/changelog.sh` & `gitlab_projects_migrate-3.1.0/.chglog/changelog.sh`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.0.1/.chglog/config.yml` & `gitlab_projects_migrate-3.1.0/.chglog/config.yml`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.0.1/.gitlab-ci.yml` & `gitlab_projects_migrate-3.1.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.0.1/.style.yapf` & `gitlab_projects_migrate-3.1.0/.style.yapf`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.0.1/.vscode/extensions.json` & `gitlab_projects_migrate-3.1.0/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.0.1/.vscode/settings.json` & `gitlab_projects_migrate-3.1.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.0.1/CHANGELOG.md` & `gitlab_projects_migrate-3.1.0/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,27 @@
 
+<a name="3.1.0"></a>
+## [3.1.0](https://gitlab.com/AdrianDC/gitlab-projects-migrate/compare/3.0.1...3.1.0) (2024-05-17)
+
+### Bug Fixes
+
+* **gitlab:** restore 'import_project' file argument as BufferedReader
+* **gitlab:** raise runtime error upon failed project imports
+
+### Cleanups
+
+* **gitlab:** ignore 'import_project' file argument typing
+
+### Features
+
+* **entrypoint:** implement prompt confirmation upon deletions
+* **entrypoint:** implement '--archive-exports FOLDER' to keep exports
+* **requirements:** prepare 'questionary' library integration
+
+
 <a name="3.0.1"></a>
 ## [3.0.1](https://gitlab.com/AdrianDC/gitlab-projects-migrate/compare/3.0.0...3.0.1) (2024-05-15)
 
 ### Bug Fixes
 
 * **entrypoint:** resolve 'output_namespace' assertion tests
```

### Comparing `gitlab_projects_migrate-3.0.1/LICENSE` & `gitlab_projects_migrate-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.0.1/PKG-INFO` & `gitlab_projects_migrate-3.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-projects-migrate
-Version: 3.0.1
+Version: 3.1.0
 Summary: Migrate GitLab projects from a GitLab group to another GitLab's group
 Home-page: https://gitlab.com/AdrianDC/gitlab-projects-migrate
 Author: Adrian DC
 Author-email: radian.dc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://gitlab.com/AdrianDC/gitlab-projects-migrate/-/issues
 Project-URL: Changelog, https://gitlab.com/AdrianDC/gitlab-projects-migrate/blob/main/CHANGELOG.md
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
 
 # gitlab-projects-migrate
 
 <!-- markdownlint-disable no-inline-html -->
 
@@ -78,52 +79,53 @@
 ## Usage
 
 <!-- prettier-ignore-start -->
 <!-- readme-help-start -->
 
 ```yaml
 usage: gitlab-projects-migrate [-h] [--version] [--update-check] [--settings] [--set GROUP KEY VAL] [-I INPUT_TOKEN]
-                               [-O OUTPUT_TOKEN] [--delete-sources] [--dry-run] [--exclude-group]
-                               [--exclude-subgroups] [--exclude-projects] [--keep-members] [--overwrite]
-                               [--set-avatar FILE] [--update-description] [--]
+                               [-O OUTPUT_TOKEN] [--archive-exports FOLDER] [--delete-sources] [--dry-run]
+                               [--exclude-group] [--exclude-subgroups] [--exclude-projects] [--keep-members]
+                               [--overwrite] [--set-avatar FILE] [--update-description] [--]
                                [input_gitlab] [input_path] [output_gitlab] [output_namespace]
 
 gitlab-projects-migrate: Migrate GitLab projects from a GitLab group to another GitLab's group
 
 internal arguments:
-  -h, --help            # Show this help message
-  --version             # Show the current version
-  --update-check        # Check for newer package updates
-  --settings            # Show the current settings path and contents
-  --set GROUP KEY VAL   # Set settings specific 'VAL' value to [GROUP] > KEY
-                        # or unset by using 'UNSET' as 'VAL'
+  -h, --help                # Show this help message
+  --version                 # Show the current version
+  --update-check            # Check for newer package updates
+  --settings                # Show the current settings path and contents
+  --set GROUP KEY VAL       # Set settings specific 'VAL' value to [GROUP] > KEY
+                            # or unset by using 'UNSET' as 'VAL'
 
 credentials arguments:
-  -I INPUT_TOKEN        # Input GitLab API token (default: GITLAB_INPUT_TOKEN or GITLAB_TOKEN environments)
-  -O OUTPUT_TOKEN       # Output GitLab API token (default: GITLAB_OUTPUT_TOKEN, GITLAB_TOKEN environments, or INPUT_TOKEN argument)
+  -I INPUT_TOKEN            # Input GitLab API token (default: GITLAB_INPUT_TOKEN or GITLAB_TOKEN environments)
+  -O OUTPUT_TOKEN           # Output GitLab API token (default: GITLAB_OUTPUT_TOKEN, GITLAB_TOKEN environments, or INPUT_TOKEN argument)
 
 migration arguments:
-  --delete-sources      # Delete sources after successful migration
-  --dry-run             # Enable dry run mode to check without saving
-  --exclude-group       # Exclude parent group migration
-  --exclude-subgroups   # Exclude children subgroups migration
-  --exclude-projects    # Exclude children projects migration
-  --keep-members        # Keep input members after importing on output GitLab
-  --overwrite           # Overwrite existing projects on output GitLab
+  --archive-exports FOLDER  # Store exported projects and groups to a folder
+  --delete-sources          # Delete sources after successful migration
+  --dry-run                 # Enable dry run mode to check without saving
+  --exclude-group           # Exclude parent group migration
+  --exclude-subgroups       # Exclude children subgroups migration
+  --exclude-projects        # Exclude children projects migration
+  --keep-members            # Keep input members after importing on output GitLab
+  --overwrite               # Overwrite existing projects on output GitLab
 
 general settings arguments:
-  --set-avatar FILE     # Set avatar of GitLab output projects and groups
-  --update-description  # Update description of GitLab output projects and groups automatically
+  --set-avatar FILE         # Set avatar of GitLab output projects and groups
+  --update-description      # Update description of GitLab output projects and groups automatically
 
 positional arguments:
-  --                    # Positional arguments separator (recommended)
-  input_gitlab          # Input GitLab URL (default: https://gitlab.com)
-  input_path            # Input GitLab group, user namespace or project path
-  output_gitlab         # Output GitLab URL (default: https://gitlab.com)
-  output_namespace      # Output GitLab group or user namespace
+  --                        # Positional arguments separator (recommended)
+  input_gitlab              # Input GitLab URL (default: https://gitlab.com)
+  input_path                # Input GitLab group, user namespace or project path
+  output_gitlab             # Output GitLab URL (default: https://gitlab.com)
+  output_namespace          # Output GitLab group or user namespace
 ```
 
 <!-- readme-help-stop -->
 <!-- prettier-ignore-end -->
 
 ---
 
@@ -137,18 +139,28 @@
 
 ```bash
 gitlab-projects-migrate --settings
 ```
 
 ---
 
+## Environment available configurations
+
+`gitlab-projects-migrate` uses `colored` for colors outputs and `questionary` for interactive menus.
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

### Comparing `gitlab_projects_migrate-3.0.1/README.md` & `gitlab_projects_migrate-3.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -43,52 +43,53 @@
 ## Usage
 
 <!-- prettier-ignore-start -->
 <!-- readme-help-start -->
 
 ```yaml
 usage: gitlab-projects-migrate [-h] [--version] [--update-check] [--settings] [--set GROUP KEY VAL] [-I INPUT_TOKEN]
-                               [-O OUTPUT_TOKEN] [--delete-sources] [--dry-run] [--exclude-group]
-                               [--exclude-subgroups] [--exclude-projects] [--keep-members] [--overwrite]
-                               [--set-avatar FILE] [--update-description] [--]
+                               [-O OUTPUT_TOKEN] [--archive-exports FOLDER] [--delete-sources] [--dry-run]
+                               [--exclude-group] [--exclude-subgroups] [--exclude-projects] [--keep-members]
+                               [--overwrite] [--set-avatar FILE] [--update-description] [--]
                                [input_gitlab] [input_path] [output_gitlab] [output_namespace]
 
 gitlab-projects-migrate: Migrate GitLab projects from a GitLab group to another GitLab's group
 
 internal arguments:
-  -h, --help            # Show this help message
-  --version             # Show the current version
-  --update-check        # Check for newer package updates
-  --settings            # Show the current settings path and contents
-  --set GROUP KEY VAL   # Set settings specific 'VAL' value to [GROUP] > KEY
-                        # or unset by using 'UNSET' as 'VAL'
+  -h, --help                # Show this help message
+  --version                 # Show the current version
+  --update-check            # Check for newer package updates
+  --settings                # Show the current settings path and contents
+  --set GROUP KEY VAL       # Set settings specific 'VAL' value to [GROUP] > KEY
+                            # or unset by using 'UNSET' as 'VAL'
 
 credentials arguments:
-  -I INPUT_TOKEN        # Input GitLab API token (default: GITLAB_INPUT_TOKEN or GITLAB_TOKEN environments)
-  -O OUTPUT_TOKEN       # Output GitLab API token (default: GITLAB_OUTPUT_TOKEN, GITLAB_TOKEN environments, or INPUT_TOKEN argument)
+  -I INPUT_TOKEN            # Input GitLab API token (default: GITLAB_INPUT_TOKEN or GITLAB_TOKEN environments)
+  -O OUTPUT_TOKEN           # Output GitLab API token (default: GITLAB_OUTPUT_TOKEN, GITLAB_TOKEN environments, or INPUT_TOKEN argument)
 
 migration arguments:
-  --delete-sources      # Delete sources after successful migration
-  --dry-run             # Enable dry run mode to check without saving
-  --exclude-group       # Exclude parent group migration
-  --exclude-subgroups   # Exclude children subgroups migration
-  --exclude-projects    # Exclude children projects migration
-  --keep-members        # Keep input members after importing on output GitLab
-  --overwrite           # Overwrite existing projects on output GitLab
+  --archive-exports FOLDER  # Store exported projects and groups to a folder
+  --delete-sources          # Delete sources after successful migration
+  --dry-run                 # Enable dry run mode to check without saving
+  --exclude-group           # Exclude parent group migration
+  --exclude-subgroups       # Exclude children subgroups migration
+  --exclude-projects        # Exclude children projects migration
+  --keep-members            # Keep input members after importing on output GitLab
+  --overwrite               # Overwrite existing projects on output GitLab
 
 general settings arguments:
-  --set-avatar FILE     # Set avatar of GitLab output projects and groups
-  --update-description  # Update description of GitLab output projects and groups automatically
+  --set-avatar FILE         # Set avatar of GitLab output projects and groups
+  --update-description      # Update description of GitLab output projects and groups automatically
 
 positional arguments:
-  --                    # Positional arguments separator (recommended)
-  input_gitlab          # Input GitLab URL (default: https://gitlab.com)
-  input_path            # Input GitLab group, user namespace or project path
-  output_gitlab         # Output GitLab URL (default: https://gitlab.com)
-  output_namespace      # Output GitLab group or user namespace
+  --                        # Positional arguments separator (recommended)
+  input_gitlab              # Input GitLab URL (default: https://gitlab.com)
+  input_path                # Input GitLab group, user namespace or project path
+  output_gitlab             # Output GitLab URL (default: https://gitlab.com)
+  output_namespace          # Output GitLab group or user namespace
 ```
 
 <!-- readme-help-stop -->
 <!-- prettier-ignore-end -->
 
 ---
 
@@ -102,18 +103,28 @@
 
 ```bash
 gitlab-projects-migrate --settings
 ```
 
 ---
 
+## Environment available configurations
+
+`gitlab-projects-migrate` uses `colored` for colors outputs and `questionary` for interactive menus.
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

### Comparing `gitlab_projects_migrate-3.0.1/gitlab_projects_migrate.egg-info/PKG-INFO` & `gitlab_projects_migrate-3.1.0/gitlab_projects_migrate.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-projects-migrate
-Version: 3.0.1
+Version: 3.1.0
 Summary: Migrate GitLab projects from a GitLab group to another GitLab's group
 Home-page: https://gitlab.com/AdrianDC/gitlab-projects-migrate
 Author: Adrian DC
 Author-email: radian.dc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://gitlab.com/AdrianDC/gitlab-projects-migrate/-/issues
 Project-URL: Changelog, https://gitlab.com/AdrianDC/gitlab-projects-migrate/blob/main/CHANGELOG.md
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
 
 # gitlab-projects-migrate
 
 <!-- markdownlint-disable no-inline-html -->
 
@@ -78,52 +79,53 @@
 ## Usage
 
 <!-- prettier-ignore-start -->
 <!-- readme-help-start -->
 
 ```yaml
 usage: gitlab-projects-migrate [-h] [--version] [--update-check] [--settings] [--set GROUP KEY VAL] [-I INPUT_TOKEN]
-                               [-O OUTPUT_TOKEN] [--delete-sources] [--dry-run] [--exclude-group]
-                               [--exclude-subgroups] [--exclude-projects] [--keep-members] [--overwrite]
-                               [--set-avatar FILE] [--update-description] [--]
+                               [-O OUTPUT_TOKEN] [--archive-exports FOLDER] [--delete-sources] [--dry-run]
+                               [--exclude-group] [--exclude-subgroups] [--exclude-projects] [--keep-members]
+                               [--overwrite] [--set-avatar FILE] [--update-description] [--]
                                [input_gitlab] [input_path] [output_gitlab] [output_namespace]
 
 gitlab-projects-migrate: Migrate GitLab projects from a GitLab group to another GitLab's group
 
 internal arguments:
-  -h, --help            # Show this help message
-  --version             # Show the current version
-  --update-check        # Check for newer package updates
-  --settings            # Show the current settings path and contents
-  --set GROUP KEY VAL   # Set settings specific 'VAL' value to [GROUP] > KEY
-                        # or unset by using 'UNSET' as 'VAL'
+  -h, --help                # Show this help message
+  --version                 # Show the current version
+  --update-check            # Check for newer package updates
+  --settings                # Show the current settings path and contents
+  --set GROUP KEY VAL       # Set settings specific 'VAL' value to [GROUP] > KEY
+                            # or unset by using 'UNSET' as 'VAL'
 
 credentials arguments:
-  -I INPUT_TOKEN        # Input GitLab API token (default: GITLAB_INPUT_TOKEN or GITLAB_TOKEN environments)
-  -O OUTPUT_TOKEN       # Output GitLab API token (default: GITLAB_OUTPUT_TOKEN, GITLAB_TOKEN environments, or INPUT_TOKEN argument)
+  -I INPUT_TOKEN            # Input GitLab API token (default: GITLAB_INPUT_TOKEN or GITLAB_TOKEN environments)
+  -O OUTPUT_TOKEN           # Output GitLab API token (default: GITLAB_OUTPUT_TOKEN, GITLAB_TOKEN environments, or INPUT_TOKEN argument)
 
 migration arguments:
-  --delete-sources      # Delete sources after successful migration
-  --dry-run             # Enable dry run mode to check without saving
-  --exclude-group       # Exclude parent group migration
-  --exclude-subgroups   # Exclude children subgroups migration
-  --exclude-projects    # Exclude children projects migration
-  --keep-members        # Keep input members after importing on output GitLab
-  --overwrite           # Overwrite existing projects on output GitLab
+  --archive-exports FOLDER  # Store exported projects and groups to a folder
+  --delete-sources          # Delete sources after successful migration
+  --dry-run                 # Enable dry run mode to check without saving
+  --exclude-group           # Exclude parent group migration
+  --exclude-subgroups       # Exclude children subgroups migration
+  --exclude-projects        # Exclude children projects migration
+  --keep-members            # Keep input members after importing on output GitLab
+  --overwrite               # Overwrite existing projects on output GitLab
 
 general settings arguments:
-  --set-avatar FILE     # Set avatar of GitLab output projects and groups
-  --update-description  # Update description of GitLab output projects and groups automatically
+  --set-avatar FILE         # Set avatar of GitLab output projects and groups
+  --update-description      # Update description of GitLab output projects and groups automatically
 
 positional arguments:
-  --                    # Positional arguments separator (recommended)
-  input_gitlab          # Input GitLab URL (default: https://gitlab.com)
-  input_path            # Input GitLab group, user namespace or project path
-  output_gitlab         # Output GitLab URL (default: https://gitlab.com)
-  output_namespace      # Output GitLab group or user namespace
+  --                        # Positional arguments separator (recommended)
+  input_gitlab              # Input GitLab URL (default: https://gitlab.com)
+  input_path                # Input GitLab group, user namespace or project path
+  output_gitlab             # Output GitLab URL (default: https://gitlab.com)
+  output_namespace          # Output GitLab group or user namespace
 ```
 
 <!-- readme-help-stop -->
 <!-- prettier-ignore-end -->
 
 ---
 
@@ -137,18 +139,28 @@
 
 ```bash
 gitlab-projects-migrate --settings
 ```
 
 ---
 
+## Environment available configurations
+
+`gitlab-projects-migrate` uses `colored` for colors outputs and `questionary` for interactive menus.
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

### Comparing `gitlab_projects_migrate-3.0.1/gitlab_projects_migrate.egg-info/SOURCES.txt` & `gitlab_projects_migrate-3.1.0/gitlab_projects_migrate.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -33,12 +33,14 @@
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
 src/types/namespaces.py
+src/types/paths.py
 src/types/strings.py
```

### Comparing `gitlab_projects_migrate-3.0.1/setup.py` & `gitlab_projects_migrate-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.0.1/src/cli/entrypoint.py` & `gitlab_projects_migrate-3.1.0/src/cli/entrypoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,24 +11,31 @@
 from gitlab.v4.objects import (
     Group as GitLabGroup,
     Namespace as GitLabNamespace,
     Project as GitLabProject,
     ProjectImport as GitLabProjectImport,
     User as GitLabUser,
 )
+import questionary
 
 # Components
 from ..features.gitlab import GitLabFeature
+from ..package.bundle import Bundle
 from ..prints.colors import Colors
+from ..prints.themes import Themes
 from ..system.platform import Platform
 from ..types.namespaces import Namespaces
+from ..types.paths import Paths
 
 # Entrypoint class, pylint: disable=too-few-public-methods,too-many-statements
 class Entrypoint:
 
+    # Constants
+    EXPORTS_PREFIX: str = f'{Bundle.NAME}-exports-'
+
     # Enumerations
     Result = Enum('Result', ['SUCCESS', 'FINALIZE', 'ERROR'])
 
     # CLI, pylint: disable=too-many-branches
     @staticmethod
     def cli(options: Namespace) -> Result:
 
@@ -145,21 +152,28 @@
                 input_gitlab,
                 output_gitlab,
                 input_project.path_with_namespace,
                 input_project.namespace['id'],
                 output_namespace.full_path,
             )
 
-            # Delete input project
+            # Delete input project after validation
             if options.delete_sources:
                 print(f'{Colors.BOLD} - GitLab input project: '
                       f'{Colors.GREEN}{input_project.path_with_namespace}'
                       f'{Colors.CYAN} ({Namespaces.text(input_project.description)})'
                       f'{Colors.RESET}')
                 Platform.flush()
+                if not Entrypoint.confirm(
+                        'project',
+                        input_project.path_with_namespace,
+                ):
+                    raise PermissionError()
+
+                # Delete input project
                 input_gitlab.project_delete(input_project.path_with_namespace)
                 print(f'{Colors.BOLD}   - Delete sources project: '
                       f'{Colors.GREEN}Success'
                       f'{Colors.RESET}')
                 print(' ')
                 Platform.flush()
 
@@ -229,21 +243,28 @@
                         project.path_with_namespace,
                         input_group.full_path,
                         output_namespace.full_path,
                     )
                     if result in [Entrypoint.Result.FINALIZE, Entrypoint.Result.ERROR]:
                         return result
 
-            # Delete input group
+            # Delete input group after validation
             if options.delete_sources:
                 print(f'{Colors.BOLD} - GitLab input group: '
                       f'{Colors.GREEN}{input_group.full_path}'
                       f'{Colors.CYAN} ({Namespaces.text(input_group.description)})'
                       f'{Colors.RESET}')
                 Platform.flush()
+                if not Entrypoint.confirm(
+                        'group',
+                        input_group.full_path,
+                ):
+                    raise PermissionError()
+
+                # Delete input group
                 input_gitlab.group_delete(input_group.full_path)
                 print(f'{Colors.BOLD}   - Delete sources group: '
                       f'{Colors.GREEN}Success'
                       f'{Colors.RESET}')
                 print(' ')
                 Platform.flush()
 
@@ -270,31 +291,62 @@
                         project.path_with_namespace,
                         input_namespace.full_path,
                         output_namespace.full_path,
                     )
                     if result in [Entrypoint.Result.FINALIZE, Entrypoint.Result.ERROR]:
                         return result
 
-                    # Delete input project
+                    # Delete input project after validation
                     if options.delete_sources:
                         print(f'{Colors.BOLD} - GitLab input project: '
                               f'{Colors.GREEN}{project.path_with_namespace}'
                               f'{Colors.CYAN} ({Namespaces.text(project.description)})'
                               f'{Colors.RESET}')
                         Platform.flush()
+                        if not Entrypoint.confirm(
+                                'project',
+                                project.path_with_namespace,
+                        ):
+                            return Entrypoint.Result.SUCCESS
+
+                        # Delete input project
                         input_gitlab.project_delete(project.path_with_namespace)
                         print(f'{Colors.BOLD}   - Delete sources project: '
                               f'{Colors.GREEN}Success'
                               f'{Colors.RESET}')
                         print(' ')
                         Platform.flush()
 
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
     # Group, pylint: disable=too-many-arguments
     @staticmethod
     def group(
         options: Namespace,
         input_gitlab: GitLabFeature,
         output_gitlab: GitLabFeature,
         criteria_input_group: str,
@@ -333,15 +385,21 @@
             return Entrypoint.Result.SUCCESS
 
         # Export group
         print(f'{Colors.BOLD}   - Exporting from: '
               f'{Colors.GREEN}{input_group.full_path}'
               f'{Colors.RESET}')
         Platform.flush()
-        with NamedTemporaryFile(suffix='.tar.gz') as file_export:
+        with NamedTemporaryFile(
+                prefix=Paths.slugify(f'{Entrypoint.EXPORTS_PREFIX}'
+                                     f'-{input_group.full_path}-'),
+                suffix='.tar.gz',
+                dir=options.archive_exports_dir,
+                delete=not options.archive_exports_dir,
+        ) as file_export:
             input_gitlab.group_export(
                 file_export.name,
                 input_group.full_path,
                 options.keep_members,
             )
 
             # Import group
@@ -457,23 +515,34 @@
 
         # Export project
         print(f'{Colors.BOLD}   - Exporting from: '
               f'{Colors.GREEN}{options.input_path}'
               f'{Colors.CYAN} / {input_subpath}'
               f'{Colors.RESET}')
         Platform.flush()
-        with NamedTemporaryFile(suffix='.tar.gz') as file_export:
+        with NamedTemporaryFile(
+                prefix=Paths.slugify(f'{Entrypoint.EXPORTS_PREFIX}'
+                                     f'-{input_project.path_with_namespace}-'),
+                suffix='.tar.gz',
+                dir=options.archive_exports_dir,
+                delete=not options.archive_exports_dir,
+        ) as file_export:
             input_gitlab.project_export(
                 file_export.name,
                 input_project.path_with_namespace,
                 options.keep_members,
             )
 
             # Existing project removal
             if options.overwrite:
+                if not Entrypoint.confirm(
+                        'project',
+                        f'{output_namespace.full_path}/{input_subpath}',
+                ):
+                    raise PermissionError()
                 output_gitlab.project_delete(
                     f'{output_namespace.full_path}/{input_subpath}')
 
             # Import project
             print(f'{Colors.BOLD}   - Importing to: '
                   f'{Colors.GREEN}{options.output_namespace}'
                   f'{Colors.CYAN} / {input_subpath}'
@@ -617,15 +686,21 @@
                 return Entrypoint.Result.SUCCESS
 
             # Export subgroup
             print(f'{Colors.BOLD}   - Exporting from: '
                   f'{Colors.GREEN}{input_subgroup.full_path}'
                   f'{Colors.RESET}')
             Platform.flush()
-            with NamedTemporaryFile(suffix='.tar.gz') as file_export:
+            with NamedTemporaryFile(
+                    prefix=Paths.slugify(f'{Entrypoint.EXPORTS_PREFIX}'
+                                         f'-{input_subgroup.full_path}-'),
+                    suffix='.tar.gz',
+                    dir=options.archive_exports_dir,
+                    delete=not options.archive_exports_dir,
+            ) as file_export:
                 input_gitlab.group_export(
                     file_export.name,
                     input_subgroup.full_path,
                     options.keep_members,
                 )
 
                 # Import subgroup
```

### Comparing `gitlab_projects_migrate-3.0.1/src/cli/main.py` & `gitlab_projects_migrate-3.1.0/src/cli/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 #!/usr/bin/env python3
 
 # Standard libraries
-from argparse import (_ArgumentGroup, ArgumentParser, Namespace, RawTextHelpFormatter)
+from argparse import (_ArgumentGroup, ArgumentParser, Namespace, RawTextHelpFormatter,
+                      SUPPRESS)
 from os import environ
+from pathlib import Path
 from shutil import get_terminal_size
 from sys import exit as sys_exit
 
 # Components
 from ..package.bundle import Bundle
 from ..package.settings import Settings
 from ..package.updates import Updates
 from ..package.version import Version
 from ..prints.colors import Colors
 from ..system.platform import Platform
+from ..types.paths import Paths
 from .entrypoint import Entrypoint
 
 # Main, pylint: disable=too-many-statements
 def main() -> None:
 
     # Variables
     group: _ArgumentGroup
@@ -104,14 +107,21 @@
         f', {Bundle.ENV_GITLAB_TOKEN} environments,'
         ' or INPUT_TOKEN argument)',
     )
 
     # Arguments migration definitions
     group = parser.add_argument_group('migration arguments')
     group.add_argument(
+        '--archive-exports',
+        dest='archive_exports',
+        action='store',
+        metavar='FOLDER',
+        help='Store exported projects and groups to a folder',
+    )
+    group.add_argument(
         '--delete-sources',
         dest='delete_sources',
         action='store_true',
         help='Delete sources after successful migration',
     )
     group.add_argument(
         '--dry-run',
@@ -162,14 +172,24 @@
     group.add_argument(
         '--update-description',
         dest='update_description',
         action='store_true',
         help='Update description of GitLab output projects and groups automatically',
     )
 
+    # Arguments hidden definitions
+    group = parser.add_argument_group('hidden arguments')
+    group.add_argument(
+        '--archive-exports-dir',
+        dest='archive_exports_dir',
+        action='store',
+        default=None,
+        help=SUPPRESS,
+    )
+
     # Arguments positional definitions
     group = parser.add_argument_group('positional arguments')
     group.add_argument(
         '--',
         dest='double_dash',
         action='store_true',
         help='Positional arguments separator (recommended)',
@@ -252,14 +272,19 @@
             or not options.output_gitlab or not options.output_namespace:
         print(' ')
         parser.print_help()
         print(' ')
         Platform.flush()
         sys_exit(1)
 
+    # Prepare archive exports
+    if options.archive_exports:
+        options.archive_exports_dir = Paths.resolve(Path('.') / options.archive_exports)
+        Path(options.archive_exports_dir).mkdir(parents=True, exist_ok=True)
+
     # Arguments adaptations
     if not options.output_token:
         options.output_token = options.input_token
 
     # Header
     print(' ')
     Platform.flush()
```

### Comparing `gitlab_projects_migrate-3.0.1/src/features/gitlab.py` & `gitlab_projects_migrate-3.1.0/src/features/gitlab.py`

 * *Files 4% similar despite different names*

```diff
@@ -337,28 +337,32 @@
                     ),
                 ),
             )
 
         # Upload project import
         with open(archive, 'rb') as file:
             project_imported = self.__gitlab.projects.import_project(
-                str(file),
+                file, # type: ignore[arg-type] # TODO: BufferedReader instead of str # pylint: disable=fixme
                 path=path,
                 name=name,
                 namespace=group,
                 overwrite=overwrite,
             )
 
         # Wait project import
         project_import = self.__gitlab.projects.get(project_imported['id'],
                                                     lazy=True).imports.get()
         while project_import.import_status not in ['finished', 'failed']:
             sleep(1)
             project_import.refresh()
 
+        # Handle failed import
+        if project_import.import_status == 'failed':
+            raise RuntimeError(project_import.import_error)
+
         # Result
         return project_import
 
     # Project reset members
     def project_reset_members(self, criteria: str) -> None:
 
         # Remove project members
```

### Comparing `gitlab_projects_migrate-3.0.1/src/package/bundle.py` & `gitlab_projects_migrate-3.1.0/src/package/bundle.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.0.1/src/package/settings.py` & `gitlab_projects_migrate-3.1.0/src/package/settings.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.0.1/src/package/updates.py` & `gitlab_projects_migrate-3.1.0/src/package/updates.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.0.1/src/package/version.py` & `gitlab_projects_migrate-3.1.0/src/package/version.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.0.1/src/prints/boxes.py` & `gitlab_projects_migrate-3.1.0/src/prints/boxes.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.0.1/src/prints/colors.py` & `gitlab_projects_migrate-3.1.0/src/prints/colors.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.0.1/src/system/platform.py` & `gitlab_projects_migrate-3.1.0/src/system/platform.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.0.1/src/types/namespaces.py` & `gitlab_projects_migrate-3.1.0/src/types/namespaces.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.0.1/src/types/strings.py` & `gitlab_projects_migrate-3.1.0/src/types/strings.py`

 * *Files identical despite different names*

