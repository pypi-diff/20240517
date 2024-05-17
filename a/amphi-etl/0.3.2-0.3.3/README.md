# Comparing `tmp/amphi-etl-0.3.2.tar.gz` & `tmp/amphi-etl-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amphi-etl-0.3.2.tar", last modified: Fri May 17 21:24:56 2024, max compression
+gzip compressed data, was "amphi-etl-0.3.3.tar", last modified: Fri May 17 21:32:31 2024, max compression
```

## Comparing `amphi-etl-0.3.2.tar` & `amphi-etl-0.3.3.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:24:56.051064 amphi-etl-0.3.2/
--rw-r--r--   0 thibaut    (501) staff       (20)     3795 2024-03-22 17:55:16.000000 amphi-etl-0.3.2/LICENSE
--rw-r--r--   0 thibaut    (501) staff       (20)      646 2024-05-17 20:22:58.000000 amphi-etl-0.3.2/MANIFEST.in
--rw-r--r--   0 thibaut    (501) staff       (20)     6889 2024-05-17 21:24:56.050816 amphi-etl-0.3.2/PKG-INFO
--rw-r--r--   0 thibaut    (501) staff       (20)     1770 2024-03-22 18:05:50.000000 amphi-etl-0.3.2/README.md
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:24:56.031102 amphi-etl-0.3.2/amphi/
--rw-r--r--   0 thibaut    (501) staff       (20)       20 2024-05-15 18:36:08.000000 amphi-etl-0.3.2/amphi/__init__.py
--rw-r--r--   0 thibaut    (501) staff       (20)      171 2024-05-17 21:22:17.000000 amphi-etl-0.3.2/amphi/_version.py
--rw-r--r--   0 thibaut    (501) staff       (20)      236 2024-05-15 18:36:22.000000 amphi-etl-0.3.2/amphi/main.py
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:24:56.031426 amphi-etl-0.3.2/amphi/theme-light/
--rw-r--r--   0 thibaut    (501) staff       (20)     2699 2024-05-17 20:44:02.000000 amphi-etl-0.3.2/amphi/theme-light/package.json
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:24:56.032335 amphi-etl-0.3.2/amphi/theme-light/static/
--rw-r--r--   0 thibaut    (501) staff       (20)      398 2024-05-17 20:44:02.000000 amphi-etl-0.3.2/amphi/theme-light/static/509.bce2b45a96e48ba3bac6.js
--rw-r--r--   0 thibaut    (501) staff       (20)     6308 2024-05-17 20:44:02.000000 amphi-etl-0.3.2/amphi/theme-light/static/remoteEntry.0ccbe26ef55bccd7ac39.js
--rw-r--r--   0 thibaut    (501) staff       (20)      118 2024-05-17 20:44:01.000000 amphi-etl-0.3.2/amphi/theme-light/static/style.js
--rw-r--r--   0 thibaut    (501) staff       (20)       20 2024-05-17 20:44:02.000000 amphi-etl-0.3.2/amphi/theme-light/static/third-party-licenses.json
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:24:56.025893 amphi-etl-0.3.2/amphi/theme-light/themes/
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:24:56.025947 amphi-etl-0.3.2/amphi/theme-light/themes/@amphi/
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:24:56.033365 amphi-etl-0.3.2/amphi/theme-light/themes/@amphi/theme-light/
--rw-r--r--   0 thibaut    (501) staff       (20)    37754 2024-05-17 20:44:02.000000 amphi-etl-0.3.2/amphi/theme-light/themes/@amphi/theme-light/index.css
--rw-r--r--   0 thibaut    (501) staff       (20)        0 2024-05-17 20:44:02.000000 amphi-etl-0.3.2/amphi/theme-light/themes/@amphi/theme-light/index.js
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:24:56.033493 amphi-etl-0.3.2/amphi/ui-component/
--rw-r--r--   0 thibaut    (501) staff       (20)     2764 2024-05-17 20:44:06.000000 amphi-etl-0.3.2/amphi/ui-component/package.json
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:24:56.035617 amphi-etl-0.3.2/amphi/ui-component/static/
--rw-r--r--   0 thibaut    (501) staff       (20)    23876 2024-05-17 20:44:06.000000 amphi-etl-0.3.2/amphi/ui-component/static/412.3b7ac64a5f90d35edd2b.js
--rw-r--r--   0 thibaut    (501) staff       (20)    23129 2024-05-17 20:44:06.000000 amphi-etl-0.3.2/amphi/ui-component/static/587.6f653927626e1058bf40.js
--rw-r--r--   0 thibaut    (501) staff       (20)     1105 2024-05-17 20:44:06.000000 amphi-etl-0.3.2/amphi/ui-component/static/599.2ee6f3f059a6e0034cf1.js
--rw-r--r--   0 thibaut    (501) staff       (20)     7130 2024-05-17 20:44:06.000000 amphi-etl-0.3.2/amphi/ui-component/static/remoteEntry.ab3f5768d0a66069663b.js
--rw-r--r--   0 thibaut    (501) staff       (20)      162 2024-05-17 20:44:05.000000 amphi-etl-0.3.2/amphi/ui-component/static/style.js
--rw-r--r--   0 thibaut    (501) staff       (20)     2453 2024-05-17 20:44:06.000000 amphi-etl-0.3.2/amphi/ui-component/static/third-party-licenses.json
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:24:56.036556 amphi-etl-0.3.2/amphi_etl.egg-info/
--rw-r--r--   0 thibaut    (501) staff       (20)     6889 2024-05-17 21:24:55.000000 amphi-etl-0.3.2/amphi_etl.egg-info/PKG-INFO
--rw-r--r--   0 thibaut    (501) staff       (20)     3238 2024-05-17 21:24:56.000000 amphi-etl-0.3.2/amphi_etl.egg-info/SOURCES.txt
--rw-r--r--   0 thibaut    (501) staff       (20)        1 2024-05-17 21:24:55.000000 amphi-etl-0.3.2/amphi_etl.egg-info/dependency_links.txt
--rw-r--r--   0 thibaut    (501) staff       (20)       42 2024-05-17 21:24:55.000000 amphi-etl-0.3.2/amphi_etl.egg-info/entry_points.txt
--rw-r--r--   0 thibaut    (501) staff       (20)       57 2024-05-17 21:24:55.000000 amphi-etl-0.3.2/amphi_etl.egg-info/requires.txt
--rw-r--r--   0 thibaut    (501) staff       (20)        6 2024-05-17 21:24:55.000000 amphi-etl-0.3.2/amphi_etl.egg-info/top_level.txt
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:24:56.026321 amphi-etl-0.3.2/config/
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:24:56.036711 amphi-etl-0.3.2/config/labconfig/
--rw-r--r--   0 thibaut    (501) staff       (20)      680 2024-05-15 22:02:31.000000 amphi-etl-0.3.2/config/labconfig/page_config.json
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:24:56.036953 amphi-etl-0.3.2/config/settings/
--rw-r--r--   0 thibaut    (501) staff       (20)     2679 2024-05-15 22:26:33.000000 amphi-etl-0.3.2/config/settings/overrides.json
--rw-r--r--   0 thibaut    (501) staff       (20)     3187 2024-05-15 18:40:20.000000 amphi-etl-0.3.2/package.json
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:24:56.026684 amphi-etl-0.3.2/packages/
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:24:56.037803 amphi-etl-0.3.2/packages/theme-light/
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:24:56.038988 amphi-etl-0.3.2/packages/theme-light/lib/
--rw-r--r--   0 thibaut    (501) staff       (20)      214 2024-05-17 20:43:59.000000 amphi-etl-0.3.2/packages/theme-light/lib/index.d.ts
--rw-r--r--   0 thibaut    (501) staff       (20)      584 2024-05-17 20:43:59.000000 amphi-etl-0.3.2/packages/theme-light/lib/index.js
--rw-r--r--   0 thibaut    (501) staff       (20)     2583 2024-05-17 20:42:53.000000 amphi-etl-0.3.2/packages/theme-light/package.json
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:24:56.039254 amphi-etl-0.3.2/packages/theme-light/src/
--rw-r--r--   0 thibaut    (501) staff       (20)      683 2024-03-22 18:05:01.000000 amphi-etl-0.3.2/packages/theme-light/src/index.ts
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:24:56.040114 amphi-etl-0.3.2/packages/theme-light/style/
--rw-r--r--   0 thibaut    (501) staff       (20)    23116 2024-05-16 05:20:56.000000 amphi-etl-0.3.2/packages/theme-light/style/index.css
--rw-r--r--   0 thibaut    (501) staff       (20)    14663 2024-05-15 22:00:45.000000 amphi-etl-0.3.2/packages/theme-light/style/variables.css
--rw-r--r--   0 thibaut    (501) staff       (20)      135 2024-03-22 18:05:01.000000 amphi-etl-0.3.2/packages/theme-light/tsconfig.json
--rw-r--r--   0 thibaut    (501) staff       (20)    62340 2024-05-17 20:43:59.000000 amphi-etl-0.3.2/packages/theme-light/tsconfig.tsbuildinfo
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:24:56.041067 amphi-etl-0.3.2/packages/ui-component/
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:24:56.043623 amphi-etl-0.3.2/packages/ui-component/lib/
--rw-r--r--   0 thibaut    (501) staff       (20)      465 2024-05-17 20:44:04.000000 amphi-etl-0.3.2/packages/ui-component/lib/BrowseFileDialog.d.ts
--rw-r--r--   0 thibaut    (501) staff       (20)     6922 2024-05-17 20:44:04.000000 amphi-etl-0.3.2/packages/ui-component/lib/BrowseFileDialog.js
--rw-r--r--   0 thibaut    (501) staff       (20)      729 2024-05-17 20:44:04.000000 amphi-etl-0.3.2/packages/ui-component/lib/Dropzone.d.ts
--rw-r--r--   0 thibaut    (501) staff       (20)     2229 2024-05-17 20:44:04.000000 amphi-etl-0.3.2/packages/ui-component/lib/Dropzone.js
--rw-r--r--   0 thibaut    (501) staff       (20)      529 2024-05-17 20:44:04.000000 amphi-etl-0.3.2/packages/ui-component/lib/icons.d.ts
--rw-r--r--   0 thibaut    (501) staff       (20)     1861 2024-05-17 20:44:04.000000 amphi-etl-0.3.2/packages/ui-component/lib/icons.js
--rw-r--r--   0 thibaut    (501) staff       (20)      255 2024-05-17 20:44:04.000000 amphi-etl-0.3.2/packages/ui-component/lib/index.d.ts
--rw-r--r--   0 thibaut    (501) staff       (20)     5217 2024-05-17 20:44:04.000000 amphi-etl-0.3.2/packages/ui-component/lib/index.js
--rw-r--r--   0 thibaut    (501) staff       (20)     1127 2024-05-17 20:44:04.000000 amphi-etl-0.3.2/packages/ui-component/lib/launcher.d.ts
--rw-r--r--   0 thibaut    (501) staff       (20)    13920 2024-05-17 20:44:04.000000 amphi-etl-0.3.2/packages/ui-component/lib/launcher.js
--rw-r--r--   0 thibaut    (501) staff       (20)     2622 2024-05-17 20:42:59.000000 amphi-etl-0.3.2/packages/ui-component/package.json
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:24:56.044680 amphi-etl-0.3.2/packages/ui-component/src/
--rw-r--r--   0 thibaut    (501) staff       (20)     7188 2024-03-22 18:05:02.000000 amphi-etl-0.3.2/packages/ui-component/src/BrowseFileDialog.tsx
--rw-r--r--   0 thibaut    (501) staff       (20)     2814 2024-03-22 18:05:02.000000 amphi-etl-0.3.2/packages/ui-component/src/Dropzone.tsx
--rw-r--r--   0 thibaut    (501) staff       (20)       74 2024-03-22 18:05:02.000000 amphi-etl-0.3.2/packages/ui-component/src/declarations.d.ts
--rw-r--r--   0 thibaut    (501) staff       (20)     1831 2024-03-22 18:05:02.000000 amphi-etl-0.3.2/packages/ui-component/src/icons.ts
--rw-r--r--   0 thibaut    (501) staff       (20)     5084 2024-05-15 17:04:08.000000 amphi-etl-0.3.2/packages/ui-component/src/index.ts
--rw-r--r--   0 thibaut    (501) staff       (20)    12567 2024-05-15 16:58:31.000000 amphi-etl-0.3.2/packages/ui-component/src/launcher.tsx
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:24:56.045944 amphi-etl-0.3.2/packages/ui-component/style/
--rw-r--r--   0 thibaut    (501) staff       (20)      403 2024-03-22 18:05:02.000000 amphi-etl-0.3.2/packages/ui-component/style/base.css
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:24:56.050321 amphi-etl-0.3.2/packages/ui-component/style/icons/
--rw-r--r--   0 thibaut    (501) staff       (20)     2857 2024-03-22 20:46:02.000000 amphi-etl-0.3.2/packages/ui-component/style/icons/amphi-square-logo.svg
--rw-r--r--   0 thibaut    (501) staff       (20)     3001 2024-03-22 20:45:41.000000 amphi-etl-0.3.2/packages/ui-component/style/icons/amphi-square-logo_nonpaths.svg
--rw-r--r--   0 thibaut    (501) staff       (20)     2838 2024-03-22 20:46:22.000000 amphi-etl-0.3.2/packages/ui-component/style/icons/amphi.svg
--rw-r--r--   0 thibaut    (501) staff       (20)     1227 2024-03-22 18:05:02.000000 amphi-etl-0.3.2/packages/ui-component/style/icons/bug-16.svg
--rw-r--r--   0 thibaut    (501) staff       (20)     1204 2024-03-22 18:05:02.000000 amphi-etl-0.3.2/packages/ui-component/style/icons/bug-24.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      465 2024-03-22 18:05:02.000000 amphi-etl-0.3.2/packages/ui-component/style/icons/code-16.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      496 2024-03-22 18:05:02.000000 amphi-etl-0.3.2/packages/ui-component/style/icons/code-24.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      432 2024-03-22 18:05:02.000000 amphi-etl-0.3.2/packages/ui-component/style/icons/docs-16.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      479 2024-03-22 18:05:02.000000 amphi-etl-0.3.2/packages/ui-component/style/icons/docs-24.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      924 2024-03-22 18:05:02.000000 amphi-etl-0.3.2/packages/ui-component/style/icons/network-24.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      330 2024-03-22 18:05:02.000000 amphi-etl-0.3.2/packages/ui-component/style/icons/p5-asterisk.svg
--rw-r--r--   0 thibaut    (501) staff       (20)     2895 2024-03-22 18:05:02.000000 amphi-etl-0.3.2/packages/ui-component/style/icons/p5-square-logo.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      687 2024-03-22 18:05:02.000000 amphi-etl-0.3.2/packages/ui-component/style/icons/pipeline-16.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      702 2024-03-22 18:05:02.000000 amphi-etl-0.3.2/packages/ui-component/style/icons/pipeline-24.svg
--rw-r--r--   0 thibaut    (501) staff       (20)     2703 2024-03-22 18:05:02.000000 amphi-etl-0.3.2/packages/ui-component/style/icons/pipeline.svg
--rw-r--r--   0 thibaut    (501) staff       (20)     2717 2024-03-22 18:05:02.000000 amphi-etl-0.3.2/packages/ui-component/style/icons/pipeline_negative.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      845 2024-03-22 18:05:02.000000 amphi-etl-0.3.2/packages/ui-component/style/icons/shield-check-24.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      472 2024-03-22 18:05:02.000000 amphi-etl-0.3.2/packages/ui-component/style/icons/upload-16.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      289 2024-03-22 18:05:02.000000 amphi-etl-0.3.2/packages/ui-component/style/index.css
--rw-r--r--   0 thibaut    (501) staff       (20)      307 2024-03-22 18:05:02.000000 amphi-etl-0.3.2/packages/ui-component/style/index.js
--rw-r--r--   0 thibaut    (501) staff       (20)    18439 2024-05-15 17:05:28.000000 amphi-etl-0.3.2/packages/ui-component/style/output.css
--rw-r--r--   0 thibaut    (501) staff       (20)      277 2024-05-15 16:52:04.000000 amphi-etl-0.3.2/packages/ui-component/tailwind.config.js
--rw-r--r--   0 thibaut    (501) staff       (20)      620 2024-03-22 18:05:02.000000 amphi-etl-0.3.2/packages/ui-component/tsconfig.json
--rw-r--r--   0 thibaut    (501) staff       (20)    70461 2024-05-17 20:44:04.000000 amphi-etl-0.3.2/packages/ui-component/tsconfig.tsbuildinfo
--rw-r--r--   0 thibaut    (501) staff       (20)     2603 2024-05-17 20:43:36.000000 amphi-etl-0.3.2/pyproject.toml
--rw-r--r--   0 thibaut    (501) staff       (20)       38 2024-05-17 21:24:56.051116 amphi-etl-0.3.2/setup.cfg
--rw-r--r--   0 thibaut    (501) staff       (20)     1745 2024-05-17 21:22:32.000000 amphi-etl-0.3.2/setup.py
--rw-r--r--   0 thibaut    (501) staff       (20)       66 2024-03-22 17:55:16.000000 amphi-etl-0.3.2/tsconfig.eslint.json
--rw-r--r--   0 thibaut    (501) staff       (20)      513 2024-03-22 17:55:16.000000 amphi-etl-0.3.2/tsconfigbase.json
--rw-r--r--   0 thibaut    (501) staff       (20)   363863 2024-05-17 20:43:49.000000 amphi-etl-0.3.2/yarn.lock
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:32:31.542816 amphi-etl-0.3.3/
+-rw-r--r--   0 thibaut    (501) staff       (20)     3795 2024-03-22 17:55:16.000000 amphi-etl-0.3.3/LICENSE
+-rw-r--r--   0 thibaut    (501) staff       (20)      646 2024-05-17 20:22:58.000000 amphi-etl-0.3.3/MANIFEST.in
+-rw-r--r--   0 thibaut    (501) staff       (20)     6889 2024-05-17 21:32:31.542576 amphi-etl-0.3.3/PKG-INFO
+-rw-r--r--   0 thibaut    (501) staff       (20)     1770 2024-03-22 18:05:50.000000 amphi-etl-0.3.3/README.md
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:32:31.521496 amphi-etl-0.3.3/amphi/
+-rw-r--r--   0 thibaut    (501) staff       (20)       20 2024-05-15 18:36:08.000000 amphi-etl-0.3.3/amphi/__init__.py
+-rw-r--r--   0 thibaut    (501) staff       (20)      171 2024-05-17 21:32:20.000000 amphi-etl-0.3.3/amphi/_version.py
+-rw-r--r--   0 thibaut    (501) staff       (20)      670 2024-05-17 21:31:20.000000 amphi-etl-0.3.3/amphi/main.py
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:32:31.521811 amphi-etl-0.3.3/amphi/theme-light/
+-rw-r--r--   0 thibaut    (501) staff       (20)     2699 2024-05-17 20:44:02.000000 amphi-etl-0.3.3/amphi/theme-light/package.json
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:32:31.522786 amphi-etl-0.3.3/amphi/theme-light/static/
+-rw-r--r--   0 thibaut    (501) staff       (20)      398 2024-05-17 20:44:02.000000 amphi-etl-0.3.3/amphi/theme-light/static/509.bce2b45a96e48ba3bac6.js
+-rw-r--r--   0 thibaut    (501) staff       (20)     6308 2024-05-17 20:44:02.000000 amphi-etl-0.3.3/amphi/theme-light/static/remoteEntry.0ccbe26ef55bccd7ac39.js
+-rw-r--r--   0 thibaut    (501) staff       (20)      118 2024-05-17 20:44:01.000000 amphi-etl-0.3.3/amphi/theme-light/static/style.js
+-rw-r--r--   0 thibaut    (501) staff       (20)       20 2024-05-17 20:44:02.000000 amphi-etl-0.3.3/amphi/theme-light/static/third-party-licenses.json
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:32:31.516285 amphi-etl-0.3.3/amphi/theme-light/themes/
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:32:31.516349 amphi-etl-0.3.3/amphi/theme-light/themes/@amphi/
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:32:31.523787 amphi-etl-0.3.3/amphi/theme-light/themes/@amphi/theme-light/
+-rw-r--r--   0 thibaut    (501) staff       (20)    37754 2024-05-17 20:44:02.000000 amphi-etl-0.3.3/amphi/theme-light/themes/@amphi/theme-light/index.css
+-rw-r--r--   0 thibaut    (501) staff       (20)        0 2024-05-17 20:44:02.000000 amphi-etl-0.3.3/amphi/theme-light/themes/@amphi/theme-light/index.js
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:32:31.523904 amphi-etl-0.3.3/amphi/ui-component/
+-rw-r--r--   0 thibaut    (501) staff       (20)     2764 2024-05-17 20:44:06.000000 amphi-etl-0.3.3/amphi/ui-component/package.json
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:32:31.526309 amphi-etl-0.3.3/amphi/ui-component/static/
+-rw-r--r--   0 thibaut    (501) staff       (20)    23876 2024-05-17 20:44:06.000000 amphi-etl-0.3.3/amphi/ui-component/static/412.3b7ac64a5f90d35edd2b.js
+-rw-r--r--   0 thibaut    (501) staff       (20)    23129 2024-05-17 20:44:06.000000 amphi-etl-0.3.3/amphi/ui-component/static/587.6f653927626e1058bf40.js
+-rw-r--r--   0 thibaut    (501) staff       (20)     1105 2024-05-17 20:44:06.000000 amphi-etl-0.3.3/amphi/ui-component/static/599.2ee6f3f059a6e0034cf1.js
+-rw-r--r--   0 thibaut    (501) staff       (20)     7130 2024-05-17 20:44:06.000000 amphi-etl-0.3.3/amphi/ui-component/static/remoteEntry.ab3f5768d0a66069663b.js
+-rw-r--r--   0 thibaut    (501) staff       (20)      162 2024-05-17 20:44:05.000000 amphi-etl-0.3.3/amphi/ui-component/static/style.js
+-rw-r--r--   0 thibaut    (501) staff       (20)     2453 2024-05-17 20:44:06.000000 amphi-etl-0.3.3/amphi/ui-component/static/third-party-licenses.json
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:32:31.527445 amphi-etl-0.3.3/amphi_etl.egg-info/
+-rw-r--r--   0 thibaut    (501) staff       (20)     6889 2024-05-17 21:32:31.000000 amphi-etl-0.3.3/amphi_etl.egg-info/PKG-INFO
+-rw-r--r--   0 thibaut    (501) staff       (20)     3238 2024-05-17 21:32:31.000000 amphi-etl-0.3.3/amphi_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 thibaut    (501) staff       (20)        1 2024-05-17 21:32:31.000000 amphi-etl-0.3.3/amphi_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 thibaut    (501) staff       (20)       42 2024-05-17 21:32:31.000000 amphi-etl-0.3.3/amphi_etl.egg-info/entry_points.txt
+-rw-r--r--   0 thibaut    (501) staff       (20)       57 2024-05-17 21:32:31.000000 amphi-etl-0.3.3/amphi_etl.egg-info/requires.txt
+-rw-r--r--   0 thibaut    (501) staff       (20)        6 2024-05-17 21:32:31.000000 amphi-etl-0.3.3/amphi_etl.egg-info/top_level.txt
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:32:31.516749 amphi-etl-0.3.3/config/
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:32:31.527595 amphi-etl-0.3.3/config/labconfig/
+-rw-r--r--   0 thibaut    (501) staff       (20)      680 2024-05-15 22:02:31.000000 amphi-etl-0.3.3/config/labconfig/page_config.json
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:32:31.527991 amphi-etl-0.3.3/config/settings/
+-rw-r--r--   0 thibaut    (501) staff       (20)     2679 2024-05-15 22:26:33.000000 amphi-etl-0.3.3/config/settings/overrides.json
+-rw-r--r--   0 thibaut    (501) staff       (20)     3187 2024-05-17 21:32:17.000000 amphi-etl-0.3.3/package.json
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:32:31.517139 amphi-etl-0.3.3/packages/
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:32:31.528932 amphi-etl-0.3.3/packages/theme-light/
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:32:31.529879 amphi-etl-0.3.3/packages/theme-light/lib/
+-rw-r--r--   0 thibaut    (501) staff       (20)      214 2024-05-17 20:43:59.000000 amphi-etl-0.3.3/packages/theme-light/lib/index.d.ts
+-rw-r--r--   0 thibaut    (501) staff       (20)      584 2024-05-17 20:43:59.000000 amphi-etl-0.3.3/packages/theme-light/lib/index.js
+-rw-r--r--   0 thibaut    (501) staff       (20)     2583 2024-05-17 20:42:53.000000 amphi-etl-0.3.3/packages/theme-light/package.json
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:32:31.530137 amphi-etl-0.3.3/packages/theme-light/src/
+-rw-r--r--   0 thibaut    (501) staff       (20)      683 2024-03-22 18:05:01.000000 amphi-etl-0.3.3/packages/theme-light/src/index.ts
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:32:31.530848 amphi-etl-0.3.3/packages/theme-light/style/
+-rw-r--r--   0 thibaut    (501) staff       (20)    23116 2024-05-16 05:20:56.000000 amphi-etl-0.3.3/packages/theme-light/style/index.css
+-rw-r--r--   0 thibaut    (501) staff       (20)    14663 2024-05-15 22:00:45.000000 amphi-etl-0.3.3/packages/theme-light/style/variables.css
+-rw-r--r--   0 thibaut    (501) staff       (20)      135 2024-03-22 18:05:01.000000 amphi-etl-0.3.3/packages/theme-light/tsconfig.json
+-rw-r--r--   0 thibaut    (501) staff       (20)    62340 2024-05-17 20:43:59.000000 amphi-etl-0.3.3/packages/theme-light/tsconfig.tsbuildinfo
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:32:31.531878 amphi-etl-0.3.3/packages/ui-component/
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:32:31.534768 amphi-etl-0.3.3/packages/ui-component/lib/
+-rw-r--r--   0 thibaut    (501) staff       (20)      465 2024-05-17 20:44:04.000000 amphi-etl-0.3.3/packages/ui-component/lib/BrowseFileDialog.d.ts
+-rw-r--r--   0 thibaut    (501) staff       (20)     6922 2024-05-17 20:44:04.000000 amphi-etl-0.3.3/packages/ui-component/lib/BrowseFileDialog.js
+-rw-r--r--   0 thibaut    (501) staff       (20)      729 2024-05-17 20:44:04.000000 amphi-etl-0.3.3/packages/ui-component/lib/Dropzone.d.ts
+-rw-r--r--   0 thibaut    (501) staff       (20)     2229 2024-05-17 20:44:04.000000 amphi-etl-0.3.3/packages/ui-component/lib/Dropzone.js
+-rw-r--r--   0 thibaut    (501) staff       (20)      529 2024-05-17 20:44:04.000000 amphi-etl-0.3.3/packages/ui-component/lib/icons.d.ts
+-rw-r--r--   0 thibaut    (501) staff       (20)     1861 2024-05-17 20:44:04.000000 amphi-etl-0.3.3/packages/ui-component/lib/icons.js
+-rw-r--r--   0 thibaut    (501) staff       (20)      255 2024-05-17 20:44:04.000000 amphi-etl-0.3.3/packages/ui-component/lib/index.d.ts
+-rw-r--r--   0 thibaut    (501) staff       (20)     5217 2024-05-17 20:44:04.000000 amphi-etl-0.3.3/packages/ui-component/lib/index.js
+-rw-r--r--   0 thibaut    (501) staff       (20)     1127 2024-05-17 20:44:04.000000 amphi-etl-0.3.3/packages/ui-component/lib/launcher.d.ts
+-rw-r--r--   0 thibaut    (501) staff       (20)    13920 2024-05-17 20:44:04.000000 amphi-etl-0.3.3/packages/ui-component/lib/launcher.js
+-rw-r--r--   0 thibaut    (501) staff       (20)     2622 2024-05-17 20:42:59.000000 amphi-etl-0.3.3/packages/ui-component/package.json
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:32:31.536460 amphi-etl-0.3.3/packages/ui-component/src/
+-rw-r--r--   0 thibaut    (501) staff       (20)     7188 2024-03-22 18:05:02.000000 amphi-etl-0.3.3/packages/ui-component/src/BrowseFileDialog.tsx
+-rw-r--r--   0 thibaut    (501) staff       (20)     2814 2024-03-22 18:05:02.000000 amphi-etl-0.3.3/packages/ui-component/src/Dropzone.tsx
+-rw-r--r--   0 thibaut    (501) staff       (20)       74 2024-03-22 18:05:02.000000 amphi-etl-0.3.3/packages/ui-component/src/declarations.d.ts
+-rw-r--r--   0 thibaut    (501) staff       (20)     1831 2024-03-22 18:05:02.000000 amphi-etl-0.3.3/packages/ui-component/src/icons.ts
+-rw-r--r--   0 thibaut    (501) staff       (20)     5084 2024-05-15 17:04:08.000000 amphi-etl-0.3.3/packages/ui-component/src/index.ts
+-rw-r--r--   0 thibaut    (501) staff       (20)    12567 2024-05-15 16:58:31.000000 amphi-etl-0.3.3/packages/ui-component/src/launcher.tsx
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:32:31.537781 amphi-etl-0.3.3/packages/ui-component/style/
+-rw-r--r--   0 thibaut    (501) staff       (20)      403 2024-03-22 18:05:02.000000 amphi-etl-0.3.3/packages/ui-component/style/base.css
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:32:31.542209 amphi-etl-0.3.3/packages/ui-component/style/icons/
+-rw-r--r--   0 thibaut    (501) staff       (20)     2857 2024-03-22 20:46:02.000000 amphi-etl-0.3.3/packages/ui-component/style/icons/amphi-square-logo.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)     3001 2024-03-22 20:45:41.000000 amphi-etl-0.3.3/packages/ui-component/style/icons/amphi-square-logo_nonpaths.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)     2838 2024-03-22 20:46:22.000000 amphi-etl-0.3.3/packages/ui-component/style/icons/amphi.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)     1227 2024-03-22 18:05:02.000000 amphi-etl-0.3.3/packages/ui-component/style/icons/bug-16.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)     1204 2024-03-22 18:05:02.000000 amphi-etl-0.3.3/packages/ui-component/style/icons/bug-24.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      465 2024-03-22 18:05:02.000000 amphi-etl-0.3.3/packages/ui-component/style/icons/code-16.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      496 2024-03-22 18:05:02.000000 amphi-etl-0.3.3/packages/ui-component/style/icons/code-24.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      432 2024-03-22 18:05:02.000000 amphi-etl-0.3.3/packages/ui-component/style/icons/docs-16.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      479 2024-03-22 18:05:02.000000 amphi-etl-0.3.3/packages/ui-component/style/icons/docs-24.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      924 2024-03-22 18:05:02.000000 amphi-etl-0.3.3/packages/ui-component/style/icons/network-24.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      330 2024-03-22 18:05:02.000000 amphi-etl-0.3.3/packages/ui-component/style/icons/p5-asterisk.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)     2895 2024-03-22 18:05:02.000000 amphi-etl-0.3.3/packages/ui-component/style/icons/p5-square-logo.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      687 2024-03-22 18:05:02.000000 amphi-etl-0.3.3/packages/ui-component/style/icons/pipeline-16.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      702 2024-03-22 18:05:02.000000 amphi-etl-0.3.3/packages/ui-component/style/icons/pipeline-24.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)     2703 2024-03-22 18:05:02.000000 amphi-etl-0.3.3/packages/ui-component/style/icons/pipeline.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)     2717 2024-03-22 18:05:02.000000 amphi-etl-0.3.3/packages/ui-component/style/icons/pipeline_negative.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      845 2024-03-22 18:05:02.000000 amphi-etl-0.3.3/packages/ui-component/style/icons/shield-check-24.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      472 2024-03-22 18:05:02.000000 amphi-etl-0.3.3/packages/ui-component/style/icons/upload-16.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      289 2024-03-22 18:05:02.000000 amphi-etl-0.3.3/packages/ui-component/style/index.css
+-rw-r--r--   0 thibaut    (501) staff       (20)      307 2024-03-22 18:05:02.000000 amphi-etl-0.3.3/packages/ui-component/style/index.js
+-rw-r--r--   0 thibaut    (501) staff       (20)    18439 2024-05-15 17:05:28.000000 amphi-etl-0.3.3/packages/ui-component/style/output.css
+-rw-r--r--   0 thibaut    (501) staff       (20)      277 2024-05-15 16:52:04.000000 amphi-etl-0.3.3/packages/ui-component/tailwind.config.js
+-rw-r--r--   0 thibaut    (501) staff       (20)      620 2024-03-22 18:05:02.000000 amphi-etl-0.3.3/packages/ui-component/tsconfig.json
+-rw-r--r--   0 thibaut    (501) staff       (20)    70461 2024-05-17 20:44:04.000000 amphi-etl-0.3.3/packages/ui-component/tsconfig.tsbuildinfo
+-rw-r--r--   0 thibaut    (501) staff       (20)     2603 2024-05-17 20:43:36.000000 amphi-etl-0.3.3/pyproject.toml
+-rw-r--r--   0 thibaut    (501) staff       (20)       38 2024-05-17 21:32:31.542860 amphi-etl-0.3.3/setup.cfg
+-rw-r--r--   0 thibaut    (501) staff       (20)     1745 2024-05-17 21:32:25.000000 amphi-etl-0.3.3/setup.py
+-rw-r--r--   0 thibaut    (501) staff       (20)       66 2024-03-22 17:55:16.000000 amphi-etl-0.3.3/tsconfig.eslint.json
+-rw-r--r--   0 thibaut    (501) staff       (20)      513 2024-03-22 17:55:16.000000 amphi-etl-0.3.3/tsconfigbase.json
+-rw-r--r--   0 thibaut    (501) staff       (20)   363863 2024-05-17 20:43:49.000000 amphi-etl-0.3.3/yarn.lock
```

### Comparing `amphi-etl-0.3.2/LICENSE` & `amphi-etl-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/MANIFEST.in` & `amphi-etl-0.3.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/PKG-INFO` & `amphi-etl-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amphi-etl
-Version: 0.3.2
+Version: 0.3.3
 Summary: Amphi is a python-based ETL
 Author: Thibaut Gourdel
 Author-email: tgourdel@amphi.ai
 License: Elastic License 2.0 \(ELv2\)
         
         **Acceptance** By using the software, you agree to all of the terms and conditions below.
```

### Comparing `amphi-etl-0.3.2/README.md` & `amphi-etl-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/amphi/theme-light/package.json` & `amphi-etl-0.3.3/amphi/theme-light/package.json`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/amphi/theme-light/static/remoteEntry.0ccbe26ef55bccd7ac39.js` & `amphi-etl-0.3.3/amphi/theme-light/static/remoteEntry.0ccbe26ef55bccd7ac39.js`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/amphi/theme-light/themes/@amphi/theme-light/index.css` & `amphi-etl-0.3.3/amphi/theme-light/themes/@amphi/theme-light/index.css`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/amphi/ui-component/package.json` & `amphi-etl-0.3.3/amphi/ui-component/package.json`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/amphi/ui-component/static/412.3b7ac64a5f90d35edd2b.js` & `amphi-etl-0.3.3/amphi/ui-component/static/412.3b7ac64a5f90d35edd2b.js`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/amphi/ui-component/static/587.6f653927626e1058bf40.js` & `amphi-etl-0.3.3/amphi/ui-component/static/587.6f653927626e1058bf40.js`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/amphi/ui-component/static/599.2ee6f3f059a6e0034cf1.js` & `amphi-etl-0.3.3/amphi/ui-component/static/599.2ee6f3f059a6e0034cf1.js`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/amphi/ui-component/static/remoteEntry.ab3f5768d0a66069663b.js` & `amphi-etl-0.3.3/amphi/ui-component/static/remoteEntry.ab3f5768d0a66069663b.js`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/amphi/ui-component/static/third-party-licenses.json` & `amphi-etl-0.3.3/amphi/ui-component/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/amphi_etl.egg-info/PKG-INFO` & `amphi-etl-0.3.3/amphi_etl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amphi-etl
-Version: 0.3.2
+Version: 0.3.3
 Summary: Amphi is a python-based ETL
 Author: Thibaut Gourdel
 Author-email: tgourdel@amphi.ai
 License: Elastic License 2.0 \(ELv2\)
         
         **Acceptance** By using the software, you agree to all of the terms and conditions below.
```

### Comparing `amphi-etl-0.3.2/amphi_etl.egg-info/SOURCES.txt` & `amphi-etl-0.3.3/amphi_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/config/labconfig/page_config.json` & `amphi-etl-0.3.3/config/labconfig/page_config.json`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/config/settings/overrides.json` & `amphi-etl-0.3.3/config/settings/overrides.json`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/package.json` & `amphi-etl-0.3.3/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.3.3'"}*

```diff
@@ -66,15 +66,15 @@
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md,.yml,.yaml}\"",
         "prettier:check": "jlpm prettier:base --check",
         "quickstart": "npm run setup:py && jlpm && jlpm deduplicate && jlpm clean:all && jlpm lint && jlpm build:prod && jlpm dist && jlpm docs && jlpm test",
         "setup:py": "python -m pip install -e \".[dev,lint,test,docs]\"",
         "test": "jlpm test:py",
         "test:py": "pytest"
     },
-    "version": "0.2.1",
+    "version": "0.3.3",
     "workspaces": {
         "packages": [
             "packages/theme-light",
             "packages/ui-component"
         ]
     }
 }
```

### Comparing `amphi-etl-0.3.2/packages/theme-light/lib/index.js` & `amphi-etl-0.3.3/packages/theme-light/lib/index.js`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/theme-light/package.json` & `amphi-etl-0.3.3/packages/theme-light/package.json`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/theme-light/src/index.ts` & `amphi-etl-0.3.3/packages/theme-light/src/index.ts`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/theme-light/style/index.css` & `amphi-etl-0.3.3/packages/theme-light/style/index.css`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/theme-light/style/variables.css` & `amphi-etl-0.3.3/packages/theme-light/style/variables.css`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/theme-light/tsconfig.tsbuildinfo` & `amphi-etl-0.3.3/packages/theme-light/tsconfig.tsbuildinfo`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/ui-component/lib/BrowseFileDialog.js` & `amphi-etl-0.3.3/packages/ui-component/lib/BrowseFileDialog.js`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/ui-component/lib/Dropzone.d.ts` & `amphi-etl-0.3.3/packages/ui-component/lib/Dropzone.d.ts`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/ui-component/lib/Dropzone.js` & `amphi-etl-0.3.3/packages/ui-component/lib/Dropzone.js`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/ui-component/lib/icons.d.ts` & `amphi-etl-0.3.3/packages/ui-component/lib/icons.d.ts`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/ui-component/lib/icons.js` & `amphi-etl-0.3.3/packages/ui-component/lib/icons.js`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/ui-component/lib/index.js` & `amphi-etl-0.3.3/packages/ui-component/lib/index.js`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/ui-component/lib/launcher.d.ts` & `amphi-etl-0.3.3/packages/ui-component/lib/launcher.d.ts`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/ui-component/lib/launcher.js` & `amphi-etl-0.3.3/packages/ui-component/lib/launcher.js`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/ui-component/package.json` & `amphi-etl-0.3.3/packages/ui-component/package.json`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/ui-component/src/BrowseFileDialog.tsx` & `amphi-etl-0.3.3/packages/ui-component/src/BrowseFileDialog.tsx`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/ui-component/src/Dropzone.tsx` & `amphi-etl-0.3.3/packages/ui-component/src/Dropzone.tsx`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/ui-component/src/icons.ts` & `amphi-etl-0.3.3/packages/ui-component/src/icons.ts`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/ui-component/src/index.ts` & `amphi-etl-0.3.3/packages/ui-component/src/index.ts`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/ui-component/src/launcher.tsx` & `amphi-etl-0.3.3/packages/ui-component/src/launcher.tsx`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/ui-component/style/icons/amphi-square-logo.svg` & `amphi-etl-0.3.3/packages/ui-component/style/icons/amphi-square-logo.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/ui-component/style/icons/amphi-square-logo_nonpaths.svg` & `amphi-etl-0.3.3/packages/ui-component/style/icons/amphi-square-logo_nonpaths.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/ui-component/style/icons/amphi.svg` & `amphi-etl-0.3.3/packages/ui-component/style/icons/amphi.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/ui-component/style/icons/bug-16.svg` & `amphi-etl-0.3.3/packages/ui-component/style/icons/bug-16.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/ui-component/style/icons/bug-24.svg` & `amphi-etl-0.3.3/packages/ui-component/style/icons/bug-24.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/ui-component/style/icons/network-24.svg` & `amphi-etl-0.3.3/packages/ui-component/style/icons/network-24.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/ui-component/style/icons/p5-square-logo.svg` & `amphi-etl-0.3.3/packages/ui-component/style/icons/p5-square-logo.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/ui-component/style/icons/pipeline-16.svg` & `amphi-etl-0.3.3/packages/ui-component/style/icons/pipeline-16.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/ui-component/style/icons/pipeline-24.svg` & `amphi-etl-0.3.3/packages/ui-component/style/icons/pipeline-24.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/ui-component/style/icons/pipeline.svg` & `amphi-etl-0.3.3/packages/ui-component/style/icons/pipeline.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/ui-component/style/icons/pipeline_negative.svg` & `amphi-etl-0.3.3/packages/ui-component/style/icons/pipeline_negative.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/ui-component/style/icons/shield-check-24.svg` & `amphi-etl-0.3.3/packages/ui-component/style/icons/shield-check-24.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/ui-component/style/output.css` & `amphi-etl-0.3.3/packages/ui-component/style/output.css`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/ui-component/tsconfig.json` & `amphi-etl-0.3.3/packages/ui-component/tsconfig.json`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/packages/ui-component/tsconfig.tsbuildinfo` & `amphi-etl-0.3.3/packages/ui-component/tsconfig.tsbuildinfo`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/pyproject.toml` & `amphi-etl-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/setup.py` & `amphi-etl-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     collect_files('amphi', 'share/jupyter/labextensions/@amphi') +
     collect_files('config/labconfig', 'etc/jupyter/labconfig') +
     collect_files('config/settings', 'share/jupyter/lab/settings')
 )
 
 setup(
     name='amphi-etl',
-    version='0.3.2',
+    version='0.3.3',
     description='Open-source and Python-based ETL',
     author='Thibaut Gourdel',
     author_email='tgourdel@amphi.ai',
     license='ELv2',
     install_requires=[
         'jupyterlab>=4.1.5',
         'jupyterlab-amphi>=0.3.1',
```

### Comparing `amphi-etl-0.3.2/tsconfigbase.json` & `amphi-etl-0.3.3/tsconfigbase.json`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.2/yarn.lock` & `amphi-etl-0.3.3/yarn.lock`

 * *Files identical despite different names*

