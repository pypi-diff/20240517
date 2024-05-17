# Comparing `tmp/jupyterlab_amphi-0.3.1.tar.gz` & `tmp/jupyterlab_amphi-0.3.2.tar.gz`

## Comparing `jupyterlab_amphi-0.3.1.tar` & `jupyterlab_amphi-0.3.2.tar`

### file list

```diff
@@ -1,152 +1,176 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/.yarnrc.yml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/MANIFEST.in
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/install.json
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/lerna.json
--rw-r--r--   0        0        0    61977 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/output.json
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/package.json
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/setup.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/tsconfig.eslint.json
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/tsconfigbase.json
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/_version.py
--rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-components-core/package.json
--rw-r--r--   0        0        0   126178 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-components-core/static/116.dc942167424d534a54cf.js
--rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-components-core/static/432.0fc640989ce2150a2305.js
--rw-r--r--   0        0        0    22345 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-components-core/static/518.f70a8c5cdb51fc55b510.js
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-components-core/static/518.f70a8c5cdb51fc55b510.js.LICENSE.txt
--rw-r--r--   0        0        0  1441744 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-components-core/static/687.e7ca374e7abf95457733.js
--rw-r--r--   0        0        0    35011 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-components-core/static/687.e7ca374e7abf95457733.js.LICENSE.txt
--rw-r--r--   0        0        0   542717 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js.LICENSE.txt
--rw-r--r--   0        0        0     7743 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-components-core/static/remoteEntry.364ddb190429da413754.js
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-components-core/static/style.js
--rw-r--r--   0        0        0   120113 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-components-core/static/third-party-licenses.json
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-components-manager/package.json
--rw-r--r--   0        0        0    26319 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-components-manager/static/104.3af22153a88493318436.js
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-components-manager/static/104.3af22153a88493318436.js.LICENSE.txt
--rw-r--r--   0        0        0    34980 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-components-manager/static/12.e1b4412a18535c560cd1.js
--rw-r--r--   0        0        0  1438322 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-components-manager/static/215.6a0c4411afe41a8a55f3.js
--rw-r--r--   0        0        0    30779 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-components-manager/static/215.6a0c4411afe41a8a55f3.js.LICENSE.txt
--rw-r--r--   0        0        0    61091 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-components-manager/static/271.3095f6e27a6de7c0174d.js
--rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-components-manager/static/432.1d493bea1143efe37c80.js
--rw-r--r--   0        0        0    15919 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-components-manager/static/454.b60aaa09eed0e7e4a124.js
--rw-r--r--   0        0        0   150147 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js.LICENSE.txt
--rw-r--r--   0        0        0   439969 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-components-manager/static/841.17235cce88409653d379.js
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-components-manager/static/841.17235cce88409653d379.js.LICENSE.txt
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js.LICENSE.txt
--rw-r--r--   0        0        0    56317 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-components-manager/static/853.805d852640d3676b903b.js
--rw-r--r--   0        0        0     9017 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-components-manager/static/remoteEntry.d25d5d91895e4e9316a4.js
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-components-manager/static/style.js
--rw-r--r--   0        0        0   140477 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-components-manager/static/third-party-licenses.json
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-editor/package.json
--rw-r--r--   0        0        0   152553 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js.LICENSE.txt
--rw-r--r--   0        0        0    32937 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-editor/static/412.66f905f315771e1a5d8b.js
--rw-r--r--   0        0        0    27297 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-editor/static/550.025783cb8476390cbadc.js
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-editor/static/631.20cdac1e84cf987a8781.js
--rw-r--r--   0        0        0  1447449 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-editor/static/735.3ffb88e804cafc3e8a8e.js
--rw-r--r--   0        0        0    36421 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-editor/static/735.3ffb88e804cafc3e8a8e.js.LICENSE.txt
--rw-r--r--   0        0        0     8701 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-editor/static/remoteEntry.12b3539515ec33e9f21c.js
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-editor/static/style.js
--rw-r--r--   0        0        0   118882 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-editor/static/third-party-licenses.json
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-log-console/package.json
--rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-log-console/static/432.8cef2a53e7a2500faa84.js
--rw-r--r--   0        0        0   751763 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-log-console/static/595.19f08543072c216d8a5f.js
--rw-r--r--   0        0        0    13950 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-log-console/static/595.19f08543072c216d8a5f.js.LICENSE.txt
--rw-r--r--   0        0        0     9026 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-log-console/static/684.386a2c35e71e2d3ba279.js
--rw-r--r--   0        0        0     7158 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-log-console/static/remoteEntry.5d3fb94cf5cf45937bfe.js
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-log-console/static/style.js
--rw-r--r--   0        0        0    64970 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-log-console/static/third-party-licenses.json
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-metadata-panel/package.json
--rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-metadata-panel/static/432.1dff82965ae8eeafd45c.js
--rw-r--r--   0        0        0    23398 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-metadata-panel/static/732.77667177c3d57faebb0c.js
--rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-metadata-panel/static/remoteEntry.732fba82fe6ebdc6be18.js
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-metadata-panel/static/style.js
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi/pipeline-metadata-panel/static/third-party-licenses.json
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi_extension/_version.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/amphi_venv/lib/python3.11/site-packages/amphi/_version.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/install.json
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/package.json
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/tsconfig.json
--rw-r--r--   0        0        0     6574 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/BrowseFileDialog.tsx
--rw-r--r--   0        0        0    14141 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/CodeGenerator.tsx
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/CustomHandle.tsx
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/PipelineComponent.tsx
--rw-r--r--   0        0        0     8053 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/PipelineService.tsx
--rw-r--r--   0        0        0     6279 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/RequestService.tsx
--rw-r--r--   0        0        0    20659 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/configUtils.tsx
--rw-r--r--   0        0        0     8092 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/connectionUtils.tsx
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/declarations.d.ts
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/generatorUtils.tsx
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/icons.ts
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/index.ts
--rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/rendererUtils.tsx
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/forms/CodeTextarea.tsx
--rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/forms/InputRegular.tsx
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/forms/TextareaRegular.tsx
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/forms/connectionSelector.tsx
--rw-r--r--   0        0        0    11667 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/forms/dataMapping.tsx
--rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/forms/keyValueColumns.tsx
--rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/forms/keyValueColumnsSelect.tsx
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/forms/keyValueForm.tsx
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/forms/selectColumn.tsx
--rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/forms/selectColumns.tsx
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/forms/selectCustomizable.tsx
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/forms/selectMultiple.tsx
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/forms/selectRegular.tsx
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/forms/selectTokenization.tsx
--rw-r--r--   0        0        0     8811 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/forms/transferData.tsx
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/forms/valuesListForm.tsx
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/style/base.css
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/style/index.css
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/style/index.js
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/style/icons/alert-triangle-fill-16.svg
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/style/icons/alert-triangle-fill-24.svg
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/style/icons/crosshair-16.svg
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/style/icons/minus-16.svg
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/style/icons/play-16.svg
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/style/icons/play-circle-16.svg
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/style/icons/plus-16.svg
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/style/icons/plus-24.svg
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/style/icons/search-16.svg
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/style/icons/search-24.svg
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/style/icons/settings-16.svg
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/style/icons/settings-24.svg
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/style/icons/trash-16.svg
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/style/icons/trash-24.svg
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/style/icons/x-16.svg
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/style/icons/x-square-16.svg
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-editor/install.json
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-editor/package.json
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-editor/pipeline-16.svg
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-editor/pipeline-24.svg
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-editor/tailwind.config.js
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-editor/tsconfig.json
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-editor/schema/extension.json
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-editor/schema/plugin copy.json
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-editor/schema/plugin.json
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-editor/src/Dropzone.tsx
--rw-r--r--   0        0        0    20622 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-editor/src/PipelineEditorWidget.tsx
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-editor/src/customEdge.tsx
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-editor/src/declarations.d.ts
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-editor/src/icons.ts
--rw-r--r--   0        0        0    18045 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-editor/src/index.ts
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-editor/style/canvas.css
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-editor/style/index.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-editor/style/index.js
--rw-r--r--   0        0        0    22125 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-editor/style/output.css
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-editor/style/pipeline-category-icon.svg
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-editor/style/react-icon.svg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-editor/style/tailwinds_preflight.css
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-editor/style/icons/api-24.svg
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-editor/style/icons/file-plus-24.svg
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-editor/style/icons/file-text-24.svg
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-editor/style/icons/monitor-24.svg
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-editor/style/icons/pipeline-brand-16.svg
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/packages/pipeline-editor/style/icons/pipeline-brand-24.svg
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/.gitignore
--rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/LICENSE
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/README.md
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     6964 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/.yarnrc.yml
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/MANIFEST.in
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/install.json
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/lerna.json
+-rw-r--r--   0        0        0    61977 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/output.json
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/package.json
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/setup.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/tsconfig.eslint.json
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/tsconfigbase.json
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/_version.py
+-rw-r--r--   0        0        0    23493 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-core/build_log.json
+-rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-core/package.json
+-rw-r--r--   0        0        0   337490 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-core/static/lib_index_js.8524d2449200481bcffc.js
+-rw-r--r--   0        0        0   277134 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-core/static/lib_index_js.8524d2449200481bcffc.js.map
+-rw-r--r--   0        0        0    31936 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-core/static/remoteEntry.79cb8756db433d8885a3.js
+-rw-r--r--   0        0        0    30897 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-core/static/remoteEntry.79cb8756db433d8885a3.js.map
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-core/static/style.js
+-rw-r--r--   0        0        0    20592 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-core/static/style_index_js.4ad7ee95dab1aa5fcfa9.js
+-rw-r--r--   0        0        0    16152 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-core/static/style_index_js.4ad7ee95dab1aa5fcfa9.js.map
+-rw-r--r--   0        0        0    89325 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-core/static/vendors-node_modules_ant-design_icons_es_icons_DeleteOutlined_js.2f946aa1f3734701343c.js
+-rw-r--r--   0        0        0    69332 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-core/static/vendors-node_modules_ant-design_icons_es_icons_DeleteOutlined_js.2f946aa1f3734701343c.js.map
+-rw-r--r--   0        0        0  6093739 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-core/static/vendors-node_modules_antd_es_index_js.f3702a4caa837b705e2f.js
+-rw-r--r--   0        0        0  5068064 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-core/static/vendors-node_modules_antd_es_index_js.f3702a4caa837b705e2f.js.map
+-rw-r--r--   0        0        0  1577186 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-core/static/vendors-node_modules_reactflow_dist_esm_index_js.e64ca0369e914dbdd2d2.js
+-rw-r--r--   0        0        0  1619404 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-core/static/vendors-node_modules_reactflow_dist_esm_index_js.e64ca0369e914dbdd2d2.js.map
+-rw-r--r--   0        0        0    23672 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-manager/build_log.json
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-manager/package.json
+-rw-r--r--   0        0        0   178262 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-manager/static/lib_index_js.381da04fdd4f00fefc97.js
+-rw-r--r--   0        0        0   144209 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-manager/static/lib_index_js.381da04fdd4f00fefc97.js.map
+-rw-r--r--   0        0        0     6263 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-manager/static/node_modules_babel_runtime_helpers_esm_objectSpread2_js.571d344d10a50cf87924.js
+-rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-manager/static/node_modules_babel_runtime_helpers_esm_objectSpread2_js.571d344d10a50cf87924.js.map
+-rw-r--r--   0        0        0    37328 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-manager/static/remoteEntry.30c9b3ec57b260a0de28.js
+-rw-r--r--   0        0        0    36378 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-manager/static/remoteEntry.30c9b3ec57b260a0de28.js.map
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-manager/static/style.js
+-rw-r--r--   0        0        0    20598 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-manager/static/style_index_js.9b53a2a59c637ddda250.js
+-rw-r--r--   0        0        0    16185 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-manager/static/style_index_js.9b53a2a59c637ddda250.js.map
+-rw-r--r--   0        0        0   862675 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-manager/static/vendors-node_modules_ace-builds_src-noconflict_ace_js.f376741fb17d86341715.js
+-rw-r--r--   0        0        0  1016740 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-manager/static/vendors-node_modules_ace-builds_src-noconflict_ace_js.f376741fb17d86341715.js.map
+-rw-r--r--   0        0        0   117027 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-manager/static/vendors-node_modules_ant-design_icons_es_icons_CheckOutlined_js-node_modules_ant-design_icons-dbfa36.64a8c72d811a7b9e80a0.js
+-rw-r--r--   0        0        0    87213 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-manager/static/vendors-node_modules_ant-design_icons_es_icons_CheckOutlined_js-node_modules_ant-design_icons-dbfa36.64a8c72d811a7b9e80a0.js.map
+-rw-r--r--   0        0        0   481165 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-manager/static/vendors-node_modules_ant-design_icons_es_icons_EyeTwoTone_js-node_modules_ant-design_icons_es-655c11.2ce12357bff85765a23b.js
+-rw-r--r--   0        0        0   441818 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-manager/static/vendors-node_modules_ant-design_icons_es_icons_EyeTwoTone_js-node_modules_ant-design_icons_es-655c11.2ce12357bff85765a23b.js.map
+-rw-r--r--   0        0        0  6066121 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-manager/static/vendors-node_modules_antd_es_index_js.fb77cb0fc352340b9517.js
+-rw-r--r--   0        0        0  5054125 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-manager/static/vendors-node_modules_antd_es_index_js.fb77cb0fc352340b9517.js.map
+-rw-r--r--   0        0        0   251891 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-manager/static/vendors-node_modules_react-ace_lib_index_js.342f83e0d9df341dbf7d.js
+-rw-r--r--   0        0        0   328024 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-manager/static/vendors-node_modules_react-ace_lib_index_js.342f83e0d9df341dbf7d.js.map
+-rw-r--r--   0        0        0    53469 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-manager/static/vendors-node_modules_react-dnd-html5-backend_dist_index_js.ecaeb6fbf4268c21d9ba.js
+-rw-r--r--   0        0        0    76311 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-manager/static/vendors-node_modules_react-dnd-html5-backend_dist_index_js.ecaeb6fbf4268c21d9ba.js.map
+-rw-r--r--   0        0        0   205216 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-manager/static/vendors-node_modules_react-dnd_dist_index_js.c19de454d59450aae505.js
+-rw-r--r--   0        0        0   223532 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-manager/static/vendors-node_modules_react-dnd_dist_index_js.c19de454d59450aae505.js.map
+-rw-r--r--   0        0        0    43836 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-manager/static/vendors-node_modules_react_jsx-runtime_js.de5e21cf2172aae5fafe.js
+-rw-r--r--   0        0        0    51438 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-components-manager/static/vendors-node_modules_react_jsx-runtime_js.de5e21cf2172aae5fafe.js.map
+-rw-r--r--   0        0        0    23490 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-editor/build_log.json
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-editor/package.json
+-rw-r--r--   0        0        0    68131 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-editor/static/lib_index_js.5751f3d0709bd368fae8.js
+-rw-r--r--   0        0        0    54109 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-editor/static/lib_index_js.5751f3d0709bd368fae8.js.map
+-rw-r--r--   0        0        0    12186 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-editor/static/node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_sourceMaps_j-f57309.2553e813f4c9a72d5500.js
+-rw-r--r--   0        0        0    12291 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-editor/static/node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_sourceMaps_j-f57309.2553e813f4c9a72d5500.js.map
+-rw-r--r--   0        0        0    34392 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-editor/static/remoteEntry.23ddc93f58265ecd7970.js
+-rw-r--r--   0        0        0    33241 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-editor/static/remoteEntry.23ddc93f58265ecd7970.js.map
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-editor/static/style.js
+-rw-r--r--   0        0        0    61376 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-editor/static/style_output_css.96f9856c3eb89ca68532.js
+-rw-r--r--   0        0        0    74508 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-editor/static/style_output_css.96f9856c3eb89ca68532.js.map
+-rw-r--r--   0        0        0  6182737 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-editor/static/vendors-node_modules_antd_es_index_js.d9589e32c6684f26e318.js
+-rw-r--r--   0        0        0  5125498 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-editor/static/vendors-node_modules_antd_es_index_js.d9589e32c6684f26e318.js.map
+-rw-r--r--   0        0        0   502045 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-editor/static/vendors-node_modules_reactflow_dist_esm_index_mjs.5c5eb21d117db51fd5ac.js
+-rw-r--r--   0        0        0   448969 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-editor/static/vendors-node_modules_reactflow_dist_esm_index_mjs.5c5eb21d117db51fd5ac.js.map
+-rw-r--r--   0        0        0    41157 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-editor/static/vendors-node_modules_reactflow_dist_style_css.d7c64ba2362242363fc6.js
+-rw-r--r--   0        0        0    43481 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-editor/static/vendors-node_modules_reactflow_dist_style_css.d7c64ba2362242363fc6.js.map
+-rw-r--r--   0        0        0    23414 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-log-console/build_log.json
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-log-console/package.json
+-rw-r--r--   0        0        0    35988 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-log-console/static/lib_index_js.7814c07b120fac8e7d7f.js
+-rw-r--r--   0        0        0    31987 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-log-console/static/lib_index_js.7814c07b120fac8e7d7f.js.map
+-rw-r--r--   0        0        0    30825 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-log-console/static/remoteEntry.73f24597acde3e18ec8b.js
+-rw-r--r--   0        0        0    29685 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-log-console/static/remoteEntry.73f24597acde3e18ec8b.js.map
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-log-console/static/style.js
+-rw-r--r--   0        0        0    21374 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-log-console/static/style_index_js.d38bbe6813c815742e03.js
+-rw-r--r--   0        0        0    17440 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-log-console/static/style_index_js.d38bbe6813c815742e03.js.map
+-rw-r--r--   0        0        0  3446416 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-log-console/static/vendors-node_modules_antd_es_alert_index_js-node_modules_antd_es_table_index_js-node_modules_-9bb28b.ce8f51ee89bb51889de1.js
+-rw-r--r--   0        0        0  3041771 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-log-console/static/vendors-node_modules_antd_es_alert_index_js-node_modules_antd_es_table_index_js-node_modules_-9bb28b.ce8f51ee89bb51889de1.js.map
+-rw-r--r--   0        0        0    23454 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-metadata-panel/build_log.json
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-metadata-panel/package.json
+-rw-r--r--   0        0        0    56397 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-metadata-panel/static/lib_index_js.8e6980268a05cb569b43.js
+-rw-r--r--   0        0        0    56665 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-metadata-panel/static/lib_index_js.8e6980268a05cb569b43.js.map
+-rw-r--r--   0        0        0    29504 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-metadata-panel/static/remoteEntry.109d842e91011fceeb5a.js
+-rw-r--r--   0        0        0    28470 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-metadata-panel/static/remoteEntry.109d842e91011fceeb5a.js.map
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-metadata-panel/static/style.js
+-rw-r--r--   0        0        0    23221 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-metadata-panel/static/style_index_js.09b417b0af24e77e2ba7.js
+-rw-r--r--   0        0        0    19798 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi/pipeline-metadata-panel/static/style_index_js.09b417b0af24e77e2ba7.js.map
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi_extension/_version.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/amphi_venv/lib/python3.11/site-packages/amphi/_version.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/install.json
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/package.json
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/tsconfig.json
+-rw-r--r--   0        0        0     6574 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/BrowseFileDialog.tsx
+-rw-r--r--   0        0        0    14657 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/CodeGenerator.tsx
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/CustomHandle.tsx
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/DndProviderWrapper.tsx
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/PipelineComponent.tsx
+-rw-r--r--   0        0        0     8053 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/PipelineService.tsx
+-rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/RequestService.tsx
+-rw-r--r--   0        0        0    20599 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/configUtils.tsx
+-rw-r--r--   0        0        0     8092 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/connectionUtils.tsx
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/declarations.d.ts
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/generatorUtils.tsx
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/icons.ts
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/index.ts
+-rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/rendererUtils.tsx
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/forms/CodeTextarea.tsx
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/forms/InputRegular.tsx
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/forms/TextareaRegular.tsx
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/forms/connectionSelector.tsx
+-rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/forms/dataMapping.tsx
+-rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/forms/keyValueColumns.tsx
+-rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/forms/keyValueColumnsSelect.tsx
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/forms/keyValueForm.tsx
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/forms/selectColumn.tsx
+-rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/forms/selectColumns.tsx
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/forms/selectCustomizable.tsx
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/forms/selectMultiple.tsx
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/forms/selectRegular.tsx
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/forms/selectTokenization.tsx
+-rw-r--r--   0        0        0     9032 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/forms/transferData.tsx
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/forms/valuesListForm.tsx
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/style/base.css
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/style/index.css
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/style/index.js
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/style/icons/alert-triangle-fill-16.svg
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/style/icons/alert-triangle-fill-24.svg
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/style/icons/crosshair-16.svg
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/style/icons/minus-16.svg
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/style/icons/play-16.svg
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/style/icons/play-circle-16.svg
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/style/icons/plus-16.svg
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/style/icons/plus-24.svg
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/style/icons/search-16.svg
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/style/icons/search-24.svg
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/style/icons/settings-16.svg
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/style/icons/settings-24.svg
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/style/icons/trash-16.svg
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/style/icons/trash-24.svg
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/style/icons/x-16.svg
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/style/icons/x-square-16.svg
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-editor/install.json
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-editor/package.json
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-editor/pipeline-16.svg
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-editor/pipeline-24.svg
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-editor/tailwind.config.js
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-editor/tsconfig.json
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-editor/schema/extension.json
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-editor/schema/plugin copy.json
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-editor/schema/plugin.json
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-editor/src/Dropzone.tsx
+-rw-r--r--   0        0        0    20782 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-editor/src/PipelineEditorWidget.tsx
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-editor/src/customEdge.tsx
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-editor/src/declarations.d.ts
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-editor/src/icons.ts
+-rw-r--r--   0        0        0    16588 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-editor/src/index.ts
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-editor/style/canvas.css
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-editor/style/index.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-editor/style/index.js
+-rw-r--r--   0        0        0    22125 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-editor/style/output.css
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-editor/style/pipeline-category-icon.svg
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-editor/style/react-icon.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-editor/style/tailwinds_preflight.css
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-editor/style/icons/api-24.svg
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-editor/style/icons/file-plus-24.svg
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-editor/style/icons/file-text-24.svg
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-editor/style/icons/monitor-24.svg
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-editor/style/icons/pipeline-brand-16.svg
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/packages/pipeline-editor/style/icons/pipeline-brand-24.svg
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/.gitignore
+-rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/README.md
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     6964 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.2/PKG-INFO
```

### Comparing `jupyterlab_amphi-0.3.1/output.json` & `jupyterlab_amphi-0.3.2/output.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/package.json` & `jupyterlab_amphi-0.3.2/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.3.2'"}*

```diff
@@ -66,15 +66,15 @@
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md,.yml,.yaml}\"",
         "prettier:check": "jlpm prettier:base --check",
         "quickstart": "npm run setup:py && jlpm && jlpm deduplicate && jlpm clean:all && jlpm lint && jlpm build:prod && jlpm dist && jlpm docs && jlpm test",
         "setup:py": "python -m pip install -e \".[dev,lint,test,docs]\"",
         "test": "jlpm test:py",
         "test:py": "pytest"
     },
-    "version": "0.3.1",
+    "version": "0.3.2",
     "workspaces": {
         "packages": [
             "packages/pipeline-editor",
             "packages/pipeline-components-manager",
             "packages/pipeline-components-core",
             "packages/pipeline-console",
             "packages/pipeline-metadata-panel"
```

### Comparing `jupyterlab_amphi-0.3.1/tsconfigbase.json` & `jupyterlab_amphi-0.3.2/tsconfigbase.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/amphi/pipeline-components-core/package.json` & `jupyterlab_amphi-0.3.2/amphi/pipeline-components-core/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9744791666666666%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.79cb8756db433d8885a3.js'}}",*

 * * "'version'": "'0.3.2'"}*

```diff
@@ -39,15 +39,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.364ddb190429da413754.js",
+            "load": "static/remoteEntry.79cb8756db433d8885a3.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../amphi/pipeline-components-core",
         "sharedPackages": {
             "@amphi/pipeline-components-manager": {
                 "bundled": false,
@@ -83,9 +83,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.0"
+    "version": "0.3.2"
 }
```

### Comparing `jupyterlab_amphi-0.3.1/amphi/pipeline-components-manager/package.json` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9702380952380952%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}", "'version'": "'0.3.2'"}*

```diff
@@ -47,19 +47,14 @@
         "lib/*.js.map",
         "lib/*.js",
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.d25d5d91895e4e9316a4.js",
-            "style": "./style"
-        },
         "extension": true,
         "outputDir": "../../amphi/pipeline-components-manager",
         "sharedPackages": {
             "@amphi/pipeline-components-manager": {
                 "bundle": false,
                 "singleton": true
             }
@@ -99,9 +94,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.0"
+    "version": "0.3.2"
 }
```

### Comparing `jupyterlab_amphi-0.3.1/amphi/pipeline-editor/package.json` & `jupyterlab_amphi-0.3.2/packages/pipeline-editor/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9702380952380952%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}", "'version'": "'0.3.2'"}*

```diff
@@ -45,19 +45,14 @@
         "lib/*.js.map",
         "lib/*.js",
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.12b3539515ec33e9f21c.js",
-            "style": "./style"
-        },
         "extension": true,
         "outputDir": "../../amphi/pipeline-editor",
         "sharedPackages": {
             "@amphi/pipeline-components-manager": {
                 "bundled": false,
                 "singleton": true
             },
@@ -103,9 +98,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.0"
+    "version": "0.3.2"
 }
```

### Comparing `jupyterlab_amphi-0.3.1/amphi/pipeline-log-console/package.json` & `jupyterlab_amphi-0.3.2/amphi/pipeline-log-console/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9756944444444444%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.73f24597acde3e18ec8b.js'}}",*

 * * "'version'": "'0.3.2'"}*

```diff
@@ -52,15 +52,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.5d3fb94cf5cf45937bfe.js",
+            "load": "static/remoteEntry.73f24597acde3e18ec8b.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../amphi/pipeline-log-console",
         "sharedPackages": {
             "@amphi/pipeline-editor": {
                 "bundled": false,
@@ -99,9 +99,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.0"
+    "version": "0.3.2"
 }
```

### Comparing `jupyterlab_amphi-0.3.1/amphi/pipeline-metadata-panel/package.json` & `jupyterlab_amphi-0.3.2/amphi/pipeline-metadata-panel/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9744791666666666%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.109d842e91011fceeb5a.js'}}",*

 * * "'version'": "'0.3.2'"}*

```diff
@@ -51,15 +51,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.732fba82fe6ebdc6be18.js",
+            "load": "static/remoteEntry.109d842e91011fceeb5a.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../amphi/pipeline-metadata-panel",
         "sharedPackages": {
             "@amphi/pipeline-editor": {
                 "bundled": false,
@@ -95,9 +95,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.0"
+    "version": "0.3.2"
 }
```

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/package.json` & `jupyterlab_amphi-0.3.2/amphi/pipeline-components-manager/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9702380952380952%*

 * *Differences: {"'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.30c9b3ec57b260a0de28.js'), "*

 * *                 "('extension', './extension'), ('style', './style')])}",*

 * * "'version'": "'0.3.2'"}*

```diff
@@ -47,14 +47,19 @@
         "lib/*.js.map",
         "lib/*.js",
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.30c9b3ec57b260a0de28.js",
+            "style": "./style"
+        },
         "extension": true,
         "outputDir": "../../amphi/pipeline-components-manager",
         "sharedPackages": {
             "@amphi/pipeline-components-manager": {
                 "bundle": false,
                 "singleton": true
             }
@@ -94,9 +99,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.1"
+    "version": "0.3.2"
 }
```

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/tsconfig.json` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/BrowseFileDialog.tsx` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/BrowseFileDialog.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/CodeGenerator.tsx` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/CodeGenerator.tsx`

 * *Files 6% similar despite different names*

```diff
@@ -256,20 +256,29 @@
         default:
           console.error("Error generating code.");
       }
 
       code += lastCodeGenerated;
     
       // If target node....  
-        if (nodeId === targetNodeId) {
-          if(!fromStart) {
+      if (nodeId === targetNodeId) {
+        if (component_type.includes('processor') || component_type.includes('input')) {
+          if (!fromStart) {
             code = lastCodeGenerated;
           }
           code += '\n' + nodeOutputs.get(nodeId);
+        } else if (component_type.includes('output')) {
+          // Add try block and indent existing code
+          const indentedCode = code.split('\n').map(line => '    ' + line).join('\n');
+          code = 'try:\n' + indentedCode + '\n    print("Pipeline Execution: SUCCESS")\n';
+          code += 'except Exception as e:\n';
+          code += '    print(f"Pipeline Execution: FAILED with error {e}")\n';
+          code += '    raise\n';  // Re-raise the exception to propagate the error status
         }
+      }
     }
 
     let envVariablesCode = '';
         // Loggers when full pipeline execution
         if (envVariablesMap.size > 0) {
           envVariablesMap.forEach((node, nodeId) => {
             // Process each logger
@@ -326,27 +335,24 @@
 ${code}
 except Exception as e:
     print(f"An error occurred: {e}")
 ${loggerCode}
 `;
 
     } else {
-      console.log('No loggers found.');
+      // console.log('No loggers found.');
     }
 
     const currentDate = new Date();
     const dateString = `${currentDate.getFullYear()}-${(currentDate.getMonth() + 1).toString().padStart(2, '0')}-${currentDate.getDate().toString().padStart(2, '0')} ${currentDate.getHours().toString().padStart(2, '0')}:${currentDate.getMinutes().toString().padStart(2, '0')}:${currentDate.getSeconds().toString().padStart(2, '0')}`;
     const dateComment = `# Source code generated by Amphi\n# Date: ${dateString}`;
     const additionalImports = `# Additional dependencies: ${Array.from(uniqueDependencies).join(', ')}`;
 
-    // Replace viarbale string 
-    console.log("Original code : " + code);
-
+    // Replace variabale string 
     code = this.convertToFString(code);
-    console.log("Var code : " + code);
 
     const generatedCode = 
 `${dateComment}
 ${additionalImports}
 ${Array.from(uniqueImports).join('\n')}
 \n${envVariablesCode}${Array.from(functions).join('\n\n')}
 ${code}`;
```

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/CustomHandle.tsx` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/CustomHandle.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/PipelineComponent.tsx` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/PipelineComponent.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/PipelineService.tsx` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/PipelineService.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/RequestService.tsx` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/RequestService.tsx`

 * *Files 5% similar despite different names*

```diff
@@ -48,32 +48,37 @@
       future.onReply = reply => {
         if (reply.content.status == "ok") {
           const future2 = context.sessionContext.session.kernel!.requestExecute({ code: "print(_amphi_metadatapanel_getcontentof(" + output_df + "))" });
           future2.onIOPub = msg => {
             if (msg.header.msg_type === 'stream') {
               const streamMsg = msg as KernelMessage.IStreamMsg;
               const output = streamMsg.content.text;
-              const regex = /([^\s,]+)\s+\(([^,]+),\s*(named|unnamed)\)/g;
+              const regex = /([^,]+)\s+\(([^,]+),\s*(named|unnamed)\)/g;
               const newItems = [];
               
               let match;
               while ((match = regex.exec(output)) !== null) {
                 const [_, name, type, namedStatus] = match;
                 newItems.push({
-                  value: name,
-                  label: name,
-                  type: type,
-                  named: namedStatus === 'named' // true if 'named', false if 'unnamed'
+                  value: name.trim(),
+                  label: name.trim(),
+                  type: type.trim(),
+                  named: namedStatus.trim() === 'named' // true if 'named', false if 'unnamed'
                 });
               }
+
+              console.log("Retrieve col, new items %o", newItems)
               
               // Update the items array with the new items, ensuring no duplicates
               setItems(items => {
                 const itemSet = new Set(items.map(item => item.value)); // Create a set of existing item values
                 const uniqueItems = newItems.filter(newItem => !itemSet.has(newItem.value));
+
+                console.log("Retrieve col, uniqueItems %o", uniqueItems)
+
                 return [...items, ...uniqueItems];
               });
 
               setLoadings(false)
             } else if (msg.header.msg_type === 'error') {
               setLoadings(false)
               const errorMsg = msg as KernelMessage.IErrorMsg;
@@ -138,18 +143,16 @@
           console.log("Other")
           setLoadings(false)
         }
       };
 
       future.onIOPub = msg => {
         if (msg.header.msg_type === 'stream') {
-          console.log("stream")
           const streamMsg = msg as KernelMessage.IStreamMsg;
           const output = streamMsg.content.text;
-          console.log("message : %o",output )
 
           const regex = /([^\s,]+)\s+\(((?:[^()]+|\([^)]*\))*)\)/g;
           const newItems = [];
           
           let match;
           while ((match = regex.exec(output)) !== null) {
             const [_, name, type, namedStatus] = match;
```

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/configUtils.tsx` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/configUtils.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,17 @@
 export const setDefaultConfig = ({
   nodeId,
   store,
   setNodes,
   defaultConfig,
 }: SetDefaultConfigProps): void => {
   const { nodeInternals } = store.getState();
-  console.log("setDefault????");
   setNodes(
     Array.from(nodeInternals.values()).map((node) => {
       if (node.id === nodeId && Object.keys(node.data).length === 1) {
-        console.log("why not working?")
         node.data = {
           ...defaultConfig,
           lastUpdated: null,
           lastExecuted: null,
         };
       }
       return node;
@@ -94,15 +92,15 @@
   context,
   componentService,
   manager,
   commands,
   handleChange,
 }: FormComponentProps) => {
 
-  const [modal2Open, setModal2Open] = useState(false);
+  const [modalOpen, setModalOpen] = useState(false);
 
   const executeUntilComponent = () => {
     commands.execute('pipeline-editor:run-pipeline-until', { nodeId: nodeId, context: context });
     handleChange(Date.now(), 'lastExecuted'); 
   };
 
   return (
@@ -115,25 +113,25 @@
         }}
       >
         <Form
         layout="vertical"
         size="small">
         {generateUIInputs({ name, nodeId, form, data, context, componentService, manager, commands, handleChange, advanced: false })}
         <div className="flex justify-center mt-1 pt-1.5 space-x-4">
-          <span onClick={() => setModal2Open(true)}
+          <span onClick={() => setModalOpen(true)}
             className="inline-flex items-center justify-center cursor-pointer group">
             <settingsIcon.react className="h-3 w-3 group-hover:text-primary" />
           </span>
-          {(type.includes('input') || type.includes('processor')) && (
+          {(type.includes('input') || type.includes('processor') || type.includes('output')) && (
             <span onClick={executeUntilComponent} className="inline-flex items-center justify-center cursor-pointer group">
               <playCircleIcon.react className="h-3 w-3 group-hover:text-primary" />
             </span>
           )}
         </div>
-        <ConfigModal modal2Open={modal2Open} setModal2Open={setModal2Open} name={name} nodeId={nodeId} form={form} data={data} context={context} componentService={componentService} manager={manager} commands={commands} handleChange={handleChange} advanced />
+        <ConfigModal modalOpen={modalOpen} setModalOpen={setModalOpen} name={name} nodeId={nodeId} form={form} data={data} context={context} componentService={componentService} manager={manager} commands={commands} handleChange={handleChange} advanced />
       </Form>
     </ConfigProvider>
 
   );
 };
 
 export const generateUIInputs = ({
@@ -394,25 +392,25 @@
   data,
   context,
   componentService,
   manager,
   commands,
   handleChange,
   advanced,
-  modal2Open,
-  setModal2Open
+  modalOpen,
+  setModalOpen
 }: ConfigModalProps) {
   return (
     <>
       <Modal
         title={name}
         centered
-        open={modal2Open}
-        onOk={() => setModal2Open(false)}
-        onCancel={() => setModal2Open(false)}
+        open={modalOpen}
+        onOk={() => setModalOpen(false)}
+        onCancel={() => setModalOpen(false)}
         width={800}
         footer={(_, { OkBtn }) => (
           <>
           <OkBtn />
           </>
         )}
       >
@@ -518,10 +516,10 @@
   data: object;
   context: any;
   componentService: any;
   manager: any
   commands: any;
   handleChange: (e: React.ChangeEvent<HTMLInputElement>) => void;
   advanced: boolean;
-  modal2Open: any;
-  setModal2Open: any;
+  modalOpen: any;
+  setModalOpen: any;
 }
```

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/connectionUtils.tsx` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/connectionUtils.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/generatorUtils.tsx` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/generatorUtils.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/icons.ts` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/index.ts` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/rendererUtils.tsx` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/rendererUtils.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 // ConfigForm.tsx
 
 // Import necessary hooks and other dependencies
 import { LabIcon } from '@jupyterlab/ui-components';
 import { xIcon } from './icons';
 import React, { useMemo } from 'react';
+import { QuestionCircleOutlined } from '@ant-design/icons';
+
 import { getConnectedEdges, Handle, useNodeId, useStore } from 'reactflow';
 import { Popconfirm } from 'antd';
 
 interface IHandleProps {
   type: string;
   Handle: any;
   Position: any;
@@ -89,15 +91,15 @@
   };
 
   return (
     <>
       <div className="component" onDoubleClick={handleDoubleClick}>
         <div className="component__header">
           {name}
-          <Popconfirm title="Sure to delete?" onConfirm={() => deleteNode()}>
+          <Popconfirm title="Sure to delete?" placement="right" onConfirm={() => deleteNode()} icon={<QuestionCircleOutlined style={{ color: 'red' }} />}>
             <div className='deletebutton'>
               <xIcon.react className="group-hover:text-primary" />
             </div>
           </Popconfirm>
         </div>
         <div className="component__body">
           <form>
```

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/forms/CodeTextarea.tsx` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/forms/CodeTextarea.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/forms/InputRegular.tsx` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/forms/InputRegular.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 import { UserOutlined, CloseOutlined, EyeInvisibleOutlined, EyeTwoTone, SearchOutlined, SettingOutlined } from '@ant-design/icons';
 import { AutoComplete, Input } from 'antd';
 import { PipelineService } from '../PipelineService';
 
 
 export const InputRegular = ({ field, value, handleChange, context, advanced }) => {
 
-  console.log("Value in inputregular %o", value)
-
   const [inputValue, setInputValue] = useState(value);
   const inputRef = useRef(null);
   const [openValue, setOpenValue] = useState(false);
 
   useEffect(() => {
     setInputValue(value);  // Update inputValue when value prop changes
   }, [value]);
@@ -37,15 +35,15 @@
       setOpenValue(true);
       return true;
     } else {
       setOpenValue(false);
       const lastDollarIndex = inputValue.lastIndexOf('{');
       if (lastDollarIndex !== -1 && lastDollarIndex < inputValue.length - 1) {
         const searchTerm = inputValue.substring(lastDollarIndex + 1);
-        console.log("Option: %o", option);
+        // console.log("Option: %o", option);
         return option.value.startsWith(searchTerm);
       }
       return false;
     }
   };
 
   const renderTitle = (title: string) => (
```

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/forms/TextareaRegular.tsx` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/forms/TextareaRegular.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/forms/connectionSelector.tsx` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/forms/connectionSelector.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/forms/dataMapping.tsx` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/forms/dataMapping.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -26,18 +26,14 @@
 
   type FormInstance<T> = GetRef<typeof Form<T>>;
   const EditableContext = React.createContext<FormInstance<any> | null>(null);
   const [loadingsInput, setLoadingsInput] = useState<boolean>();
   const [loadingsOutput, setLoadingsOutput] = useState<boolean>();
   const [items, setItems] = useState<Option[]>([]);
 
-  useEffect(() => {
-    console.log("ITEMS %o", items)
-  }, [items]);
-
   interface Item {
     input: any;
     key: React.Key;
     value: string;
     type: string;
   }
   
@@ -162,15 +158,14 @@
   
   type ColumnTypes = Exclude<EditableTableProps['columns'], undefined>;
   
   const [dataSource, setDataSource] = useState<DataType[]>(defaultValue || []);
   
 
     useEffect(() => {
-      console.log("datasource %o", dataSource)
       handleChange(dataSource, field.id);
     }, [dataSource]);
 
     const customizeRenderEmpty = () => (
       <div style={{ textAlign: 'center' }}>
         <Empty image={Empty.PRESENTED_IMAGE_SIMPLE} />
       </div>
@@ -334,16 +329,14 @@
 const FieldValueInput: React.FC<FieldValueProps> = ({ field, value = {}, onChange }) => {
   const [name, setName] = useState<string>('');
   const [type, setType] = useState<string>('');
   const [nameType, setNameType] = useState('');
   const inputRef = useRef<InputRef>(null);
   const [items, setItems] = useState(field.typeOptions);
 
-  console.log("items %o", items);
-
   const triggerChange = (changedValue: { name?: string; type?: string }) => {
     onChange?.({ name, type, ...value, ...changedValue });
   };
 
   const onNameChange = (e: React.ChangeEvent<HTMLInputElement>) => {
     const newName = e.target.value || '';
     setName(newName);
```

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/forms/keyValueColumns.tsx` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/forms/keyValueColumns.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/forms/keyValueColumnsSelect.tsx` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/forms/keyValueColumnsSelect.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/forms/keyValueForm.tsx` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/forms/keyValueForm.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/forms/selectColumn.tsx` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/forms/selectColumn.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/forms/selectColumns.tsx` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/forms/selectColumns.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/forms/selectCustomizable.tsx` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/forms/selectCustomizable.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/forms/selectMultiple.tsx` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/forms/selectMultiple.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/forms/selectRegular.tsx` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/forms/selectRegular.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/forms/selectTokenization.tsx` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/forms/selectTokenization.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/forms/transferData.tsx` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/forms/transferData.tsx`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import { KernelMessage } from '@jupyterlab/services';
 import difference from 'lodash/difference';
-import React, { useEffect, useState } from 'react';
+import React, { useEffect, useState, useRef, useMemo, useCallback } from 'react';
 import { DndProvider, useDrag, useDrop } from "react-dnd";
 
 import { HTML5Backend } from "react-dnd-html5-backend";
 import { CodeGenerator } from '../CodeGenerator';
 import { PipelineService } from '../PipelineService';
 import { RequestService } from '../RequestService';
+import DndProviderWrapper from '../DndProviderWrapper';
 
 import type { GetProp, TableColumnsType, TableProps, TransferProps } from 'antd';
 import { Button, Space, Table, Tag, Transfer } from 'antd';
 import { FieldDescriptor } from '../configUtils';
 
 // implementation based on ant design and https://github.com/ant-design/ant-design/issues/12817#issuecomment-683288556
 
@@ -84,27 +85,26 @@
       type: 'DragableBodyRow',
       item: { type: 'DragableBodyRow', index },
       collect: (monitor) => ({
         isDragging: monitor.isDragging(),
       }),
     });
 
-    drop(drag(ref));
+    drag(drop(ref));
 
     return (
       <tr
         ref={ref}
         className={`${className}${isOver ? dropClassName : ''} draggable`}
-        style={{ cursor: 'move', ...style }}
+        style={{ cursor: 'move', opacity: isOver ? 0.5 : 1, ...style }} // Added opacity change
         {...restProps}
       />
     );
   };
 
-
   // Customize Table Transfer
   const TableTransfer = ({ leftColumns, rightColumns, ...restProps }: TableTransferProps) => (
     <Transfer {...restProps}>
       {({
         direction,
         filteredItems,
         onItemSelect,
@@ -167,52 +167,53 @@
           
             setTargetKeys(newKeys);
             const savedSchema = { sourceData: sourceData, targetKeys: newKeys }
             handleChange(savedSchema, field.id);
           };
 
           return (
-            <DndProvider backend={HTML5Backend}>
+            <DndProviderWrapper>
               <Table
-                rowSelection={rowSelection}
-                columns={columns}
-                dataSource={filteredItems}
-                components={{
-                  body: {
-                    row: DragableBodyRow,
-                  },
-                }}
-                size="small"
-                style={{ pointerEvents: listDisabled ? 'none' : undefined }}
-                onRow={(record, idx) => ({
-                  index: idx, // Pass the correct index to the row
-                  rowDrop,
-                  onClick: () => {
-                    if (record.disabled) {
-                      return;
-                    }
-                    onItemSelect(record.key, !listSelectedKeys.includes(record.key)); // Toggle selection
-                  },
-                })}
-              />
-            </DndProvider>
-
+                  rowSelection={rowSelection}
+                  columns={columns}
+                  dataSource={filteredItems}
+                  components={{
+                    body: {
+                      row: DragableBodyRow,
+                    },
+                  }}
+                  size="small"
+                  style={{ pointerEvents: listDisabled ? 'none' : undefined }}
+                  onRow={(record, idx) => ({
+                    index: idx, // Pass the correct index to the row
+                    rowDrop,
+                    onClick: () => {
+                      if (record.disabled) {
+                        return;
+                      }
+                      onItemSelect(record.key, !listSelectedKeys.includes(record.key)); // Toggle selection
+                    },
+                  })}
+                />
+              </DndProviderWrapper>
           );
         }
 
       }}
     </Transfer>
   );
 
   const [items, setItems] = useState([]);
   const [sourceData, setSourceData] = useState<RecordType[]>([]);
   const [targetKeys, setTargetKeys] = useState<TransferProps['targetKeys']>([]);
   const [loadings, setLoadings] = useState<boolean>();
 
   useEffect(() => {
+    console.log("Transfer Data, items %o", items)
+
     setSourceData(items.map(item => ({
         ...item,
         key: item.value,
         title: item.value
     })));
   }, [items]);
```

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/src/forms/valuesListForm.tsx` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/src/forms/valuesListForm.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/style/icons/alert-triangle-fill-24.svg` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/style/icons/alert-triangle-fill-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/style/icons/settings-16.svg` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/style/icons/settings-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/style/icons/settings-24.svg` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/style/icons/settings-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/style/icons/trash-16.svg` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/style/icons/trash-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/style/icons/trash-24.svg` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/style/icons/trash-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-components-manager/style/icons/x-square-16.svg` & `jupyterlab_amphi-0.3.2/packages/pipeline-components-manager/style/icons/x-square-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-editor/package.json` & `jupyterlab_amphi-0.3.2/amphi/pipeline-editor/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9702380952380952%*

 * *Differences: {"'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.23ddc93f58265ecd7970.js'), "*

 * *                 "('extension', './extension'), ('style', './style')])}",*

 * * "'version'": "'0.3.2'"}*

```diff
@@ -45,14 +45,19 @@
         "lib/*.js.map",
         "lib/*.js",
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.23ddc93f58265ecd7970.js",
+            "style": "./style"
+        },
         "extension": true,
         "outputDir": "../../amphi/pipeline-editor",
         "sharedPackages": {
             "@amphi/pipeline-components-manager": {
                 "bundled": false,
                 "singleton": true
             },
@@ -98,9 +103,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.1"
+    "version": "0.3.2"
 }
```

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-editor/pipeline-16.svg` & `jupyterlab_amphi-0.3.2/packages/pipeline-editor/pipeline-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-editor/pipeline-24.svg` & `jupyterlab_amphi-0.3.2/packages/pipeline-editor/pipeline-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-editor/tsconfig.json` & `jupyterlab_amphi-0.3.2/packages/pipeline-editor/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-editor/schema/plugin copy.json` & `jupyterlab_amphi-0.3.2/packages/pipeline-editor/schema/plugin copy.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-editor/schema/plugin.json` & `jupyterlab_amphi-0.3.2/packages/pipeline-editor/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-editor/src/Dropzone.tsx` & `jupyterlab_amphi-0.3.2/packages/pipeline-editor/src/Dropzone.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-editor/src/PipelineEditorWidget.tsx` & `jupyterlab_amphi-0.3.2/packages/pipeline-editor/src/PipelineEditorWidget.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   DocumentWidget
 } from '@jupyterlab/docregistry';
 import { IDefaultFileBrowser, IFileBrowserFactory } from '@jupyterlab/filebrowser';
 import { Toolbar as UIToolbar, buildIcon, extensionIcon, inspectorIcon, listIcon, runIcon, saveIcon } from '@jupyterlab/ui-components';
 import { ISettingRegistry } from '@jupyterlab/settingregistry';
 import { Drag } from '@lumino/dragdrop';
 
-import React, { useCallback, useRef, useState } from 'react';
+import React, { useCallback, useRef, useState, useEffect } from 'react';
 import ReactFlow, {
   Background,
   Controls,
   Panel,
   ReactFlowProvider,
   addEdge,
   getConnectedEdges,
@@ -338,17 +338,15 @@
       </div>
     );
   }
 
   function Sidebar() {
 
     const [sidebarOpen, setSideBarOpen] = useState(false);
-    const handleViewSidebar = () => {
-      setSideBarOpen(!sidebarOpen);
-    };
+
     const sidebarClass = sidebarOpen ? "" : "open";
 
     const onDragStart = (event, nodeType, config) => {
       event.dataTransfer.setData('application/reactflow', nodeType);
       // Here, you can add more data as needed
       event.dataTransfer.setData('additionalData', config);
       event.dataTransfer.effectAllowed = 'move';
@@ -375,27 +373,30 @@
       if (!categorizedComponents[category]['_']) {  // Maintain a simple placeholder for main categories without explicit subcategories
         categorizedComponents[category]['_'] = [];
       }
       categorizedComponents[category]['_'].push(component);
     }
   });
 
+
   // Transforming categorized components into tree data structure
   const treeData = Object.keys(categorizedComponents).map((category, index) => {
     const subCategories = Object.keys(categorizedComponents[category]);
     let children = [];
 
     subCategories.forEach((subCat, subIndex) => {
       if (subCat === '_') {  // Handling main category direct children
         children.push(...categorizedComponents[category][subCat].map((component, childIndex) => ({
           title: (
             <span
               draggable
               className="palette-component"
               onDragStart={(event) => onDragStart(event, component._id, component.getDefaultConfig ? component.getDefaultConfig() : '')}
+              key={`category-${index}-item-${childIndex}`} // Add this line
+
             >
               {component._name}
             </span>
           ),
           key: `category-${index}-item-${childIndex}`,
           isLeaf: true,
           icon: <component._icon.react height="14px" width="14px;"/>
@@ -405,53 +406,56 @@
           title: <span className="palette-component-category">{subCat.charAt(0).toUpperCase() + subCat.slice(1)}</span>,
           key: `category-${index}-sub-${subIndex}`,
           children: categorizedComponents[category][subCat].map((component, childIndex) => ({
             title: (
               <span
                 draggable
                 className="palette-component"
-                onDragStart={(event) => onDragStart(event, component._id, component.getDefaultConfig ? component.getDefaultConfig() : '')
-              }>
+                onDragStart={(event) => onDragStart(event, component._id, component.getDefaultConfig ? component.getDefaultConfig() : '')}
+                key={`category-${index}-sub-${subIndex}-item-${childIndex}`} // Add this line
+              >
                 {component._name}
               </span>
             ),
             key: `category-${index}-sub-${subIndex}-item-${childIndex}`,
             isLeaf: true,
             icon: <component._icon.react height="14px" width="14px;"/>
           }))
         });
       }
     });
 
+    
+
     return {
       title: <span className="palette-component-category">{category.charAt(0).toUpperCase() + category.slice(1)}</span>,
       key: `category-${index}`,
       children: children
     };
   });
 
   // Output tree data (for debugging, you might want to console.log or use it directly in your components)
   console.log(treeData);
 
-
-
     return (
 
       <aside className={sidebarClass} title={'Components'}>
-
+        
         <div className="description">
           <extensionIcon.react tag="span" width="24px" float="left" marginRight="8px" />
           Drag and drop components.
         </div>
+       
         <DirectoryTree
           selectable={false}
           multiple
           blockNode
           defaultExpandAll
           treeData={treeData}
+          key={"palette-components"}
         />
       </aside>
     );
   }
 
   return (
     <div className="palette" id="pipeline-panel">
```

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-editor/src/customEdge.tsx` & `jupyterlab_amphi-0.3.2/packages/pipeline-editor/src/customEdge.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-editor/src/icons.ts` & `jupyterlab_amphi-0.3.2/packages/pipeline-editor/src/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-editor/src/index.ts` & `jupyterlab_amphi-0.3.2/packages/pipeline-editor/src/index.ts`

 * *Files 4% similar despite different names*

```diff
@@ -302,14 +302,16 @@
           commands.execute('pipeline-console:open', {}).catch(reason => {
             console.error(
               `An error occurred during the execution of ${command}.\n${reason}`
             );
           });
         }
 
+
+
         const current = getCurrent(args);
         if (!current) {
           return;
         }
 
         if (!current.context.sessionContext.session) {
           Notification.error('The pipeline cannot be run because the local Python engine cannot be found.', {
@@ -346,15 +348,15 @@
 
           const code = args.code.toString();
           let packages: string[];
           const imports = PipelineService.extractPythonImportPackages(code);
           packages = PipelineService.extractPackageNames(imports);
           const lines = code.split(/\r?\n/); // Split the code into lines
           const dependencyLine = lines[2]; // Extract dependencies from the third line (index 2, as arrays are zero-indexed)
-          const dependencies = dependencyLine.startsWith("# Additional imports: ") // Assuming the structure is "# Additional imports: package1, package2, ..."
+          const dependencies = dependencyLine.startsWith("# Additional dependencies: ") // Assuming the structure is "# Additional imports: package1, package2, ..."
             ? dependencyLine.split(': ')[1].split(',').map(pkg => pkg.trim())
             : [];
           packages = [...packages, ...dependencies];
 
           if (packages.length > 0 && packages[0] != null && packages[0] !== '') {
             const pips_code = PipelineService.getInstallCommandsFromPackageNames(packages).join('\n');
             // Install packages
@@ -384,65 +386,28 @@
         });
 
         // Third, run pipeline code
         current.context.sessionContext.ready.then(async () => {
 
         try {
         // Create promise to track success or failure of the request
-        const delegate = new PromiseDelegate<ReadonlyJSONValue>();
-        const start = performance.now();
 
-        Notification.promise(delegate.promise, {
-          // Message when the task is pending
-          pending: { message: 'Running...', options: { autoClose: false } },
-          // Message when the task finished successfully
-          success: {
-            message: (result: any) => `Pipeline execution successful after ${result.delayInSeconds} seconds.`,
-            options: {
-              autoClose: 3000
-            }
-          },
-          // Message when the task finished with errors
-          error: {
-            message: () => 'Pipeline execution failed. Check error messages in the Log Console.',
-            options: {
-              actions: [
-                {
-                  label: 'Log Console',
-                  callback: () => {
-                    const command = 'pipeline-console:open';
-                    commands.execute(command, {}).catch(reason => {
-                      console.error(
-                        `An error occurred during the execution of ${command}.\n${reason}`
-                      );
-                    });
-                  }
-                }
-              ],
-              autoClose: 5000
-            }
-          }
-        });
 
             const future = current.context.sessionContext.session.kernel!.requestExecute({ code: args.code });
 
             future.onReply = reply => {
 
-              const end = performance.now();
-              const delay = end - start;
-              const delayInSeconds = (delay / 1000).toFixed(1);
-
               if (reply.content.status == "ok") {
-                delegate.resolve({ delayInSeconds });
+                console.log("Execution: OK")
               } else if (reply.content.status == "error") {
-                delegate.reject({ delayInSeconds });
+                console.error("Execution: error")
               } else if (reply.content.status == "abort") {
-                delegate.reject({ delayInSeconds });
+                console.log("Execution: abort")
               } else {
-                delegate.reject({ delayInSeconds });
+                console.log("Execution: unknown")
               }
             };
 
             future.onIOPub = msg => {
 
               if (msg.header.msg_type === 'stream') {
                 const streamMsg = msg as KernelMessage.IStreamMsg;
```

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-editor/style/canvas.css` & `jupyterlab_amphi-0.3.2/packages/pipeline-editor/style/canvas.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-editor/style/output.css` & `jupyterlab_amphi-0.3.2/packages/pipeline-editor/style/output.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-editor/style/pipeline-category-icon.svg` & `jupyterlab_amphi-0.3.2/packages/pipeline-editor/style/pipeline-category-icon.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-editor/style/react-icon.svg` & `jupyterlab_amphi-0.3.2/packages/pipeline-editor/style/react-icon.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-editor/style/icons/api-24.svg` & `jupyterlab_amphi-0.3.2/packages/pipeline-editor/style/icons/api-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-editor/style/icons/file-plus-24.svg` & `jupyterlab_amphi-0.3.2/packages/pipeline-editor/style/icons/file-plus-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-editor/style/icons/file-text-24.svg` & `jupyterlab_amphi-0.3.2/packages/pipeline-editor/style/icons/file-text-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-editor/style/icons/pipeline-brand-16.svg` & `jupyterlab_amphi-0.3.2/packages/pipeline-editor/style/icons/pipeline-brand-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/packages/pipeline-editor/style/icons/pipeline-brand-24.svg` & `jupyterlab_amphi-0.3.2/packages/pipeline-editor/style/icons/pipeline-brand-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/LICENSE` & `jupyterlab_amphi-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/README.md` & `jupyterlab_amphi-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/pyproject.toml` & `jupyterlab_amphi-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.1/PKG-INFO` & `jupyterlab_amphi-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab-amphi
-Version: 0.3.1
+Version: 0.3.2
 Dynamic: Keywords
 Summary: Amphi is a micro ETL for Jupyterlab.
 Project-URL: Homepage, https://amphi.ai
 Project-URL: Bug Tracker, https://github.com/amphi-ai/jupyterlab-amphi/issues
 Project-URL: Repository, https://github.com/amphi-ai/jupyterlab-amphi.git
 Author-email: Thibaut Gourdel <tgourdel@amphi.ai>
 License: Elastic License 2.0 \(ELv2\)
```

