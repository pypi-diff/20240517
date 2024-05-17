# Comparing `tmp/jupyterlab_new_launcher-0.3.0.tar.gz` & `tmp/jupyterlab_new_launcher-0.3.1.tar.gz`

## Comparing `jupyterlab_new_launcher-0.3.0.tar` & `jupyterlab_new_launcher-0.3.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/.copier-answers.yml
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/babel.config.js
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/jest.config.js
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/junit.xml
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/setup.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/tsconfig.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/tsconfig.test.json
--rw-r--r--   0        0        0   376569 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/yarn.lock
--rw-r--r--   0        0        0    54951 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/docs/images/dialog.png
--rw-r--r--   0        0        0    58321 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/docs/images/launcher.png
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/_version.py
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/labextension/package.json
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/package.json.orig
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/plugin.json
--rw-r--r--   0        0        0    11071 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/labextension/static/728.5be4ee0b94a07decd5f8.js
--rw-r--r--   0        0        0    28571 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/labextension/static/787.d3e306a9eb8983db2644.js
--rw-r--r--   0        0        0     7174 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/labextension/static/remoteEntry.697e41989e560bf8e1db.js
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/labextension/static/style.js
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/schema/plugin.json
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/src/commands.ts
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/src/database.ts
--rw-r--r--   0        0        0     9601 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/src/dialogs.tsx
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/src/icons.ts
--rw-r--r--   0        0        0     6052 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/src/index.ts
--rw-r--r--   0        0        0     4729 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/src/item.ts
--rw-r--r--   0        0        0    10204 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/src/launcher.tsx
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/src/svg.d.ts
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/src/types.ts
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/src/typings.d.ts
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/src/__tests__/jupyterlab_new_launcher.spec.ts
--rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/src/components/base-table.tsx
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/src/components/card.tsx
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/src/components/section.tsx
--rw-r--r--   0        0        0    12213 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/src/components/table.tsx
--rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/style/index.js
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/style/webkit.raw.css
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/style/icons/code-server.svg
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/style/icons/md/LICENSE
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/style/icons/md/file.svg
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/style/icons/md/star.svg
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/ui-tests/playwright.config.js
--rw-r--r--   0        0        0   148126 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/ui-tests/yarn.lock
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts
--rw-r--r--   0        0        0    27608 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-linux.png
--rw-r--r--   0        0        0    28063 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-search-in-individual-linux.png
--rw-r--r--   0        0        0    33928 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-with-starred-linux.png
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/.gitignore
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/LICENSE
--rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/README.md
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/.copier-answers.yml
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/babel.config.js
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/jest.config.js
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/junit.xml
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/setup.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/tsconfig.test.json
+-rw-r--r--   0        0        0   376569 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/yarn.lock
+-rw-r--r--   0        0        0    54951 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/docs/images/dialog.png
+-rw-r--r--   0        0        0    58321 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/docs/images/launcher.png
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/jupyterlab_new_launcher/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/jupyterlab_new_launcher/_version.py
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/jupyterlab_new_launcher/labextension/package.json
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/package.json.orig
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/plugin.json
+-rw-r--r--   0        0        0    11071 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/jupyterlab_new_launcher/labextension/static/728.5be4ee0b94a07decd5f8.js
+-rw-r--r--   0        0        0    28610 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/jupyterlab_new_launcher/labextension/static/787.5cb95a8042fdc8bc6875.js
+-rw-r--r--   0        0        0     7174 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/jupyterlab_new_launcher/labextension/static/remoteEntry.ac4adbf49c65a77e94cf.js
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/jupyterlab_new_launcher/labextension/static/style.js
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/jupyterlab_new_launcher/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/schema/plugin.json
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/src/commands.ts
+-rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/src/database.ts
+-rw-r--r--   0        0        0     9601 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/src/dialogs.tsx
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/src/icons.ts
+-rw-r--r--   0        0        0     6052 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/src/index.ts
+-rw-r--r--   0        0        0     4729 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/src/item.ts
+-rw-r--r--   0        0        0    10204 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/src/launcher.tsx
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/src/svg.d.ts
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/src/types.ts
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/src/typings.d.ts
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/src/__tests__/jupyterlab_new_launcher.spec.ts
+-rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/src/components/base-table.tsx
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/src/components/card.tsx
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/src/components/section.tsx
+-rw-r--r--   0        0        0    12213 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/src/components/table.tsx
+-rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/style/index.js
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/style/webkit.raw.css
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/style/icons/code-server.svg
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/style/icons/md/LICENSE
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/style/icons/md/file.svg
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/style/icons/md/star.svg
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0   148126 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/ui-tests/yarn.lock
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts
+-rw-r--r--   0        0        0    27608 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-linux.png
+-rw-r--r--   0        0        0    28063 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-search-in-individual-linux.png
+-rw-r--r--   0        0        0    33928 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-with-starred-linux.png
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/README.md
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.1/PKG-INFO
```

### Comparing `jupyterlab_new_launcher-0.3.0/.copier-answers.yml` & `jupyterlab_new_launcher-0.3.1/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/RELEASE.md` & `jupyterlab_new_launcher-0.3.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/jest.config.js` & `jupyterlab_new_launcher-0.3.1/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/package.json` & `jupyterlab_new_launcher-0.3.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.3.1'"}*

```diff
@@ -195,9 +195,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.3.0"
+    "version": "0.3.1"
 }
```

### Comparing `jupyterlab_new_launcher-0.3.0/tsconfig.json` & `jupyterlab_new_launcher-0.3.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/yarn.lock` & `jupyterlab_new_launcher-0.3.1/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/docs/images/dialog.png` & `jupyterlab_new_launcher-0.3.1/docs/images/dialog.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/docs/images/launcher.png` & `jupyterlab_new_launcher-0.3.1/docs/images/launcher.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/__init__.py` & `jupyterlab_new_launcher-0.3.1/jupyterlab_new_launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/labextension/package.json` & `jupyterlab_new_launcher-0.3.1/jupyterlab_new_launcher/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9788194444444445%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.ac4adbf49c65a77e94cf.js'}}",*

 * * "'version'": "'0.3.1'"}*

```diff
@@ -108,15 +108,15 @@
         "src/**/*.{ts,tsx}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/nebari-dev/jupyterlab-new-launcher",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.697e41989e560bf8e1db.js",
+            "load": "static/remoteEntry.ac4adbf49c65a77e94cf.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "@jupyterlab/launcher-extension",
             "@jupyterlab/apputils-extension:sessionDialogs"
         ],
         "extension": true,
@@ -200,9 +200,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.3.0"
+    "version": "0.3.1"
 }
```

### Comparing `jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/package.json.orig` & `jupyterlab_new_launcher-0.3.1/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.3.1'"}*

```diff
@@ -195,9 +195,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.3.0"
+    "version": "0.3.1"
 }
```

### Comparing `jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/plugin.json` & `jupyterlab_new_launcher-0.3.1/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/labextension/static/728.5be4ee0b94a07decd5f8.js` & `jupyterlab_new_launcher-0.3.1/jupyterlab_new_launcher/labextension/static/728.5be4ee0b94a07decd5f8.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/labextension/static/787.d3e306a9eb8983db2644.js` & `jupyterlab_new_launcher-0.3.1/jupyterlab_new_launcher/labextension/static/787.5cb95a8042fdc8bc6875.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -6,47 +6,47 @@
                 default: () => V
             });
             var a = n(626),
                 s = n(923),
                 o = n(670),
                 r = n(260),
                 l = n(825),
-                c = n(265),
-                i = n(527),
+                i = n(265),
+                c = n(527),
                 d = n(53),
                 m = n(345),
                 u = n.n(m);
-            const h = new i.LabIcon({
+            const h = new c.LabIcon({
                     name: "jupyterlab-new-launcher:star",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">\n  <path class="jp-icon3 jp-star-filled" fill="rgb(97,97,97)" d="M12 17.27L18.18 21l-1.64-7.03L22 9.24l-7.19-.61L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21z" />\n  <path class="jp-icon3 jp-star-border" fill="rgb(97,97,97)" d="M22 9.24l-7.19-.62L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21 12 17.27 18.18 21l-1.63-7.03L22 9.24zM12 15.4l-3.76 2.27 1-4.28-3.32-2.88 4.38-.38L12 6.1l1.71 4.04 4.38.38-3.32 2.88 1 4.28L12 15.4z" />\n</svg>\n'
                 }),
-                p = new i.LabIcon({
+                p = new c.LabIcon({
                     name: "jupyterlab-new-launcher:file",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">\n  <path class="jp-icon3" fill="rgb(97,97,97)" d="M13.81 22H6C4.89 22 4 21.11 4 20V4C4 2.9 4.89 2 6 2H14L20 8V13.09C19.67 13.04 19.34 13 19 13S18.33 13.04 18 13.09V9H13V4H6V20H13.09C13.21 20.72 13.46 21.39 13.81 22M23 18H20V15H18V18H15V20H18V23H20V20H23V18Z" />\n</svg>'
                 }),
-                g = new i.LabIcon({
+                g = new c.LabIcon({
                     name: "jupyterlab-new-launcher:code-server",
                     svgstr: '<svg width="64" viewBox="0 0 2250 2250" version="1.1" xmlns="http://www.w3.org/2000/svg" style="fill-rule:evenodd;clip-rule:evenodd;stroke-linejoin:round;stroke-miterlimit:2;">\n<g class="jp-icon0" fill="#000" style="fill-rule:nonzero;">\n  <path d="M1991.66,1034.72c-38.493,0 -64.144,-22.57 -64.144,-68.897l-0,-266.084c-0,-169.867 -69.982,-263.709 -250.762,-263.709l-83.976,0l-0,179.368l25.661,0c71.144,0 104.967,39.201 104.967,109.285l0,235.201c0,102.156 30.324,143.733 96.806,165.114c-66.482,20.196 -96.806,62.958 -96.806,165.114l0,174.621c0,48.7 0,96.216 -12.829,144.917c-12.829,45.141 -33.823,87.903 -62.98,124.726c-16.329,21.386 -34.991,39.202 -55.981,55.835l-0,23.755l83.971,-0c180.781,-0 250.763,-93.843 250.763,-263.709l-0,-266.084c-0,-47.516 24.485,-68.897 64.144,-68.897l47.822,-0l-0,-179.37l-46.656,-0l0,-1.186Z"/>\n  <path d="M1420.16,706.904l-258.923,0c-5.833,0 -10.495,-4.752 -10.495,-10.691l-0,-20.192c-0,-5.941 4.662,-10.692 10.495,-10.692l260.089,0c5.83,0 10.495,4.751 10.495,10.692l0,20.192c0,5.939 -5.833,10.691 -11.661,10.691Z" />\n  <path d="M1464.48,963.474l-188.942,0c-5.833,0 -10.501,-4.754 -10.501,-10.693l0,-20.192c0,-5.938 4.668,-10.691 10.501,-10.691l188.942,-0c5.833,-0 10.495,4.753 10.495,10.691l-0,20.192c-0,4.754 -4.662,10.693 -10.495,10.693Z"/>\n  <path d="M1539.12,835.188l-377.885,0c-5.833,0 -10.495,-4.75 -10.495,-10.689l-0,-20.196c-0,-5.939 4.662,-10.69 10.495,-10.69l376.719,0c5.833,0 10.499,4.751 10.499,10.69l-0,20.196c-0,4.75 -3.5,10.689 -9.333,10.689Z"/>\n  <path d="M861.493,765.074c25.658,0 51.319,2.376 75.811,8.316l0,-48.705c0,-68.897 34.989,-109.285 104.971,-109.285l25.658,0l-0,-179.368l-83.977,0c-180.781,0 -250.758,93.842 -250.758,263.709l0,87.901c40.819,-14.252 83.977,-22.568 128.295,-22.568Z"/>\n  <path d="M1618.44,1411.25c-18.662,-150.861 -132.962,-276.776 -279.919,-305.285c-40.818,-8.314 -81.642,-9.504 -121.295,-2.376c-1.166,-0 -1.166,-1.189 -2.332,-1.189c-64.148,-136.605 -201.772,-226.884 -351.063,-226.884c-149.289,-0 -285.747,87.905 -351.062,224.51c-1.166,-0 -1.166,1.188 -2.332,1.188c-41.987,-4.753 -83.975,-2.379 -125.963,8.314c-144.623,35.634 -254.257,159.175 -274.085,308.847c-2.332,15.441 -3.499,30.883 -3.499,45.141c0,45.136 30.325,86.713 74.645,92.652c54.817,8.317 102.636,-34.448 101.469,-89.089c0,-8.317 0,-17.821 1.167,-26.134c9.331,-76.025 66.48,-140.168 141.123,-157.99c23.328,-5.939 46.654,-7.124 68.814,-3.559c71.146,9.502 141.124,-27.324 171.449,-91.467c22.162,-47.516 57.151,-89.094 103.804,-111.664c51.314,-24.946 109.633,-28.506 163.286,-9.499c55.979,20.192 97.966,62.954 123.627,116.409c26.824,52.27 39.653,89.093 96.805,96.221c23.325,3.559 88.639,2.374 113.132,1.185c47.82,0 95.64,16.631 129.463,51.079c22.156,23.757 38.485,53.455 45.486,86.715c10.495,53.455 -2.334,106.908 -33.825,147.296c-22.162,28.509 -52.485,49.89 -86.308,59.394c-16.329,4.754 -32.657,5.939 -48.986,5.939l-257.757,0c-51.314,0 -92.138,-41.573 -92.138,-93.842l0,-348.049c0,-14.251 -11.661,-26.13 -25.658,-26.13l-36.156,0c-71.148,1.185 -128.295,81.964 -128.295,167.488l-0,312.415c-0,92.652 73.476,167.488 164.451,167.488c0,0 404.714,-1.19 410.544,-1.19c93.304,-9.503 179.614,-58.204 237.927,-133.04c58.319,-72.46 85.142,-167.492 73.481,-264.894Z"/>\n</g></svg>'
                 });
             var v = n(602);
             class f {
                 constructor(e) {
                     var t, n, a, s, o;
                     this._options = e, this._refreshLastUsed = new v.Signal(this), this._refreshClock = null, this._lastUsed = null;
                     const {
                         item: r,
                         commands: l,
-                        lastUsedDatabase: c,
-                        favoritesDatabase: i,
+                        lastUsedDatabase: i,
+                        favoritesDatabase: c,
                         cwd: d
                     } = e, m = {
                         ...r.args,
                         cwd: d
                     };
-                    this.command = r.command, this.args = m, this.category = r.category, this.rank = r.rank, this.kernelIconUrl = r.kernelIconUrl, this.metadata = null !== (t = r.metadata) && void 0 !== t ? t : {}, this.iconClass = l.iconClass(r.command, m), this.icon = l.icon(r.command, m), this.caption = l.caption(r.command, m), this.label = l.label(r.command, m), this.lastUsed = c.get(r), this.starred = null !== (n = i.get(r)) && void 0 !== n && n;
+                    this.command = r.command, this.args = m, this.category = r.category, this.rank = r.rank, this.kernelIconUrl = r.kernelIconUrl, this.metadata = null !== (t = r.metadata) && void 0 !== t ? t : {}, this.iconClass = l.iconClass(r.command, m), this.icon = l.icon(r.command, m), this.caption = l.caption(r.command, m), this.label = l.label(r.command, m), this.lastUsed = i.get(r), this.starred = null !== (n = c.get(r)) && void 0 !== n && n;
                     const u = this.metadata.kernel;
                     if (u) {
                         const e = (null !== (a = u.conda_env_name) && void 0 !== a ? a : "").match(/(?<namespace>.+)-(?<duplicate>\1)-(?<environment>.+)/);
                         if (e && this.metadata) {
                             const t = e.groups;
                             this.label = null !== (s = u.conda_language) && void 0 !== s ? s : t.environment, this.metadata = {
                                 ...this.metadata,
@@ -116,27 +116,27 @@
                     a = e.rows.sort(((e, a) => {
                         var s;
                         return (null !== (s = n(e.data, a.data)) && void 0 !== s ? s : 0) * t.sortDirection
                     }))
                 }
                 const o = e.columns.filter((e => (!e.isAvailable || e.isAvailable()) && !e.isHidden)),
                     [r, l] = u().useState({}),
-                    c = a.map((t => {
+                    i = a.map((t => {
                         const n = o.map((e => u().createElement("td", {
                             key: e.id + "-" + t.key,
                             className: r[e.id] ? "jp-mod-col-resized" : ""
                         }, e.renderCell(t.data))));
                         return u().createElement("tr", {
                             key: t.key,
                             "data-key": t.key,
                             onClick: e.onRowClick,
                             className: "jp-sortable-table-tr"
                         }, n)
                     })),
-                    i = o.map((e => u().createElement(y, {
+                    c = o.map((e => u().createElement(y, {
                         label: e.label,
                         id: e.id,
                         state: t,
                         key: e.id,
                         onSort: () => {
                             var a;
                             (a = e.id) === t.sortKey ? n({
@@ -155,24 +155,24 @@
                         },
                         minWidth: e.minWidth
                     })));
                 return u().createElement("table", {
                     className: _
                 }, u().createElement("thead", null, u().createElement("tr", {
                     className: "jp-sortable-table-tr"
-                }, i)), u().createElement("tbody", null, c))
+                }, c)), u().createElement("tbody", null, i))
             }
 
             function y(e) {
                 var t;
                 const n = e.id === e.state.sortKey,
-                    a = n && 1 !== e.state.sortDirection ? i.caretDownIcon : i.caretUpIcon,
+                    a = n && 1 !== e.state.sortDirection ? c.caretDownIcon : c.caretUpIcon,
                     [s, o] = u().useState(null),
                     r = u().useRef(null),
-                    [l, c] = u().useState(!1),
+                    [l, i] = u().useState(!1),
                     [d, h] = (0, m.useState)(null);
                 requestAnimationFrame((() => {
                     if (r.current) {
                         const {
                             left: e
                         } = r.current.getBoundingClientRect();
                         h(e)
@@ -185,15 +185,15 @@
                                     if (!r.current) throw Error("Cannot resize: no reference to the current table");
                                     console.warn("Resize cache for column was not available"), n = r.current.getBoundingClientRect().left
                                 } else n = d;
                                 o(t.clientX - n), e.onResize()
                             }
                         },
                         n = e => {
-                            l && (document.body.classList.remove(v), c(!1), e.stopImmediatePropagation())
+                            l && (document.body.classList.remove(v), i(!1), e.stopImmediatePropagation())
                         };
                     return document.body.addEventListener("pointermove", t), document.body.addEventListener("pointerup", n), () => {
                         document.body.removeEventListener("pointermove", t), document.body.removeEventListener("pointerup", n)
                     }
                 }));
                 const p = [];
                 n && p.push("jp-sorted-header"), l && p.push("jp-header-resizing");
@@ -205,15 +205,15 @@
                     onClick: () => e.onSort(),
                     className: p.join(" "),
                     "data-id": e.id,
                     style: {
                         width: null !== s ? `${Math.max(null!==(t=e.minWidth)&&void 0!==t?t:50,s)}px` : ""
                     },
                     onPointerDown: e => {
-                        e.target instanceof HTMLElement && e.target.className === g && (document.body.classList.add(v), c(!0))
+                        e.target instanceof HTMLElement && e.target.className === g && (document.body.classList.add(v), i(!0))
                     }
                 }, u().createElement("div", {
                     className: "jp-sortable-table-th-wrapper"
                 }, u().createElement("label", null, e.label), u().createElement(a.react, {
                     tag: "span",
                     className: "jp-sort-icon"
                 })), u().createElement("div", {
@@ -260,16 +260,16 @@
 
             function I(e) {
                 var t, n, a, s;
                 const {
                     trans: o
                 } = e;
                 let r, l;
-                const [c, d] = m.useState("");
-                e.showSearchBox ? (r = c, l = d) : r = e.query;
+                const [i, d] = m.useState("");
+                e.showSearchBox ? (r = i, l = d) : r = e.query;
                 const [, u] = m.useReducer((e => e + 1), 0), p = new Set;
                 for (const n of e.items) {
                     const e = null === (t = n.metadata) || void 0 === t ? void 0 : t.kernel;
                     if (e)
                         for (const t of Object.keys(e)) p.add(t)
                 }
                 const g = [...p].map((e => ({
@@ -285,16 +285,16 @@
                         })())
                     },
                     sort: (t, n) => {
                         var a, s;
                         const o = null === (a = t.metadata) || void 0 === a ? void 0 : a.kernel,
                             r = null === (s = n.metadata) || void 0 === s ? void 0 : s.kernel,
                             l = o ? o[e] : void 0,
-                            c = r ? r[e] : void 0;
-                        return l === c ? 0 : l ? c ? "string" == typeof l && "string" == typeof c ? l.localeCompare(c) : l > c ? 1 : -1 : -1 : 1
+                            i = r ? r[e] : void 0;
+                        return l === i ? 0 : l ? i ? "string" == typeof l && "string" == typeof i ? l.localeCompare(i) : l > i ? 1 : -1 : -1 : 1
                     }
                 })));
                 e.showWidgetType && g.push({
                     id: "widget-type",
                     label: o.__("Type"),
                     renderCell: e => e.command.split(":")[0],
                     sort: (e, t) => e.command.localeCompare(t.command)
@@ -323,26 +323,26 @@
                         }, t.label[0].toUpperCase())), m.createElement("span", {
                             className: "jp-TableKernelItem-label"
                         }, t.label))),
                         sort: (e, t) => e.label.localeCompare(t.label)
                     }, ...g, {
                         id: "last-used",
                         label: o.__("Last Used"),
-                        renderCell: e => m.createElement(i.UseSignal, {
+                        renderCell: e => m.createElement(c.UseSignal, {
                             signal: e.refreshLastUsed
                         }, (() => m.createElement(S, {
                             title: e.lastUsed ? b.Time.format(e.lastUsed) : o.__("No information about last use of this kernel is available in the layout database")
                         }, e.lastUsed ? b.Time.formatHuman(e.lastUsed) : o.__("Never")))),
                         sort: (e, t) => e.lastUsed === t.lastUsed ? 0 : e.lastUsed ? t.lastUsed && e.lastUsed > t.lastUsed ? 1 : -1 : 1
                     }, {
                         id: "star",
                         label: "",
                         renderCell: e => {
                             const t = e.starred,
-                                n = t ? o.__("Click to add this kernel to favourites") : o.__("Click to remove the kernel from favourites");
+                                n = t ? o.__("Click to remove the kernel from favourites") : o.__("Click to add this kernel to favourites");
                             return m.createElement("button", {
                                 className: t ? `${D} jp-mod-starred` : D,
                                 title: n,
                                 onClick: t => {
                                     e.toggleStar(), u(), t.stopPropagation()
                                 }
                             }, m.createElement(h.react, {
@@ -366,30 +366,30 @@
                     };
                 return m.useEffect((() => (e.settings.changed.connect(x), () => {
                     e.settings.changed.disconnect(x)
                 }))), m.createElement("div", {
                     className: "jp-NewLauncher-table"
                 }, e.showSearchBox ? m.createElement("div", {
                     className: "jp-Launcher-searchBox"
-                }, m.createElement(i.FilterBox, {
+                }, m.createElement(c.FilterBox, {
                     placeholder: o.__("Filter kernels"),
                     updateFilter: (e, t) => {
                         l(null != t ? t : "")
                     },
                     initialQuery: "",
                     useFuzzyFilter: !1
                 })) : null, m.createElement("div", {
                     className: "jp-NewLauncher-table-scroller",
                     onContextMenu: t => {
                         var n;
                         t.preventDefault();
-                        const a = new i.MenuSvg({
+                        const a = new c.MenuSvg({
                                 commands: e.commands
                             }),
-                            s = new i.MenuSvg({
+                            s = new c.MenuSvg({
                                 commands: e.commands
                             });
                         for (const e of _) s.addItem({
                             command: E.toggleColumn,
                             args: {
                                 id: e.id,
                                 label: e.label
@@ -444,59 +444,60 @@
 
             function U(e) {
                 const [t, n] = m.useState(e.open);
                 return m.createElement("details", {
                     onToggle: t => {
                         n(t.currentTarget.open), e.onToggled && e.onToggled(t.currentTarget.open)
                     },
-                    className: (0, i.classes)(e.className, "jp-CollapsibleSection"),
+                    className: (0, c.classes)(e.className, "jp-CollapsibleSection"),
                     open: t
                 }, m.createElement("summary", null, m.createElement("div", {
                     className: "jp-CollapsibleSection-CollapserIconWrapper",
                     "aria-hidden": "true"
-                }, m.createElement(i.caretRightIcon.react, {
+                }, m.createElement(c.caretRightIcon.react, {
                     className: "jp-CollapsibleSection-CollapserIcon"
                 })), m.createElement(e.icon.react, {
                     tag: "span",
                     className: "jp-CollapsibleSection-CategoryIcon"
                 }), m.createElement("h3", {
                     className: "jp-CollapsibleSection-Title"
                 }, e.title)), m.createElement("div", {
                     className: "jp-Launcher-CardGroup jp-Launcher-cardContainer"
                 }, e.children))
             }
 
             function x(e) {
+                var t;
                 const {
-                    item: t
+                    item: n
                 } = e;
                 return m.createElement("div", {
-                    onClick: () => t.execute(),
+                    onClick: () => n.execute(),
                     className: "jp-Launcher-TypeCard jp-LauncherCard",
-                    title: t.caption,
+                    title: null !== (t = n.caption) && void 0 !== t ? t : n.label,
                     tabIndex: 0
                 }, m.createElement("div", {
                     className: "jp-LauncherCard-icon"
-                }, m.createElement(i.LabIcon.resolveReact, {
-                    icon: t.icon,
-                    iconClass: (0, i.classes)(t.iconClass, "jp-Icon-cover")
+                }, m.createElement(c.LabIcon.resolveReact, {
+                    icon: n.icon,
+                    iconClass: (0, c.classes)(n.iconClass, "jp-Icon-cover")
                 })), m.createElement("div", {
                     className: "jp-LauncherCard-label"
-                }, m.createElement("p", null, t.label)))
+                }, m.createElement("p", null, n.label)))
             }
 
             function B(e) {
                 var t;
                 const {
                     trans: n,
                     cwd: a,
                     typeItems: s,
                     otherItems: o,
                     favouritesChanged: r
-                } = e, [l, c] = m.useState(""), [, d] = m.useReducer((e => e + 1), 0), [u, g] = m.useState(e.settings.composite.starredSection), [v, f] = m.useState(e.settings.composite.searchAllSections), b = () => {
+                } = e, [l, i] = m.useState(""), [, d] = m.useReducer((e => e + 1), 0), [u, g] = m.useState(e.settings.composite.starredSection), [v, f] = m.useState(e.settings.composite.searchAllSections), b = () => {
                     const t = e.settings.composite.starredSection;
                     u !== t && g(t);
                     const n = e.settings.composite.searchAllSections;
                     v !== n && f(n)
                 };
                 if (m.useEffect((() => (e.settings.changed.connect(b), () => {
                         e.settings.changed.disconnect(b)
@@ -525,18 +526,18 @@
                 }, m.createElement("h3", null, n.__("Current folder:"), " ", m.createElement("code", null, a || "/"))), m.createElement("div", {
                     className: "jp-NewLauncher-OtherItems"
                 }, o.map((e => m.createElement(x, {
                     item: e,
                     trans: n
                 }))))), v ? m.createElement("div", {
                     className: "jp-Launcher-searchBox"
-                }, m.createElement(i.FilterBox, {
+                }, m.createElement(c.FilterBox, {
                     placeholder: n.__("Filter"),
                     updateFilter: (e, t) => {
-                        c(null != t ? t : "")
+                        i(null != t ? t : "")
                     },
                     initialQuery: "",
                     useFuzzyFilter: !1
                 })) : null, m.createElement(U, {
                     className: "jp-Launcher-openByType",
                     title: n.__("Create Empty"),
                     icon: p,
@@ -557,28 +558,28 @@
                     query: l,
                     settings: e.settings,
                     trans: n,
                     onClick: e => e.execute()
                 }) : "No starred items") : null, m.createElement(U, {
                     className: "jp-Launcher-openByKernel jp-Launcher-launchNotebook",
                     title: n.__("Launch New Notebook"),
-                    icon: i.notebookIcon,
+                    icon: c.notebookIcon,
                     open: "collapsed" !== y["launch-notebook"]
                 }, m.createElement(I, {
                     items: e.notebookItems,
                     commands: e.commands,
                     showSearchBox: !v,
                     query: l,
                     settings: e.settings,
                     trans: n,
                     onClick: e => e.execute()
                 })), m.createElement(U, {
                     className: "jp-Launcher-openByKernel jp-Launcher-launchConsole",
                     title: n.__("Launch New Console"),
-                    icon: i.consoleIcon,
+                    icon: c.consoleIcon,
                     open: "collapsed" !== y["launch-console"]
                 }, m.createElement(I, {
                     items: e.consoleItems,
                     commands: e.commands,
                     showSearchBox: !v,
                     query: l,
                     settings: e.settings,
@@ -603,33 +604,33 @@
                         t = [...this.model.items()],
                         n = e.__("Notebook"),
                         a = e.__("Console"),
                         s = [n, a],
                         o = this._settings.composite.utilityCommands,
                         r = t.filter((e => o.includes(e.command))).map(this.renderCommand),
                         l = t.filter((e => (!e.category || !s.includes(e.category)) && !o.includes(e.command) || e.command === K)),
-                        c = {
+                        i = {
                             "terminal:create-new": 3,
                             "fileeditor:create-new": 6,
                             "fileeditor:create-new-markdown-file": 5
                         };
-                    for (const e of l) e.command in c && (e.rank = c[e.command]);
-                    const i = [{
+                    for (const e of l) e.command in i && (e.rank = i[e.command]);
+                    const c = [{
                             command: "notebook:create-new",
                             rank: 1
                         }, {
                             command: "console:create",
                             rank: 4
                         }, ...l].sort(((e, t) => {
                             var n, a;
                             return (null !== (n = null == e ? void 0 : e.rank) && void 0 !== n ? n : 0) - (null !== (a = null == t ? void 0 : t.rank) && void 0 !== a ? a : 0)
                         })),
                         d = t.filter((e => e.category && e.category === n && e.command !== K)).map(this.renderKernelCommand),
                         u = t.filter((e => e.category && e.category === a && e.command !== K)).map(this.renderKernelCommand),
-                        h = i.map(this.renderCommand);
+                        h = c.map(this.renderCommand);
                     return m.createElement(B, {
                         trans: this.trans,
                         cwd: this.cwd,
                         commands: this.commands,
                         typeItems: h,
                         notebookItems: d,
                         consoleItems: u,
@@ -639,15 +640,15 @@
                     })
                 }
             }
             class A extends s.SessionContextDialogs {
                 constructor(e) {
                     var t;
                     super(e), this.options = e;
-                    const n = null !== (t = e.translator) && void 0 !== t ? t : c.nullTranslator;
+                    const n = null !== (t = e.translator) && void 0 !== t ? t : i.nullTranslator;
                     this.trans = n.load("jupyterlab")
                 }
                 async selectKernel(e) {
                     const t = this.trans;
                     if (e.isDisposed) return Promise.resolve();
                     let n = t.__("Cancel");
                     e.hasNoKernel && (n = e.kernelDisplayName);
@@ -657,57 +658,57 @@
                             label: t.__("Select"),
                             ariaLabel: t.__("Select Kernel"),
                             className: "jp-KernelSelector-SelectButton"
                         })],
                         o = e.kernelPreference.autoStartDefault,
                         r = "boolean" == typeof o,
                         l = await this.options.settingRegistry.load(k),
-                        c = new s.Dialog({
+                        i = new s.Dialog({
                             title: t.__("Select Kernel"),
                             body: new R({
                                 data: {
                                     specs: e.specsManager.specs,
                                     sessions: e.sessionManager.running(),
                                     preference: e.kernelPreference
                                 },
                                 name: e.name,
                                 commands: this.options.commands,
                                 favoritesDatabase: this.options.database.favorites,
                                 lastUsedDatabase: this.options.database.lastUsed,
                                 settings: l,
                                 trans: t,
                                 acceptDialog: () => {
-                                    c.resolve(1)
+                                    i.resolve(1)
                                 }
                             }),
                             buttons: a,
                             checkbox: r ? {
                                 label: t.__("Always start the preferred kernel"),
                                 caption: t.__("Remember my choice and always start the preferred kernel"),
                                 checked: o
                             } : null
                         });
-                    c.node.classList.add("jp-KernelSelector-Dialog");
-                    const i = await c.launch();
-                    if (e.isDisposed || !i.button.accept) return;
-                    r && null !== i.isChecked && (e.kernelPreference = {
+                    i.node.classList.add("jp-KernelSelector-Dialog");
+                    const c = await i.launch();
+                    if (e.isDisposed || !c.button.accept) return;
+                    r && null !== c.isChecked && (e.kernelPreference = {
                         ...e.kernelPreference,
-                        autoStartDefault: i.isChecked
+                        autoStartDefault: c.isChecked
                     });
-                    const d = i.value;
+                    const d = c.value;
                     if (null === d && !e.hasNoKernel) return e.shutdown();
                     d && await e.changeKernel(d)
                 }
             }
             const M = {
                 id: "jupyterlab-new-launcher:dialogs",
                 description: "Session dialogs for redesigned JupyterLab launcher",
                 provides: s.ISessionContextDialogs,
                 autoStart: !0,
-                requires: [c.ITranslator, j, l.ISettingRegistry],
+                requires: [i.ITranslator, j, l.ISettingRegistry],
                 activate: (e, t, n, a) => new A({
                     translator: t,
                     database: n,
                     commands: e.commands,
                     settingRegistry: a
                 })
             };
@@ -880,17 +881,17 @@
                     }
                 },
                 V = [{
                     id: k,
                     description: "A redesigned JupyterLab launcher",
                     provides: r.ILauncher,
                     autoStart: !0,
-                    requires: [c.ITranslator, l.ISettingRegistry, j],
+                    requires: [i.ITranslator, l.ISettingRegistry, j],
                     optional: [a.ILabShell, s.ICommandPalette, o.IDefaultFileBrowser],
-                    activate: function(e, t, n, a, o, l, c) {
+                    activate: function(e, t, n, a, o, l, i) {
                         const {
                             commands: m,
                             shell: u
                         } = e, h = t.load("jupyterlab-new-launcher"), p = new r.LauncherModel;
                         if (-1 !== navigator.userAgent.indexOf("AppleWebKit") && -1 === navigator.userAgent.indexOf("Chrome")) {
                             const e = function(e) {
                                 const t = document.createElement("style");
@@ -933,18 +934,18 @@
                                         const r = t[o];
                                         t[o] = a, t[s] = r, await n.set("columnOrder", t)
                                     }
                                 })
                             }(e, h, t)
                         })), m.addCommand(E.create, {
                             label: h.__("New Launcher"),
-                            icon: e => e.toolbar ? i.addIcon : void 0,
+                            icon: e => e.toolbar ? c.addIcon : void 0,
                             execute: async e => {
                                 var r, l;
-                                const g = null !== (l = null !== (r = e.cwd) && void 0 !== r ? r : null == c ? void 0 : c.model.path) && void 0 !== l ? l : "",
+                                const g = null !== (l = null !== (r = e.cwd) && void 0 !== r ? r : null == i ? void 0 : i.model.path) && void 0 !== l ? l : "",
                                     v = "launcher-" + W.id++,
                                     f = await n.load(k);
                                 await Promise.all([a.lastUsed.ready, a.favorites.ready]);
                                 const b = new T({
                                     model: p,
                                     cwd: g,
                                     callback: e => {
@@ -954,34 +955,34 @@
                                     },
                                     commands: m,
                                     translator: t,
                                     lastUsedDatabase: a.lastUsed,
                                     favoritesDatabase: a.favorites,
                                     settings: f
                                 });
-                                b.model = p, b.title.icon = i.launcherIcon, b.title.label = h.__("Launcher");
+                                b.model = p, b.title.icon = c.launcherIcon, b.title.label = h.__("Launcher");
                                 const _ = new s.MainAreaWidget({
                                     content: b
                                 });
                                 if (_.title.closable = !!Array.from(u.widgets("main")).length, _.id = v, u.add(_, "main", {
                                         activate: e.activate,
                                         ref: e.ref
                                     }), o && o.layoutModified.connect((() => {
                                         _.title.closable = Array.from(o.widgets("main")).length > 1
-                                    }), _), c) {
+                                    }), _), i) {
                                     const e = e => {
                                         b.cwd = e.path
                                     };
-                                    c.model.pathChanged.connect(e), b.disposed.connect((() => {
-                                        c.model.pathChanged.disconnect(e)
+                                    i.model.pathChanged.connect(e), b.disposed.connect((() => {
+                                        i.model.pathChanged.disconnect(e)
                                     }))
                                 }
                                 return _
                             }
-                        }), o && Promise.all([e.restored, null == c ? void 0 : c.model.restored]).then((() => {
+                        }), o && Promise.all([e.restored, null == i ? void 0 : i.model.restored]).then((() => {
                             o.layoutModified.connect((() => {
                                 o.isEmpty("main") && m.execute(E.create)
                             }))
                         })), l && l.addItem({
                             command: E.create,
                             category: h.__("Launcher")
                         }), o && (o.addButtonEnabled = !0, o.addRequested.connect(((e, t) => {
```

### Comparing `jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/labextension/static/remoteEntry.697e41989e560bf8e1db.js` & `jupyterlab_new_launcher-0.3.1/jupyterlab_new_launcher/labextension/static/remoteEntry.ac4adbf49c65a77e94cf.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -44,18 +44,18 @@
     }, m.d = (e, r) => {
         for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
         728: "5be4ee0b94a07decd5f8",
-        787: "d3e306a9eb8983db2644"
+        787: "5cb95a8042fdc8bc6875"
     } [e] + ".js?v=" + {
         728: "5be4ee0b94a07decd5f8",
-        787: "d3e306a9eb8983db2644"
+        787: "5cb95a8042fdc8bc6875"
     } [e], m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -106,15 +106,15 @@
                     var a = o[e] = o[e] || {},
                         u = a[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (a[r] = {
                         get: () => m.e(787).then((() => () => m(787))),
                         from: i,
                         eager: !1
                     })
-                })("jupyterlab-new-launcher", "0.3.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("jupyterlab-new-launcher", "0.3.1"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         m.g.importScripts && (e = m.g.location + "");
         var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/labextension/static/third-party-licenses.json` & `jupyterlab_new_launcher-0.3.1/jupyterlab_new_launcher/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/schema/plugin.json` & `jupyterlab_new_launcher-0.3.1/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/src/commands.ts` & `jupyterlab_new_launcher-0.3.1/src/commands.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/src/database.ts` & `jupyterlab_new_launcher-0.3.1/src/database.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/src/dialogs.tsx` & `jupyterlab_new_launcher-0.3.1/src/dialogs.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/src/icons.ts` & `jupyterlab_new_launcher-0.3.1/src/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/src/index.ts` & `jupyterlab_new_launcher-0.3.1/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/src/item.ts` & `jupyterlab_new_launcher-0.3.1/src/item.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/src/launcher.tsx` & `jupyterlab_new_launcher-0.3.1/src/launcher.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/src/types.ts` & `jupyterlab_new_launcher-0.3.1/src/types.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/src/components/base-table.tsx` & `jupyterlab_new_launcher-0.3.1/src/components/base-table.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/src/components/card.tsx` & `jupyterlab_new_launcher-0.3.1/src/components/card.tsx`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   item: IItem;
 }): React.ReactElement {
   const { item } = props;
   return (
     <div
       onClick={() => item.execute()}
       className="jp-Launcher-TypeCard jp-LauncherCard"
-      title={item.caption}
+      title={item.caption ?? item.label}
       tabIndex={0}
     >
       <div className="jp-LauncherCard-icon">
         <LabIcon.resolveReact
           icon={item.icon}
           iconClass={classes(item.iconClass, 'jp-Icon-cover')}
         />
```

### Comparing `jupyterlab_new_launcher-0.3.0/src/components/section.tsx` & `jupyterlab_new_launcher-0.3.1/src/components/section.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/src/components/table.tsx` & `jupyterlab_new_launcher-0.3.1/src/components/table.tsx`

 * *Files 0% similar despite different names*

```diff
@@ -226,16 +226,16 @@
     },
     {
       id: 'star',
       label: '',
       renderCell: (row: IKernelItem) => {
         const starred = row.starred;
         const title = starred
-          ? trans.__('Click to add this kernel to favourites')
-          : trans.__('Click to remove the kernel from favourites');
+          ? trans.__('Click to remove the kernel from favourites')
+          : trans.__('Click to add this kernel to favourites');
         return (
           <button
             className={
               starred
                 ? `${STAR_BUTTON_CLASS} jp-mod-starred`
                 : STAR_BUTTON_CLASS
             }
```

### Comparing `jupyterlab_new_launcher-0.3.0/style/base.css` & `jupyterlab_new_launcher-0.3.1/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/style/icons/code-server.svg` & `jupyterlab_new_launcher-0.3.1/style/icons/code-server.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/style/icons/md/LICENSE` & `jupyterlab_new_launcher-0.3.1/style/icons/md/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/ui-tests/README.md` & `jupyterlab_new_launcher-0.3.1/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/ui-tests/yarn.lock` & `jupyterlab_new_launcher-0.3.1/ui-tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts` & `jupyterlab_new_launcher-0.3.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-linux.png` & `jupyterlab_new_launcher-0.3.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-search-in-individual-linux.png` & `jupyterlab_new_launcher-0.3.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-search-in-individual-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-with-starred-linux.png` & `jupyterlab_new_launcher-0.3.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-with-starred-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/.gitignore` & `jupyterlab_new_launcher-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/LICENSE` & `jupyterlab_new_launcher-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/README.md` & `jupyterlab_new_launcher-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/pyproject.toml` & `jupyterlab_new_launcher-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.0/PKG-INFO` & `jupyterlab_new_launcher-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab-new-launcher
-Version: 0.3.0
+Version: 0.3.1
 Dynamic: Keywords
 Summary: A redesigned JupyterLab launcher
 Project-URL: Homepage, https://github.com/nebari-dev/jupyterlab-new-launcher
 Project-URL: Bug Tracker, https://github.com/nebari-dev/jupyterlab-new-launcher/issues
 Project-URL: Repository, https://github.com/nebari-dev/jupyterlab-new-launcher.git
 Author-email: Nebari development team <internal-it@quansight.com>
 License: BSD 3-Clause License
```

