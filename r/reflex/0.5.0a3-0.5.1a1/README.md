# Comparing `tmp/reflex-0.5.0a3.tar.gz` & `tmp/reflex-0.5.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-0.5.0a3.tar", max compression
+gzip compressed data, was "reflex-0.5.1a1.tar", max compression
```

## Comparing `reflex-0.5.0a3.tar` & `reflex-0.5.1a1.tar`

### file list

```diff
@@ -1,520 +1,522 @@
--rw-r--r--   0        0        0    11358 2023-07-20 22:42:41.698164 reflex-0.5.0a3/LICENSE
--rw-r--r--   0        0        0     9842 2024-05-07 15:33:05.680965 reflex-0.5.0a3/README.md
--rw-r--r--   0        0        0     2974 2024-05-13 23:06:02.764016 reflex-0.5.0a3/pyproject.toml
--rw-r--r--   0        0        0     4286 2023-11-09 03:24:59.498329 reflex-0.5.0a3/reflex/.templates/apps/blank/assets/favicon.ico
--rw-r--r--   0        0        0        0 2023-11-09 03:24:59.498383 reflex-0.5.0a3/reflex/.templates/apps/blank/code/__init__.py
--rw-r--r--   0        0        0      926 2024-05-09 00:05:27.334397 reflex-0.5.0a3/reflex/.templates/apps/blank/code/blank.py
--rw-r--r--   0        0        0       32 2023-11-09 03:24:59.498951 reflex-0.5.0a3/reflex/.templates/apps/demo/.gitignore
--rw-r--r--   0        0        0     4286 2023-11-09 03:24:59.499075 reflex-0.5.0a3/reflex/.templates/apps/demo/assets/favicon.ico
--rw-r--r--   0        0        0     1475 2023-11-09 03:24:59.499137 reflex-0.5.0a3/reflex/.templates/apps/demo/assets/github.svg
--rw-r--r--   0        0        0     1899 2023-11-09 03:24:59.499199 reflex-0.5.0a3/reflex/.templates/apps/demo/assets/icon.svg
--rw-r--r--   0        0        0     5403 2023-11-09 03:24:59.499298 reflex-0.5.0a3/reflex/.templates/apps/demo/assets/logo.svg
--rw-r--r--   0        0        0      807 2023-11-09 03:24:59.499362 reflex-0.5.0a3/reflex/.templates/apps/demo/assets/paneleft.svg
--rw-r--r--   0        0        0       32 2023-11-09 03:24:59.499458 reflex-0.5.0a3/reflex/.templates/apps/demo/code/__init__.py
--rw-r--r--   0        0        0     2927 2024-05-13 23:05:41.140799 reflex-0.5.0a3/reflex/.templates/apps/demo/code/demo.py
--rw-r--r--   0        0        0      194 2023-11-09 03:24:59.499716 reflex-0.5.0a3/reflex/.templates/apps/demo/code/pages/__init__.py
--rw-r--r--   0        0        0      706 2024-02-17 20:02:02.399560 reflex-0.5.0a3/reflex/.templates/apps/demo/code/pages/chatapp.py
--rw-r--r--   0        0        0    10906 2024-04-24 21:16:40.835599 reflex-0.5.0a3/reflex/.templates/apps/demo/code/pages/datatable.py
--rw-r--r--   0        0        0     8381 2024-04-24 21:16:40.835772 reflex-0.5.0a3/reflex/.templates/apps/demo/code/pages/forms.py
--rw-r--r--   0        0        0     8519 2024-03-20 23:54:55.830529 reflex-0.5.0a3/reflex/.templates/apps/demo/code/pages/graphing.py
--rw-r--r--   0        0        0     1822 2024-02-17 20:02:02.400769 reflex-0.5.0a3/reflex/.templates/apps/demo/code/pages/home.py
--rw-r--r--   0        0        0     4722 2024-02-17 20:02:02.400919 reflex-0.5.0a3/reflex/.templates/apps/demo/code/sidebar.py
--rw-r--r--   0        0        0      510 2023-11-09 03:24:59.500529 reflex-0.5.0a3/reflex/.templates/apps/demo/code/state.py
--rw-r--r--   0        0        0      912 2023-11-09 03:24:59.500616 reflex-0.5.0a3/reflex/.templates/apps/demo/code/states/form_state.py
--rw-r--r--   0        0        0     1189 2023-11-09 03:24:59.500682 reflex-0.5.0a3/reflex/.templates/apps/demo/code/states/pie_state.py
--rw-r--r--   0        0        0     1486 2024-02-17 20:02:02.401042 reflex-0.5.0a3/reflex/.templates/apps/demo/code/styles.py
--rw-r--r--   0        0        0        0 2023-11-09 03:24:59.500792 reflex-0.5.0a3/reflex/.templates/apps/demo/code/webui/__init__.py
--rw-r--r--   0        0        0      120 2023-11-09 03:24:59.500879 reflex-0.5.0a3/reflex/.templates/apps/demo/code/webui/components/__init__.py
--rw-r--r--   0        0        0     3584 2024-02-17 20:02:02.401162 reflex-0.5.0a3/reflex/.templates/apps/demo/code/webui/components/chat.py
--rw-r--r--   0        0        0      680 2023-11-09 03:24:59.500996 reflex-0.5.0a3/reflex/.templates/apps/demo/code/webui/components/loading_icon.py
--rw-r--r--   0        0        0     1829 2024-02-17 20:02:02.401269 reflex-0.5.0a3/reflex/.templates/apps/demo/code/webui/components/modal.py
--rw-r--r--   0        0        0     2251 2024-02-17 20:02:02.401372 reflex-0.5.0a3/reflex/.templates/apps/demo/code/webui/components/navbar.py
--rw-r--r--   0        0        0     1735 2024-02-17 20:02:02.401457 reflex-0.5.0a3/reflex/.templates/apps/demo/code/webui/components/sidebar.py
--rw-r--r--   0        0        0     4001 2023-11-09 03:24:59.501230 reflex-0.5.0a3/reflex/.templates/apps/demo/code/webui/state.py
--rw-r--r--   0        0        0     2281 2024-02-17 20:02:02.401582 reflex-0.5.0a3/reflex/.templates/apps/demo/code/webui/styles.py
--rw-r--r--   0        0        0       74 2023-10-22 18:57:13.188650 reflex-0.5.0a3/reflex/.templates/jinja/app/rxconfig.py.jinja2
--rw-r--r--   0        0        0      127 2024-03-20 23:54:55.833038 reflex-0.5.0a3/reflex/.templates/jinja/custom_components/README.md.jinja2
--rw-r--r--   0        0        0       32 2024-03-20 23:54:55.833129 reflex-0.5.0a3/reflex/.templates/jinja/custom_components/__init__.py.jinja2
--rw-r--r--   0        0        0      826 2024-03-20 23:54:55.833525 reflex-0.5.0a3/reflex/.templates/jinja/custom_components/demo_app.py.jinja2
--rw-r--r--   0        0        0      614 2024-04-04 14:57:26.374812 reflex-0.5.0a3/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2
--rw-r--r--   0        0        0     2403 2024-04-05 17:14:14.457446 reflex-0.5.0a3/reflex/.templates/jinja/custom_components/src.py.jinja2
--rw-r--r--   0        0        0      548 2023-10-22 18:57:13.188813 reflex-0.5.0a3/reflex/.templates/jinja/web/package.json.jinja2
--rw-r--r--   0        0        0      930 2024-03-20 23:54:55.834237 reflex-0.5.0a3/reflex/.templates/jinja/web/pages/_app.js.jinja2
--rw-r--r--   0        0        0      182 2023-07-20 22:42:41.708822 reflex-0.5.0a3/reflex/.templates/jinja/web/pages/_document.js.jinja2
--rw-r--r--   0        0        0      400 2024-02-06 00:51:31.970380 reflex-0.5.0a3/reflex/.templates/jinja/web/pages/base_page.js.jinja2
--rw-r--r--   0        0        0       86 2023-10-22 18:57:13.188983 reflex-0.5.0a3/reflex/.templates/jinja/web/pages/component.js.jinja2
--rw-r--r--   0        0        0      882 2023-12-01 04:51:31.091531 reflex-0.5.0a3/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
--rw-r--r--   0        0        0      343 2024-04-04 14:57:26.375114 reflex-0.5.0a3/reflex/.templates/jinja/web/pages/index.js.jinja2
--rw-r--r--   0        0        0      388 2024-04-05 17:14:14.457553 reflex-0.5.0a3/reflex/.templates/jinja/web/pages/stateful_component.js.jinja2
--rw-r--r--   0        0        0      101 2023-12-01 04:51:31.092250 reflex-0.5.0a3/reflex/.templates/jinja/web/pages/stateful_components.js.jinja2
--rw-r--r--   0        0        0     3883 2024-02-06 00:51:31.970618 reflex-0.5.0a3/reflex/.templates/jinja/web/pages/utils.js.jinja2
--rw-r--r--   0        0        0      141 2023-12-06 18:41:46.628030 reflex-0.5.0a3/reflex/.templates/jinja/web/styles/styles.css.jinja2
--rw-r--r--   0        0        0      761 2024-05-11 03:29:42.707807 reflex-0.5.0a3/reflex/.templates/jinja/web/tailwind.config.js.jinja2
--rw-r--r--   0        0        0     3790 2024-03-20 23:54:55.834608 reflex-0.5.0a3/reflex/.templates/jinja/web/utils/context.js.jinja2
--rw-r--r--   0        0        0       37 2023-12-06 19:37:00.189183 reflex-0.5.0a3/reflex/.templates/jinja/web/utils/theme.js.jinja2
--rw-r--r--   0        0        0      417 2023-07-20 22:42:41.709243 reflex-0.5.0a3/reflex/.templates/web/.gitignore
--rw-r--r--   0        0        0      595 2023-10-30 01:36:56.133208 reflex-0.5.0a3/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js
--rw-r--r--   0        0        0      645 2024-03-20 23:54:55.835034 reflex-0.5.0a3/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js
--rw-r--r--   0        0        0       97 2023-10-22 18:57:13.190257 reflex-0.5.0a3/reflex/.templates/web/jsconfig.json
--rw-r--r--   0        0        0      118 2023-11-22 05:49:24.669539 reflex-0.5.0a3/reflex/.templates/web/next.config.js
--rw-r--r--   0        0        0       82 2023-07-20 22:42:41.710359 reflex-0.5.0a3/reflex/.templates/web/postcss.config.js
--rw-r--r--   0        0        0       59 2023-07-20 22:42:41.710616 reflex-0.5.0a3/reflex/.templates/web/styles/tailwind.css
--rw-r--r--   0        0        0     1254 2023-09-16 20:27:37.277783 reflex-0.5.0a3/reflex/.templates/web/utils/client_side_routing.js
--rw-r--r--   0        0        0     1622 2024-02-06 00:51:31.970968 reflex-0.5.0a3/reflex/.templates/web/utils/helpers/dataeditor.js
--rw-r--r--   0        0        0      528 2024-05-05 01:15:24.052298 reflex-0.5.0a3/reflex/.templates/web/utils/helpers/debounce.js
--rw-r--r--   0        0        0     1152 2023-11-22 05:49:24.669991 reflex-0.5.0a3/reflex/.templates/web/utils/helpers/range.js
--rw-r--r--   0        0        0      566 2024-05-05 01:15:24.052363 reflex-0.5.0a3/reflex/.templates/web/utils/helpers/throttle.js
--rw-r--r--   0        0        0    22511 2024-05-05 01:15:24.052487 reflex-0.5.0a3/reflex/.templates/web/utils/state.js
--rw-r--r--   0        0        0     5831 2024-05-09 00:05:27.334655 reflex-0.5.0a3/reflex/__init__.py
--rw-r--r--   0        0        0     7791 2024-05-09 12:11:15.217578 reflex-0.5.0a3/reflex/__init__.pyi
--rw-r--r--   0        0        0      108 2023-08-05 17:01:44.301997 reflex-0.5.0a3/reflex/__main__.py
--rw-r--r--   0        0        0      373 2023-07-20 22:42:41.710893 reflex-0.5.0a3/reflex/admin.py
--rw-r--r--   0        0        0    46314 2024-05-09 00:05:27.335022 reflex-0.5.0a3/reflex/app.py
--rw-r--r--   0        0        0     1152 2024-05-05 01:15:24.053241 reflex-0.5.0a3/reflex/app_module_for_backend.py
--rw-r--r--   0        0        0     4213 2024-05-09 00:05:27.335300 reflex-0.5.0a3/reflex/base.py
--rw-r--r--   0        0        0       27 2023-07-20 22:42:41.711176 reflex-0.5.0a3/reflex/compiler/__init__.py
--rw-r--r--   0        0        0    17455 2024-05-07 15:33:05.682544 reflex-0.5.0a3/reflex/compiler/compiler.py
--rw-r--r--   0        0        0     4344 2024-03-20 23:54:55.838388 reflex-0.5.0a3/reflex/compiler/templates.py
--rw-r--r--   0        0        0    13274 2024-05-09 00:05:27.335443 reflex-0.5.0a3/reflex/compiler/utils.py
--rw-r--r--   0        0        0      552 2024-05-05 01:15:24.053486 reflex-0.5.0a3/reflex/components/__init__.py
--rw-r--r--   0        0        0      325 2024-02-06 00:51:31.973078 reflex-0.5.0a3/reflex/components/base/__init__.py
--rw-r--r--   0        0        0      573 2024-02-06 00:51:31.973178 reflex-0.5.0a3/reflex/components/base/app_wrap.py
--rw-r--r--   0        0        0     2890 2024-04-24 19:31:24.924269 reflex-0.5.0a3/reflex/components/base/app_wrap.pyi
--rw-r--r--   0        0        0     1234 2024-04-04 14:57:26.376921 reflex-0.5.0a3/reflex/components/base/bare.py
--rw-r--r--   0        0        0      151 2023-07-20 22:42:41.711762 reflex-0.5.0a3/reflex/components/base/body.py
--rw-r--r--   0        0        0     3206 2024-04-24 19:31:56.503225 reflex-0.5.0a3/reflex/components/base/body.pyi
--rw-r--r--   0        0        0      583 2024-03-20 23:54:55.839153 reflex-0.5.0a3/reflex/components/base/document.py
--rw-r--r--   0        0        0    14232 2024-04-24 19:31:51.758673 reflex-0.5.0a3/reflex/components/base/document.pyi
--rw-r--r--   0        0        0      312 2024-02-06 00:51:31.973871 reflex-0.5.0a3/reflex/components/base/fragment.py
--rw-r--r--   0        0        0     3218 2024-04-24 19:31:51.784884 reflex-0.5.0a3/reflex/components/base/fragment.pyi
--rw-r--r--   0        0        0      297 2023-12-05 17:15:35.585518 reflex-0.5.0a3/reflex/components/base/head.py
--rw-r--r--   0        0        0     6002 2024-04-24 19:31:53.335977 reflex-0.5.0a3/reflex/components/base/head.pyi
--rw-r--r--   0        0        0      929 2023-07-20 22:42:41.711911 reflex-0.5.0a3/reflex/components/base/link.py
--rw-r--r--   0        0        0     6990 2024-04-24 19:31:27.077164 reflex-0.5.0a3/reflex/components/base/link.pyi
--rw-r--r--   0        0        0     1438 2023-09-16 20:27:37.279391 reflex-0.5.0a3/reflex/components/base/meta.py
--rw-r--r--   0        0        0    12804 2024-04-24 19:31:22.783259 reflex-0.5.0a3/reflex/components/base/meta.pyi
--rw-r--r--   0        0        0     2298 2023-10-30 01:36:56.136333 reflex-0.5.0a3/reflex/components/base/script.py
--rw-r--r--   0        0        0     4500 2024-04-24 19:31:45.804898 reflex-0.5.0a3/reflex/components/base/script.pyi
--rw-r--r--   0        0        0     6378 2024-02-17 20:02:02.406461 reflex-0.5.0a3/reflex/components/chakra/__init__.py
--rw-r--r--   0        0        0     5242 2024-02-07 21:49:00.589344 reflex-0.5.0a3/reflex/components/chakra/base.py
--rw-r--r--   0        0        0    10917 2024-04-24 19:31:39.254151 reflex-0.5.0a3/reflex/components/chakra/base.pyi
--rw-r--r--   0        0        0      459 2024-02-17 20:02:02.406937 reflex-0.5.0a3/reflex/components/chakra/datadisplay/__init__.py
--rw-r--r--   0        0        0      352 2024-02-07 21:48:43.271089 reflex-0.5.0a3/reflex/components/chakra/datadisplay/badge.py
--rw-r--r--   0        0        0     3654 2024-04-24 19:31:56.520176 reflex-0.5.0a3/reflex/components/chakra/datadisplay/badge.pyi
--rw-r--r--   0        0        0      174 2024-02-17 20:02:02.407242 reflex-0.5.0a3/reflex/components/chakra/datadisplay/code.py
--rw-r--r--   0        0        0     3229 2024-04-24 19:31:20.836024 reflex-0.5.0a3/reflex/components/chakra/datadisplay/code.pyi
--rw-r--r--   0        0        0      657 2024-02-07 21:48:43.271979 reflex-0.5.0a3/reflex/components/chakra/datadisplay/divider.py
--rw-r--r--   0        0        0     3934 2024-04-24 19:31:33.713586 reflex-0.5.0a3/reflex/components/chakra/datadisplay/divider.pyi
--rw-r--r--   0        0        0      180 2024-02-07 21:48:43.272341 reflex-0.5.0a3/reflex/components/chakra/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     3251 2024-04-24 19:31:32.872876 reflex-0.5.0a3/reflex/components/chakra/datadisplay/keyboard_key.pyi
--rw-r--r--   0        0        0     1484 2024-05-05 01:15:24.053780 reflex-0.5.0a3/reflex/components/chakra/datadisplay/list.py
--rw-r--r--   0        0        0    12991 2024-05-05 01:15:24.053953 reflex-0.5.0a3/reflex/components/chakra/datadisplay/list.pyi
--rw-r--r--   0        0        0     2149 2024-02-07 21:48:43.272980 reflex-0.5.0a3/reflex/components/chakra/datadisplay/stat.py
--rw-r--r--   0        0        0    17461 2024-04-24 19:31:58.481785 reflex-0.5.0a3/reflex/components/chakra/datadisplay/stat.pyi
--rw-r--r--   0        0        0     9122 2024-02-07 21:48:43.273484 reflex-0.5.0a3/reflex/components/chakra/datadisplay/table.py
--rw-r--r--   0        0        0    27252 2024-04-24 19:32:01.076794 reflex-0.5.0a3/reflex/components/chakra/datadisplay/table.pyi
--rw-r--r--   0        0        0     2294 2024-02-07 21:48:43.273971 reflex-0.5.0a3/reflex/components/chakra/datadisplay/tag.py
--rw-r--r--   0        0        0    15734 2024-04-24 19:31:39.394572 reflex-0.5.0a3/reflex/components/chakra/datadisplay/tag.pyi
--rw-r--r--   0        0        0      384 2024-02-06 00:51:31.976988 reflex-0.5.0a3/reflex/components/chakra/disclosure/__init__.py
--rw-r--r--   0        0        0     3510 2024-04-24 21:16:40.836539 reflex-0.5.0a3/reflex/components/chakra/disclosure/accordion.py
--rw-r--r--   0        0        0    15803 2024-04-24 19:31:46.785267 reflex-0.5.0a3/reflex/components/chakra/disclosure/accordion.pyi
--rw-r--r--   0        0        0     3295 2024-02-07 21:48:43.274669 reflex-0.5.0a3/reflex/components/chakra/disclosure/tabs.py
--rw-r--r--   0        0        0    18525 2024-04-24 19:31:51.181381 reflex-0.5.0a3/reflex/components/chakra/disclosure/tabs.pyi
--rw-r--r--   0        0        0     1732 2024-02-07 21:48:43.274917 reflex-0.5.0a3/reflex/components/chakra/disclosure/transition.py
--rw-r--r--   0        0        0    20003 2024-04-24 19:31:47.452515 reflex-0.5.0a3/reflex/components/chakra/disclosure/transition.pyi
--rw-r--r--   0        0        0      278 2024-02-07 21:48:43.275325 reflex-0.5.0a3/reflex/components/chakra/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0     3258 2024-04-24 19:31:21.739444 reflex-0.5.0a3/reflex/components/chakra/disclosure/visuallyhidden.pyi
--rw-r--r--   0        0        0      313 2024-02-06 00:51:31.977813 reflex-0.5.0a3/reflex/components/chakra/feedback/__init__.py
--rw-r--r--   0        0        0     1623 2024-02-07 21:48:43.275534 reflex-0.5.0a3/reflex/components/chakra/feedback/alert.py
--rw-r--r--   0        0        0    12381 2024-04-24 19:31:36.018582 reflex-0.5.0a3/reflex/components/chakra/feedback/alert.pyi
--rw-r--r--   0        0        0     2006 2024-02-07 21:48:43.275746 reflex-0.5.0a3/reflex/components/chakra/feedback/circularprogress.py
--rw-r--r--   0        0        0     7637 2024-04-24 19:31:35.464688 reflex-0.5.0a3/reflex/components/chakra/feedback/circularprogress.pyi
--rw-r--r--   0        0        0      871 2024-02-07 21:48:43.275966 reflex-0.5.0a3/reflex/components/chakra/feedback/progress.py
--rw-r--r--   0        0        0     4278 2024-04-24 19:31:39.746055 reflex-0.5.0a3/reflex/components/chakra/feedback/progress.pyi
--rw-r--r--   0        0        0     1776 2024-02-07 21:48:43.276180 reflex-0.5.0a3/reflex/components/chakra/feedback/skeleton.py
--rw-r--r--   0        0        0    10690 2024-04-24 19:32:01.405002 reflex-0.5.0a3/reflex/components/chakra/feedback/skeleton.pyi
--rw-r--r--   0        0        0      704 2024-02-07 21:48:43.276461 reflex-0.5.0a3/reflex/components/chakra/feedback/spinner.py
--rw-r--r--   0        0        0     4107 2024-04-24 19:31:21.992081 reflex-0.5.0a3/reflex/components/chakra/feedback/spinner.pyi
--rw-r--r--   0        0        0     1453 2024-02-17 20:02:02.409691 reflex-0.5.0a3/reflex/components/chakra/forms/__init__.py
--rw-r--r--   0        0        0     2395 2024-02-07 21:48:43.276688 reflex-0.5.0a3/reflex/components/chakra/forms/button.py
--rw-r--r--   0        0        0    10545 2024-04-24 19:32:02.037829 reflex-0.5.0a3/reflex/components/chakra/forms/button.pyi
--rw-r--r--   0        0        0     2764 2024-02-07 21:48:43.277006 reflex-0.5.0a3/reflex/components/chakra/forms/checkbox.py
--rw-r--r--   0        0        0    10301 2024-04-24 19:31:34.287807 reflex-0.5.0a3/reflex/components/chakra/forms/checkbox.pyi
--rw-r--r--   0        0        0     2860 2024-02-17 20:02:02.410102 reflex-0.5.0a3/reflex/components/chakra/forms/colormodeswitch.py
--rw-r--r--   0        0        0    18459 2024-04-24 19:31:24.856589 reflex-0.5.0a3/reflex/components/chakra/forms/colormodeswitch.pyi
--rw-r--r--   0        0        0      246 2024-02-06 00:51:31.979244 reflex-0.5.0a3/reflex/components/chakra/forms/date_picker.py
--rw-r--r--   0        0        0     5841 2024-04-24 19:31:54.024641 reflex-0.5.0a3/reflex/components/chakra/forms/date_picker.pyi
--rw-r--r--   0        0        0      280 2024-02-06 00:51:31.979387 reflex-0.5.0a3/reflex/components/chakra/forms/date_time_picker.py
--rw-r--r--   0        0        0     5854 2024-04-24 19:31:40.823621 reflex-0.5.0a3/reflex/components/chakra/forms/date_time_picker.pyi
--rw-r--r--   0        0        0     2110 2024-02-07 21:48:43.277649 reflex-0.5.0a3/reflex/components/chakra/forms/editable.py
--rw-r--r--   0        0        0    13339 2024-04-24 19:31:15.703021 reflex-0.5.0a3/reflex/components/chakra/forms/editable.pyi
--rw-r--r--   0        0        0      246 2024-02-06 00:51:31.979682 reflex-0.5.0a3/reflex/components/chakra/forms/email.py
--rw-r--r--   0        0        0     5825 2024-04-24 19:31:50.788652 reflex-0.5.0a3/reflex/components/chakra/forms/email.pyi
--rw-r--r--   0        0        0     2579 2024-03-20 23:54:55.839690 reflex-0.5.0a3/reflex/components/chakra/forms/form.py
--rw-r--r--   0        0        0    20619 2024-04-24 19:31:56.858215 reflex-0.5.0a3/reflex/components/chakra/forms/form.pyi
--rw-r--r--   0        0        0      935 2024-02-06 00:51:31.980162 reflex-0.5.0a3/reflex/components/chakra/forms/iconbutton.py
--rw-r--r--   0        0        0     4668 2024-04-24 19:31:50.346409 reflex-0.5.0a3/reflex/components/chakra/forms/iconbutton.pyi
--rw-r--r--   0        0        0     4312 2024-03-20 23:54:55.840321 reflex-0.5.0a3/reflex/components/chakra/forms/input.py
--rw-r--r--   0        0        0    21514 2024-04-24 19:31:59.673777 reflex-0.5.0a3/reflex/components/chakra/forms/input.pyi
--rw-r--r--   0        0        0    12940 2024-02-06 00:51:31.980569 reflex-0.5.0a3/reflex/components/chakra/forms/multiselect.py
--rw-r--r--   0        0        0     4334 2024-02-07 21:48:43.278754 reflex-0.5.0a3/reflex/components/chakra/forms/numberinput.py
--rw-r--r--   0        0        0    18093 2024-04-24 19:31:56.097983 reflex-0.5.0a3/reflex/components/chakra/forms/numberinput.pyi
--rw-r--r--   0        0        0      256 2024-02-06 00:51:31.980851 reflex-0.5.0a3/reflex/components/chakra/forms/password.py
--rw-r--r--   0        0        0     5834 2024-04-24 19:31:37.858051 reflex-0.5.0a3/reflex/components/chakra/forms/password.pyi
--rw-r--r--   0        0        0     6503 2024-04-12 01:14:12.262063 reflex-0.5.0a3/reflex/components/chakra/forms/pininput.py
--rw-r--r--   0        0        0     9369 2024-05-05 01:15:24.054063 reflex-0.5.0a3/reflex/components/chakra/forms/pininput.pyi
--rw-r--r--   0        0        0     3172 2024-04-12 01:14:12.263122 reflex-0.5.0a3/reflex/components/chakra/forms/radio.py
--rw-r--r--   0        0        0     8410 2024-04-24 19:31:17.428977 reflex-0.5.0a3/reflex/components/chakra/forms/radio.pyi
--rw-r--r--   0        0        0     4543 2024-04-12 01:14:12.263746 reflex-0.5.0a3/reflex/components/chakra/forms/rangeslider.py
--rw-r--r--   0        0        0    13939 2024-04-24 19:31:59.377848 reflex-0.5.0a3/reflex/components/chakra/forms/rangeslider.pyi
--rw-r--r--   0        0        0     3624 2024-02-07 21:48:43.280461 reflex-0.5.0a3/reflex/components/chakra/forms/select.py
--rw-r--r--   0        0        0     8868 2024-04-24 19:31:48.346816 reflex-0.5.0a3/reflex/components/chakra/forms/select.pyi
--rw-r--r--   0        0        0     3532 2024-02-07 21:48:43.280779 reflex-0.5.0a3/reflex/components/chakra/forms/slider.py
--rw-r--r--   0        0        0    17461 2024-04-24 19:32:01.264082 reflex-0.5.0a3/reflex/components/chakra/forms/slider.pyi
--rw-r--r--   0        0        0     1838 2024-02-07 21:48:43.281044 reflex-0.5.0a3/reflex/components/chakra/forms/switch.py
--rw-r--r--   0        0        0     6531 2024-04-24 19:31:48.016708 reflex-0.5.0a3/reflex/components/chakra/forms/switch.pyi
--rw-r--r--   0        0        0     2474 2024-02-09 10:00:28.809203 reflex-0.5.0a3/reflex/components/chakra/forms/textarea.py
--rw-r--r--   0        0        0     5419 2024-04-24 19:31:51.889720 reflex-0.5.0a3/reflex/components/chakra/forms/textarea.pyi
--rw-r--r--   0        0        0      246 2024-02-06 00:51:31.982573 reflex-0.5.0a3/reflex/components/chakra/forms/time_picker.py
--rw-r--r--   0        0        0     5841 2024-04-24 19:31:46.686774 reflex-0.5.0a3/reflex/components/chakra/forms/time_picker.pyi
--rw-r--r--   0        0        0      487 2024-02-17 20:02:02.413006 reflex-0.5.0a3/reflex/components/chakra/layout/__init__.py
--rw-r--r--   0        0        0      315 2024-02-07 21:48:43.281752 reflex-0.5.0a3/reflex/components/chakra/layout/aspect_ratio.py
--rw-r--r--   0        0        0     3379 2024-04-24 19:31:52.881611 reflex-0.5.0a3/reflex/components/chakra/layout/aspect_ratio.pyi
--rw-r--r--   0        0        0      755 2024-02-07 21:48:43.281982 reflex-0.5.0a3/reflex/components/chakra/layout/box.py
--rw-r--r--   0        0        0     3662 2024-04-24 19:31:18.516418 reflex-0.5.0a3/reflex/components/chakra/layout/box.pyi
--rw-r--r--   0        0        0     2967 2024-02-07 21:48:43.282202 reflex-0.5.0a3/reflex/components/chakra/layout/card.py
--rw-r--r--   0        0        0    13850 2024-04-24 19:31:48.005155 reflex-0.5.0a3/reflex/components/chakra/layout/card.pyi
--rw-r--r--   0        0        0      389 2024-02-07 21:48:43.282417 reflex-0.5.0a3/reflex/components/chakra/layout/center.py
--rw-r--r--   0        0        0     8692 2024-04-24 19:31:24.264440 reflex-0.5.0a3/reflex/components/chakra/layout/center.pyi
--rw-r--r--   0        0        0      354 2024-02-07 21:48:43.282843 reflex-0.5.0a3/reflex/components/chakra/layout/container.py
--rw-r--r--   0        0        0     3431 2024-04-24 19:31:47.990635 reflex-0.5.0a3/reflex/components/chakra/layout/container.pyi
--rw-r--r--   0        0        0      715 2024-02-07 21:48:43.283082 reflex-0.5.0a3/reflex/components/chakra/layout/flex.py
--rw-r--r--   0        0        0     4138 2024-04-24 19:31:44.830583 reflex-0.5.0a3/reflex/components/chakra/layout/flex.pyi
--rw-r--r--   0        0        0     4318 2024-02-07 21:48:43.283328 reflex-0.5.0a3/reflex/components/chakra/layout/grid.py
--rw-r--r--   0        0        0    13853 2024-04-24 19:31:41.333938 reflex-0.5.0a3/reflex/components/chakra/layout/grid.pyi
--rw-r--r--   0        0        0      179 2024-02-07 21:48:43.283579 reflex-0.5.0a3/reflex/components/chakra/layout/spacer.py
--rw-r--r--   0        0        0     3230 2024-04-24 19:31:48.988499 reflex-0.5.0a3/reflex/components/chakra/layout/spacer.pyi
--rw-r--r--   0        0        0     1077 2024-02-07 21:48:43.283791 reflex-0.5.0a3/reflex/components/chakra/layout/stack.py
--rw-r--r--   0        0        0    12219 2024-04-24 19:31:34.279618 reflex-0.5.0a3/reflex/components/chakra/layout/stack.pyi
--rw-r--r--   0        0        0     1463 2024-02-07 21:48:43.284089 reflex-0.5.0a3/reflex/components/chakra/layout/wrap.py
--rw-r--r--   0        0        0     6943 2024-04-24 19:31:33.351664 reflex-0.5.0a3/reflex/components/chakra/layout/wrap.pyi
--rw-r--r--   0        0        0      190 2024-02-06 00:51:31.985088 reflex-0.5.0a3/reflex/components/chakra/media/__init__.py
--rw-r--r--   0        0        0     1668 2024-02-07 21:48:43.284332 reflex-0.5.0a3/reflex/components/chakra/media/avatar.py
--rw-r--r--   0        0        0    10445 2024-04-24 19:31:27.389378 reflex-0.5.0a3/reflex/components/chakra/media/avatar.pyi
--rw-r--r--   0        0        0     2462 2024-04-24 21:16:40.836689 reflex-0.5.0a3/reflex/components/chakra/media/icon.py
--rw-r--r--   0        0        0     6271 2024-04-24 19:31:19.854478 reflex-0.5.0a3/reflex/components/chakra/media/icon.pyi
--rw-r--r--   0        0        0     2400 2024-02-07 21:48:43.284781 reflex-0.5.0a3/reflex/components/chakra/media/image.py
--rw-r--r--   0        0        0     5423 2024-04-24 19:31:52.691354 reflex-0.5.0a3/reflex/components/chakra/media/image.pyi
--rw-r--r--   0        0        0      419 2024-02-06 00:51:31.986093 reflex-0.5.0a3/reflex/components/chakra/navigation/__init__.py
--rw-r--r--   0        0        0     2925 2024-02-07 21:48:43.285023 reflex-0.5.0a3/reflex/components/chakra/navigation/breadcrumb.py
--rw-r--r--   0        0        0    13575 2024-04-24 19:32:01.936776 reflex-0.5.0a3/reflex/components/chakra/navigation/breadcrumb.pyi
--rw-r--r--   0        0        0     1475 2024-02-06 00:51:31.986318 reflex-0.5.0a3/reflex/components/chakra/navigation/link.py
--rw-r--r--   0        0        0     3999 2024-04-24 19:31:19.850596 reflex-0.5.0a3/reflex/components/chakra/navigation/link.pyi
--rw-r--r--   0        0        0      521 2024-02-06 00:51:31.986581 reflex-0.5.0a3/reflex/components/chakra/navigation/linkoverlay.py
--rw-r--r--   0        0        0     6233 2024-04-24 19:31:59.056993 reflex-0.5.0a3/reflex/components/chakra/navigation/linkoverlay.pyi
--rw-r--r--   0        0        0     2935 2024-02-07 21:48:43.285634 reflex-0.5.0a3/reflex/components/chakra/navigation/stepper.py
--rw-r--r--   0        0        0    27922 2024-04-24 19:31:59.991438 reflex-0.5.0a3/reflex/components/chakra/navigation/stepper.pyi
--rw-r--r--   0        0        0      850 2024-02-06 00:51:31.987014 reflex-0.5.0a3/reflex/components/chakra/overlay/__init__.py
--rw-r--r--   0        0        0     5200 2024-02-07 21:48:43.285952 reflex-0.5.0a3/reflex/components/chakra/overlay/alertdialog.py
--rw-r--r--   0        0        0    23985 2024-04-24 19:31:53.441920 reflex-0.5.0a3/reflex/components/chakra/overlay/alertdialog.pyi
--rw-r--r--   0        0        0     5186 2024-02-06 00:51:31.987467 reflex-0.5.0a3/reflex/components/chakra/overlay/drawer.py
--rw-r--r--   0        0        0    25406 2024-04-24 19:32:02.090146 reflex-0.5.0a3/reflex/components/chakra/overlay/drawer.pyi
--rw-r--r--   0        0        0     6974 2024-02-07 21:48:43.286352 reflex-0.5.0a3/reflex/components/chakra/overlay/menu.py
--rw-r--r--   0        0        0    28682 2024-04-24 19:32:03.285218 reflex-0.5.0a3/reflex/components/chakra/overlay/menu.pyi
--rw-r--r--   0        0        0     5270 2024-02-07 21:48:43.286588 reflex-0.5.0a3/reflex/components/chakra/overlay/modal.py
--rw-r--r--   0        0        0    23549 2024-04-24 19:32:01.507839 reflex-0.5.0a3/reflex/components/chakra/overlay/modal.pyi
--rw-r--r--   0        0        0     5967 2024-02-07 21:48:43.286836 reflex-0.5.0a3/reflex/components/chakra/overlay/popover.py
--rw-r--r--   0        0        0    29893 2024-04-24 19:32:01.594206 reflex-0.5.0a3/reflex/components/chakra/overlay/popover.pyi
--rw-r--r--   0        0        0     2127 2024-02-07 21:48:43.287207 reflex-0.5.0a3/reflex/components/chakra/overlay/tooltip.py
--rw-r--r--   0        0        0     6060 2024-04-24 19:31:15.213215 reflex-0.5.0a3/reflex/components/chakra/overlay/tooltip.pyi
--rw-r--r--   0        0        0      271 2024-02-06 00:51:31.988661 reflex-0.5.0a3/reflex/components/chakra/typography/__init__.py
--rw-r--r--   0        0        0      379 2024-02-07 21:48:43.287449 reflex-0.5.0a3/reflex/components/chakra/typography/heading.py
--rw-r--r--   0        0        0     3706 2024-04-24 19:31:17.288584 reflex-0.5.0a3/reflex/components/chakra/typography/heading.pyi
--rw-r--r--   0        0        0      671 2024-02-07 21:48:43.287662 reflex-0.5.0a3/reflex/components/chakra/typography/highlight.py
--rw-r--r--   0        0        0     3645 2024-04-24 19:31:37.053293 reflex-0.5.0a3/reflex/components/chakra/typography/highlight.pyi
--rw-r--r--   0        0        0      328 2024-02-07 21:48:43.287874 reflex-0.5.0a3/reflex/components/chakra/typography/span.py
--rw-r--r--   0        0        0     3372 2024-04-24 19:31:23.281815 reflex-0.5.0a3/reflex/components/chakra/typography/span.pyi
--rw-r--r--   0        0        0      472 2024-02-07 21:48:43.288076 reflex-0.5.0a3/reflex/components/chakra/typography/text.py
--rw-r--r--   0        0        0     3596 2024-04-24 19:31:50.785304 reflex-0.5.0a3/reflex/components/chakra/typography/text.pyi
--rw-r--r--   0        0        0    75744 2024-05-11 03:29:42.708073 reflex-0.5.0a3/reflex/components/component.py
--rw-r--r--   0        0        0      857 2024-04-25 16:52:48.840950 reflex-0.5.0a3/reflex/components/core/__init__.py
--rw-r--r--   0        0        0     5943 2024-04-04 14:57:26.386161 reflex-0.5.0a3/reflex/components/core/banner.py
--rw-r--r--   0        0        0    17164 2024-04-24 19:32:01.784962 reflex-0.5.0a3/reflex/components/core/banner.pyi
--rw-r--r--   0        0        0     1873 2024-02-06 00:51:31.991625 reflex-0.5.0a3/reflex/components/core/client_side_routing.py
--rw-r--r--   0        0        0     6264 2024-04-24 19:31:22.918462 reflex-0.5.0a3/reflex/components/core/client_side_routing.pyi
--rw-r--r--   0        0        0      590 2024-02-17 20:02:02.417474 reflex-0.5.0a3/reflex/components/core/colors.py
--rw-r--r--   0        0        0     6005 2024-05-07 15:33:05.683015 reflex-0.5.0a3/reflex/components/core/cond.py
--rw-r--r--   0        0        0     4888 2024-05-09 00:05:27.335942 reflex-0.5.0a3/reflex/components/core/debounce.py
--rw-r--r--   0        0        0     4216 2024-04-25 16:52:48.841425 reflex-0.5.0a3/reflex/components/core/debounce.pyi
--rw-r--r--   0        0        0     4334 2024-05-11 03:29:42.708393 reflex-0.5.0a3/reflex/components/core/foreach.py
--rw-r--r--   0        0        0     1284 2024-05-05 01:15:24.054752 reflex-0.5.0a3/reflex/components/core/html.py
--rw-r--r--   0        0        0     6616 2024-04-25 05:29:57.085054 reflex-0.5.0a3/reflex/components/core/html.pyi
--rw-r--r--   0        0        0       30 2024-02-07 21:48:43.290204 reflex-0.5.0a3/reflex/components/core/layout/__init__.py
--rw-r--r--   0        0        0     9484 2024-05-07 15:33:05.683232 reflex-0.5.0a3/reflex/components/core/match.py
--rw-r--r--   0        0        0     1907 2024-04-04 14:19:59.331992 reflex-0.5.0a3/reflex/components/core/responsive.py
--rw-r--r--   0        0        0    10193 2024-05-05 01:15:24.055101 reflex-0.5.0a3/reflex/components/core/upload.py
--rw-r--r--   0        0        0    17147 2024-04-25 16:52:48.841883 reflex-0.5.0a3/reflex/components/core/upload.pyi
--rw-r--r--   0        0        0      357 2024-04-05 17:14:14.460655 reflex-0.5.0a3/reflex/components/datadisplay/__init__.py
--rw-r--r--   0        0        0    11363 2024-05-07 15:33:05.683354 reflex-0.5.0a3/reflex/components/datadisplay/code.py
--rw-r--r--   0        0        0    31213 2024-05-07 15:33:05.683489 reflex-0.5.0a3/reflex/components/datadisplay/code.pyi
--rw-r--r--   0        0        0    12632 2024-02-06 00:51:31.995005 reflex-0.5.0a3/reflex/components/datadisplay/dataeditor.py
--rw-r--r--   0        0        0    10485 2024-04-24 19:31:43.237754 reflex-0.5.0a3/reflex/components/datadisplay/dataeditor.pyi
--rw-r--r--   0        0        0     2562 2024-04-05 17:14:14.460754 reflex-0.5.0a3/reflex/components/datadisplay/logo.py
--rw-r--r--   0        0        0       73 2023-11-26 20:56:44.132351 reflex-0.5.0a3/reflex/components/el/__init__.py
--rw-r--r--   0        0        0      113 2023-11-26 20:56:44.132431 reflex-0.5.0a3/reflex/components/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-11-26 20:56:44.132596 reflex-0.5.0a3/reflex/components/el/constants/html.py
--rw-r--r--   0        0        0    15554 2023-11-26 20:56:44.132713 reflex-0.5.0a3/reflex/components/el/constants/react.py
--rw-r--r--   0        0        0     1713 2023-11-26 20:56:44.132789 reflex-0.5.0a3/reflex/components/el/constants/reflex.py
--rw-r--r--   0        0        0      494 2023-12-01 04:51:31.098496 reflex-0.5.0a3/reflex/components/el/element.py
--rw-r--r--   0        0        0     3213 2024-04-24 19:32:01.854505 reflex-0.5.0a3/reflex/components/el/element.pyi
--rw-r--r--   0        0        0     3529 2024-03-20 23:54:55.843475 reflex-0.5.0a3/reflex/components/el/elements/__init__.py
--rw-r--r--   0        0        0     1982 2024-02-17 20:02:02.419390 reflex-0.5.0a3/reflex/components/el/elements/base.py
--rw-r--r--   0        0        0     6340 2024-04-24 19:31:34.952107 reflex-0.5.0a3/reflex/components/el/elements/base.pyi
--rw-r--r--   0        0        0    20103 2024-04-25 16:52:48.842221 reflex-0.5.0a3/reflex/components/el/elements/forms.py
--rw-r--r--   0        0        0    99555 2024-04-25 16:52:48.842962 reflex-0.5.0a3/reflex/components/el/elements/forms.pyi
--rw-r--r--   0        0        0     3610 2024-02-06 00:51:31.998070 reflex-0.5.0a3/reflex/components/el/elements/inline.py
--rw-r--r--   0        0        0   164607 2024-04-24 19:32:05.408521 reflex-0.5.0a3/reflex/components/el/elements/inline.pyi
--rw-r--r--   0        0        0     7929 2024-03-20 23:54:55.844702 reflex-0.5.0a3/reflex/components/el/elements/media.py
--rw-r--r--   0        0        0    93567 2024-04-24 19:32:03.850879 reflex-0.5.0a3/reflex/components/el/elements/media.pyi
--rw-r--r--   0        0        0     1337 2023-11-26 20:56:44.134404 reflex-0.5.0a3/reflex/components/el/elements/metadata.py
--rw-r--r--   0        0        0    28031 2024-04-24 19:32:01.554937 reflex-0.5.0a3/reflex/components/el/elements/metadata.pyi
--rw-r--r--   0        0        0     1569 2023-11-26 20:56:44.134590 reflex-0.5.0a3/reflex/components/el/elements/other.py
--rw-r--r--   0        0        0    42033 2024-04-24 19:31:59.581160 reflex-0.5.0a3/reflex/components/el/elements/other.pyi
--rw-r--r--   0        0        0     1406 2024-02-17 20:02:02.421306 reflex-0.5.0a3/reflex/components/el/elements/scripts.py
--rw-r--r--   0        0        0    19615 2024-04-24 19:31:22.715670 reflex-0.5.0a3/reflex/components/el/elements/scripts.pyi
--rw-r--r--   0        0        0     1535 2024-02-17 20:02:02.421507 reflex-0.5.0a3/reflex/components/el/elements/sectioning.py
--rw-r--r--   0        0        0    87242 2024-04-24 19:32:04.046011 reflex-0.5.0a3/reflex/components/el/elements/sectioning.pyi
--rw-r--r--   0        0        0     2767 2024-02-17 20:02:02.421759 reflex-0.5.0a3/reflex/components/el/elements/tables.py
--rw-r--r--   0        0        0    61849 2024-04-24 19:32:03.007985 reflex-0.5.0a3/reflex/components/el/elements/tables.pyi
--rw-r--r--   0        0        0     2432 2024-02-17 20:02:02.421997 reflex-0.5.0a3/reflex/components/el/elements/typography.py
--rw-r--r--   0        0        0    89115 2024-04-24 19:32:04.312119 reflex-0.5.0a3/reflex/components/el/elements/typography.pyi
--rw-r--r--   0        0        0       88 2024-02-06 00:51:31.999860 reflex-0.5.0a3/reflex/components/gridjs/__init__.py
--rw-r--r--   0        0        0     4300 2024-02-06 00:51:32.000048 reflex-0.5.0a3/reflex/components/gridjs/datatable.py
--rw-r--r--   0        0        0     7053 2024-04-24 19:31:36.593992 reflex-0.5.0a3/reflex/components/gridjs/datatable.pyi
--rw-r--r--   0        0        0      501 2024-02-06 00:51:32.000350 reflex-0.5.0a3/reflex/components/literals.py
--rw-r--r--   0        0        0       73 2024-02-07 21:48:43.293647 reflex-0.5.0a3/reflex/components/lucide/__init__.py
--rw-r--r--   0        0        0    34077 2024-05-09 00:05:27.336308 reflex-0.5.0a3/reflex/components/lucide/icon.py
--rw-r--r--   0        0        0    37918 2024-05-05 01:15:24.056110 reflex-0.5.0a3/reflex/components/lucide/icon.pyi
--rw-r--r--   0        0        0       87 2024-02-06 00:51:32.000748 reflex-0.5.0a3/reflex/components/markdown/__init__.py
--rw-r--r--   0        0        0    10867 2024-05-09 00:05:27.336466 reflex-0.5.0a3/reflex/components/markdown/markdown.py
--rw-r--r--   0        0        0     5100 2024-05-09 00:05:27.336616 reflex-0.5.0a3/reflex/components/markdown/markdown.pyi
--rw-r--r--   0        0        0       44 2024-02-06 00:51:32.001397 reflex-0.5.0a3/reflex/components/media/__init__.py
--rw-r--r--   0        0        0      102 2024-02-06 00:51:32.001492 reflex-0.5.0a3/reflex/components/media/icon.py
--rw-r--r--   0        0        0       79 2024-02-06 00:51:32.001557 reflex-0.5.0a3/reflex/components/moment/__init__.py
--rw-r--r--   0        0        0     3925 2024-02-06 00:51:32.001623 reflex-0.5.0a3/reflex/components/moment/moment.py
--rw-r--r--   0        0        0     6870 2024-04-24 19:31:51.190910 reflex-0.5.0a3/reflex/components/moment/moment.pyi
--rw-r--r--   0        0        0      239 2024-02-06 00:51:32.001924 reflex-0.5.0a3/reflex/components/next/__init__.py
--rw-r--r--   0        0        0      189 2024-01-08 22:19:50.677879 reflex-0.5.0a3/reflex/components/next/base.py
--rw-r--r--   0        0        0     3233 2024-04-24 19:31:43.822514 reflex-0.5.0a3/reflex/components/next/base.pyi
--rw-r--r--   0        0        0     3831 2024-01-08 22:19:50.678013 reflex-0.5.0a3/reflex/components/next/image.py
--rw-r--r--   0        0        0     5795 2024-04-24 19:31:33.244479 reflex-0.5.0a3/reflex/components/next/image.pyi
--rw-r--r--   0        0        0      503 2024-02-06 00:51:32.002304 reflex-0.5.0a3/reflex/components/next/link.py
--rw-r--r--   0        0        0     3461 2024-04-24 19:31:15.603661 reflex-0.5.0a3/reflex/components/next/link.pyi
--rw-r--r--   0        0        0      730 2024-01-08 22:19:50.678316 reflex-0.5.0a3/reflex/components/next/video.py
--rw-r--r--   0        0        0     3429 2024-04-24 19:31:46.249185 reflex-0.5.0a3/reflex/components/next/video.pyi
--rw-r--r--   0        0        0       77 2024-02-06 00:51:32.002529 reflex-0.5.0a3/reflex/components/plotly/__init__.py
--rw-r--r--   0        0        0      964 2024-03-20 23:54:55.846069 reflex-0.5.0a3/reflex/components/plotly/plotly.py
--rw-r--r--   0        0        0     6865 2024-04-24 19:31:24.224015 reflex-0.5.0a3/reflex/components/plotly/plotly.pyi
--rw-r--r--   0        0        0      112 2024-02-17 20:02:02.423429 reflex-0.5.0a3/reflex/components/radix/__init__.py
--rw-r--r--   0        0        0      214 2024-02-17 20:02:02.423526 reflex-0.5.0a3/reflex/components/radix/primitives/__init__.py
--rw-r--r--   0        0        0    16159 2024-05-13 23:05:40.957488 reflex-0.5.0a3/reflex/components/radix/primitives/accordion.py
--rw-r--r--   0        0        0    37999 2024-05-11 03:29:42.708959 reflex-0.5.0a3/reflex/components/radix/primitives/accordion.pyi
--rw-r--r--   0        0        0      869 2024-02-06 00:51:32.004050 reflex-0.5.0a3/reflex/components/radix/primitives/base.py
--rw-r--r--   0        0        0     6478 2024-04-24 19:31:44.069976 reflex-0.5.0a3/reflex/components/radix/primitives/base.pyi
--rw-r--r--   0        0        0     8660 2024-03-20 23:54:55.846917 reflex-0.5.0a3/reflex/components/radix/primitives/drawer.py
--rw-r--r--   0        0        0    34484 2024-04-24 19:32:02.551316 reflex-0.5.0a3/reflex/components/radix/primitives/drawer.pyi
--rw-r--r--   0        0        0     4964 2024-05-11 03:29:42.709212 reflex-0.5.0a3/reflex/components/radix/primitives/form.py
--rw-r--r--   0        0        0    48138 2024-05-07 15:33:05.684481 reflex-0.5.0a3/reflex/components/radix/primitives/form.pyi
--rw-r--r--   0        0        0     4160 2024-05-07 15:33:05.684814 reflex-0.5.0a3/reflex/components/radix/primitives/progress.py
--rw-r--r--   0        0        0    22874 2024-05-07 15:33:05.685122 reflex-0.5.0a3/reflex/components/radix/primitives/progress.pyi
--rw-r--r--   0        0        0     5198 2024-05-07 15:33:05.685275 reflex-0.5.0a3/reflex/components/radix/primitives/slider.py
--rw-r--r--   0        0        0    16877 2024-05-07 15:33:05.685394 reflex-0.5.0a3/reflex/components/radix/primitives/slider.pyi
--rw-r--r--   0        0        0      292 2024-02-17 20:02:02.426799 reflex-0.5.0a3/reflex/components/radix/themes/__init__.py
--rw-r--r--   0        0        0     8294 2024-04-26 18:47:21.875701 reflex-0.5.0a3/reflex/components/radix/themes/base.py
--rw-r--r--   0        0        0    26971 2024-05-05 01:15:24.056523 reflex-0.5.0a3/reflex/components/radix/themes/base.pyi
--rw-r--r--   0        0        0     5543 2024-05-13 23:05:41.231938 reflex-0.5.0a3/reflex/components/radix/themes/color_mode.py
--rw-r--r--   0        0        0    22145 2024-05-13 23:05:41.232088 reflex-0.5.0a3/reflex/components/radix/themes/color_mode.pyi
--rw-r--r--   0        0        0     2440 2024-05-09 00:05:27.336999 reflex-0.5.0a3/reflex/components/radix/themes/components/__init__.py
--rw-r--r--   0        0        0     3267 2024-03-20 23:54:55.849529 reflex-0.5.0a3/reflex/components/radix/themes/components/alert_dialog.py
--rw-r--r--   0        0        0    24434 2024-04-24 19:31:57.706076 reflex-0.5.0a3/reflex/components/radix/themes/components/alert_dialog.pyi
--rw-r--r--   0        0        0      400 2024-02-17 20:02:02.428862 reflex-0.5.0a3/reflex/components/radix/themes/components/aspect_ratio.py
--rw-r--r--   0        0        0     3640 2024-04-24 19:31:17.911074 reflex-0.5.0a3/reflex/components/radix/themes/components/aspect_ratio.pyi
--rw-r--r--   0        0        0      989 2024-03-20 23:54:55.849841 reflex-0.5.0a3/reflex/components/radix/themes/components/avatar.py
--rw-r--r--   0        0        0     6562 2024-04-24 19:31:52.410239 reflex-0.5.0a3/reflex/components/radix/themes/components/avatar.pyi
--rw-r--r--   0        0        0      821 2024-04-26 18:47:21.876311 reflex-0.5.0a3/reflex/components/radix/themes/components/badge.py
--rw-r--r--   0        0        0     9347 2024-04-26 18:47:21.876509 reflex-0.5.0a3/reflex/components/radix/themes/components/badge.pyi
--rw-r--r--   0        0        0     1125 2024-04-26 18:47:21.876620 reflex-0.5.0a3/reflex/components/radix/themes/components/button.py
--rw-r--r--   0        0        0    11939 2024-04-26 18:47:21.876761 reflex-0.5.0a3/reflex/components/radix/themes/components/button.pyi
--rw-r--r--   0        0        0     2378 2024-03-20 23:54:55.850376 reflex-0.5.0a3/reflex/components/radix/themes/components/callout.py
--rw-r--r--   0        0        0    38710 2024-04-24 19:32:02.594947 reflex-0.5.0a3/reflex/components/radix/themes/components/callout.pyi
--rw-r--r--   0        0        0      659 2024-02-17 20:02:02.430724 reflex-0.5.0a3/reflex/components/radix/themes/components/card.py
--rw-r--r--   0        0        0     7200 2024-04-24 19:31:48.002992 reflex-0.5.0a3/reflex/components/radix/themes/components/card.pyi
--rw-r--r--   0        0        0     4679 2024-03-20 23:54:55.851297 reflex-0.5.0a3/reflex/components/radix/themes/components/checkbox.py
--rw-r--r--   0        0        0    20877 2024-04-24 19:32:01.819836 reflex-0.5.0a3/reflex/components/radix/themes/components/checkbox.pyi
--rw-r--r--   0        0        0     1301 2024-04-26 18:47:21.876837 reflex-0.5.0a3/reflex/components/radix/themes/components/checkbox_cards.py
--rw-r--r--   0        0        0     9591 2024-04-26 18:47:21.876955 reflex-0.5.0a3/reflex/components/radix/themes/components/checkbox_cards.pyi
--rw-r--r--   0        0        0     1024 2024-04-26 18:47:21.877018 reflex-0.5.0a3/reflex/components/radix/themes/components/checkbox_group.py
--rw-r--r--   0        0        0     9012 2024-04-26 18:47:21.877125 reflex-0.5.0a3/reflex/components/radix/themes/components/checkbox_group.pyi
--rw-r--r--   0        0        0     5049 2024-03-20 23:54:55.852012 reflex-0.5.0a3/reflex/components/radix/themes/components/context_menu.py
--rw-r--r--   0        0        0    31192 2024-04-24 19:32:03.158519 reflex-0.5.0a3/reflex/components/radix/themes/components/context_menu.pyi
--rw-r--r--   0        0        0     1508 2024-04-26 18:47:21.877372 reflex-0.5.0a3/reflex/components/radix/themes/components/data_list.py
--rw-r--r--   0        0        0    15403 2024-04-26 18:47:21.877634 reflex-0.5.0a3/reflex/components/radix/themes/components/data_list.pyi
--rw-r--r--   0        0        0     2600 2024-03-20 23:54:55.852519 reflex-0.5.0a3/reflex/components/radix/themes/components/dialog.py
--rw-r--r--   0        0        0    24895 2024-04-24 19:32:02.097223 reflex-0.5.0a3/reflex/components/radix/themes/components/dialog.pyi
--rw-r--r--   0        0        0    11256 2024-03-20 23:54:55.852973 reflex-0.5.0a3/reflex/components/radix/themes/components/dropdown_menu.py
--rw-r--r--   0        0        0    37901 2024-04-24 19:32:02.303816 reflex-0.5.0a3/reflex/components/radix/themes/components/dropdown_menu.pyi
--rw-r--r--   0        0        0     2405 2024-03-20 23:54:55.853285 reflex-0.5.0a3/reflex/components/radix/themes/components/hover_card.py
--rw-r--r--   0        0        0    17744 2024-04-24 19:31:56.396802 reflex-0.5.0a3/reflex/components/radix/themes/components/hover_card.pyi
--rw-r--r--   0        0        0     2940 2024-05-09 00:05:27.337231 reflex-0.5.0a3/reflex/components/radix/themes/components/icon_button.py
--rw-r--r--   0        0        0    12126 2024-05-07 15:33:05.685671 reflex-0.5.0a3/reflex/components/radix/themes/components/icon_button.pyi
--rw-r--r--   0        0        0     1015 2024-03-20 23:54:55.853906 reflex-0.5.0a3/reflex/components/radix/themes/components/inset.py
--rw-r--r--   0        0        0     7889 2024-04-24 19:31:39.003439 reflex-0.5.0a3/reflex/components/radix/themes/components/inset.pyi
--rw-r--r--   0        0        0     3177 2024-03-20 23:54:55.854041 reflex-0.5.0a3/reflex/components/radix/themes/components/popover.py
--rw-r--r--   0        0        0    17404 2024-04-24 19:32:01.605821 reflex-0.5.0a3/reflex/components/radix/themes/components/popover.pyi
--rw-r--r--   0        0        0     1598 2024-05-09 00:05:27.337432 reflex-0.5.0a3/reflex/components/radix/themes/components/progress.py
--rw-r--r--   0        0        0     6676 2024-05-09 00:05:27.337586 reflex-0.5.0a3/reflex/components/radix/themes/components/progress.pyi
--rw-r--r--   0        0        0      762 2024-04-26 18:47:21.878308 reflex-0.5.0a3/reflex/components/radix/themes/components/radio.py
--rw-r--r--   0        0        0     5924 2024-04-26 18:47:21.878424 reflex-0.5.0a3/reflex/components/radix/themes/components/radio.pyi
--rw-r--r--   0        0        0     1250 2024-04-26 18:47:21.878499 reflex-0.5.0a3/reflex/components/radix/themes/components/radio_cards.py
--rw-r--r--   0        0        0     9561 2024-04-26 18:47:21.878615 reflex-0.5.0a3/reflex/components/radix/themes/components/radio_cards.pyi
--rw-r--r--   0        0        0     6233 2024-04-24 21:16:40.838796 reflex-0.5.0a3/reflex/components/radix/themes/components/radio_group.py
--rw-r--r--   0        0        0    24106 2024-04-24 19:32:02.212695 reflex-0.5.0a3/reflex/components/radix/themes/components/radio_group.pyi
--rw-r--r--   0        0        0      920 2024-03-20 23:54:55.855386 reflex-0.5.0a3/reflex/components/radix/themes/components/scroll_area.py
--rw-r--r--   0        0        0     4427 2024-04-24 19:31:54.699499 reflex-0.5.0a3/reflex/components/radix/themes/components/scroll_area.pyi
--rw-r--r--   0        0        0     1292 2024-04-26 18:47:21.878708 reflex-0.5.0a3/reflex/components/radix/themes/components/segmented_control.py
--rw-r--r--   0        0        0     9507 2024-04-26 18:47:21.878829 reflex-0.5.0a3/reflex/components/radix/themes/components/segmented_control.pyi
--rw-r--r--   0        0        0     8028 2024-04-05 17:14:14.462095 reflex-0.5.0a3/reflex/components/radix/themes/components/select.py
--rw-r--r--   0        0        0    45123 2024-04-24 19:32:01.973018 reflex-0.5.0a3/reflex/components/radix/themes/components/select.pyi
--rw-r--r--   0        0        0      868 2024-03-20 23:54:55.856979 reflex-0.5.0a3/reflex/components/radix/themes/components/separator.py
--rw-r--r--   0        0        0     6078 2024-04-24 19:32:00.501335 reflex-0.5.0a3/reflex/components/radix/themes/components/separator.pyi
--rw-r--r--   0        0        0      643 2024-04-26 18:47:21.878906 reflex-0.5.0a3/reflex/components/radix/themes/components/skeleton.py
--rw-r--r--   0        0        0     4289 2024-04-26 18:47:21.879004 reflex-0.5.0a3/reflex/components/radix/themes/components/skeleton.pyi
--rw-r--r--   0        0        0     3234 2024-03-20 23:54:55.857144 reflex-0.5.0a3/reflex/components/radix/themes/components/slider.py
--rw-r--r--   0        0        0     8162 2024-04-24 19:31:52.441948 reflex-0.5.0a3/reflex/components/radix/themes/components/slider.pyi
--rw-r--r--   0        0        0      431 2024-04-26 18:47:21.879090 reflex-0.5.0a3/reflex/components/radix/themes/components/spinner.py
--rw-r--r--   0        0        0     3845 2024-04-26 18:47:21.879165 reflex-0.5.0a3/reflex/components/radix/themes/components/spinner.pyi
--rw-r--r--   0        0        0     1976 2024-02-17 20:02:02.440152 reflex-0.5.0a3/reflex/components/radix/themes/components/switch.py
--rw-r--r--   0        0        0     7404 2024-04-24 19:31:46.185370 reflex-0.5.0a3/reflex/components/radix/themes/components/switch.pyi
--rw-r--r--   0        0        0     3111 2024-03-20 23:54:55.857388 reflex-0.5.0a3/reflex/components/radix/themes/components/table.py
--rw-r--r--   0        0        0    47387 2024-04-24 19:32:03.411460 reflex-0.5.0a3/reflex/components/radix/themes/components/table.pyi
--rw-r--r--   0        0        0     2986 2024-05-07 15:33:05.685861 reflex-0.5.0a3/reflex/components/radix/themes/components/tabs.py
--rw-r--r--   0        0        0    19119 2024-05-07 15:33:05.685968 reflex-0.5.0a3/reflex/components/radix/themes/components/tabs.pyi
--rw-r--r--   0        0        0     3233 2024-02-17 20:02:02.441460 reflex-0.5.0a3/reflex/components/radix/themes/components/text_area.py
--rw-r--r--   0        0        0    11711 2024-04-24 19:31:45.665204 reflex-0.5.0a3/reflex/components/radix/themes/components/text_area.pyi
--rw-r--r--   0        0        0     6527 2024-05-09 00:05:27.337867 reflex-0.5.0a3/reflex/components/radix/themes/components/text_field.py
--rw-r--r--   0        0        0    26637 2024-05-09 00:05:27.338008 reflex-0.5.0a3/reflex/components/radix/themes/components/text_field.pyi
--rw-r--r--   0        0        0     4465 2024-02-17 20:02:02.442324 reflex-0.5.0a3/reflex/components/radix/themes/components/tooltip.py
--rw-r--r--   0        0        0     8092 2024-04-24 19:31:32.491941 reflex-0.5.0a3/reflex/components/radix/themes/components/tooltip.pyi
--rw-r--r--   0        0        0      811 2024-04-04 14:19:59.340548 reflex-0.5.0a3/reflex/components/radix/themes/layout/__init__.py
--rw-r--r--   0        0        0     1211 2024-04-26 18:47:21.880131 reflex-0.5.0a3/reflex/components/radix/themes/layout/base.py
--rw-r--r--   0        0        0     7663 2024-04-26 18:47:21.880279 reflex-0.5.0a3/reflex/components/radix/themes/layout/base.pyi
--rw-r--r--   0        0        0      281 2024-02-07 21:48:43.318485 reflex-0.5.0a3/reflex/components/radix/themes/layout/box.py
--rw-r--r--   0        0        0     6462 2024-04-24 19:31:52.197501 reflex-0.5.0a3/reflex/components/radix/themes/layout/box.pyi
--rw-r--r--   0        0        0      509 2024-05-07 15:33:05.686074 reflex-0.5.0a3/reflex/components/radix/themes/layout/center.py
--rw-r--r--   0        0        0     8271 2024-05-07 15:33:05.686180 reflex-0.5.0a3/reflex/components/radix/themes/layout/center.pyi
--rw-r--r--   0        0        0     1405 2024-05-05 01:15:24.057627 reflex-0.5.0a3/reflex/components/radix/themes/layout/container.py
--rw-r--r--   0        0        0     5247 2024-05-05 01:15:24.057873 reflex-0.5.0a3/reflex/components/radix/themes/layout/container.pyi
--rw-r--r--   0        0        0     1374 2024-03-20 23:54:55.859776 reflex-0.5.0a3/reflex/components/radix/themes/layout/flex.py
--rw-r--r--   0        0        0     8501 2024-04-24 19:31:47.609497 reflex-0.5.0a3/reflex/components/radix/themes/layout/flex.pyi
--rw-r--r--   0        0        0     1498 2024-03-20 23:54:55.860131 reflex-0.5.0a3/reflex/components/radix/themes/layout/grid.py
--rw-r--r--   0        0        0     8907 2024-04-24 19:31:44.336304 reflex-0.5.0a3/reflex/components/radix/themes/layout/grid.pyi
--rw-r--r--   0        0        0     4991 2024-05-07 15:33:05.686298 reflex-0.5.0a3/reflex/components/radix/themes/layout/list.py
--rw-r--r--   0        0        0    28927 2024-05-07 15:33:05.686398 reflex-0.5.0a3/reflex/components/radix/themes/layout/list.pyi
--rw-r--r--   0        0        0      458 2024-02-07 21:48:43.320250 reflex-0.5.0a3/reflex/components/radix/themes/layout/section.py
--rw-r--r--   0        0        0     6758 2024-04-24 19:31:48.032806 reflex-0.5.0a3/reflex/components/radix/themes/layout/section.pyi
--rw-r--r--   0        0        0      492 2024-05-07 15:33:05.686501 reflex-0.5.0a3/reflex/components/radix/themes/layout/spacer.py
--rw-r--r--   0        0        0     8271 2024-05-07 15:33:05.686608 reflex-0.5.0a3/reflex/components/radix/themes/layout/spacer.pyi
--rw-r--r--   0        0        0     1522 2024-05-05 01:15:24.058360 reflex-0.5.0a3/reflex/components/radix/themes/layout/stack.py
--rw-r--r--   0        0        0    22132 2024-05-05 01:15:24.058618 reflex-0.5.0a3/reflex/components/radix/themes/layout/stack.pyi
--rw-r--r--   0        0        0      343 2024-02-17 20:02:02.446123 reflex-0.5.0a3/reflex/components/radix/themes/typography/__init__.py
--rw-r--r--   0        0        0      408 2024-01-08 22:19:50.686081 reflex-0.5.0a3/reflex/components/radix/themes/typography/base.py
--rw-r--r--   0        0        0      799 2024-02-07 21:48:43.321231 reflex-0.5.0a3/reflex/components/radix/themes/typography/blockquote.py
--rw-r--r--   0        0        0     9316 2024-04-24 19:31:18.815043 reflex-0.5.0a3/reflex/components/radix/themes/typography/blockquote.pyi
--rw-r--r--   0        0        0      909 2024-02-07 21:48:43.321463 reflex-0.5.0a3/reflex/components/radix/themes/typography/code.py
--rw-r--r--   0        0        0     9513 2024-04-24 19:31:42.716182 reflex-0.5.0a3/reflex/components/radix/themes/typography/code.pyi
--rw-r--r--   0        0        0     1324 2024-02-07 21:48:43.322172 reflex-0.5.0a3/reflex/components/radix/themes/typography/heading.py
--rw-r--r--   0        0        0    10106 2024-04-24 19:31:48.004994 reflex-0.5.0a3/reflex/components/radix/themes/typography/heading.pyi
--rw-r--r--   0        0        0     3291 2024-05-05 01:15:24.058911 reflex-0.5.0a3/reflex/components/radix/themes/typography/link.py
--rw-r--r--   0        0        0    12144 2024-05-05 01:15:24.059174 reflex-0.5.0a3/reflex/components/radix/themes/typography/link.pyi
--rw-r--r--   0        0        0     2604 2024-03-20 23:54:55.863112 reflex-0.5.0a3/reflex/components/radix/themes/typography/text.py
--rw-r--r--   0        0        0    57238 2024-04-24 19:32:03.568126 reflex-0.5.0a3/reflex/components/radix/themes/typography/text.pyi
--rw-r--r--   0        0        0      144 2024-02-06 00:51:32.026767 reflex-0.5.0a3/reflex/components/react_player/__init__.py
--rw-r--r--   0        0        0      185 2024-02-06 00:51:32.026827 reflex-0.5.0a3/reflex/components/react_player/audio.py
--rw-r--r--   0        0        0     4327 2024-04-24 19:31:20.559612 reflex-0.5.0a3/reflex/components/react_player/audio.pyi
--rw-r--r--   0        0        0     1087 2024-02-06 00:51:32.027069 reflex-0.5.0a3/reflex/components/react_player/react_player.py
--rw-r--r--   0        0        0     4354 2024-04-24 19:31:40.833679 reflex-0.5.0a3/reflex/components/react_player/react_player.pyi
--rw-r--r--   0        0        0      185 2024-02-06 00:51:32.027295 reflex-0.5.0a3/reflex/components/react_player/video.py
--rw-r--r--   0        0        0     4327 2024-04-24 19:31:23.657166 reflex-0.5.0a3/reflex/components/react_player/video.pyi
--rw-r--r--   0        0        0     2373 2024-02-06 00:51:32.027723 reflex-0.5.0a3/reflex/components/recharts/__init__.py
--rw-r--r--   0        0        0    19595 2024-02-06 00:51:32.027828 reflex-0.5.0a3/reflex/components/recharts/cartesian.py
--rw-r--r--   0        0        0    84151 2024-04-24 19:32:04.125732 reflex-0.5.0a3/reflex/components/recharts/cartesian.pyi
--rw-r--r--   0        0        0    18493 2024-02-06 00:51:32.028086 reflex-0.5.0a3/reflex/components/recharts/charts.py
--rw-r--r--   0        0        0    48757 2024-04-24 19:32:04.230664 reflex-0.5.0a3/reflex/components/recharts/charts.pyi
--rw-r--r--   0        0        0     5624 2024-04-25 02:07:40.442483 reflex-0.5.0a3/reflex/components/recharts/general.py
--rw-r--r--   0        0        0    22787 2024-04-24 19:31:57.383382 reflex-0.5.0a3/reflex/components/recharts/general.pyi
--rw-r--r--   0        0        0    10410 2024-02-06 00:51:32.028623 reflex-0.5.0a3/reflex/components/recharts/polar.py
--rw-r--r--   0        0        0    24326 2024-04-24 19:32:02.075893 reflex-0.5.0a3/reflex/components/recharts/polar.pyi
--rw-r--r--   0        0        0     2870 2024-02-06 00:51:32.028787 reflex-0.5.0a3/reflex/components/recharts/recharts.py
--rw-r--r--   0        0        0     8535 2024-04-24 19:31:59.348537 reflex-0.5.0a3/reflex/components/recharts/recharts.pyi
--rw-r--r--   0        0        0       68 2024-05-05 01:15:24.059268 reflex-0.5.0a3/reflex/components/sonner/__init__.py
--rw-r--r--   0        0        0     7638 2024-05-05 01:15:24.059336 reflex-0.5.0a3/reflex/components/sonner/toast.py
--rw-r--r--   0        0        0     7635 2024-05-05 01:15:24.059415 reflex-0.5.0a3/reflex/components/sonner/toast.pyi
--rw-r--r--   0        0        0      109 2024-02-06 00:51:32.028942 reflex-0.5.0a3/reflex/components/suneditor/__init__.py
--rw-r--r--   0        0        0     7360 2024-02-06 00:51:32.029131 reflex-0.5.0a3/reflex/components/suneditor/editor.py
--rw-r--r--   0        0        0    10330 2024-04-24 19:32:02.124688 reflex-0.5.0a3/reflex/components/suneditor/editor.pyi
--rw-r--r--   0        0        0      152 2024-02-06 00:51:32.029339 reflex-0.5.0a3/reflex/components/tags/__init__.py
--rw-r--r--   0        0        0      447 2023-07-20 22:42:41.717618 reflex-0.5.0a3/reflex/components/tags/cond_tag.py
--rw-r--r--   0        0        0     3927 2024-05-09 06:53:37.971823 reflex-0.5.0a3/reflex/components/tags/iter_tag.py
--rw-r--r--   0        0        0      387 2024-02-06 00:51:32.029522 reflex-0.5.0a3/reflex/components/tags/match_tag.py
--rw-r--r--   0        0        0     2778 2024-03-20 23:54:55.863973 reflex-0.5.0a3/reflex/components/tags/tag.py
--rw-r--r--   0        0        0      587 2023-07-20 22:42:41.717805 reflex-0.5.0a3/reflex/components/tags/tagless.py
--rw-r--r--   0        0        0    10673 2024-05-09 00:05:27.338296 reflex-0.5.0a3/reflex/config.py
--rw-r--r--   0        0        0     3318 2024-04-05 17:14:06.329003 reflex-0.5.0a3/reflex/config.pyi
--rw-r--r--   0        0        0     2036 2024-05-07 15:33:05.687073 reflex-0.5.0a3/reflex/constants/__init__.py
--rw-r--r--   0        0        0     5640 2024-05-07 15:33:05.687194 reflex-0.5.0a3/reflex/constants/base.py
--rw-r--r--   0        0        0     2980 2024-04-24 19:34:30.973419 reflex-0.5.0a3/reflex/constants/base.pyi
--rw-r--r--   0        0        0     1625 2024-05-07 15:33:05.687387 reflex-0.5.0a3/reflex/constants/colors.py
--rw-r--r--   0        0        0     4207 2024-04-12 01:14:12.277724 reflex-0.5.0a3/reflex/constants/compiler.py
--rw-r--r--   0        0        0     1331 2024-01-08 22:19:50.692361 reflex-0.5.0a3/reflex/constants/config.py
--rw-r--r--   0        0        0     1268 2024-03-20 23:54:55.865280 reflex-0.5.0a3/reflex/constants/custom_components.py
--rw-r--r--   0        0        0     2668 2024-03-20 00:01:07.211135 reflex-0.5.0a3/reflex/constants/event.py
--rw-r--r--   0        0        0     3419 2024-05-05 01:15:24.059627 reflex-0.5.0a3/reflex/constants/installer.py
--rw-r--r--   0        0        0     2144 2024-05-05 01:15:24.059871 reflex-0.5.0a3/reflex/constants/route.py
--rw-r--r--   0        0        0      636 2024-02-06 00:51:32.030238 reflex-0.5.0a3/reflex/constants/style.py
--rw-r--r--   0        0        0       36 2024-03-20 23:54:55.865552 reflex-0.5.0a3/reflex/custom_components/__init__.py
--rw-r--r--   0        0        0    32298 2024-05-13 23:05:41.048157 reflex-0.5.0a3/reflex/custom_components/custom_components.py
--rw-r--r--   0        0        0    27893 2024-05-05 01:15:24.060128 reflex-0.5.0a3/reflex/event.py
--rw-r--r--   0        0        0      608 2024-05-09 00:05:27.338786 reflex-0.5.0a3/reflex/experimental/__init__.py
--rw-r--r--   0        0        0     2196 2024-04-24 21:16:40.840090 reflex-0.5.0a3/reflex/experimental/hooks.py
--rw-r--r--   0        0        0     7234 2024-05-07 15:33:05.687514 reflex-0.5.0a3/reflex/experimental/layout.py
--rw-r--r--   0        0        0      281 2024-04-12 01:14:12.278217 reflex-0.5.0a3/reflex/experimental/misc.py
--rw-r--r--   0        0        0      111 2023-07-20 22:42:41.719277 reflex-0.5.0a3/reflex/middleware/__init__.py
--rw-r--r--   0        0        0     1484 2024-03-28 17:56:29.082526 reflex-0.5.0a3/reflex/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1169 2023-12-01 04:51:31.116521 reflex-0.5.0a3/reflex/middleware/middleware.py
--rw-r--r--   0        0        0    13227 2024-05-09 00:05:27.338971 reflex-0.5.0a3/reflex/model.py
--rw-r--r--   0        0        0     2077 2024-04-24 21:16:40.840737 reflex-0.5.0a3/reflex/page.py
--rw-r--r--   0        0        0    17826 2024-05-05 01:15:24.060260 reflex-0.5.0a3/reflex/reflex.py
--rw-r--r--   0        0        0     4198 2024-05-05 01:15:24.060365 reflex-0.5.0a3/reflex/route.py
--rw-r--r--   0        0        0   105748 2024-05-09 00:05:27.339322 reflex-0.5.0a3/reflex/state.py
--rw-r--r--   0        0        0     9405 2024-05-11 03:29:42.709528 reflex-0.5.0a3/reflex/style.py
--rw-r--r--   0        0        0    30743 2024-05-07 15:33:05.688166 reflex-0.5.0a3/reflex/testing.py
--rw-r--r--   0        0        0       24 2023-11-09 03:24:59.510665 reflex-0.5.0a3/reflex/utils/__init__.py
--rw-r--r--   0        0        0     8573 2024-02-06 00:51:32.031946 reflex-0.5.0a3/reflex/utils/build.py
--rw-r--r--   0        0        0     1255 2024-04-12 01:14:12.279414 reflex-0.5.0a3/reflex/utils/compat.py
--rw-r--r--   0        0        0     5182 2024-04-24 21:16:40.841356 reflex-0.5.0a3/reflex/utils/console.py
--rw-r--r--   0        0        0      504 2024-02-06 00:51:32.032065 reflex-0.5.0a3/reflex/utils/exceptions.py
--rw-r--r--   0        0        0    10406 2024-05-07 15:33:05.688300 reflex-0.5.0a3/reflex/utils/exec.py
--rw-r--r--   0        0        0     2270 2024-04-12 01:14:12.279905 reflex-0.5.0a3/reflex/utils/export.py
--rw-r--r--   0        0        0    22652 2024-04-24 21:16:40.841498 reflex-0.5.0a3/reflex/utils/format.py
--rw-r--r--   0        0        0     2309 2024-04-24 21:16:40.841612 reflex-0.5.0a3/reflex/utils/imports.py
--rw-r--r--   0        0        0     4737 2024-02-06 00:51:32.033457 reflex-0.5.0a3/reflex/utils/path_ops.py
--rw-r--r--   0        0        0    51212 2024-05-09 00:05:27.339607 reflex-0.5.0a3/reflex/utils/prerequisites.py
--rw-r--r--   0        0        0    11242 2024-05-07 15:33:05.688585 reflex-0.5.0a3/reflex/utils/processes.py
--rw-r--r--   0        0        0    30637 2024-05-05 01:15:24.061383 reflex-0.5.0a3/reflex/utils/pyi_generator.py
--rw-r--r--   0        0        0     9037 2024-04-24 21:16:40.842319 reflex-0.5.0a3/reflex/utils/serializers.py
--rw-r--r--   0        0        0     4688 2024-05-07 15:33:05.688896 reflex-0.5.0a3/reflex/utils/telemetry.py
--rw-r--r--   0        0        0    14842 2024-05-09 00:05:27.339984 reflex-0.5.0a3/reflex/utils/types.py
--rw-r--r--   0        0        0     2609 2023-10-22 18:57:13.223189 reflex-0.5.0a3/reflex/utils/watch.py
--rw-r--r--   0        0        0    67317 2024-04-25 16:52:48.845338 reflex-0.5.0a3/reflex/vars.py
--rw-r--r--   0        0        0     5583 2024-04-04 14:57:26.401034 reflex-0.5.0a3/reflex/vars.pyi
--rw-r--r--   0        0        0    12089 1970-01-01 00:00:00.000000 reflex-0.5.0a3/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-20 22:42:41.698164 reflex-0.5.1a1/LICENSE
+-rw-r--r--   0        0        0     9842 2024-05-07 15:33:05.680965 reflex-0.5.1a1/README.md
+-rw-r--r--   0        0        0     2974 2024-05-17 15:40:18.668308 reflex-0.5.1a1/pyproject.toml
+-rw-r--r--   0        0        0     4286 2023-11-09 03:24:59.498329 reflex-0.5.1a1/reflex/.templates/apps/blank/assets/favicon.ico
+-rw-r--r--   0        0        0        0 2023-11-09 03:24:59.498383 reflex-0.5.1a1/reflex/.templates/apps/blank/code/__init__.py
+-rw-r--r--   0        0        0      926 2024-05-09 00:05:27.334397 reflex-0.5.1a1/reflex/.templates/apps/blank/code/blank.py
+-rw-r--r--   0        0        0       32 2023-11-09 03:24:59.498951 reflex-0.5.1a1/reflex/.templates/apps/demo/.gitignore
+-rw-r--r--   0        0        0     4286 2023-11-09 03:24:59.499075 reflex-0.5.1a1/reflex/.templates/apps/demo/assets/favicon.ico
+-rw-r--r--   0        0        0     1475 2023-11-09 03:24:59.499137 reflex-0.5.1a1/reflex/.templates/apps/demo/assets/github.svg
+-rw-r--r--   0        0        0     1899 2023-11-09 03:24:59.499199 reflex-0.5.1a1/reflex/.templates/apps/demo/assets/icon.svg
+-rw-r--r--   0        0        0     5403 2023-11-09 03:24:59.499298 reflex-0.5.1a1/reflex/.templates/apps/demo/assets/logo.svg
+-rw-r--r--   0        0        0      807 2023-11-09 03:24:59.499362 reflex-0.5.1a1/reflex/.templates/apps/demo/assets/paneleft.svg
+-rw-r--r--   0        0        0       32 2023-11-09 03:24:59.499458 reflex-0.5.1a1/reflex/.templates/apps/demo/code/__init__.py
+-rw-r--r--   0        0        0     2927 2024-05-17 15:27:52.896857 reflex-0.5.1a1/reflex/.templates/apps/demo/code/demo.py
+-rw-r--r--   0        0        0      194 2023-11-09 03:24:59.499716 reflex-0.5.1a1/reflex/.templates/apps/demo/code/pages/__init__.py
+-rw-r--r--   0        0        0      706 2024-02-17 20:02:02.399560 reflex-0.5.1a1/reflex/.templates/apps/demo/code/pages/chatapp.py
+-rw-r--r--   0        0        0    10906 2024-04-24 21:16:40.835599 reflex-0.5.1a1/reflex/.templates/apps/demo/code/pages/datatable.py
+-rw-r--r--   0        0        0     8381 2024-04-24 21:16:40.835772 reflex-0.5.1a1/reflex/.templates/apps/demo/code/pages/forms.py
+-rw-r--r--   0        0        0     8519 2024-03-20 23:54:55.830529 reflex-0.5.1a1/reflex/.templates/apps/demo/code/pages/graphing.py
+-rw-r--r--   0        0        0     1822 2024-02-17 20:02:02.400769 reflex-0.5.1a1/reflex/.templates/apps/demo/code/pages/home.py
+-rw-r--r--   0        0        0     4722 2024-02-17 20:02:02.400919 reflex-0.5.1a1/reflex/.templates/apps/demo/code/sidebar.py
+-rw-r--r--   0        0        0      510 2023-11-09 03:24:59.500529 reflex-0.5.1a1/reflex/.templates/apps/demo/code/state.py
+-rw-r--r--   0        0        0      912 2023-11-09 03:24:59.500616 reflex-0.5.1a1/reflex/.templates/apps/demo/code/states/form_state.py
+-rw-r--r--   0        0        0     1189 2023-11-09 03:24:59.500682 reflex-0.5.1a1/reflex/.templates/apps/demo/code/states/pie_state.py
+-rw-r--r--   0        0        0     1486 2024-02-17 20:02:02.401042 reflex-0.5.1a1/reflex/.templates/apps/demo/code/styles.py
+-rw-r--r--   0        0        0        0 2023-11-09 03:24:59.500792 reflex-0.5.1a1/reflex/.templates/apps/demo/code/webui/__init__.py
+-rw-r--r--   0        0        0      120 2023-11-09 03:24:59.500879 reflex-0.5.1a1/reflex/.templates/apps/demo/code/webui/components/__init__.py
+-rw-r--r--   0        0        0     3584 2024-02-17 20:02:02.401162 reflex-0.5.1a1/reflex/.templates/apps/demo/code/webui/components/chat.py
+-rw-r--r--   0        0        0      680 2023-11-09 03:24:59.500996 reflex-0.5.1a1/reflex/.templates/apps/demo/code/webui/components/loading_icon.py
+-rw-r--r--   0        0        0     1829 2024-02-17 20:02:02.401269 reflex-0.5.1a1/reflex/.templates/apps/demo/code/webui/components/modal.py
+-rw-r--r--   0        0        0     2251 2024-02-17 20:02:02.401372 reflex-0.5.1a1/reflex/.templates/apps/demo/code/webui/components/navbar.py
+-rw-r--r--   0        0        0     1735 2024-02-17 20:02:02.401457 reflex-0.5.1a1/reflex/.templates/apps/demo/code/webui/components/sidebar.py
+-rw-r--r--   0        0        0     4001 2023-11-09 03:24:59.501230 reflex-0.5.1a1/reflex/.templates/apps/demo/code/webui/state.py
+-rw-r--r--   0        0        0     2281 2024-02-17 20:02:02.401582 reflex-0.5.1a1/reflex/.templates/apps/demo/code/webui/styles.py
+-rw-r--r--   0        0        0       74 2023-10-22 18:57:13.188650 reflex-0.5.1a1/reflex/.templates/jinja/app/rxconfig.py.jinja2
+-rw-r--r--   0        0        0      127 2024-03-20 23:54:55.833038 reflex-0.5.1a1/reflex/.templates/jinja/custom_components/README.md.jinja2
+-rw-r--r--   0        0        0       32 2024-03-20 23:54:55.833129 reflex-0.5.1a1/reflex/.templates/jinja/custom_components/__init__.py.jinja2
+-rw-r--r--   0        0        0      826 2024-03-20 23:54:55.833525 reflex-0.5.1a1/reflex/.templates/jinja/custom_components/demo_app.py.jinja2
+-rw-r--r--   0        0        0      614 2024-04-04 14:57:26.374812 reflex-0.5.1a1/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2
+-rw-r--r--   0        0        0     2403 2024-04-05 17:14:14.457446 reflex-0.5.1a1/reflex/.templates/jinja/custom_components/src.py.jinja2
+-rw-r--r--   0        0        0      548 2023-10-22 18:57:13.188813 reflex-0.5.1a1/reflex/.templates/jinja/web/package.json.jinja2
+-rw-r--r--   0        0        0      930 2024-03-20 23:54:55.834237 reflex-0.5.1a1/reflex/.templates/jinja/web/pages/_app.js.jinja2
+-rw-r--r--   0        0        0      182 2023-07-20 22:42:41.708822 reflex-0.5.1a1/reflex/.templates/jinja/web/pages/_document.js.jinja2
+-rw-r--r--   0        0        0      400 2024-02-06 00:51:31.970380 reflex-0.5.1a1/reflex/.templates/jinja/web/pages/base_page.js.jinja2
+-rw-r--r--   0        0        0       86 2023-10-22 18:57:13.188983 reflex-0.5.1a1/reflex/.templates/jinja/web/pages/component.js.jinja2
+-rw-r--r--   0        0        0      882 2023-12-01 04:51:31.091531 reflex-0.5.1a1/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
+-rw-r--r--   0        0        0      343 2024-04-04 14:57:26.375114 reflex-0.5.1a1/reflex/.templates/jinja/web/pages/index.js.jinja2
+-rw-r--r--   0        0        0      388 2024-04-05 17:14:14.457553 reflex-0.5.1a1/reflex/.templates/jinja/web/pages/stateful_component.js.jinja2
+-rw-r--r--   0        0        0      101 2023-12-01 04:51:31.092250 reflex-0.5.1a1/reflex/.templates/jinja/web/pages/stateful_components.js.jinja2
+-rw-r--r--   0        0        0     3883 2024-02-06 00:51:31.970618 reflex-0.5.1a1/reflex/.templates/jinja/web/pages/utils.js.jinja2
+-rw-r--r--   0        0        0      141 2023-12-06 18:41:46.628030 reflex-0.5.1a1/reflex/.templates/jinja/web/styles/styles.css.jinja2
+-rw-r--r--   0        0        0      761 2024-05-17 15:27:52.897129 reflex-0.5.1a1/reflex/.templates/jinja/web/tailwind.config.js.jinja2
+-rw-r--r--   0        0        0     3790 2024-03-20 23:54:55.834608 reflex-0.5.1a1/reflex/.templates/jinja/web/utils/context.js.jinja2
+-rw-r--r--   0        0        0       37 2023-12-06 19:37:00.189183 reflex-0.5.1a1/reflex/.templates/jinja/web/utils/theme.js.jinja2
+-rw-r--r--   0        0        0      417 2023-07-20 22:42:41.709243 reflex-0.5.1a1/reflex/.templates/web/.gitignore
+-rw-r--r--   0        0        0      595 2023-10-30 01:36:56.133208 reflex-0.5.1a1/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js
+-rw-r--r--   0        0        0      645 2024-03-20 23:54:55.835034 reflex-0.5.1a1/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js
+-rw-r--r--   0        0        0       97 2023-10-22 18:57:13.190257 reflex-0.5.1a1/reflex/.templates/web/jsconfig.json
+-rw-r--r--   0        0        0      118 2023-11-22 05:49:24.669539 reflex-0.5.1a1/reflex/.templates/web/next.config.js
+-rw-r--r--   0        0        0       82 2023-07-20 22:42:41.710359 reflex-0.5.1a1/reflex/.templates/web/postcss.config.js
+-rw-r--r--   0        0        0       59 2023-07-20 22:42:41.710616 reflex-0.5.1a1/reflex/.templates/web/styles/tailwind.css
+-rw-r--r--   0        0        0     1254 2023-09-16 20:27:37.277783 reflex-0.5.1a1/reflex/.templates/web/utils/client_side_routing.js
+-rw-r--r--   0        0        0     1622 2024-02-06 00:51:31.970968 reflex-0.5.1a1/reflex/.templates/web/utils/helpers/dataeditor.js
+-rw-r--r--   0        0        0      528 2024-05-05 01:15:24.052298 reflex-0.5.1a1/reflex/.templates/web/utils/helpers/debounce.js
+-rw-r--r--   0        0        0     1152 2023-11-22 05:49:24.669991 reflex-0.5.1a1/reflex/.templates/web/utils/helpers/range.js
+-rw-r--r--   0        0        0      566 2024-05-05 01:15:24.052363 reflex-0.5.1a1/reflex/.templates/web/utils/helpers/throttle.js
+-rw-r--r--   0        0        0    22617 2024-05-17 15:27:52.897284 reflex-0.5.1a1/reflex/.templates/web/utils/state.js
+-rw-r--r--   0        0        0     5831 2024-05-09 00:05:27.334655 reflex-0.5.1a1/reflex/__init__.py
+-rw-r--r--   0        0        0     7791 2024-05-09 12:11:15.217578 reflex-0.5.1a1/reflex/__init__.pyi
+-rw-r--r--   0        0        0      108 2023-08-05 17:01:44.301997 reflex-0.5.1a1/reflex/__main__.py
+-rw-r--r--   0        0        0      373 2023-07-20 22:42:41.710893 reflex-0.5.1a1/reflex/admin.py
+-rw-r--r--   0        0        0    47198 2024-05-17 15:27:52.897494 reflex-0.5.1a1/reflex/app.py
+-rw-r--r--   0        0        0     1152 2024-05-05 01:15:24.053241 reflex-0.5.1a1/reflex/app_module_for_backend.py
+-rw-r--r--   0        0        0     4274 2024-05-17 15:27:52.897654 reflex-0.5.1a1/reflex/base.py
+-rw-r--r--   0        0        0       27 2023-07-20 22:42:41.711176 reflex-0.5.1a1/reflex/compiler/__init__.py
+-rw-r--r--   0        0        0    17455 2024-05-07 15:33:05.682544 reflex-0.5.1a1/reflex/compiler/compiler.py
+-rw-r--r--   0        0        0     4344 2024-03-20 23:54:55.838388 reflex-0.5.1a1/reflex/compiler/templates.py
+-rw-r--r--   0        0        0    13274 2024-05-09 00:05:27.335443 reflex-0.5.1a1/reflex/compiler/utils.py
+-rw-r--r--   0        0        0      552 2024-05-05 01:15:24.053486 reflex-0.5.1a1/reflex/components/__init__.py
+-rw-r--r--   0        0        0      325 2024-02-06 00:51:31.973078 reflex-0.5.1a1/reflex/components/base/__init__.py
+-rw-r--r--   0        0        0      573 2024-02-06 00:51:31.973178 reflex-0.5.1a1/reflex/components/base/app_wrap.py
+-rw-r--r--   0        0        0     2890 2024-04-24 19:31:24.924269 reflex-0.5.1a1/reflex/components/base/app_wrap.pyi
+-rw-r--r--   0        0        0     1234 2024-04-04 14:57:26.376921 reflex-0.5.1a1/reflex/components/base/bare.py
+-rw-r--r--   0        0        0      151 2023-07-20 22:42:41.711762 reflex-0.5.1a1/reflex/components/base/body.py
+-rw-r--r--   0        0        0     3206 2024-04-24 19:31:56.503225 reflex-0.5.1a1/reflex/components/base/body.pyi
+-rw-r--r--   0        0        0      583 2024-03-20 23:54:55.839153 reflex-0.5.1a1/reflex/components/base/document.py
+-rw-r--r--   0        0        0    14232 2024-04-24 19:31:51.758673 reflex-0.5.1a1/reflex/components/base/document.pyi
+-rw-r--r--   0        0        0      312 2024-02-06 00:51:31.973871 reflex-0.5.1a1/reflex/components/base/fragment.py
+-rw-r--r--   0        0        0     3218 2024-04-24 19:31:51.784884 reflex-0.5.1a1/reflex/components/base/fragment.pyi
+-rw-r--r--   0        0        0      297 2023-12-05 17:15:35.585518 reflex-0.5.1a1/reflex/components/base/head.py
+-rw-r--r--   0        0        0     6002 2024-04-24 19:31:53.335977 reflex-0.5.1a1/reflex/components/base/head.pyi
+-rw-r--r--   0        0        0      929 2023-07-20 22:42:41.711911 reflex-0.5.1a1/reflex/components/base/link.py
+-rw-r--r--   0        0        0     6990 2024-04-24 19:31:27.077164 reflex-0.5.1a1/reflex/components/base/link.pyi
+-rw-r--r--   0        0        0     1438 2023-09-16 20:27:37.279391 reflex-0.5.1a1/reflex/components/base/meta.py
+-rw-r--r--   0        0        0    12804 2024-04-24 19:31:22.783259 reflex-0.5.1a1/reflex/components/base/meta.pyi
+-rw-r--r--   0        0        0     2298 2023-10-30 01:36:56.136333 reflex-0.5.1a1/reflex/components/base/script.py
+-rw-r--r--   0        0        0     4500 2024-04-24 19:31:45.804898 reflex-0.5.1a1/reflex/components/base/script.pyi
+-rw-r--r--   0        0        0     6378 2024-02-17 20:02:02.406461 reflex-0.5.1a1/reflex/components/chakra/__init__.py
+-rw-r--r--   0        0        0     5242 2024-02-07 21:49:00.589344 reflex-0.5.1a1/reflex/components/chakra/base.py
+-rw-r--r--   0        0        0    10917 2024-04-24 19:31:39.254151 reflex-0.5.1a1/reflex/components/chakra/base.pyi
+-rw-r--r--   0        0        0      459 2024-02-17 20:02:02.406937 reflex-0.5.1a1/reflex/components/chakra/datadisplay/__init__.py
+-rw-r--r--   0        0        0      352 2024-02-07 21:48:43.271089 reflex-0.5.1a1/reflex/components/chakra/datadisplay/badge.py
+-rw-r--r--   0        0        0     3654 2024-04-24 19:31:56.520176 reflex-0.5.1a1/reflex/components/chakra/datadisplay/badge.pyi
+-rw-r--r--   0        0        0      174 2024-02-17 20:02:02.407242 reflex-0.5.1a1/reflex/components/chakra/datadisplay/code.py
+-rw-r--r--   0        0        0     3229 2024-04-24 19:31:20.836024 reflex-0.5.1a1/reflex/components/chakra/datadisplay/code.pyi
+-rw-r--r--   0        0        0      657 2024-02-07 21:48:43.271979 reflex-0.5.1a1/reflex/components/chakra/datadisplay/divider.py
+-rw-r--r--   0        0        0     3934 2024-04-24 19:31:33.713586 reflex-0.5.1a1/reflex/components/chakra/datadisplay/divider.pyi
+-rw-r--r--   0        0        0      180 2024-02-07 21:48:43.272341 reflex-0.5.1a1/reflex/components/chakra/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     3251 2024-04-24 19:31:32.872876 reflex-0.5.1a1/reflex/components/chakra/datadisplay/keyboard_key.pyi
+-rw-r--r--   0        0        0     1484 2024-05-05 01:15:24.053780 reflex-0.5.1a1/reflex/components/chakra/datadisplay/list.py
+-rw-r--r--   0        0        0    12991 2024-05-05 01:15:24.053953 reflex-0.5.1a1/reflex/components/chakra/datadisplay/list.pyi
+-rw-r--r--   0        0        0     2149 2024-02-07 21:48:43.272980 reflex-0.5.1a1/reflex/components/chakra/datadisplay/stat.py
+-rw-r--r--   0        0        0    17461 2024-04-24 19:31:58.481785 reflex-0.5.1a1/reflex/components/chakra/datadisplay/stat.pyi
+-rw-r--r--   0        0        0     9122 2024-02-07 21:48:43.273484 reflex-0.5.1a1/reflex/components/chakra/datadisplay/table.py
+-rw-r--r--   0        0        0    27252 2024-04-24 19:32:01.076794 reflex-0.5.1a1/reflex/components/chakra/datadisplay/table.pyi
+-rw-r--r--   0        0        0     2294 2024-02-07 21:48:43.273971 reflex-0.5.1a1/reflex/components/chakra/datadisplay/tag.py
+-rw-r--r--   0        0        0    15734 2024-04-24 19:31:39.394572 reflex-0.5.1a1/reflex/components/chakra/datadisplay/tag.pyi
+-rw-r--r--   0        0        0      384 2024-02-06 00:51:31.976988 reflex-0.5.1a1/reflex/components/chakra/disclosure/__init__.py
+-rw-r--r--   0        0        0     3510 2024-04-24 21:16:40.836539 reflex-0.5.1a1/reflex/components/chakra/disclosure/accordion.py
+-rw-r--r--   0        0        0    15803 2024-04-24 19:31:46.785267 reflex-0.5.1a1/reflex/components/chakra/disclosure/accordion.pyi
+-rw-r--r--   0        0        0     3295 2024-02-07 21:48:43.274669 reflex-0.5.1a1/reflex/components/chakra/disclosure/tabs.py
+-rw-r--r--   0        0        0    18525 2024-04-24 19:31:51.181381 reflex-0.5.1a1/reflex/components/chakra/disclosure/tabs.pyi
+-rw-r--r--   0        0        0     1732 2024-02-07 21:48:43.274917 reflex-0.5.1a1/reflex/components/chakra/disclosure/transition.py
+-rw-r--r--   0        0        0    20003 2024-04-24 19:31:47.452515 reflex-0.5.1a1/reflex/components/chakra/disclosure/transition.pyi
+-rw-r--r--   0        0        0      278 2024-02-07 21:48:43.275325 reflex-0.5.1a1/reflex/components/chakra/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0     3258 2024-04-24 19:31:21.739444 reflex-0.5.1a1/reflex/components/chakra/disclosure/visuallyhidden.pyi
+-rw-r--r--   0        0        0      313 2024-02-06 00:51:31.977813 reflex-0.5.1a1/reflex/components/chakra/feedback/__init__.py
+-rw-r--r--   0        0        0     1623 2024-02-07 21:48:43.275534 reflex-0.5.1a1/reflex/components/chakra/feedback/alert.py
+-rw-r--r--   0        0        0    12381 2024-04-24 19:31:36.018582 reflex-0.5.1a1/reflex/components/chakra/feedback/alert.pyi
+-rw-r--r--   0        0        0     2006 2024-02-07 21:48:43.275746 reflex-0.5.1a1/reflex/components/chakra/feedback/circularprogress.py
+-rw-r--r--   0        0        0     7637 2024-04-24 19:31:35.464688 reflex-0.5.1a1/reflex/components/chakra/feedback/circularprogress.pyi
+-rw-r--r--   0        0        0      871 2024-02-07 21:48:43.275966 reflex-0.5.1a1/reflex/components/chakra/feedback/progress.py
+-rw-r--r--   0        0        0     4278 2024-04-24 19:31:39.746055 reflex-0.5.1a1/reflex/components/chakra/feedback/progress.pyi
+-rw-r--r--   0        0        0     1776 2024-02-07 21:48:43.276180 reflex-0.5.1a1/reflex/components/chakra/feedback/skeleton.py
+-rw-r--r--   0        0        0    10690 2024-04-24 19:32:01.405002 reflex-0.5.1a1/reflex/components/chakra/feedback/skeleton.pyi
+-rw-r--r--   0        0        0      704 2024-02-07 21:48:43.276461 reflex-0.5.1a1/reflex/components/chakra/feedback/spinner.py
+-rw-r--r--   0        0        0     4107 2024-04-24 19:31:21.992081 reflex-0.5.1a1/reflex/components/chakra/feedback/spinner.pyi
+-rw-r--r--   0        0        0     1453 2024-02-17 20:02:02.409691 reflex-0.5.1a1/reflex/components/chakra/forms/__init__.py
+-rw-r--r--   0        0        0     2395 2024-02-07 21:48:43.276688 reflex-0.5.1a1/reflex/components/chakra/forms/button.py
+-rw-r--r--   0        0        0    10545 2024-04-24 19:32:02.037829 reflex-0.5.1a1/reflex/components/chakra/forms/button.pyi
+-rw-r--r--   0        0        0     2764 2024-02-07 21:48:43.277006 reflex-0.5.1a1/reflex/components/chakra/forms/checkbox.py
+-rw-r--r--   0        0        0    10301 2024-04-24 19:31:34.287807 reflex-0.5.1a1/reflex/components/chakra/forms/checkbox.pyi
+-rw-r--r--   0        0        0     2860 2024-02-17 20:02:02.410102 reflex-0.5.1a1/reflex/components/chakra/forms/colormodeswitch.py
+-rw-r--r--   0        0        0    18459 2024-04-24 19:31:24.856589 reflex-0.5.1a1/reflex/components/chakra/forms/colormodeswitch.pyi
+-rw-r--r--   0        0        0      246 2024-02-06 00:51:31.979244 reflex-0.5.1a1/reflex/components/chakra/forms/date_picker.py
+-rw-r--r--   0        0        0     5841 2024-04-24 19:31:54.024641 reflex-0.5.1a1/reflex/components/chakra/forms/date_picker.pyi
+-rw-r--r--   0        0        0      280 2024-02-06 00:51:31.979387 reflex-0.5.1a1/reflex/components/chakra/forms/date_time_picker.py
+-rw-r--r--   0        0        0     5854 2024-04-24 19:31:40.823621 reflex-0.5.1a1/reflex/components/chakra/forms/date_time_picker.pyi
+-rw-r--r--   0        0        0     2110 2024-02-07 21:48:43.277649 reflex-0.5.1a1/reflex/components/chakra/forms/editable.py
+-rw-r--r--   0        0        0    13339 2024-04-24 19:31:15.703021 reflex-0.5.1a1/reflex/components/chakra/forms/editable.pyi
+-rw-r--r--   0        0        0      246 2024-02-06 00:51:31.979682 reflex-0.5.1a1/reflex/components/chakra/forms/email.py
+-rw-r--r--   0        0        0     5825 2024-04-24 19:31:50.788652 reflex-0.5.1a1/reflex/components/chakra/forms/email.pyi
+-rw-r--r--   0        0        0     2579 2024-03-20 23:54:55.839690 reflex-0.5.1a1/reflex/components/chakra/forms/form.py
+-rw-r--r--   0        0        0    20619 2024-04-24 19:31:56.858215 reflex-0.5.1a1/reflex/components/chakra/forms/form.pyi
+-rw-r--r--   0        0        0      935 2024-02-06 00:51:31.980162 reflex-0.5.1a1/reflex/components/chakra/forms/iconbutton.py
+-rw-r--r--   0        0        0     4668 2024-04-24 19:31:50.346409 reflex-0.5.1a1/reflex/components/chakra/forms/iconbutton.pyi
+-rw-r--r--   0        0        0     4312 2024-03-20 23:54:55.840321 reflex-0.5.1a1/reflex/components/chakra/forms/input.py
+-rw-r--r--   0        0        0    21514 2024-04-24 19:31:59.673777 reflex-0.5.1a1/reflex/components/chakra/forms/input.pyi
+-rw-r--r--   0        0        0    12940 2024-02-06 00:51:31.980569 reflex-0.5.1a1/reflex/components/chakra/forms/multiselect.py
+-rw-r--r--   0        0        0     4334 2024-02-07 21:48:43.278754 reflex-0.5.1a1/reflex/components/chakra/forms/numberinput.py
+-rw-r--r--   0        0        0    18093 2024-04-24 19:31:56.097983 reflex-0.5.1a1/reflex/components/chakra/forms/numberinput.pyi
+-rw-r--r--   0        0        0      256 2024-02-06 00:51:31.980851 reflex-0.5.1a1/reflex/components/chakra/forms/password.py
+-rw-r--r--   0        0        0     5834 2024-04-24 19:31:37.858051 reflex-0.5.1a1/reflex/components/chakra/forms/password.pyi
+-rw-r--r--   0        0        0     6503 2024-04-12 01:14:12.262063 reflex-0.5.1a1/reflex/components/chakra/forms/pininput.py
+-rw-r--r--   0        0        0     9369 2024-05-05 01:15:24.054063 reflex-0.5.1a1/reflex/components/chakra/forms/pininput.pyi
+-rw-r--r--   0        0        0     3172 2024-04-12 01:14:12.263122 reflex-0.5.1a1/reflex/components/chakra/forms/radio.py
+-rw-r--r--   0        0        0     8410 2024-04-24 19:31:17.428977 reflex-0.5.1a1/reflex/components/chakra/forms/radio.pyi
+-rw-r--r--   0        0        0     4543 2024-04-12 01:14:12.263746 reflex-0.5.1a1/reflex/components/chakra/forms/rangeslider.py
+-rw-r--r--   0        0        0    13939 2024-04-24 19:31:59.377848 reflex-0.5.1a1/reflex/components/chakra/forms/rangeslider.pyi
+-rw-r--r--   0        0        0     3624 2024-02-07 21:48:43.280461 reflex-0.5.1a1/reflex/components/chakra/forms/select.py
+-rw-r--r--   0        0        0     8868 2024-04-24 19:31:48.346816 reflex-0.5.1a1/reflex/components/chakra/forms/select.pyi
+-rw-r--r--   0        0        0     3532 2024-02-07 21:48:43.280779 reflex-0.5.1a1/reflex/components/chakra/forms/slider.py
+-rw-r--r--   0        0        0    17461 2024-04-24 19:32:01.264082 reflex-0.5.1a1/reflex/components/chakra/forms/slider.pyi
+-rw-r--r--   0        0        0     1838 2024-02-07 21:48:43.281044 reflex-0.5.1a1/reflex/components/chakra/forms/switch.py
+-rw-r--r--   0        0        0     6531 2024-04-24 19:31:48.016708 reflex-0.5.1a1/reflex/components/chakra/forms/switch.pyi
+-rw-r--r--   0        0        0     2474 2024-02-09 10:00:28.809203 reflex-0.5.1a1/reflex/components/chakra/forms/textarea.py
+-rw-r--r--   0        0        0     5419 2024-04-24 19:31:51.889720 reflex-0.5.1a1/reflex/components/chakra/forms/textarea.pyi
+-rw-r--r--   0        0        0      246 2024-02-06 00:51:31.982573 reflex-0.5.1a1/reflex/components/chakra/forms/time_picker.py
+-rw-r--r--   0        0        0     5841 2024-04-24 19:31:46.686774 reflex-0.5.1a1/reflex/components/chakra/forms/time_picker.pyi
+-rw-r--r--   0        0        0      487 2024-02-17 20:02:02.413006 reflex-0.5.1a1/reflex/components/chakra/layout/__init__.py
+-rw-r--r--   0        0        0      315 2024-02-07 21:48:43.281752 reflex-0.5.1a1/reflex/components/chakra/layout/aspect_ratio.py
+-rw-r--r--   0        0        0     3379 2024-04-24 19:31:52.881611 reflex-0.5.1a1/reflex/components/chakra/layout/aspect_ratio.pyi
+-rw-r--r--   0        0        0      755 2024-02-07 21:48:43.281982 reflex-0.5.1a1/reflex/components/chakra/layout/box.py
+-rw-r--r--   0        0        0     3662 2024-04-24 19:31:18.516418 reflex-0.5.1a1/reflex/components/chakra/layout/box.pyi
+-rw-r--r--   0        0        0     2967 2024-02-07 21:48:43.282202 reflex-0.5.1a1/reflex/components/chakra/layout/card.py
+-rw-r--r--   0        0        0    13850 2024-04-24 19:31:48.005155 reflex-0.5.1a1/reflex/components/chakra/layout/card.pyi
+-rw-r--r--   0        0        0      389 2024-02-07 21:48:43.282417 reflex-0.5.1a1/reflex/components/chakra/layout/center.py
+-rw-r--r--   0        0        0     8692 2024-04-24 19:31:24.264440 reflex-0.5.1a1/reflex/components/chakra/layout/center.pyi
+-rw-r--r--   0        0        0      354 2024-02-07 21:48:43.282843 reflex-0.5.1a1/reflex/components/chakra/layout/container.py
+-rw-r--r--   0        0        0     3431 2024-04-24 19:31:47.990635 reflex-0.5.1a1/reflex/components/chakra/layout/container.pyi
+-rw-r--r--   0        0        0      715 2024-02-07 21:48:43.283082 reflex-0.5.1a1/reflex/components/chakra/layout/flex.py
+-rw-r--r--   0        0        0     4138 2024-04-24 19:31:44.830583 reflex-0.5.1a1/reflex/components/chakra/layout/flex.pyi
+-rw-r--r--   0        0        0     4318 2024-02-07 21:48:43.283328 reflex-0.5.1a1/reflex/components/chakra/layout/grid.py
+-rw-r--r--   0        0        0    13853 2024-04-24 19:31:41.333938 reflex-0.5.1a1/reflex/components/chakra/layout/grid.pyi
+-rw-r--r--   0        0        0      179 2024-02-07 21:48:43.283579 reflex-0.5.1a1/reflex/components/chakra/layout/spacer.py
+-rw-r--r--   0        0        0     3230 2024-04-24 19:31:48.988499 reflex-0.5.1a1/reflex/components/chakra/layout/spacer.pyi
+-rw-r--r--   0        0        0     1077 2024-02-07 21:48:43.283791 reflex-0.5.1a1/reflex/components/chakra/layout/stack.py
+-rw-r--r--   0        0        0    12219 2024-04-24 19:31:34.279618 reflex-0.5.1a1/reflex/components/chakra/layout/stack.pyi
+-rw-r--r--   0        0        0     1463 2024-02-07 21:48:43.284089 reflex-0.5.1a1/reflex/components/chakra/layout/wrap.py
+-rw-r--r--   0        0        0     6943 2024-04-24 19:31:33.351664 reflex-0.5.1a1/reflex/components/chakra/layout/wrap.pyi
+-rw-r--r--   0        0        0      190 2024-02-06 00:51:31.985088 reflex-0.5.1a1/reflex/components/chakra/media/__init__.py
+-rw-r--r--   0        0        0     1668 2024-02-07 21:48:43.284332 reflex-0.5.1a1/reflex/components/chakra/media/avatar.py
+-rw-r--r--   0        0        0    10445 2024-04-24 19:31:27.389378 reflex-0.5.1a1/reflex/components/chakra/media/avatar.pyi
+-rw-r--r--   0        0        0     2462 2024-04-24 21:16:40.836689 reflex-0.5.1a1/reflex/components/chakra/media/icon.py
+-rw-r--r--   0        0        0     6271 2024-04-24 19:31:19.854478 reflex-0.5.1a1/reflex/components/chakra/media/icon.pyi
+-rw-r--r--   0        0        0     2400 2024-02-07 21:48:43.284781 reflex-0.5.1a1/reflex/components/chakra/media/image.py
+-rw-r--r--   0        0        0     5423 2024-04-24 19:31:52.691354 reflex-0.5.1a1/reflex/components/chakra/media/image.pyi
+-rw-r--r--   0        0        0      419 2024-02-06 00:51:31.986093 reflex-0.5.1a1/reflex/components/chakra/navigation/__init__.py
+-rw-r--r--   0        0        0     2925 2024-02-07 21:48:43.285023 reflex-0.5.1a1/reflex/components/chakra/navigation/breadcrumb.py
+-rw-r--r--   0        0        0    13575 2024-04-24 19:32:01.936776 reflex-0.5.1a1/reflex/components/chakra/navigation/breadcrumb.pyi
+-rw-r--r--   0        0        0     1475 2024-02-06 00:51:31.986318 reflex-0.5.1a1/reflex/components/chakra/navigation/link.py
+-rw-r--r--   0        0        0     3999 2024-04-24 19:31:19.850596 reflex-0.5.1a1/reflex/components/chakra/navigation/link.pyi
+-rw-r--r--   0        0        0      521 2024-02-06 00:51:31.986581 reflex-0.5.1a1/reflex/components/chakra/navigation/linkoverlay.py
+-rw-r--r--   0        0        0     6233 2024-04-24 19:31:59.056993 reflex-0.5.1a1/reflex/components/chakra/navigation/linkoverlay.pyi
+-rw-r--r--   0        0        0     2935 2024-02-07 21:48:43.285634 reflex-0.5.1a1/reflex/components/chakra/navigation/stepper.py
+-rw-r--r--   0        0        0    27922 2024-04-24 19:31:59.991438 reflex-0.5.1a1/reflex/components/chakra/navigation/stepper.pyi
+-rw-r--r--   0        0        0      850 2024-02-06 00:51:31.987014 reflex-0.5.1a1/reflex/components/chakra/overlay/__init__.py
+-rw-r--r--   0        0        0     5200 2024-02-07 21:48:43.285952 reflex-0.5.1a1/reflex/components/chakra/overlay/alertdialog.py
+-rw-r--r--   0        0        0    23985 2024-04-24 19:31:53.441920 reflex-0.5.1a1/reflex/components/chakra/overlay/alertdialog.pyi
+-rw-r--r--   0        0        0     5186 2024-02-06 00:51:31.987467 reflex-0.5.1a1/reflex/components/chakra/overlay/drawer.py
+-rw-r--r--   0        0        0    25406 2024-04-24 19:32:02.090146 reflex-0.5.1a1/reflex/components/chakra/overlay/drawer.pyi
+-rw-r--r--   0        0        0     6974 2024-02-07 21:48:43.286352 reflex-0.5.1a1/reflex/components/chakra/overlay/menu.py
+-rw-r--r--   0        0        0    28682 2024-04-24 19:32:03.285218 reflex-0.5.1a1/reflex/components/chakra/overlay/menu.pyi
+-rw-r--r--   0        0        0     5270 2024-02-07 21:48:43.286588 reflex-0.5.1a1/reflex/components/chakra/overlay/modal.py
+-rw-r--r--   0        0        0    23549 2024-04-24 19:32:01.507839 reflex-0.5.1a1/reflex/components/chakra/overlay/modal.pyi
+-rw-r--r--   0        0        0     5967 2024-02-07 21:48:43.286836 reflex-0.5.1a1/reflex/components/chakra/overlay/popover.py
+-rw-r--r--   0        0        0    29893 2024-04-24 19:32:01.594206 reflex-0.5.1a1/reflex/components/chakra/overlay/popover.pyi
+-rw-r--r--   0        0        0     2127 2024-02-07 21:48:43.287207 reflex-0.5.1a1/reflex/components/chakra/overlay/tooltip.py
+-rw-r--r--   0        0        0     6060 2024-04-24 19:31:15.213215 reflex-0.5.1a1/reflex/components/chakra/overlay/tooltip.pyi
+-rw-r--r--   0        0        0      271 2024-02-06 00:51:31.988661 reflex-0.5.1a1/reflex/components/chakra/typography/__init__.py
+-rw-r--r--   0        0        0      379 2024-02-07 21:48:43.287449 reflex-0.5.1a1/reflex/components/chakra/typography/heading.py
+-rw-r--r--   0        0        0     3706 2024-04-24 19:31:17.288584 reflex-0.5.1a1/reflex/components/chakra/typography/heading.pyi
+-rw-r--r--   0        0        0      671 2024-02-07 21:48:43.287662 reflex-0.5.1a1/reflex/components/chakra/typography/highlight.py
+-rw-r--r--   0        0        0     3645 2024-04-24 19:31:37.053293 reflex-0.5.1a1/reflex/components/chakra/typography/highlight.pyi
+-rw-r--r--   0        0        0      328 2024-02-07 21:48:43.287874 reflex-0.5.1a1/reflex/components/chakra/typography/span.py
+-rw-r--r--   0        0        0     3372 2024-04-24 19:31:23.281815 reflex-0.5.1a1/reflex/components/chakra/typography/span.pyi
+-rw-r--r--   0        0        0      472 2024-02-07 21:48:43.288076 reflex-0.5.1a1/reflex/components/chakra/typography/text.py
+-rw-r--r--   0        0        0     3596 2024-04-24 19:31:50.785304 reflex-0.5.1a1/reflex/components/chakra/typography/text.pyi
+-rw-r--r--   0        0        0    77001 2024-05-17 15:27:52.897895 reflex-0.5.1a1/reflex/components/component.py
+-rw-r--r--   0        0        0      943 2024-05-17 15:27:52.898146 reflex-0.5.1a1/reflex/components/core/__init__.py
+-rw-r--r--   0        0        0     8043 2024-05-17 15:27:52.898347 reflex-0.5.1a1/reflex/components/core/banner.py
+-rw-r--r--   0        0        0    22528 2024-05-17 15:27:52.898447 reflex-0.5.1a1/reflex/components/core/banner.pyi
+-rw-r--r--   0        0        0     1873 2024-02-06 00:51:31.991625 reflex-0.5.1a1/reflex/components/core/client_side_routing.py
+-rw-r--r--   0        0        0     6264 2024-04-24 19:31:22.918462 reflex-0.5.1a1/reflex/components/core/client_side_routing.pyi
+-rw-r--r--   0        0        0      590 2024-02-17 20:02:02.417474 reflex-0.5.1a1/reflex/components/core/colors.py
+-rw-r--r--   0        0        0     6005 2024-05-17 15:27:52.898667 reflex-0.5.1a1/reflex/components/core/cond.py
+-rw-r--r--   0        0        0     4820 2024-05-17 15:27:52.898774 reflex-0.5.1a1/reflex/components/core/debounce.py
+-rw-r--r--   0        0        0     4216 2024-04-25 16:52:48.841425 reflex-0.5.1a1/reflex/components/core/debounce.pyi
+-rw-r--r--   0        0        0     4732 2024-05-17 15:27:52.898885 reflex-0.5.1a1/reflex/components/core/foreach.py
+-rw-r--r--   0        0        0     1284 2024-05-05 01:15:24.054752 reflex-0.5.1a1/reflex/components/core/html.py
+-rw-r--r--   0        0        0     6616 2024-04-25 05:29:57.085054 reflex-0.5.1a1/reflex/components/core/html.pyi
+-rw-r--r--   0        0        0       30 2024-02-07 21:48:43.290204 reflex-0.5.1a1/reflex/components/core/layout/__init__.py
+-rw-r--r--   0        0        0     9484 2024-05-07 15:33:05.683232 reflex-0.5.1a1/reflex/components/core/match.py
+-rw-r--r--   0        0        0     1907 2024-04-04 14:19:59.331992 reflex-0.5.1a1/reflex/components/core/responsive.py
+-rw-r--r--   0        0        0    10146 2024-05-17 15:27:52.899088 reflex-0.5.1a1/reflex/components/core/upload.py
+-rw-r--r--   0        0        0    17147 2024-04-25 16:52:48.841883 reflex-0.5.1a1/reflex/components/core/upload.pyi
+-rw-r--r--   0        0        0      357 2024-04-05 17:14:14.460655 reflex-0.5.1a1/reflex/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0    11363 2024-05-07 15:33:05.683354 reflex-0.5.1a1/reflex/components/datadisplay/code.py
+-rw-r--r--   0        0        0    31213 2024-05-07 15:33:05.683489 reflex-0.5.1a1/reflex/components/datadisplay/code.pyi
+-rw-r--r--   0        0        0    12632 2024-02-06 00:51:31.995005 reflex-0.5.1a1/reflex/components/datadisplay/dataeditor.py
+-rw-r--r--   0        0        0    10485 2024-04-24 19:31:43.237754 reflex-0.5.1a1/reflex/components/datadisplay/dataeditor.pyi
+-rw-r--r--   0        0        0     2562 2024-04-05 17:14:14.460754 reflex-0.5.1a1/reflex/components/datadisplay/logo.py
+-rw-r--r--   0        0        0       73 2023-11-26 20:56:44.132351 reflex-0.5.1a1/reflex/components/el/__init__.py
+-rw-r--r--   0        0        0      113 2023-11-26 20:56:44.132431 reflex-0.5.1a1/reflex/components/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-11-26 20:56:44.132596 reflex-0.5.1a1/reflex/components/el/constants/html.py
+-rw-r--r--   0        0        0    15554 2023-11-26 20:56:44.132713 reflex-0.5.1a1/reflex/components/el/constants/react.py
+-rw-r--r--   0        0        0     1713 2023-11-26 20:56:44.132789 reflex-0.5.1a1/reflex/components/el/constants/reflex.py
+-rw-r--r--   0        0        0      494 2023-12-01 04:51:31.098496 reflex-0.5.1a1/reflex/components/el/element.py
+-rw-r--r--   0        0        0     3213 2024-04-24 19:32:01.854505 reflex-0.5.1a1/reflex/components/el/element.pyi
+-rw-r--r--   0        0        0     3529 2024-03-20 23:54:55.843475 reflex-0.5.1a1/reflex/components/el/elements/__init__.py
+-rw-r--r--   0        0        0     1982 2024-02-17 20:02:02.419390 reflex-0.5.1a1/reflex/components/el/elements/base.py
+-rw-r--r--   0        0        0     6340 2024-04-24 19:31:34.952107 reflex-0.5.1a1/reflex/components/el/elements/base.pyi
+-rw-r--r--   0        0        0    20167 2024-05-17 15:27:52.899317 reflex-0.5.1a1/reflex/components/el/elements/forms.py
+-rw-r--r--   0        0        0    99555 2024-04-25 16:52:48.842962 reflex-0.5.1a1/reflex/components/el/elements/forms.pyi
+-rw-r--r--   0        0        0     3610 2024-02-06 00:51:31.998070 reflex-0.5.1a1/reflex/components/el/elements/inline.py
+-rw-r--r--   0        0        0   164607 2024-04-24 19:32:05.408521 reflex-0.5.1a1/reflex/components/el/elements/inline.pyi
+-rw-r--r--   0        0        0     8467 2024-05-17 15:27:52.899524 reflex-0.5.1a1/reflex/components/el/elements/media.py
+-rw-r--r--   0        0        0    93669 2024-05-17 15:27:52.899772 reflex-0.5.1a1/reflex/components/el/elements/media.pyi
+-rw-r--r--   0        0        0     1337 2023-11-26 20:56:44.134404 reflex-0.5.1a1/reflex/components/el/elements/metadata.py
+-rw-r--r--   0        0        0    28031 2024-04-24 19:32:01.554937 reflex-0.5.1a1/reflex/components/el/elements/metadata.pyi
+-rw-r--r--   0        0        0     1569 2023-11-26 20:56:44.134590 reflex-0.5.1a1/reflex/components/el/elements/other.py
+-rw-r--r--   0        0        0    42033 2024-04-24 19:31:59.581160 reflex-0.5.1a1/reflex/components/el/elements/other.pyi
+-rw-r--r--   0        0        0     1406 2024-02-17 20:02:02.421306 reflex-0.5.1a1/reflex/components/el/elements/scripts.py
+-rw-r--r--   0        0        0    19615 2024-04-24 19:31:22.715670 reflex-0.5.1a1/reflex/components/el/elements/scripts.pyi
+-rw-r--r--   0        0        0     1535 2024-02-17 20:02:02.421507 reflex-0.5.1a1/reflex/components/el/elements/sectioning.py
+-rw-r--r--   0        0        0    87242 2024-04-24 19:32:04.046011 reflex-0.5.1a1/reflex/components/el/elements/sectioning.pyi
+-rw-r--r--   0        0        0     2767 2024-02-17 20:02:02.421759 reflex-0.5.1a1/reflex/components/el/elements/tables.py
+-rw-r--r--   0        0        0    61849 2024-04-24 19:32:03.007985 reflex-0.5.1a1/reflex/components/el/elements/tables.pyi
+-rw-r--r--   0        0        0     2432 2024-02-17 20:02:02.421997 reflex-0.5.1a1/reflex/components/el/elements/typography.py
+-rw-r--r--   0        0        0    89115 2024-04-24 19:32:04.312119 reflex-0.5.1a1/reflex/components/el/elements/typography.pyi
+-rw-r--r--   0        0        0       88 2024-02-06 00:51:31.999860 reflex-0.5.1a1/reflex/components/gridjs/__init__.py
+-rw-r--r--   0        0        0     4304 2024-05-17 15:27:52.899989 reflex-0.5.1a1/reflex/components/gridjs/datatable.py
+-rw-r--r--   0        0        0     7053 2024-04-24 19:31:36.593992 reflex-0.5.1a1/reflex/components/gridjs/datatable.pyi
+-rw-r--r--   0        0        0      501 2024-02-06 00:51:32.000350 reflex-0.5.1a1/reflex/components/literals.py
+-rw-r--r--   0        0        0       73 2024-02-07 21:48:43.293647 reflex-0.5.1a1/reflex/components/lucide/__init__.py
+-rw-r--r--   0        0        0    34077 2024-05-09 00:05:27.336308 reflex-0.5.1a1/reflex/components/lucide/icon.py
+-rw-r--r--   0        0        0    37918 2024-05-05 01:15:24.056110 reflex-0.5.1a1/reflex/components/lucide/icon.pyi
+-rw-r--r--   0        0        0       87 2024-02-06 00:51:32.000748 reflex-0.5.1a1/reflex/components/markdown/__init__.py
+-rw-r--r--   0        0        0    10867 2024-05-09 00:05:27.336466 reflex-0.5.1a1/reflex/components/markdown/markdown.py
+-rw-r--r--   0        0        0     5100 2024-05-09 00:05:27.336616 reflex-0.5.1a1/reflex/components/markdown/markdown.pyi
+-rw-r--r--   0        0        0       44 2024-02-06 00:51:32.001397 reflex-0.5.1a1/reflex/components/media/__init__.py
+-rw-r--r--   0        0        0      102 2024-02-06 00:51:32.001492 reflex-0.5.1a1/reflex/components/media/icon.py
+-rw-r--r--   0        0        0       79 2024-02-06 00:51:32.001557 reflex-0.5.1a1/reflex/components/moment/__init__.py
+-rw-r--r--   0        0        0     3925 2024-02-06 00:51:32.001623 reflex-0.5.1a1/reflex/components/moment/moment.py
+-rw-r--r--   0        0        0     6870 2024-04-24 19:31:51.190910 reflex-0.5.1a1/reflex/components/moment/moment.pyi
+-rw-r--r--   0        0        0      239 2024-02-06 00:51:32.001924 reflex-0.5.1a1/reflex/components/next/__init__.py
+-rw-r--r--   0        0        0      189 2024-01-08 22:19:50.677879 reflex-0.5.1a1/reflex/components/next/base.py
+-rw-r--r--   0        0        0     3233 2024-04-24 19:31:43.822514 reflex-0.5.1a1/reflex/components/next/base.pyi
+-rw-r--r--   0        0        0     3831 2024-01-08 22:19:50.678013 reflex-0.5.1a1/reflex/components/next/image.py
+-rw-r--r--   0        0        0     5795 2024-04-24 19:31:33.244479 reflex-0.5.1a1/reflex/components/next/image.pyi
+-rw-r--r--   0        0        0      503 2024-02-06 00:51:32.002304 reflex-0.5.1a1/reflex/components/next/link.py
+-rw-r--r--   0        0        0     3461 2024-04-24 19:31:15.603661 reflex-0.5.1a1/reflex/components/next/link.pyi
+-rw-r--r--   0        0        0      730 2024-01-08 22:19:50.678316 reflex-0.5.1a1/reflex/components/next/video.py
+-rw-r--r--   0        0        0     3429 2024-04-24 19:31:46.249185 reflex-0.5.1a1/reflex/components/next/video.pyi
+-rw-r--r--   0        0        0       77 2024-02-06 00:51:32.002529 reflex-0.5.1a1/reflex/components/plotly/__init__.py
+-rw-r--r--   0        0        0      964 2024-03-20 23:54:55.846069 reflex-0.5.1a1/reflex/components/plotly/plotly.py
+-rw-r--r--   0        0        0     6865 2024-04-24 19:31:24.224015 reflex-0.5.1a1/reflex/components/plotly/plotly.pyi
+-rw-r--r--   0        0        0      906 2024-05-17 15:27:52.900055 reflex-0.5.1a1/reflex/components/props.py
+-rw-r--r--   0        0        0      112 2024-02-17 20:02:02.423429 reflex-0.5.1a1/reflex/components/radix/__init__.py
+-rw-r--r--   0        0        0      214 2024-02-17 20:02:02.423526 reflex-0.5.1a1/reflex/components/radix/primitives/__init__.py
+-rw-r--r--   0        0        0    16159 2024-05-17 15:27:52.900174 reflex-0.5.1a1/reflex/components/radix/primitives/accordion.py
+-rw-r--r--   0        0        0    37999 2024-05-17 15:27:52.900675 reflex-0.5.1a1/reflex/components/radix/primitives/accordion.pyi
+-rw-r--r--   0        0        0      869 2024-02-06 00:51:32.004050 reflex-0.5.1a1/reflex/components/radix/primitives/base.py
+-rw-r--r--   0        0        0     6478 2024-04-24 19:31:44.069976 reflex-0.5.1a1/reflex/components/radix/primitives/base.pyi
+-rw-r--r--   0        0        0     8660 2024-03-20 23:54:55.846917 reflex-0.5.1a1/reflex/components/radix/primitives/drawer.py
+-rw-r--r--   0        0        0    34484 2024-04-24 19:32:02.551316 reflex-0.5.1a1/reflex/components/radix/primitives/drawer.pyi
+-rw-r--r--   0        0        0     4964 2024-05-17 15:27:52.901266 reflex-0.5.1a1/reflex/components/radix/primitives/form.py
+-rw-r--r--   0        0        0    48138 2024-05-07 15:33:05.684481 reflex-0.5.1a1/reflex/components/radix/primitives/form.pyi
+-rw-r--r--   0        0        0     4160 2024-05-07 15:33:05.684814 reflex-0.5.1a1/reflex/components/radix/primitives/progress.py
+-rw-r--r--   0        0        0    22874 2024-05-07 15:33:05.685122 reflex-0.5.1a1/reflex/components/radix/primitives/progress.pyi
+-rw-r--r--   0        0        0     5198 2024-05-07 15:33:05.685275 reflex-0.5.1a1/reflex/components/radix/primitives/slider.py
+-rw-r--r--   0        0        0    16877 2024-05-07 15:33:05.685394 reflex-0.5.1a1/reflex/components/radix/primitives/slider.pyi
+-rw-r--r--   0        0        0      292 2024-02-17 20:02:02.426799 reflex-0.5.1a1/reflex/components/radix/themes/__init__.py
+-rw-r--r--   0        0        0     8294 2024-04-26 18:47:21.875701 reflex-0.5.1a1/reflex/components/radix/themes/base.py
+-rw-r--r--   0        0        0    26971 2024-05-05 01:15:24.056523 reflex-0.5.1a1/reflex/components/radix/themes/base.pyi
+-rw-r--r--   0        0        0     5543 2024-05-17 15:27:52.901396 reflex-0.5.1a1/reflex/components/radix/themes/color_mode.py
+-rw-r--r--   0        0        0    22145 2024-05-17 15:27:52.901528 reflex-0.5.1a1/reflex/components/radix/themes/color_mode.pyi
+-rw-r--r--   0        0        0     2440 2024-05-09 00:05:27.336999 reflex-0.5.1a1/reflex/components/radix/themes/components/__init__.py
+-rw-r--r--   0        0        0     3267 2024-03-20 23:54:55.849529 reflex-0.5.1a1/reflex/components/radix/themes/components/alert_dialog.py
+-rw-r--r--   0        0        0    24434 2024-04-24 19:31:57.706076 reflex-0.5.1a1/reflex/components/radix/themes/components/alert_dialog.pyi
+-rw-r--r--   0        0        0      400 2024-02-17 20:02:02.428862 reflex-0.5.1a1/reflex/components/radix/themes/components/aspect_ratio.py
+-rw-r--r--   0        0        0     3640 2024-04-24 19:31:17.911074 reflex-0.5.1a1/reflex/components/radix/themes/components/aspect_ratio.pyi
+-rw-r--r--   0        0        0      989 2024-03-20 23:54:55.849841 reflex-0.5.1a1/reflex/components/radix/themes/components/avatar.py
+-rw-r--r--   0        0        0     6562 2024-04-24 19:31:52.410239 reflex-0.5.1a1/reflex/components/radix/themes/components/avatar.pyi
+-rw-r--r--   0        0        0      821 2024-04-26 18:47:21.876311 reflex-0.5.1a1/reflex/components/radix/themes/components/badge.py
+-rw-r--r--   0        0        0     9347 2024-04-26 18:47:21.876509 reflex-0.5.1a1/reflex/components/radix/themes/components/badge.pyi
+-rw-r--r--   0        0        0     1125 2024-04-26 18:47:21.876620 reflex-0.5.1a1/reflex/components/radix/themes/components/button.py
+-rw-r--r--   0        0        0    11939 2024-04-26 18:47:21.876761 reflex-0.5.1a1/reflex/components/radix/themes/components/button.pyi
+-rw-r--r--   0        0        0     2378 2024-03-20 23:54:55.850376 reflex-0.5.1a1/reflex/components/radix/themes/components/callout.py
+-rw-r--r--   0        0        0    38710 2024-04-24 19:32:02.594947 reflex-0.5.1a1/reflex/components/radix/themes/components/callout.pyi
+-rw-r--r--   0        0        0      659 2024-02-17 20:02:02.430724 reflex-0.5.1a1/reflex/components/radix/themes/components/card.py
+-rw-r--r--   0        0        0     7200 2024-04-24 19:31:48.002992 reflex-0.5.1a1/reflex/components/radix/themes/components/card.pyi
+-rw-r--r--   0        0        0     4679 2024-03-20 23:54:55.851297 reflex-0.5.1a1/reflex/components/radix/themes/components/checkbox.py
+-rw-r--r--   0        0        0    20877 2024-04-24 19:32:01.819836 reflex-0.5.1a1/reflex/components/radix/themes/components/checkbox.pyi
+-rw-r--r--   0        0        0     1301 2024-04-26 18:47:21.876837 reflex-0.5.1a1/reflex/components/radix/themes/components/checkbox_cards.py
+-rw-r--r--   0        0        0     9591 2024-04-26 18:47:21.876955 reflex-0.5.1a1/reflex/components/radix/themes/components/checkbox_cards.pyi
+-rw-r--r--   0        0        0     1024 2024-04-26 18:47:21.877018 reflex-0.5.1a1/reflex/components/radix/themes/components/checkbox_group.py
+-rw-r--r--   0        0        0     9012 2024-04-26 18:47:21.877125 reflex-0.5.1a1/reflex/components/radix/themes/components/checkbox_group.pyi
+-rw-r--r--   0        0        0     5049 2024-03-20 23:54:55.852012 reflex-0.5.1a1/reflex/components/radix/themes/components/context_menu.py
+-rw-r--r--   0        0        0    31192 2024-04-24 19:32:03.158519 reflex-0.5.1a1/reflex/components/radix/themes/components/context_menu.pyi
+-rw-r--r--   0        0        0     1508 2024-04-26 18:47:21.877372 reflex-0.5.1a1/reflex/components/radix/themes/components/data_list.py
+-rw-r--r--   0        0        0    15403 2024-04-26 18:47:21.877634 reflex-0.5.1a1/reflex/components/radix/themes/components/data_list.pyi
+-rw-r--r--   0        0        0     2600 2024-03-20 23:54:55.852519 reflex-0.5.1a1/reflex/components/radix/themes/components/dialog.py
+-rw-r--r--   0        0        0    24895 2024-04-24 19:32:02.097223 reflex-0.5.1a1/reflex/components/radix/themes/components/dialog.pyi
+-rw-r--r--   0        0        0    11256 2024-03-20 23:54:55.852973 reflex-0.5.1a1/reflex/components/radix/themes/components/dropdown_menu.py
+-rw-r--r--   0        0        0    37901 2024-04-24 19:32:02.303816 reflex-0.5.1a1/reflex/components/radix/themes/components/dropdown_menu.pyi
+-rw-r--r--   0        0        0     2405 2024-03-20 23:54:55.853285 reflex-0.5.1a1/reflex/components/radix/themes/components/hover_card.py
+-rw-r--r--   0        0        0    17744 2024-04-24 19:31:56.396802 reflex-0.5.1a1/reflex/components/radix/themes/components/hover_card.pyi
+-rw-r--r--   0        0        0     2940 2024-05-09 00:05:27.337231 reflex-0.5.1a1/reflex/components/radix/themes/components/icon_button.py
+-rw-r--r--   0        0        0    12126 2024-05-07 15:33:05.685671 reflex-0.5.1a1/reflex/components/radix/themes/components/icon_button.pyi
+-rw-r--r--   0        0        0     1015 2024-03-20 23:54:55.853906 reflex-0.5.1a1/reflex/components/radix/themes/components/inset.py
+-rw-r--r--   0        0        0     7889 2024-04-24 19:31:39.003439 reflex-0.5.1a1/reflex/components/radix/themes/components/inset.pyi
+-rw-r--r--   0        0        0     3177 2024-03-20 23:54:55.854041 reflex-0.5.1a1/reflex/components/radix/themes/components/popover.py
+-rw-r--r--   0        0        0    17404 2024-04-24 19:32:01.605821 reflex-0.5.1a1/reflex/components/radix/themes/components/popover.pyi
+-rw-r--r--   0        0        0     1598 2024-05-09 00:05:27.337432 reflex-0.5.1a1/reflex/components/radix/themes/components/progress.py
+-rw-r--r--   0        0        0     6676 2024-05-09 00:05:27.337586 reflex-0.5.1a1/reflex/components/radix/themes/components/progress.pyi
+-rw-r--r--   0        0        0      762 2024-04-26 18:47:21.878308 reflex-0.5.1a1/reflex/components/radix/themes/components/radio.py
+-rw-r--r--   0        0        0     5924 2024-04-26 18:47:21.878424 reflex-0.5.1a1/reflex/components/radix/themes/components/radio.pyi
+-rw-r--r--   0        0        0     1250 2024-04-26 18:47:21.878499 reflex-0.5.1a1/reflex/components/radix/themes/components/radio_cards.py
+-rw-r--r--   0        0        0     9561 2024-04-26 18:47:21.878615 reflex-0.5.1a1/reflex/components/radix/themes/components/radio_cards.pyi
+-rw-r--r--   0        0        0     6233 2024-04-24 21:16:40.838796 reflex-0.5.1a1/reflex/components/radix/themes/components/radio_group.py
+-rw-r--r--   0        0        0    24106 2024-04-24 19:32:02.212695 reflex-0.5.1a1/reflex/components/radix/themes/components/radio_group.pyi
+-rw-r--r--   0        0        0      920 2024-03-20 23:54:55.855386 reflex-0.5.1a1/reflex/components/radix/themes/components/scroll_area.py
+-rw-r--r--   0        0        0     4427 2024-04-24 19:31:54.699499 reflex-0.5.1a1/reflex/components/radix/themes/components/scroll_area.pyi
+-rw-r--r--   0        0        0     1292 2024-04-26 18:47:21.878708 reflex-0.5.1a1/reflex/components/radix/themes/components/segmented_control.py
+-rw-r--r--   0        0        0     9507 2024-04-26 18:47:21.878829 reflex-0.5.1a1/reflex/components/radix/themes/components/segmented_control.pyi
+-rw-r--r--   0        0        0     8028 2024-04-05 17:14:14.462095 reflex-0.5.1a1/reflex/components/radix/themes/components/select.py
+-rw-r--r--   0        0        0    45123 2024-04-24 19:32:01.973018 reflex-0.5.1a1/reflex/components/radix/themes/components/select.pyi
+-rw-r--r--   0        0        0      868 2024-03-20 23:54:55.856979 reflex-0.5.1a1/reflex/components/radix/themes/components/separator.py
+-rw-r--r--   0        0        0     6078 2024-04-24 19:32:00.501335 reflex-0.5.1a1/reflex/components/radix/themes/components/separator.pyi
+-rw-r--r--   0        0        0      643 2024-04-26 18:47:21.878906 reflex-0.5.1a1/reflex/components/radix/themes/components/skeleton.py
+-rw-r--r--   0        0        0     4289 2024-04-26 18:47:21.879004 reflex-0.5.1a1/reflex/components/radix/themes/components/skeleton.pyi
+-rw-r--r--   0        0        0     3234 2024-03-20 23:54:55.857144 reflex-0.5.1a1/reflex/components/radix/themes/components/slider.py
+-rw-r--r--   0        0        0     8162 2024-04-24 19:31:52.441948 reflex-0.5.1a1/reflex/components/radix/themes/components/slider.pyi
+-rw-r--r--   0        0        0      431 2024-04-26 18:47:21.879090 reflex-0.5.1a1/reflex/components/radix/themes/components/spinner.py
+-rw-r--r--   0        0        0     3845 2024-04-26 18:47:21.879165 reflex-0.5.1a1/reflex/components/radix/themes/components/spinner.pyi
+-rw-r--r--   0        0        0     1976 2024-02-17 20:02:02.440152 reflex-0.5.1a1/reflex/components/radix/themes/components/switch.py
+-rw-r--r--   0        0        0     7404 2024-04-24 19:31:46.185370 reflex-0.5.1a1/reflex/components/radix/themes/components/switch.pyi
+-rw-r--r--   0        0        0     3111 2024-03-20 23:54:55.857388 reflex-0.5.1a1/reflex/components/radix/themes/components/table.py
+-rw-r--r--   0        0        0    47387 2024-04-24 19:32:03.411460 reflex-0.5.1a1/reflex/components/radix/themes/components/table.pyi
+-rw-r--r--   0        0        0     2985 2024-05-17 15:27:52.902376 reflex-0.5.1a1/reflex/components/radix/themes/components/tabs.py
+-rw-r--r--   0        0        0    19119 2024-05-07 15:33:05.685968 reflex-0.5.1a1/reflex/components/radix/themes/components/tabs.pyi
+-rw-r--r--   0        0        0     3233 2024-02-17 20:02:02.441460 reflex-0.5.1a1/reflex/components/radix/themes/components/text_area.py
+-rw-r--r--   0        0        0    11711 2024-04-24 19:31:45.665204 reflex-0.5.1a1/reflex/components/radix/themes/components/text_area.pyi
+-rw-r--r--   0        0        0     6527 2024-05-09 00:05:27.337867 reflex-0.5.1a1/reflex/components/radix/themes/components/text_field.py
+-rw-r--r--   0        0        0    26637 2024-05-09 00:05:27.338008 reflex-0.5.1a1/reflex/components/radix/themes/components/text_field.pyi
+-rw-r--r--   0        0        0     4465 2024-02-17 20:02:02.442324 reflex-0.5.1a1/reflex/components/radix/themes/components/tooltip.py
+-rw-r--r--   0        0        0     8092 2024-04-24 19:31:32.491941 reflex-0.5.1a1/reflex/components/radix/themes/components/tooltip.pyi
+-rw-r--r--   0        0        0      811 2024-04-04 14:19:59.340548 reflex-0.5.1a1/reflex/components/radix/themes/layout/__init__.py
+-rw-r--r--   0        0        0     1211 2024-04-26 18:47:21.880131 reflex-0.5.1a1/reflex/components/radix/themes/layout/base.py
+-rw-r--r--   0        0        0     7663 2024-04-26 18:47:21.880279 reflex-0.5.1a1/reflex/components/radix/themes/layout/base.pyi
+-rw-r--r--   0        0        0      281 2024-02-07 21:48:43.318485 reflex-0.5.1a1/reflex/components/radix/themes/layout/box.py
+-rw-r--r--   0        0        0     6462 2024-04-24 19:31:52.197501 reflex-0.5.1a1/reflex/components/radix/themes/layout/box.pyi
+-rw-r--r--   0        0        0      509 2024-05-07 15:33:05.686074 reflex-0.5.1a1/reflex/components/radix/themes/layout/center.py
+-rw-r--r--   0        0        0     8271 2024-05-07 15:33:05.686180 reflex-0.5.1a1/reflex/components/radix/themes/layout/center.pyi
+-rw-r--r--   0        0        0     1405 2024-05-05 01:15:24.057627 reflex-0.5.1a1/reflex/components/radix/themes/layout/container.py
+-rw-r--r--   0        0        0     5247 2024-05-05 01:15:24.057873 reflex-0.5.1a1/reflex/components/radix/themes/layout/container.pyi
+-rw-r--r--   0        0        0     1374 2024-03-20 23:54:55.859776 reflex-0.5.1a1/reflex/components/radix/themes/layout/flex.py
+-rw-r--r--   0        0        0     8501 2024-04-24 19:31:47.609497 reflex-0.5.1a1/reflex/components/radix/themes/layout/flex.pyi
+-rw-r--r--   0        0        0     1498 2024-03-20 23:54:55.860131 reflex-0.5.1a1/reflex/components/radix/themes/layout/grid.py
+-rw-r--r--   0        0        0     8907 2024-04-24 19:31:44.336304 reflex-0.5.1a1/reflex/components/radix/themes/layout/grid.pyi
+-rw-r--r--   0        0        0     4991 2024-05-07 15:33:05.686298 reflex-0.5.1a1/reflex/components/radix/themes/layout/list.py
+-rw-r--r--   0        0        0    28927 2024-05-07 15:33:05.686398 reflex-0.5.1a1/reflex/components/radix/themes/layout/list.pyi
+-rw-r--r--   0        0        0      458 2024-02-07 21:48:43.320250 reflex-0.5.1a1/reflex/components/radix/themes/layout/section.py
+-rw-r--r--   0        0        0     6758 2024-04-24 19:31:48.032806 reflex-0.5.1a1/reflex/components/radix/themes/layout/section.pyi
+-rw-r--r--   0        0        0      492 2024-05-07 15:33:05.686501 reflex-0.5.1a1/reflex/components/radix/themes/layout/spacer.py
+-rw-r--r--   0        0        0     8271 2024-05-07 15:33:05.686608 reflex-0.5.1a1/reflex/components/radix/themes/layout/spacer.pyi
+-rw-r--r--   0        0        0     1522 2024-05-05 01:15:24.058360 reflex-0.5.1a1/reflex/components/radix/themes/layout/stack.py
+-rw-r--r--   0        0        0    22132 2024-05-05 01:15:24.058618 reflex-0.5.1a1/reflex/components/radix/themes/layout/stack.pyi
+-rw-r--r--   0        0        0      343 2024-02-17 20:02:02.446123 reflex-0.5.1a1/reflex/components/radix/themes/typography/__init__.py
+-rw-r--r--   0        0        0      408 2024-01-08 22:19:50.686081 reflex-0.5.1a1/reflex/components/radix/themes/typography/base.py
+-rw-r--r--   0        0        0      799 2024-02-07 21:48:43.321231 reflex-0.5.1a1/reflex/components/radix/themes/typography/blockquote.py
+-rw-r--r--   0        0        0     9316 2024-04-24 19:31:18.815043 reflex-0.5.1a1/reflex/components/radix/themes/typography/blockquote.pyi
+-rw-r--r--   0        0        0      909 2024-02-07 21:48:43.321463 reflex-0.5.1a1/reflex/components/radix/themes/typography/code.py
+-rw-r--r--   0        0        0     9513 2024-04-24 19:31:42.716182 reflex-0.5.1a1/reflex/components/radix/themes/typography/code.pyi
+-rw-r--r--   0        0        0     1324 2024-02-07 21:48:43.322172 reflex-0.5.1a1/reflex/components/radix/themes/typography/heading.py
+-rw-r--r--   0        0        0    10106 2024-04-24 19:31:48.004994 reflex-0.5.1a1/reflex/components/radix/themes/typography/heading.pyi
+-rw-r--r--   0        0        0     3291 2024-05-05 01:15:24.058911 reflex-0.5.1a1/reflex/components/radix/themes/typography/link.py
+-rw-r--r--   0        0        0    12144 2024-05-05 01:15:24.059174 reflex-0.5.1a1/reflex/components/radix/themes/typography/link.pyi
+-rw-r--r--   0        0        0     2604 2024-03-20 23:54:55.863112 reflex-0.5.1a1/reflex/components/radix/themes/typography/text.py
+-rw-r--r--   0        0        0    57238 2024-04-24 19:32:03.568126 reflex-0.5.1a1/reflex/components/radix/themes/typography/text.pyi
+-rw-r--r--   0        0        0      144 2024-02-06 00:51:32.026767 reflex-0.5.1a1/reflex/components/react_player/__init__.py
+-rw-r--r--   0        0        0      185 2024-02-06 00:51:32.026827 reflex-0.5.1a1/reflex/components/react_player/audio.py
+-rw-r--r--   0        0        0     4327 2024-04-24 19:31:20.559612 reflex-0.5.1a1/reflex/components/react_player/audio.pyi
+-rw-r--r--   0        0        0     1087 2024-02-06 00:51:32.027069 reflex-0.5.1a1/reflex/components/react_player/react_player.py
+-rw-r--r--   0        0        0     4354 2024-04-24 19:31:40.833679 reflex-0.5.1a1/reflex/components/react_player/react_player.pyi
+-rw-r--r--   0        0        0      185 2024-02-06 00:51:32.027295 reflex-0.5.1a1/reflex/components/react_player/video.py
+-rw-r--r--   0        0        0     4327 2024-04-24 19:31:23.657166 reflex-0.5.1a1/reflex/components/react_player/video.pyi
+-rw-r--r--   0        0        0     2373 2024-02-06 00:51:32.027723 reflex-0.5.1a1/reflex/components/recharts/__init__.py
+-rw-r--r--   0        0        0    19595 2024-02-06 00:51:32.027828 reflex-0.5.1a1/reflex/components/recharts/cartesian.py
+-rw-r--r--   0        0        0    84151 2024-04-24 19:32:04.125732 reflex-0.5.1a1/reflex/components/recharts/cartesian.pyi
+-rw-r--r--   0        0        0    18493 2024-02-06 00:51:32.028086 reflex-0.5.1a1/reflex/components/recharts/charts.py
+-rw-r--r--   0        0        0    48757 2024-04-24 19:32:04.230664 reflex-0.5.1a1/reflex/components/recharts/charts.pyi
+-rw-r--r--   0        0        0     5624 2024-04-25 02:07:40.442483 reflex-0.5.1a1/reflex/components/recharts/general.py
+-rw-r--r--   0        0        0    22787 2024-04-24 19:31:57.383382 reflex-0.5.1a1/reflex/components/recharts/general.pyi
+-rw-r--r--   0        0        0    10410 2024-02-06 00:51:32.028623 reflex-0.5.1a1/reflex/components/recharts/polar.py
+-rw-r--r--   0        0        0    24326 2024-04-24 19:32:02.075893 reflex-0.5.1a1/reflex/components/recharts/polar.pyi
+-rw-r--r--   0        0        0     2870 2024-02-06 00:51:32.028787 reflex-0.5.1a1/reflex/components/recharts/recharts.py
+-rw-r--r--   0        0        0     8535 2024-04-24 19:31:59.348537 reflex-0.5.1a1/reflex/components/recharts/recharts.pyi
+-rw-r--r--   0        0        0       68 2024-05-05 01:15:24.059268 reflex-0.5.1a1/reflex/components/sonner/__init__.py
+-rw-r--r--   0        0        0     9822 2024-05-17 15:27:52.902701 reflex-0.5.1a1/reflex/components/sonner/toast.py
+-rw-r--r--   0        0        0     8164 2024-05-17 15:27:52.902804 reflex-0.5.1a1/reflex/components/sonner/toast.pyi
+-rw-r--r--   0        0        0      109 2024-02-06 00:51:32.028942 reflex-0.5.1a1/reflex/components/suneditor/__init__.py
+-rw-r--r--   0        0        0     7360 2024-02-06 00:51:32.029131 reflex-0.5.1a1/reflex/components/suneditor/editor.py
+-rw-r--r--   0        0        0    10330 2024-04-24 19:32:02.124688 reflex-0.5.1a1/reflex/components/suneditor/editor.pyi
+-rw-r--r--   0        0        0      152 2024-02-06 00:51:32.029339 reflex-0.5.1a1/reflex/components/tags/__init__.py
+-rw-r--r--   0        0        0      447 2023-07-20 22:42:41.717618 reflex-0.5.1a1/reflex/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     3927 2024-05-09 06:53:37.971823 reflex-0.5.1a1/reflex/components/tags/iter_tag.py
+-rw-r--r--   0        0        0      387 2024-02-06 00:51:32.029522 reflex-0.5.1a1/reflex/components/tags/match_tag.py
+-rw-r--r--   0        0        0     2778 2024-03-20 23:54:55.863973 reflex-0.5.1a1/reflex/components/tags/tag.py
+-rw-r--r--   0        0        0      587 2023-07-20 22:42:41.717805 reflex-0.5.1a1/reflex/components/tags/tagless.py
+-rw-r--r--   0        0        0    10772 2024-05-17 15:27:52.903057 reflex-0.5.1a1/reflex/config.py
+-rw-r--r--   0        0        0     3318 2024-04-05 17:14:06.329003 reflex-0.5.1a1/reflex/config.pyi
+-rw-r--r--   0        0        0     2036 2024-05-07 15:33:05.687073 reflex-0.5.1a1/reflex/constants/__init__.py
+-rw-r--r--   0        0        0     5640 2024-05-07 15:33:05.687194 reflex-0.5.1a1/reflex/constants/base.py
+-rw-r--r--   0        0        0     2980 2024-04-24 19:34:30.973419 reflex-0.5.1a1/reflex/constants/base.pyi
+-rw-r--r--   0        0        0     1625 2024-05-07 15:33:05.687387 reflex-0.5.1a1/reflex/constants/colors.py
+-rw-r--r--   0        0        0     4207 2024-05-17 15:27:52.903463 reflex-0.5.1a1/reflex/constants/compiler.py
+-rw-r--r--   0        0        0     1331 2024-01-08 22:19:50.692361 reflex-0.5.1a1/reflex/constants/config.py
+-rw-r--r--   0        0        0     1268 2024-03-20 23:54:55.865280 reflex-0.5.1a1/reflex/constants/custom_components.py
+-rw-r--r--   0        0        0     2668 2024-03-20 00:01:07.211135 reflex-0.5.1a1/reflex/constants/event.py
+-rw-r--r--   0        0        0     3419 2024-05-17 15:27:52.903553 reflex-0.5.1a1/reflex/constants/installer.py
+-rw-r--r--   0        0        0     2144 2024-05-05 01:15:24.059871 reflex-0.5.1a1/reflex/constants/route.py
+-rw-r--r--   0        0        0      636 2024-02-06 00:51:32.030238 reflex-0.5.1a1/reflex/constants/style.py
+-rw-r--r--   0        0        0       36 2024-03-20 23:54:55.865552 reflex-0.5.1a1/reflex/custom_components/__init__.py
+-rw-r--r--   0        0        0    32298 2024-05-17 15:27:52.903711 reflex-0.5.1a1/reflex/custom_components/custom_components.py
+-rw-r--r--   0        0        0    28047 2024-05-17 15:27:52.903847 reflex-0.5.1a1/reflex/event.py
+-rw-r--r--   0        0        0      778 2024-05-17 15:27:52.903951 reflex-0.5.1a1/reflex/experimental/__init__.py
+-rw-r--r--   0        0        0     6597 2024-05-17 15:27:52.904025 reflex-0.5.1a1/reflex/experimental/client_state.py
+-rw-r--r--   0        0        0     2196 2024-04-24 21:16:40.840090 reflex-0.5.1a1/reflex/experimental/hooks.py
+-rw-r--r--   0        0        0     7234 2024-05-07 15:33:05.687514 reflex-0.5.1a1/reflex/experimental/layout.py
+-rw-r--r--   0        0        0      281 2024-04-12 01:14:12.278217 reflex-0.5.1a1/reflex/experimental/misc.py
+-rw-r--r--   0        0        0      111 2023-07-20 22:42:41.719277 reflex-0.5.1a1/reflex/middleware/__init__.py
+-rw-r--r--   0        0        0     1484 2024-03-28 17:56:29.082526 reflex-0.5.1a1/reflex/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1169 2023-12-01 04:51:31.116521 reflex-0.5.1a1/reflex/middleware/middleware.py
+-rw-r--r--   0        0        0    13227 2024-05-09 00:05:27.338971 reflex-0.5.1a1/reflex/model.py
+-rw-r--r--   0        0        0     2077 2024-04-24 21:16:40.840737 reflex-0.5.1a1/reflex/page.py
+-rw-r--r--   0        0        0    17826 2024-05-05 01:15:24.060260 reflex-0.5.1a1/reflex/reflex.py
+-rw-r--r--   0        0        0     4198 2024-05-05 01:15:24.060365 reflex-0.5.1a1/reflex/route.py
+-rw-r--r--   0        0        0   107161 2024-05-17 15:27:52.904231 reflex-0.5.1a1/reflex/state.py
+-rw-r--r--   0        0        0     9389 2024-05-17 15:27:52.904359 reflex-0.5.1a1/reflex/style.py
+-rw-r--r--   0        0        0    31461 2024-05-17 15:27:52.904579 reflex-0.5.1a1/reflex/testing.py
+-rw-r--r--   0        0        0       24 2023-11-09 03:24:59.510665 reflex-0.5.1a1/reflex/utils/__init__.py
+-rw-r--r--   0        0        0     8573 2024-02-06 00:51:32.031946 reflex-0.5.1a1/reflex/utils/build.py
+-rw-r--r--   0        0        0     1255 2024-04-12 01:14:12.279414 reflex-0.5.1a1/reflex/utils/compat.py
+-rw-r--r--   0        0        0     5182 2024-04-24 21:16:40.841356 reflex-0.5.1a1/reflex/utils/console.py
+-rw-r--r--   0        0        0     2163 2024-05-17 15:27:52.904769 reflex-0.5.1a1/reflex/utils/exceptions.py
+-rw-r--r--   0        0        0    10406 2024-05-07 15:33:05.688300 reflex-0.5.1a1/reflex/utils/exec.py
+-rw-r--r--   0        0        0     2270 2024-04-12 01:14:12.279905 reflex-0.5.1a1/reflex/utils/export.py
+-rw-r--r--   0        0        0    25149 2024-05-17 15:27:52.905126 reflex-0.5.1a1/reflex/utils/format.py
+-rw-r--r--   0        0        0     2309 2024-04-24 21:16:40.841612 reflex-0.5.1a1/reflex/utils/imports.py
+-rw-r--r--   0        0        0     4737 2024-02-06 00:51:32.033457 reflex-0.5.1a1/reflex/utils/path_ops.py
+-rw-r--r--   0        0        0    52920 2024-05-17 15:27:52.905328 reflex-0.5.1a1/reflex/utils/prerequisites.py
+-rw-r--r--   0        0        0    11972 2024-05-17 15:27:52.905465 reflex-0.5.1a1/reflex/utils/processes.py
+-rw-r--r--   0        0        0    30637 2024-05-05 01:15:24.061383 reflex-0.5.1a1/reflex/utils/pyi_generator.py
+-rw-r--r--   0        0        0     9037 2024-04-24 21:16:40.842319 reflex-0.5.1a1/reflex/utils/serializers.py
+-rw-r--r--   0        0        0     4735 2024-05-17 15:27:52.905576 reflex-0.5.1a1/reflex/utils/telemetry.py
+-rw-r--r--   0        0        0    15152 2024-05-17 15:27:52.905672 reflex-0.5.1a1/reflex/utils/types.py
+-rw-r--r--   0        0        0     2609 2023-10-22 18:57:13.223189 reflex-0.5.1a1/reflex/utils/watch.py
+-rw-r--r--   0        0        0    69074 2024-05-17 15:27:52.905875 reflex-0.5.1a1/reflex/vars.py
+-rw-r--r--   0        0        0     5753 2024-05-17 15:27:52.906104 reflex-0.5.1a1/reflex/vars.pyi
+-rw-r--r--   0        0        0    12089 1970-01-01 00:00:00.000000 reflex-0.5.1a1/PKG-INFO
```

### Comparing `reflex-0.5.0a3/LICENSE` & `reflex-0.5.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/README.md` & `reflex-0.5.1a1/README.md`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/pyproject.toml` & `reflex-0.5.1a1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reflex"
-version = "0.5.0a3"
+version = "0.5.1a1"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@reflex.dev>",
     "Alek Petuskey <alek@reflex.dev>",
     "Masen Furer <masen@reflex.dev>",
     "Elijah Ahianyo <elijah@reflex.dev>",
```

### Comparing `reflex-0.5.0a3/reflex/.templates/apps/blank/assets/favicon.ico` & `reflex-0.5.1a1/reflex/.templates/apps/blank/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/apps/blank/code/blank.py` & `reflex-0.5.1a1/reflex/.templates/apps/blank/code/blank.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/apps/demo/assets/favicon.ico` & `reflex-0.5.1a1/reflex/.templates/apps/demo/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/apps/demo/assets/github.svg` & `reflex-0.5.1a1/reflex/.templates/apps/demo/assets/github.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/apps/demo/assets/icon.svg` & `reflex-0.5.1a1/reflex/.templates/apps/demo/assets/icon.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/apps/demo/assets/logo.svg` & `reflex-0.5.1a1/reflex/.templates/apps/demo/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/apps/demo/assets/paneleft.svg` & `reflex-0.5.1a1/reflex/.templates/apps/demo/assets/paneleft.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/apps/demo/code/demo.py` & `reflex-0.5.1a1/reflex/.templates/apps/demo/code/demo.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/apps/demo/code/pages/chatapp.py` & `reflex-0.5.1a1/reflex/.templates/apps/demo/code/pages/chatapp.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/apps/demo/code/pages/datatable.py` & `reflex-0.5.1a1/reflex/.templates/apps/demo/code/pages/datatable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/apps/demo/code/pages/forms.py` & `reflex-0.5.1a1/reflex/.templates/apps/demo/code/pages/forms.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/apps/demo/code/pages/graphing.py` & `reflex-0.5.1a1/reflex/.templates/apps/demo/code/pages/graphing.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/apps/demo/code/pages/home.py` & `reflex-0.5.1a1/reflex/.templates/apps/demo/code/pages/home.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/apps/demo/code/sidebar.py` & `reflex-0.5.1a1/reflex/.templates/apps/demo/code/sidebar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/apps/demo/code/states/form_state.py` & `reflex-0.5.1a1/reflex/.templates/apps/demo/code/states/form_state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/apps/demo/code/states/pie_state.py` & `reflex-0.5.1a1/reflex/.templates/apps/demo/code/states/pie_state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/apps/demo/code/styles.py` & `reflex-0.5.1a1/reflex/.templates/apps/demo/code/styles.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/apps/demo/code/webui/components/chat.py` & `reflex-0.5.1a1/reflex/.templates/apps/demo/code/webui/components/chat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/apps/demo/code/webui/components/loading_icon.py` & `reflex-0.5.1a1/reflex/.templates/apps/demo/code/webui/components/loading_icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/apps/demo/code/webui/components/modal.py` & `reflex-0.5.1a1/reflex/.templates/apps/demo/code/webui/components/modal.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/apps/demo/code/webui/components/navbar.py` & `reflex-0.5.1a1/reflex/.templates/apps/demo/code/webui/components/navbar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/apps/demo/code/webui/components/sidebar.py` & `reflex-0.5.1a1/reflex/.templates/apps/demo/code/webui/components/sidebar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/apps/demo/code/webui/state.py` & `reflex-0.5.1a1/reflex/.templates/apps/demo/code/webui/state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/apps/demo/code/webui/styles.py` & `reflex-0.5.1a1/reflex/.templates/apps/demo/code/webui/styles.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/jinja/custom_components/demo_app.py.jinja2` & `reflex-0.5.1a1/reflex/.templates/jinja/custom_components/demo_app.py.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2` & `reflex-0.5.1a1/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/jinja/custom_components/src.py.jinja2` & `reflex-0.5.1a1/reflex/.templates/jinja/custom_components/src.py.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/jinja/web/package.json.jinja2` & `reflex-0.5.1a1/reflex/.templates/jinja/web/package.json.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/jinja/web/pages/_app.js.jinja2` & `reflex-0.5.1a1/reflex/.templates/jinja/web/pages/_app.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/jinja/web/pages/custom_component.js.jinja2` & `reflex-0.5.1a1/reflex/.templates/jinja/web/pages/custom_component.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/jinja/web/pages/utils.js.jinja2` & `reflex-0.5.1a1/reflex/.templates/jinja/web/pages/utils.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/jinja/web/tailwind.config.js.jinja2` & `reflex-0.5.1a1/reflex/.templates/jinja/web/tailwind.config.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/jinja/web/utils/context.js.jinja2` & `reflex-0.5.1a1/reflex/.templates/jinja/web/utils/context.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js` & `reflex-0.5.1a1/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js` & `reflex-0.5.1a1/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/web/utils/client_side_routing.js` & `reflex-0.5.1a1/reflex/.templates/web/utils/client_side_routing.js`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/web/utils/helpers/dataeditor.js` & `reflex-0.5.1a1/reflex/.templates/web/utils/helpers/dataeditor.js`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/web/utils/helpers/debounce.js` & `reflex-0.5.1a1/reflex/.templates/web/utils/helpers/debounce.js`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/web/utils/helpers/range.js` & `reflex-0.5.1a1/reflex/.templates/web/utils/helpers/range.js`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/web/utils/helpers/throttle.js` & `reflex-0.5.1a1/reflex/.templates/web/utils/helpers/throttle.js`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/.templates/web/utils/state.js` & `reflex-0.5.1a1/reflex/.templates/web/utils/state.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -132,16 +132,21 @@
  * @param socket The socket object to send the event on.
  *
  * @returns True if the event was sent, false if it was handled locally.
  */
 export const applyEvent = async (event, socket) => {
     // Handle special events
     if (event.name == "_redirect") {
-        if (event.payload.external) window.open(event.payload.path, "_blank");
-        else Router.push(event.payload.path);
+        if (event.payload.external) {
+            window.open(event.payload.path, "_blank");
+        } else if (event.payload.replace) {
+            Router.replace(event.payload.path);
+        } else {
+            Router.push(event.payload.path);
+        }
         return false;
     }
 
     if (event.name == "_console") {
         console.log(event.payload.message);
         return false;
     }
```

### Comparing `reflex-0.5.0a3/reflex/__init__.py` & `reflex-0.5.1a1/reflex/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/__init__.pyi` & `reflex-0.5.1a1/reflex/__init__.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/app.py` & `reflex-0.5.1a1/reflex/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,22 +37,22 @@
 
 from reflex import constants
 from reflex.admin import AdminDash
 from reflex.base import Base
 from reflex.compiler import compiler
 from reflex.compiler import utils as compiler_utils
 from reflex.compiler.compiler import ExecutorSafeFunctions
-from reflex.components import connection_modal, connection_pulser
 from reflex.components.base.app_wrap import AppWrap
 from reflex.components.base.fragment import Fragment
 from reflex.components.component import (
     Component,
     ComponentStyle,
     evaluate_style_namespaces,
 )
+from reflex.components.core import connection_pulser, connection_toaster
 from reflex.components.core.client_side_routing import (
     Default404Page,
     wait_for_client_redirect,
 )
 from reflex.components.core.upload import Upload, get_upload_dir
 from reflex.components.radix import themes
 from reflex.config import get_config
@@ -87,15 +87,15 @@
 
 def default_overlay_component() -> Component:
     """Default overlay_component attribute for App.
 
     Returns:
         The default overlay_component, which is a connection_modal.
     """
-    return Fragment.create(connection_pulser(), connection_modal())
+    return Fragment.create(connection_pulser(), connection_toaster())
 
 
 class OverlayFragment(Fragment):
     """Alias for Fragment, used to wrap the overlay_component."""
 
     pass
 
@@ -399,25 +399,28 @@
         Args:
             component: The component function to call or Component to return as-is.
 
         Returns:
             The generated component.
 
         Raises:
+            VarOperationTypeError: When an invalid component var related function is passed.
             TypeError: When an invalid component function is passed.
             exceptions.MatchTypeError: If the return types of match cases in rx.match are different.
         """
+        from reflex.utils.exceptions import VarOperationTypeError
+
         try:
             return component if isinstance(component, Component) else component()
         except exceptions.MatchTypeError:
             raise
         except TypeError as e:
             message = str(e)
             if "BaseVar" in message or "ComputedVar" in message:
-                raise TypeError(
+                raise VarOperationTypeError(
                     "You may be trying to use an invalid Python function on a state var. "
                     "When referencing a var inside your render code, only limited var operations are supported. "
                     "See the var operation docs here: https://reflex.dev/docs/vars/var-operations/"
                 ) from e
             raise e
 
     def add_page(
@@ -551,19 +554,21 @@
 
     def _check_routes_conflict(self, new_route: str):
         """Verify if there is any conflict between the new route and any existing route.
 
         Based on conflicts that NextJS would throw if not intercepted.
 
         Raises:
-            ValueError: exception showing which conflict exist with the route to be added
+            RouteValueError: exception showing which conflict exist with the route to be added
 
         Args:
             new_route: the route being newly added.
         """
+        from reflex.utils.exceptions import RouteValueError
+
         if "[" not in new_route:
             return
 
         segments = (
             constants.RouteRegex.SINGLE_SEGMENT,
             constants.RouteRegex.DOUBLE_SEGMENT,
             constants.RouteRegex.SINGLE_CATCHALL_SEGMENT,
@@ -572,15 +577,15 @@
         for route in self.pages:
             replaced_route = replace_brackets_with_keywords(route)
             for rw, r, nr in zip(
                 replaced_route.split("/"), route.split("/"), new_route.split("/")
             ):
                 if rw in segments and r != nr:
                     # If the slugs in the segments of both routes are not the same, then the route is invalid
-                    raise ValueError(
+                    raise RouteValueError(
                         f"You cannot use different slug names for the same dynamic path in  {route} and {new_route} ('{r}' != '{nr}')"
                     )
                 elif rw not in segments and r != nr:
                     # if the section being compared in both routes is not a dynamic segment(i.e not wrapped in brackets)
                     # then we are guaranteed that the route is valid and there's no need checking the rest.
                     # eg. /posts/[id]/info/[slug1] and /posts/[id]/info1/[slug1] is always going to be valid since
                     # info1 will break away into its own tree.
@@ -751,16 +756,18 @@
     def _compile(self, export: bool = False):
         """Compile the app and output it to the pages folder.
 
         Args:
             export: Whether to compile the app for export.
 
         Raises:
-            RuntimeError: When any page uses state, but no rx.State subclass is defined.
+            ReflexRuntimeError: When any page uses state, but no rx.State subclass is defined.
         """
+        from reflex.utils.exceptions import ReflexRuntimeError
+
         # Render a default 404 page if the user didn't supply one
         if constants.Page404.SLUG not in self.pages:
             self.add_custom_404_page()
 
         # Add the optional endpoints (_upload)
         self._add_optional_endpoints()
 
@@ -833,15 +840,15 @@
             page_components,
         ) = compiler.compile_stateful_components(self.pages.values())
 
         progress.advance(task)
 
         # Catch "static" apps (that do not define a rx.State subclass) which are trying to access rx.State.
         if code_uses_state_contexts(stateful_components_code) and self.state is None:
-            raise RuntimeError(
+            raise ReflexRuntimeError(
                 "To access rx.State in frontend components, at least one "
                 "subclass of rx.State must be defined in the app."
             )
         compile_results.append((stateful_components_path, stateful_components_code))
 
         # Compile the root document before fork.
         compile_results.append(
@@ -1056,59 +1063,69 @@
     Args:
         app: The app to process the event for.
         event: The event to process.
         sid: The Socket.IO session id.
         headers: The client headers.
         client_ip: The client_ip.
 
+    Raises:
+        ReflexError: If a reflex specific error occurs during processing the event.
+
     Yields:
         The state updates after processing the event.
     """
-    # Add request data to the state.
-    router_data = event.router_data
-    router_data.update(
-        {
-            constants.RouteVar.QUERY: format.format_query_params(event.router_data),
-            constants.RouteVar.CLIENT_TOKEN: event.token,
-            constants.RouteVar.SESSION_ID: sid,
-            constants.RouteVar.HEADERS: headers,
-            constants.RouteVar.CLIENT_IP: client_ip,
-        }
-    )
-    # Get the state for the session exclusively.
-    async with app.state_manager.modify_state(event.substate_token) as state:
-        # re-assign only when the value is different
-        if state.router_data != router_data:
-            # assignment will recurse into substates and force recalculation of
-            # dependent ComputedVar (dynamic route variables)
-            state.router_data = router_data
-            state.router = RouterData(router_data)
-
-        # Preprocess the event.
-        update = await app._preprocess(state, event)
-
-        # If there was an update, yield it.
-        if update is not None:
-            yield update
+    from reflex.utils import telemetry
+    from reflex.utils.exceptions import ReflexError
 
-        # Only process the event if there is no update.
-        else:
-            if app._process_background(state, event) is not None:
-                # `final=True` allows the frontend send more events immediately.
-                yield StateUpdate(final=True)
-                return
+    try:
+        # Add request data to the state.
+        router_data = event.router_data
+        router_data.update(
+            {
+                constants.RouteVar.QUERY: format.format_query_params(event.router_data),
+                constants.RouteVar.CLIENT_TOKEN: event.token,
+                constants.RouteVar.SESSION_ID: sid,
+                constants.RouteVar.HEADERS: headers,
+                constants.RouteVar.CLIENT_IP: client_ip,
+            }
+        )
+        # Get the state for the session exclusively.
+        async with app.state_manager.modify_state(event.substate_token) as state:
+            # re-assign only when the value is different
+            if state.router_data != router_data:
+                # assignment will recurse into substates and force recalculation of
+                # dependent ComputedVar (dynamic route variables)
+                state.router_data = router_data
+                state.router = RouterData(router_data)
 
-            # Process the event synchronously.
-            async for update in state._process(event):
-                # Postprocess the event.
-                update = await app._postprocess(state, event, update)
+            # Preprocess the event.
+            update = await app._preprocess(state, event)
 
-                # Yield the update.
+            # If there was an update, yield it.
+            if update is not None:
                 yield update
 
+            # Only process the event if there is no update.
+            else:
+                if app._process_background(state, event) is not None:
+                    # `final=True` allows the frontend send more events immediately.
+                    yield StateUpdate(final=True)
+                    return
+
+                # Process the event synchronously.
+                async for update in state._process(event):
+                    # Postprocess the event.
+                    update = await app._postprocess(state, event, update)
+
+                    # Yield the update.
+                    yield update
+    except ReflexError as ex:
+        telemetry.send("error", context="backend", detail=str(ex))
+        raise
+
 
 async def ping() -> str:
     """Test API endpoint.
 
     Returns:
         The response.
     """
@@ -1133,18 +1150,20 @@
             files: The file(s) to upload.
 
         Returns:
             StreamingResponse yielding newline-delimited JSON of StateUpdate
             emitted by the upload handler.
 
         Raises:
-            ValueError: if there are no args with supported annotation.
-            TypeError: if a background task is used as the handler.
+            UploadValueError: if there are no args with supported annotation.
+            UploadTypeError: if a background task is used as the handler.
             HTTPException: when the request does not include token / handler headers.
         """
+        from reflex.utils.exceptions import UploadTypeError, UploadValueError
+
         token = request.headers.get("reflex-client-token")
         handler = request.headers.get("reflex-event-handler")
 
         if not token or not handler:
             raise HTTPException(
                 status_code=400,
                 detail="Missing reflex-client-token or reflex-event-handler header.",
@@ -1162,30 +1181,30 @@
 
         # get handler function
         func = getattr(type(current_state), handler.split(".")[-1])
 
         # check if there exists any handler args with annotation, List[UploadFile]
         if isinstance(func, EventHandler):
             if func.is_background:
-                raise TypeError(
+                raise UploadTypeError(
                     f"@rx.background is not supported for upload handler `{handler}`.",
                 )
             func = func.fn
         if isinstance(func, functools.partial):
             func = func.func
         for k, v in get_type_hints(func).items():
             if types.is_generic_alias(v) and types._issubclass(
                 get_args(v)[0],
                 UploadFile,
             ):
                 handler_upload_param = (k, v)
                 break
 
         if not handler_upload_param:
-            raise ValueError(
+            raise UploadValueError(
                 f"`{handler}` handler should have a parameter annotated as "
                 "List[rx.UploadFile]"
             )
 
         # Make a copy of the files as they are closed after the request.
         # This behaviour changed from fastapi 0.103.0 to 0.103.1 as the
         # AsyncExitStack was removed from the request scope and is now
```

### Comparing `reflex-0.5.0a3/reflex/app_module_for_backend.py` & `reflex-0.5.1a1/reflex/app_module_for_backend.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/base.py` & `reflex-0.5.1a1/reflex/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define the base Reflex class."""
+
 from __future__ import annotations
 
 import os
 from typing import TYPE_CHECKING, Any, List, Type
 
 try:
     import pydantic.v1 as pydantic
@@ -22,23 +23,25 @@
     """Ensure that the field's name does not shadow an existing attribute of the model.
 
     Args:
         bases: List of base models to check for shadowed attrs.
         field_name: name of attribute
 
     Raises:
-        NameError: If state var field shadows another in its parent state
+        VarNameError: If state var field shadows another in its parent state
     """
+    from reflex.utils.exceptions import VarNameError
+
     reload = os.getenv(constants.RELOAD_CONFIG) == "True"
     for base in bases:
         try:
             if not reload and getattr(base, field_name, None):
                 pass
         except TypeError as te:
-            raise NameError(
+            raise VarNameError(
                 f'State var "{field_name}" in {base} has been shadowed by a substate var; '
                 f'use a different field name instead".'
             ) from te
 
 
 # monkeypatch pydantic validate_field_name method to skip validating
 # shadowed state vars when reloading app via utils.prerequisites.get_app(reload=True)
```

### Comparing `reflex-0.5.0a3/reflex/compiler/compiler.py` & `reflex-0.5.1a1/reflex/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/compiler/templates.py` & `reflex-0.5.1a1/reflex/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/compiler/utils.py` & `reflex-0.5.1a1/reflex/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/__init__.py` & `reflex-0.5.1a1/reflex/components/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/base/app_wrap.py` & `reflex-0.5.1a1/reflex/components/base/app_wrap.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/base/app_wrap.pyi` & `reflex-0.5.1a1/reflex/components/base/app_wrap.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/base/bare.py` & `reflex-0.5.1a1/reflex/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/base/body.pyi` & `reflex-0.5.1a1/reflex/components/base/body.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/base/document.py` & `reflex-0.5.1a1/reflex/components/base/document.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/base/document.pyi` & `reflex-0.5.1a1/reflex/components/base/document.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/base/fragment.pyi` & `reflex-0.5.1a1/reflex/components/base/fragment.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/base/head.pyi` & `reflex-0.5.1a1/reflex/components/base/head.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/base/link.py` & `reflex-0.5.1a1/reflex/components/base/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/base/link.pyi` & `reflex-0.5.1a1/reflex/components/base/link.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/base/meta.py` & `reflex-0.5.1a1/reflex/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/base/meta.pyi` & `reflex-0.5.1a1/reflex/components/base/meta.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/base/script.py` & `reflex-0.5.1a1/reflex/components/base/script.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/base/script.pyi` & `reflex-0.5.1a1/reflex/components/base/script.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/__init__.py` & `reflex-0.5.1a1/reflex/components/chakra/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/base.py` & `reflex-0.5.1a1/reflex/components/chakra/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/base.pyi` & `reflex-0.5.1a1/reflex/components/chakra/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/datadisplay/badge.pyi` & `reflex-0.5.1a1/reflex/components/chakra/datadisplay/badge.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/datadisplay/code.pyi` & `reflex-0.5.1a1/reflex/components/chakra/datadisplay/code.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/datadisplay/divider.py` & `reflex-0.5.1a1/reflex/components/chakra/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/datadisplay/divider.pyi` & `reflex-0.5.1a1/reflex/components/chakra/datadisplay/divider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/datadisplay/keyboard_key.pyi` & `reflex-0.5.1a1/reflex/components/chakra/datadisplay/keyboard_key.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/datadisplay/list.py` & `reflex-0.5.1a1/reflex/components/chakra/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/datadisplay/list.pyi` & `reflex-0.5.1a1/reflex/components/chakra/datadisplay/list.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/datadisplay/stat.py` & `reflex-0.5.1a1/reflex/components/chakra/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/datadisplay/stat.pyi` & `reflex-0.5.1a1/reflex/components/chakra/datadisplay/stat.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/datadisplay/table.py` & `reflex-0.5.1a1/reflex/components/chakra/datadisplay/table.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/datadisplay/table.pyi` & `reflex-0.5.1a1/reflex/components/chakra/datadisplay/table.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/datadisplay/tag.py` & `reflex-0.5.1a1/reflex/components/chakra/datadisplay/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/datadisplay/tag.pyi` & `reflex-0.5.1a1/reflex/components/chakra/datadisplay/tag.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/disclosure/accordion.py` & `reflex-0.5.1a1/reflex/components/chakra/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/disclosure/accordion.pyi` & `reflex-0.5.1a1/reflex/components/chakra/disclosure/accordion.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/disclosure/tabs.py` & `reflex-0.5.1a1/reflex/components/chakra/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/disclosure/tabs.pyi` & `reflex-0.5.1a1/reflex/components/chakra/disclosure/tabs.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/disclosure/transition.py` & `reflex-0.5.1a1/reflex/components/chakra/disclosure/transition.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/disclosure/transition.pyi` & `reflex-0.5.1a1/reflex/components/chakra/disclosure/transition.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/disclosure/visuallyhidden.pyi` & `reflex-0.5.1a1/reflex/components/chakra/disclosure/visuallyhidden.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/feedback/alert.py` & `reflex-0.5.1a1/reflex/components/chakra/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/feedback/alert.pyi` & `reflex-0.5.1a1/reflex/components/chakra/feedback/alert.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/feedback/circularprogress.py` & `reflex-0.5.1a1/reflex/components/chakra/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/feedback/circularprogress.pyi` & `reflex-0.5.1a1/reflex/components/chakra/feedback/circularprogress.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/feedback/progress.py` & `reflex-0.5.1a1/reflex/components/chakra/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/feedback/progress.pyi` & `reflex-0.5.1a1/reflex/components/chakra/feedback/progress.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/feedback/skeleton.py` & `reflex-0.5.1a1/reflex/components/chakra/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/feedback/skeleton.pyi` & `reflex-0.5.1a1/reflex/components/chakra/feedback/skeleton.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/feedback/spinner.py` & `reflex-0.5.1a1/reflex/components/chakra/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/feedback/spinner.pyi` & `reflex-0.5.1a1/reflex/components/chakra/feedback/spinner.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/__init__.py` & `reflex-0.5.1a1/reflex/components/chakra/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/button.py` & `reflex-0.5.1a1/reflex/components/chakra/forms/button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/button.pyi` & `reflex-0.5.1a1/reflex/components/chakra/forms/button.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/checkbox.py` & `reflex-0.5.1a1/reflex/components/chakra/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/checkbox.pyi` & `reflex-0.5.1a1/reflex/components/chakra/forms/checkbox.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/colormodeswitch.py` & `reflex-0.5.1a1/reflex/components/chakra/forms/colormodeswitch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/colormodeswitch.pyi` & `reflex-0.5.1a1/reflex/components/chakra/forms/colormodeswitch.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/date_picker.pyi` & `reflex-0.5.1a1/reflex/components/chakra/forms/date_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/date_time_picker.pyi` & `reflex-0.5.1a1/reflex/components/chakra/forms/date_time_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/editable.py` & `reflex-0.5.1a1/reflex/components/chakra/forms/editable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/editable.pyi` & `reflex-0.5.1a1/reflex/components/chakra/forms/editable.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/email.pyi` & `reflex-0.5.1a1/reflex/components/chakra/forms/email.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/form.py` & `reflex-0.5.1a1/reflex/components/chakra/forms/form.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/form.pyi` & `reflex-0.5.1a1/reflex/components/chakra/forms/form.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/iconbutton.py` & `reflex-0.5.1a1/reflex/components/chakra/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/iconbutton.pyi` & `reflex-0.5.1a1/reflex/components/chakra/forms/iconbutton.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/input.py` & `reflex-0.5.1a1/reflex/components/chakra/forms/input.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/input.pyi` & `reflex-0.5.1a1/reflex/components/chakra/forms/input.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/multiselect.py` & `reflex-0.5.1a1/reflex/components/chakra/forms/multiselect.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/numberinput.py` & `reflex-0.5.1a1/reflex/components/chakra/forms/numberinput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/numberinput.pyi` & `reflex-0.5.1a1/reflex/components/chakra/forms/numberinput.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/password.pyi` & `reflex-0.5.1a1/reflex/components/chakra/forms/password.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/pininput.py` & `reflex-0.5.1a1/reflex/components/chakra/forms/pininput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/pininput.pyi` & `reflex-0.5.1a1/reflex/components/chakra/forms/pininput.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/radio.py` & `reflex-0.5.1a1/reflex/components/chakra/forms/radio.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/radio.pyi` & `reflex-0.5.1a1/reflex/components/chakra/forms/radio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/rangeslider.py` & `reflex-0.5.1a1/reflex/components/chakra/forms/rangeslider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/rangeslider.pyi` & `reflex-0.5.1a1/reflex/components/chakra/forms/rangeslider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/select.py` & `reflex-0.5.1a1/reflex/components/chakra/forms/select.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/select.pyi` & `reflex-0.5.1a1/reflex/components/chakra/forms/select.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/slider.py` & `reflex-0.5.1a1/reflex/components/chakra/forms/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/slider.pyi` & `reflex-0.5.1a1/reflex/components/chakra/forms/slider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/switch.py` & `reflex-0.5.1a1/reflex/components/chakra/forms/switch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/switch.pyi` & `reflex-0.5.1a1/reflex/components/chakra/forms/switch.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/textarea.py` & `reflex-0.5.1a1/reflex/components/chakra/forms/textarea.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/textarea.pyi` & `reflex-0.5.1a1/reflex/components/chakra/forms/textarea.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/forms/time_picker.pyi` & `reflex-0.5.1a1/reflex/components/chakra/forms/time_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/layout/aspect_ratio.pyi` & `reflex-0.5.1a1/reflex/components/chakra/layout/aspect_ratio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/layout/box.py` & `reflex-0.5.1a1/reflex/components/chakra/layout/box.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/layout/box.pyi` & `reflex-0.5.1a1/reflex/components/chakra/layout/box.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/layout/card.py` & `reflex-0.5.1a1/reflex/components/chakra/layout/card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/layout/card.pyi` & `reflex-0.5.1a1/reflex/components/chakra/layout/card.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/layout/center.pyi` & `reflex-0.5.1a1/reflex/components/chakra/layout/center.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/layout/container.pyi` & `reflex-0.5.1a1/reflex/components/chakra/layout/container.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/layout/flex.py` & `reflex-0.5.1a1/reflex/components/chakra/layout/flex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/layout/flex.pyi` & `reflex-0.5.1a1/reflex/components/chakra/layout/flex.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/layout/grid.py` & `reflex-0.5.1a1/reflex/components/chakra/layout/grid.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/layout/grid.pyi` & `reflex-0.5.1a1/reflex/components/chakra/layout/grid.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/layout/spacer.pyi` & `reflex-0.5.1a1/reflex/components/chakra/layout/spacer.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/layout/stack.py` & `reflex-0.5.1a1/reflex/components/chakra/layout/stack.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/layout/stack.pyi` & `reflex-0.5.1a1/reflex/components/chakra/layout/stack.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/layout/wrap.py` & `reflex-0.5.1a1/reflex/components/chakra/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/layout/wrap.pyi` & `reflex-0.5.1a1/reflex/components/chakra/layout/wrap.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/media/avatar.py` & `reflex-0.5.1a1/reflex/components/chakra/media/avatar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/media/avatar.pyi` & `reflex-0.5.1a1/reflex/components/chakra/media/avatar.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/media/icon.py` & `reflex-0.5.1a1/reflex/components/chakra/media/icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/media/icon.pyi` & `reflex-0.5.1a1/reflex/components/chakra/media/icon.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/media/image.py` & `reflex-0.5.1a1/reflex/components/chakra/media/image.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/media/image.pyi` & `reflex-0.5.1a1/reflex/components/chakra/media/image.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/navigation/breadcrumb.py` & `reflex-0.5.1a1/reflex/components/chakra/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/navigation/breadcrumb.pyi` & `reflex-0.5.1a1/reflex/components/chakra/navigation/breadcrumb.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/navigation/link.py` & `reflex-0.5.1a1/reflex/components/chakra/navigation/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/navigation/link.pyi` & `reflex-0.5.1a1/reflex/components/chakra/navigation/link.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/navigation/linkoverlay.py` & `reflex-0.5.1a1/reflex/components/chakra/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/navigation/linkoverlay.pyi` & `reflex-0.5.1a1/reflex/components/chakra/navigation/linkoverlay.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/navigation/stepper.py` & `reflex-0.5.1a1/reflex/components/chakra/navigation/stepper.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/navigation/stepper.pyi` & `reflex-0.5.1a1/reflex/components/chakra/navigation/stepper.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/overlay/__init__.py` & `reflex-0.5.1a1/reflex/components/chakra/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/overlay/alertdialog.py` & `reflex-0.5.1a1/reflex/components/chakra/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/overlay/alertdialog.pyi` & `reflex-0.5.1a1/reflex/components/chakra/overlay/alertdialog.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/overlay/drawer.py` & `reflex-0.5.1a1/reflex/components/chakra/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/overlay/drawer.pyi` & `reflex-0.5.1a1/reflex/components/chakra/overlay/drawer.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/overlay/menu.py` & `reflex-0.5.1a1/reflex/components/chakra/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/overlay/menu.pyi` & `reflex-0.5.1a1/reflex/components/chakra/overlay/menu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/overlay/modal.py` & `reflex-0.5.1a1/reflex/components/chakra/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/overlay/modal.pyi` & `reflex-0.5.1a1/reflex/components/chakra/overlay/modal.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/overlay/popover.py` & `reflex-0.5.1a1/reflex/components/chakra/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/overlay/popover.pyi` & `reflex-0.5.1a1/reflex/components/chakra/overlay/popover.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/overlay/tooltip.py` & `reflex-0.5.1a1/reflex/components/chakra/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/overlay/tooltip.pyi` & `reflex-0.5.1a1/reflex/components/chakra/overlay/tooltip.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/typography/heading.pyi` & `reflex-0.5.1a1/reflex/components/chakra/typography/heading.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/typography/highlight.py` & `reflex-0.5.1a1/reflex/components/chakra/typography/highlight.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/typography/highlight.pyi` & `reflex-0.5.1a1/reflex/components/chakra/typography/highlight.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/typography/span.pyi` & `reflex-0.5.1a1/reflex/components/chakra/typography/span.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/chakra/typography/text.pyi` & `reflex-0.5.1a1/reflex/components/chakra/typography/text.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/component.py` & `reflex-0.5.1a1/reflex/components/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,15 +237,15 @@
             "react": "useEffect",
             "react-draggable": ["DraggableCore", rx.ImportVar(tag="Draggable", is_default=True)],
         }
         ```
         """
         return {}
 
-    def add_hooks(self) -> list[str]:
+    def add_hooks(self) -> list[str | Var]:
         """Add hooks inside the component function.
 
         Hooks are pieces of literal Javascript code that is inserted inside the
         React component function.
 
         Each logical hook should be a separate string in the list.
 
@@ -370,15 +370,15 @@
 
         # Iterate through the kwargs and set the props.
         for key, value in kwargs.items():
             if key.startswith("on_") and key not in triggers and key not in props:
                 raise ValueError(
                     f"The {(comp_name := type(self).__name__)} does not take in an `{key}` event trigger. If {comp_name}"
                     f" is a third party component make sure to add `{key}` to the component's event triggers. "
-                    f"visit https://reflex.dev/docs/wrapping-react/logic/#event-triggers for more info."
+                    f"visit https://reflex.dev/docs/wrapping-react/guide/#event-triggers for more info."
                 )
             if key in triggers:
                 # Event triggers are bound to event chains.
                 field_type = EventChain
             elif key in props:
                 # Set the field type.
                 field_type = fields[key].type_
@@ -727,14 +727,15 @@
 
         Returns:
             The component.
         """
         # Import here to avoid circular imports.
         from reflex.components.base.bare import Bare
         from reflex.components.base.fragment import Fragment
+        from reflex.utils.exceptions import ComponentTypeError
 
         # Translate deprecated props to new names.
         new_prop_names = [
             prop for prop in cls.get_props() if prop in ["type", "min", "max"]
         ]
         for prop in new_prop_names:
             under_prop = f"{prop}_"
@@ -753,15 +754,15 @@
 
         def validate_children(children):
             for child in children:
                 if isinstance(child, tuple):
                     validate_children(child)
                 # Make sure the child is a valid type.
                 if not types._isinstance(child, ComponentChild):
-                    raise TypeError(
+                    raise ComponentTypeError(
                         "Children of Reflex components must be other components, "
                         "state vars, or primitive Python types. "
                         f"Got child {child} of type {type(child)}.",
                     )
 
         # Validate all the children.
         validate_children(children)
@@ -1260,19 +1261,28 @@
             _imports.setdefault("react", set()).update(
                 {
                     ImportVar(tag="useRef"),
                     ImportVar(tag="useEffect"),
                 },
             )
 
+        other_imports = []
         user_hooks = self._get_hooks()
-        if user_hooks is not None and isinstance(user_hooks, Var):
-            _imports = imports.merge_imports(_imports, user_hooks._var_data.imports)  # type: ignore
+        if (
+            user_hooks is not None
+            and isinstance(user_hooks, Var)
+            and user_hooks._var_data is not None
+            and user_hooks._var_data.imports
+        ):
+            other_imports.append(user_hooks._var_data.imports)
+        other_imports.extend(
+            hook_imports for hook_imports in self._get_added_hooks().values()
+        )
 
-        return _imports
+        return imports.merge_imports(_imports, *other_imports)
 
     def _get_imports(self) -> imports.ImportDict:
         """Get all the libraries and fields that are used by the component.
 
         Returns:
             The imports needed by the component.
         """
@@ -1411,14 +1421,44 @@
                 if hook is not None
             },
             **self._get_vars_hooks(),
             **self._get_events_hooks(),
             **self._get_special_hooks(),
         }
 
+    def _get_added_hooks(self) -> dict[str, imports.ImportDict]:
+        """Get the hooks added via `add_hooks` method.
+
+        Returns:
+            The deduplicated hooks and imports added by the component and parent components.
+        """
+        code = {}
+
+        def extract_var_hooks(hook: Var):
+            _imports = {}
+            if hook._var_data is not None:
+                for sub_hook in hook._var_data.hooks:
+                    code[sub_hook] = {}
+                if hook._var_data.imports:
+                    _imports = hook._var_data.imports
+            if str(hook) in code:
+                code[str(hook)] = imports.merge_imports(code[str(hook)], _imports)
+            else:
+                code[str(hook)] = _imports
+
+        # Add the hook code from add_hooks for each parent class (this is reversed to preserve
+        # the order of the hooks in the final output)
+        for clz in reversed(tuple(self._iter_parent_classes_with_method("add_hooks"))):
+            for hook in clz.add_hooks(self):
+                if isinstance(hook, Var):
+                    extract_var_hooks(hook)
+                else:
+                    code[hook] = {}
+        return code
+
     def _get_hooks(self) -> str | None:
         """Get the React hooks for this component.
 
         Downstream components should override this method to add their own hooks.
 
         Returns:
             The hooks for just this component.
@@ -1449,19 +1489,15 @@
         code = {}
 
         # Add the hook code for this component.
         hooks = self._get_hooks()
         if hooks is not None:
             code[hooks] = None
 
-        # Add the hook code from add_hooks for each parent class (this is reversed to preserve
-        # the order of the hooks in the final output)
-        for clz in reversed(tuple(self._iter_parent_classes_with_method("add_hooks"))):
-            for hook in clz.add_hooks(self):
-                code[hook] = None
+        code.update(self._get_added_hooks())
 
         # Add the hook code for the children.
         for child in self.children:
             code = {**code, **child._get_all_hooks()}
 
         return code
 
@@ -2087,16 +2123,16 @@
             for arg in event_args:
                 if arg._var_data is None:
                     continue
                 for hook in arg._var_data.hooks:
                     var_deps.extend(cls._get_hook_deps(hook))
             memo_var_data = VarData.merge(
                 *[var._var_data for var in event_args],
-                VarData(  # type: ignore
-                    imports={"react": {ImportVar(tag="useCallback")}},
+                VarData(
+                    imports={"react": [ImportVar(tag="useCallback")]},
                 ),
             )
 
             # Store the memoized function name and hook code for this event trigger.
             trigger_memo[event_trigger] = (
                 Var.create_safe(memo_name)._replace(
                     _var_type=EventChain, merge_var_data=memo_var_data
```

### Comparing `reflex-0.5.0a3/reflex/components/core/__init__.py` & `reflex-0.5.1a1/reflex/components/core/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 """Core Reflex components."""
 
 from . import layout as layout
-from .banner import ConnectionBanner, ConnectionModal, ConnectionPulser
+from .banner import (
+    ConnectionBanner,
+    ConnectionModal,
+    ConnectionPulser,
+    ConnectionToaster,
+)
 from .colors import color
 from .cond import Cond, color_mode_cond, cond
 from .debounce import DebounceInput
 from .foreach import Foreach
 from .html import Html
 from .match import Match
 from .responsive import (
@@ -22,13 +27,14 @@
     get_upload_dir,
     get_upload_url,
     selected_files,
 )
 
 connection_banner = ConnectionBanner.create
 connection_modal = ConnectionModal.create
+connection_toaster = ConnectionToaster.create
 connection_pulser = ConnectionPulser.create
 debounce_input = DebounceInput.create
 foreach = Foreach.create
 html = Html.create
 match = Match.create
 upload = UploadNamespace()
```

### Comparing `reflex-0.5.0a3/reflex/components/core/banner.py` & `reflex-0.5.1a1/reflex/components/core/banner.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,44 +12,58 @@
 from reflex.components.radix.themes.components.dialog import (
     DialogContent,
     DialogRoot,
     DialogTitle,
 )
 from reflex.components.radix.themes.layout import Flex
 from reflex.components.radix.themes.typography.text import Text
+from reflex.components.sonner.toast import Toaster, ToastProps
 from reflex.constants import Dirs, Hooks, Imports
+from reflex.constants.compiler import CompileVars
 from reflex.utils import imports
+from reflex.utils.serializers import serialize
 from reflex.vars import Var, VarData
 
 connect_error_var_data: VarData = VarData(  # type: ignore
     imports=Imports.EVENTS,
     hooks={Hooks.EVENTS: None},
 )
 
+connect_errors: Var = Var.create_safe(
+    value=CompileVars.CONNECT_ERROR,
+    _var_is_local=True,
+    _var_is_string=False,
+    _var_data=connect_error_var_data,
+)
+
 connection_error: Var = Var.create_safe(
     value="(connectErrors.length > 0) ? connectErrors[connectErrors.length - 1].message : ''",
     _var_is_local=False,
     _var_is_string=False,
-)._replace(merge_var_data=connect_error_var_data)
+    _var_data=connect_error_var_data,
+)
 
 connection_errors_count: Var = Var.create_safe(
     value="connectErrors.length",
     _var_is_string=False,
     _var_is_local=False,
-)._replace(merge_var_data=connect_error_var_data)
+    _var_data=connect_error_var_data,
+)
 
 has_connection_errors: Var = Var.create_safe(
     value="connectErrors.length > 0",
     _var_is_string=False,
-)._replace(_var_type=bool, merge_var_data=connect_error_var_data)
+    _var_data=connect_error_var_data,
+).to(bool)
 
 has_too_many_connection_errors: Var = Var.create_safe(
     value="connectErrors.length >= 2",
     _var_is_string=False,
-)._replace(_var_type=bool, merge_var_data=connect_error_var_data)
+    _var_data=connect_error_var_data,
+).to(bool)
 
 
 class WebsocketTargetURL(Bare):
     """A component that renders the websocket target URL."""
 
     def _get_imports(self) -> imports.ImportDict:
         return {
@@ -77,14 +91,72 @@
         "Cannot connect to server: ",
         connection_error,
         ". Check if server is reachable at ",
         WebsocketTargetURL.create(),
     ]
 
 
+class ConnectionToaster(Toaster):
+    """A connection toaster component."""
+
+    def add_hooks(self) -> list[str]:
+        """Add the hooks for the connection toaster.
+
+        Returns:
+            The hooks for the connection toaster.
+        """
+        toast_id = "websocket-error"
+        target_url = WebsocketTargetURL.create()
+        props = ToastProps(  # type: ignore
+            description=Var.create(
+                f"`Check if server is reachable at ${target_url}`",
+                _var_is_string=False,
+                _var_is_local=False,
+            ),
+            close_button=True,
+            duration=120000,
+            id=toast_id,
+        )
+        hook = Var.create(
+            f"""
+const toast_props = {serialize(props)};
+const [userDismissed, setUserDismissed] = useState(false);
+useEffect(() => {{
+    if ({has_too_many_connection_errors}) {{
+        if (!userDismissed) {{
+            toast.error(
+                `Cannot connect to server: {connection_error}.`,
+                {{...toast_props, onDismiss: () => setUserDismissed(true)}},
+            )
+        }}
+    }} else {{
+        toast.dismiss("{toast_id}");
+        setUserDismissed(false);  // after reconnection reset dismissed state
+    }}
+}}, [{connect_errors}]);"""
+        )
+
+        hook._var_data = VarData.merge(  # type: ignore
+            connect_errors._var_data,
+            VarData(
+                imports={
+                    "react": [
+                        imports.ImportVar(tag="useEffect"),
+                        imports.ImportVar(tag="useState"),
+                    ],
+                    **target_url._get_imports(),
+                }
+            ),
+        )
+        return [
+            Hooks.EVENTS,
+            hook,  # type: ignore
+        ]
+
+
 class ConnectionBanner(Component):
     """A connection banner component."""
 
     @classmethod
     def create(cls, comp: Optional[Component] = None) -> Component:
         """Create a connection banner component.
 
@@ -154,16 +226,16 @@
         """
         return super().create(
             "wifi_off",
             color=props.pop("color", "crimson"),
             size=props.pop("size", 32),
             z_index=props.pop("z_index", 9999),
             position=props.pop("position", "fixed"),
-            bottom=props.pop("botton", "30px"),
-            right=props.pop("right", "30px"),
+            bottom=props.pop("botton", "33px"),
+            right=props.pop("right", "33px"),
             animation=Var.create(f"${{pulse}} 1s infinite", _var_is_string=True),
             **props,
         )
 
     def _get_imports(self) -> imports.ImportDict:
         return imports.merge_imports(
             super()._get_imports(),
@@ -197,11 +269,12 @@
             The connection pulser component.
         """
         return super().create(
             cond(
                 has_connection_errors,
                 WifiOffPulse.create(**props),
             ),
+            title=f"Connection Error: {connection_error}",
             position="fixed",
             width="100vw",
             height="0",
         )
```

### Comparing `reflex-0.5.0a3/reflex/components/core/banner.pyi` & `reflex-0.5.1a1/reflex/components/radix/primitives/slider.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,32 @@
-"""Stub file for reflex/components/core/banner.py"""
+"""Stub file for reflex/components/radix/primitives/slider.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Optional
-from reflex.components.base.bare import Bare
-from reflex.components.component import Component
-from reflex.components.core.cond import cond
-from reflex.components.el.elements.typography import Div
-from reflex.components.lucide.icon import Icon
-from reflex.components.radix.themes.components.dialog import (
-    DialogContent,
-    DialogRoot,
-    DialogTitle,
-)
-from reflex.components.radix.themes.layout import Flex
-from reflex.components.radix.themes.typography.text import Text
-from reflex.constants import Dirs, Hooks, Imports
-from reflex.utils import imports
-from reflex.vars import Var, VarData
-
-connect_error_var_data: VarData
-connection_error: Var
-connection_errors_count: Var
-has_connection_errors: Var
-has_too_many_connection_errors: Var
+from typing import Any, Dict, List, Literal
+from reflex.components.component import Component, ComponentNamespace
+from reflex.components.radix.primitives.base import RadixPrimitiveComponentWithClassName
+from reflex.style import Style
+from reflex.vars import Var
+
+LiteralSliderOrientation = Literal["horizontal", "vertical"]
+LiteralSliderDir = Literal["ltr", "rtl"]
 
-class WebsocketTargetURL(Bare):
+class SliderComponent(RadixPrimitiveComponentWithClassName):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        contents: Optional[Union[Var[str], str]] = None,
+        as_child: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -85,30 +71,58 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "WebsocketTargetURL":
-        """Create a websocket target URL component.
+    ) -> "SliderComponent":
+        """Create the component.
+
+        Args:
+            *children: The children of the component.
+            as_child: Change the default rendered element for the one passed as a child.
+            style: The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: The props of the component.
 
         Returns:
-            The websocket target URL component.
+            The component.
         """
         ...
 
-def default_connection_error() -> list[str | Var | Component]: ...
-
-class ConnectionBanner(Component):
+class SliderRoot(SliderComponent):
+    def get_event_triggers(self) -> Dict[str, Any]: ...
+    def add_style(self) -> Style | None: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
+        default_value: Optional[Union[Var[List[int]], List[int]]] = None,
+        value: Optional[Union[Var[List[int]], List[int]]] = None,
+        name: Optional[Union[Var[str], str]] = None,
+        disabled: Optional[Union[Var[bool], bool]] = None,
+        orientation: Optional[
+            Union[
+                Var[Literal["horizontal", "vertical"]],
+                Literal["horizontal", "vertical"],
+            ]
+        ] = None,
+        dir: Optional[Union[Var[Literal["ltr", "rtl"]], Literal["ltr", "rtl"]]] = None,
+        inverted: Optional[Union[Var[bool], bool]] = None,
+        min: Optional[Union[Var[int], int]] = None,
+        max: Optional[Union[Var[int], int]] = None,
+        step: Optional[Union[Var[int], int]] = None,
+        min_steps_between_thumbs: Optional[Union[Var[int], int]] = None,
+        as_child: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -152,32 +166,48 @@
         ] = None,
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_value_change: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_value_commit: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         **props
-    ) -> "ConnectionBanner":
-        """Create a connection banner component.
+    ) -> "SliderRoot":
+        """Create the component.
 
         Args:
-            comp: The component to render when there's a server connection error.
+            *children: The children of the component.
+            as_child: Change the default rendered element for the one passed as a child.
+            style: The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: The props of the component.
 
         Returns:
-            The connection banner component.
+            The component.
         """
         ...
 
-class ConnectionModal(Component):
+class SliderTrack(SliderComponent):
+    def add_style(self) -> Style | None: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
+        as_child: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -222,32 +252,41 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "ConnectionModal":
-        """Create a connection banner component.
+    ) -> "SliderTrack":
+        """Create the component.
 
         Args:
-            comp: The component to render when there's a server connection error.
+            *children: The children of the component.
+            as_child: Change the default rendered element for the one passed as a child.
+            style: The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: The props of the component.
 
         Returns:
-            The connection banner component.
+            The component.
         """
         ...
 
-class WifiOffPulse(Icon):
+class SliderRange(SliderComponent):
+    def add_style(self) -> Style | None: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        size: Optional[Union[Var[int], int]] = None,
+        as_child: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -292,78 +331,41 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "WifiOffPulse":
-        """Create a wifi_off icon with an animated opacity pulse.
+    ) -> "SliderRange":
+        """Create the component.
 
         Args:
-            size: The size of the icon in pixels.
+            *children: The children of the component.
+            as_child: Change the default rendered element for the one passed as a child.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: The properties of the component.
+            **props: The props of the component.
 
         Returns:
-            The icon component with default props applied.
+            The component.
         """
         ...
 
-class ConnectionPulser(Div):
+class SliderThumb(SliderComponent):
+    def add_style(self) -> Style | None: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        access_key: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        auto_capitalize: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        content_editable: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        context_menu: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        dir: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        draggable: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        enter_key_hint: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        hidden: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        input_mode: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        item_prop: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        lang: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        role: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        slot: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        spell_check: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        tab_index: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
-        title: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
-        ] = None,
+        as_child: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -408,39 +410,36 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "ConnectionPulser":
-        """Create a connection pulser component.
+    ) -> "SliderThumb":
+        """Create the component.
 
         Args:
-            access_key:  Provides a hint for generating a keyboard shortcut for the current element.
-            auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
-            content_editable: Indicates whether the element's content is editable.
-            context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
-            dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
-            draggable: Defines whether the element can be dragged.
-            enter_key_hint: Hints what media types the media element is able to play.
-            hidden: Defines whether the element is hidden.
-            input_mode: Defines the type of the element.
-            item_prop: Defines the name of the element for metadata purposes.
-            lang: Defines the language used in the element.
-            role: Defines the role of the element.
-            slot: Assigns a slot in a shadow DOM shadow tree to an element.
-            spell_check: Defines whether the element may be checked for spelling errors.
-            tab_index: Defines the position of the current element in the tabbing order.
-            title: Defines a tooltip for the element.
+            *children: The children of the component.
+            as_child: Change the default rendered element for the one passed as a child.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: The properties of the component.
+            **props: The props of the component.
 
         Returns:
-            The connection pulser component.
+            The component.
         """
         ...
+
+class Slider(ComponentNamespace):
+    root = staticmethod(SliderRoot.create)
+    track = staticmethod(SliderTrack.create)
+    range = staticmethod(SliderRange.create)
+    thumb = staticmethod(SliderThumb.create)
+
+    @staticmethod
+    def __call__(**props) -> Component: ...
+
+slider = Slider()
```

### Comparing `reflex-0.5.0a3/reflex/components/core/client_side_routing.py` & `reflex-0.5.1a1/reflex/components/core/client_side_routing.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/core/client_side_routing.pyi` & `reflex-0.5.1a1/reflex/components/core/client_side_routing.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/core/colors.py` & `reflex-0.5.1a1/reflex/components/core/colors.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/core/cond.py` & `reflex-0.5.1a1/reflex/components/core/cond.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from reflex.constants import Dirs
 from reflex.constants.colors import Color
 from reflex.style import LIGHT_COLOR_MODE, color_mode
 from reflex.utils import format, imports
 from reflex.vars import BaseVar, Var, VarData
 
 _IS_TRUE_IMPORT = {
-    f"/{Dirs.STATE_PATH}": {imports.ImportVar(tag="isTrue")},
+    f"/{Dirs.STATE_PATH}": [imports.ImportVar(tag="isTrue")],
 }
 
 
 class Cond(MemoizationLeaf):
     """Render one of two components based on a condition."""
 
     # The cond to determine which component to render.
```

### Comparing `reflex-0.5.0a3/reflex/components/core/debounce.py` & `reflex-0.5.1a1/reflex/components/core/debounce.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,21 +105,19 @@
         # Set the child element to wrap, including any imports/hooks from the child.
         props.setdefault(
             "element",
             Var.create_safe(
                 "{%s}" % (child.alias or child.tag),
                 _var_is_local=False,
                 _var_is_string=False,
-            )._replace(
-                _var_type=Type[Component],
-                merge_var_data=VarData(  # type: ignore
+                _var_data=VarData(
                     imports=child._get_imports(),
                     hooks=child._get_hooks_internal(),
                 ),
-            ),
+            ).to(Type[Component]),
         )
 
         component = super().create(**props)
         component._get_style = child._get_style
         component.event_triggers.update(child.event_triggers)
         component.children = child.children
         component._rename_props = child._rename_props
```

### Comparing `reflex-0.5.0a3/reflex/components/core/debounce.pyi` & `reflex-0.5.1a1/reflex/components/core/debounce.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/core/foreach.py` & `reflex-0.5.1a1/reflex/components/core/foreach.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import inspect
 from typing import Any, Callable, Iterable
 
 from reflex.components.base.fragment import Fragment
 from reflex.components.component import Component
 from reflex.components.tags import IterTag
 from reflex.constants import MemoizationMode
+from reflex.state import ComponentState
 from reflex.utils import console
 from reflex.vars import Var
 
 
 class ForeachVarError(TypeError):
     """Raised when the iterable type is Any."""
 
@@ -46,14 +47,15 @@
             **props: The attributes to pass to each child component (deprecated).
 
         Returns:
             The foreach component.
 
         Raises:
             ForeachVarError: If the iterable is of type Any.
+            TypeError: If the render function is a ComponentState.
         """
         if props:
             console.deprecate(
                 feature_name="Passing props to rx.foreach",
                 reason="it does not have the intended effect and may be confusing",
                 deprecation_version="0.5.0",
                 removal_version="0.6.0",
@@ -61,14 +63,23 @@
         iterable = Var.create_safe(iterable)
         if iterable._var_type == Any:
             raise ForeachVarError(
                 f"Could not foreach over var `{iterable._var_full_name}` of type Any. "
                 "(If you are trying to foreach over a state var, add a type annotation to the var). "
                 "See https://reflex.dev/docs/library/layout/foreach/"
             )
+
+        if (
+            hasattr(render_fn, "__qualname__")
+            and render_fn.__qualname__ == ComponentState.create.__qualname__
+        ):
+            raise TypeError(
+                "Using a ComponentState as `render_fn` inside `rx.foreach` is not supported yet."
+            )
+
         component = cls(
             iterable=iterable,
             render_fn=render_fn,
         )
         # Keep a ref to a rendered component to determine correct imports/hooks/styles.
         component.children = [component._render().render_component()]
         return component
```

### Comparing `reflex-0.5.0a3/reflex/components/core/html.py` & `reflex-0.5.1a1/reflex/components/core/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/core/html.pyi` & `reflex-0.5.1a1/reflex/components/core/html.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/core/match.py` & `reflex-0.5.1a1/reflex/components/core/match.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/core/responsive.py` & `reflex-0.5.1a1/reflex/components/core/responsive.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/core/upload.py` & `reflex-0.5.1a1/reflex/components/core/upload.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,20 +20,20 @@
     parse_args_spec,
 )
 from reflex.utils import imports
 from reflex.vars import BaseVar, CallableVar, Var, VarData
 
 DEFAULT_UPLOAD_ID: str = "default"
 
-upload_files_context_var_data: VarData = VarData(  # type: ignore
+upload_files_context_var_data: VarData = VarData(
     imports={
-        "react": {imports.ImportVar(tag="useContext")},
-        f"/{Dirs.CONTEXTS_PATH}": {
+        "react": [imports.ImportVar(tag="useContext")],
+        f"/{Dirs.CONTEXTS_PATH}": [
             imports.ImportVar(tag="UploadFilesContext"),
-        },
+        ],
     },
     hooks={
         "const [filesById, setFilesById] = useContext(UploadFilesContext);": None,
     },
 )
 
 
@@ -114,22 +114,21 @@
         os.environ.get("REFLEX_UPLOADED_FILES_DIR", "./uploaded_files")
     )
     uploaded_files_dir.mkdir(parents=True, exist_ok=True)
     return uploaded_files_dir
 
 
 uploaded_files_url_prefix: Var = Var.create_safe(
-    "${getBackendURL(env.UPLOAD)}"
-)._replace(
-    merge_var_data=VarData(  # type: ignore
+    "${getBackendURL(env.UPLOAD)}",
+    _var_data=VarData(
         imports={
-            f"/{Dirs.STATE_PATH}": {imports.ImportVar(tag="getBackendURL")},
-            "/env.json": {imports.ImportVar(tag="env", is_default=True)},
+            f"/{Dirs.STATE_PATH}": [imports.ImportVar(tag="getBackendURL")],
+            "/env.json": [imports.ImportVar(tag="env", is_default=True)],
         }
-    )
+    ),
 )
 
 
 def get_upload_url(file_path: str) -> Var[str]:
     """Get the URL of an uploaded file.
 
     Args:
```

### Comparing `reflex-0.5.0a3/reflex/components/core/upload.pyi` & `reflex-0.5.1a1/reflex/components/core/upload.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/datadisplay/code.py` & `reflex-0.5.1a1/reflex/components/datadisplay/code.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/datadisplay/code.pyi` & `reflex-0.5.1a1/reflex/components/datadisplay/code.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/datadisplay/dataeditor.py` & `reflex-0.5.1a1/reflex/components/datadisplay/dataeditor.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/datadisplay/dataeditor.pyi` & `reflex-0.5.1a1/reflex/components/datadisplay/dataeditor.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/datadisplay/logo.py` & `reflex-0.5.1a1/reflex/components/datadisplay/logo.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/el/constants/html.py` & `reflex-0.5.1a1/reflex/components/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/el/constants/react.py` & `reflex-0.5.1a1/reflex/components/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/el/constants/reflex.py` & `reflex-0.5.1a1/reflex/components/el/constants/reflex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/el/element.pyi` & `reflex-0.5.1a1/reflex/components/el/element.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/el/elements/__init__.py` & `reflex-0.5.1a1/reflex/components/el/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/el/elements/base.py` & `reflex-0.5.1a1/reflex/components/el/elements/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/el/elements/base.pyi` & `reflex-0.5.1a1/reflex/components/el/elements/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/el/elements/forms.py` & `reflex-0.5.1a1/reflex/components/el/elements/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,21 +212,25 @@
         form_refs = {}
         for ref in self._get_all_refs():
             # when ref start with refs_ it's an array of refs, so we need different method
             # to collect data
             if ref.startswith("refs_"):
                 ref_var = Var.create_safe(ref[:-3]).as_ref()
                 form_refs[ref[5:-3]] = Var.create_safe(
-                    f"getRefValues({str(ref_var)})", _var_is_local=False
-                )._replace(merge_var_data=ref_var._var_data)
+                    f"getRefValues({str(ref_var)})",
+                    _var_is_local=False,
+                    _var_data=ref_var._var_data,
+                )
             else:
                 ref_var = Var.create_safe(ref).as_ref()
                 form_refs[ref[4:]] = Var.create_safe(
-                    f"getRefValue({str(ref_var)})", _var_is_local=False
-                )._replace(merge_var_data=ref_var._var_data)
+                    f"getRefValue({str(ref_var)})",
+                    _var_is_local=False,
+                    _var_data=ref_var._var_data,
+                )
         return form_refs
 
     def _get_vars(self, include_children: bool = True) -> Iterator[Var]:
         yield from super()._get_vars(include_children=include_children)
         yield from self._get_form_refs().values()
 
     def _exclude_props(self) -> list[str]:
@@ -615,22 +619,24 @@
                 raise ValueError(
                     "Cannot combine `enter_key_submit` with `on_key_down`.",
                 )
             tag.add_props(
                 on_key_down=Var.create_safe(
                     f"(e) => enterKeySubmitOnKeyDown(e, {self.enter_key_submit._var_name_unwrapped})",
                     _var_is_local=False,
-                )._replace(merge_var_data=self.enter_key_submit._var_data),
+                    _var_data=self.enter_key_submit._var_data,
+                )
             )
         if self.auto_height is not None:
             tag.add_props(
                 on_input=Var.create_safe(
                     f"(e) => autoHeightOnInput(e, {self.auto_height._var_name_unwrapped})",
                     _var_is_local=False,
-                )._replace(merge_var_data=self.auto_height._var_data),
+                    _var_data=self.auto_height._var_data,
+                )
             )
         return tag
 
     def get_event_triggers(self) -> Dict[str, Any]:
         """Get the event triggers that pass the component's value to the handler.
 
         Returns:
```

### Comparing `reflex-0.5.0a3/reflex/components/el/elements/forms.pyi` & `reflex-0.5.1a1/reflex/components/el/elements/forms.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/el/elements/inline.py` & `reflex-0.5.1a1/reflex/components/el/elements/inline.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/el/elements/inline.pyi` & `reflex-0.5.1a1/reflex/components/el/elements/inline.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/el/elements/media.py` & `reflex-0.5.1a1/reflex/components/el/elements/media.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Element classes. This is an auto-generated file. Do not edit. See ../generate.py."""
 from typing import Any, Union
 
+from reflex import Component
 from reflex.vars import Var as Var
 
 from .base import BaseHTML
 
 
 class Area(BaseHTML):
     """Display the area element."""
@@ -112,14 +113,32 @@
 
     # A set of source sizes and URLs for responsive images
     src_set: Var[Union[str, int, bool]]
 
     # The name of the map to use with the image
     use_map: Var[Union[str, int, bool]]
 
+    @classmethod
+    def create(cls, *children, **props) -> Component:
+        """Override create method to apply source attribute to value if user fails to pass in attribute.
+
+        Args:
+            *children: The children of the component.
+            **props: The props of the component.
+
+        Returns:
+            The component.
+
+        """
+        return (
+            super().create(src=children[0], **props)
+            if children
+            else super().create(*children, **props)
+        )
+
 
 class Map(BaseHTML):
     """Display the map element."""
 
     tag = "map"
 
     # Name of the map, referenced by the 'usemap' attribute in 'img' and 'object' elements
```

### Comparing `reflex-0.5.0a3/reflex/components/el/elements/media.pyi` & `reflex-0.5.1a1/reflex/components/el/elements/media.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Any, Union
+from reflex import Component
 from reflex.vars import Var as Var
 from .base import BaseHTML
 
 class Area(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
@@ -466,15 +467,15 @@
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
     ) -> "Img":
-        """Create the component.
+        """Override create method to apply source attribute to value if user fails to pass in attribute.
 
         Args:
             *children: The children of the component.
             align: Image alignment with respect to its surrounding elements
             alt: Alternative text for the image
             cross_origin: Configures the CORS requests for the image
             decoding: How the image should be decoded
@@ -508,14 +509,15 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
+
         """
         ...
 
 class Map(BaseHTML):
     @overload
     @classmethod
     def create(  # type: ignore
```

### Comparing `reflex-0.5.0a3/reflex/components/el/elements/metadata.py` & `reflex-0.5.1a1/reflex/components/el/elements/metadata.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/el/elements/metadata.pyi` & `reflex-0.5.1a1/reflex/components/el/elements/metadata.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/el/elements/other.py` & `reflex-0.5.1a1/reflex/components/el/elements/other.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/el/elements/other.pyi` & `reflex-0.5.1a1/reflex/components/el/elements/other.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/el/elements/scripts.py` & `reflex-0.5.1a1/reflex/components/el/elements/scripts.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/el/elements/scripts.pyi` & `reflex-0.5.1a1/reflex/components/el/elements/scripts.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/el/elements/sectioning.py` & `reflex-0.5.1a1/reflex/components/el/elements/sectioning.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/el/elements/sectioning.pyi` & `reflex-0.5.1a1/reflex/components/el/elements/sectioning.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/el/elements/tables.py` & `reflex-0.5.1a1/reflex/components/el/elements/tables.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/el/elements/tables.pyi` & `reflex-0.5.1a1/reflex/components/el/elements/tables.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/el/elements/typography.py` & `reflex-0.5.1a1/reflex/components/el/elements/typography.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/el/elements/typography.pyi` & `reflex-0.5.1a1/reflex/components/el/elements/typography.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/gridjs/datatable.py` & `reflex-0.5.1a1/reflex/components/gridjs/datatable.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,20 +110,22 @@
 
     def _render(self) -> Tag:
         if isinstance(self.data, Var) and types.is_dataframe(self.data._var_type):
             self.columns = BaseVar(
                 _var_name=f"{self.data._var_name}.columns",
                 _var_type=List[Any],
                 _var_full_name_needs_state_prefix=True,
-            )._replace(merge_var_data=self.data._var_data)
+                _var_data=self.data._var_data,
+            )
             self.data = BaseVar(
                 _var_name=f"{self.data._var_name}.data",
                 _var_type=List[List[Any]],
                 _var_full_name_needs_state_prefix=True,
-            )._replace(merge_var_data=self.data._var_data)
+                _var_data=self.data._var_data,
+            )
         if types.is_dataframe(type(self.data)):
             # If given a pandas df break up the data and columns
             data = serialize(self.data)
             assert isinstance(data, dict), "Serialized dataframe should be a dict."
             self.columns = Var.create_safe(data["columns"])
             self.data = Var.create_safe(data["data"])
```

### Comparing `reflex-0.5.0a3/reflex/components/gridjs/datatable.pyi` & `reflex-0.5.1a1/reflex/components/gridjs/datatable.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/lucide/icon.py` & `reflex-0.5.1a1/reflex/components/lucide/icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/lucide/icon.pyi` & `reflex-0.5.1a1/reflex/components/lucide/icon.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/markdown/markdown.py` & `reflex-0.5.1a1/reflex/components/markdown/markdown.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/markdown/markdown.pyi` & `reflex-0.5.1a1/reflex/components/markdown/markdown.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/moment/moment.py` & `reflex-0.5.1a1/reflex/components/moment/moment.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/moment/moment.pyi` & `reflex-0.5.1a1/reflex/components/moment/moment.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/next/base.pyi` & `reflex-0.5.1a1/reflex/components/next/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/next/image.py` & `reflex-0.5.1a1/reflex/components/next/image.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/next/image.pyi` & `reflex-0.5.1a1/reflex/components/next/image.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/next/link.pyi` & `reflex-0.5.1a1/reflex/components/next/link.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/next/video.py` & `reflex-0.5.1a1/reflex/components/next/video.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/next/video.pyi` & `reflex-0.5.1a1/reflex/components/next/video.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/plotly/plotly.py` & `reflex-0.5.1a1/reflex/components/plotly/plotly.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/plotly/plotly.pyi` & `reflex-0.5.1a1/reflex/components/plotly/plotly.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/primitives/accordion.py` & `reflex-0.5.1a1/reflex/components/radix/primitives/accordion.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/primitives/accordion.pyi` & `reflex-0.5.1a1/reflex/components/radix/primitives/accordion.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/primitives/base.py` & `reflex-0.5.1a1/reflex/components/radix/primitives/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/primitives/base.pyi` & `reflex-0.5.1a1/reflex/components/radix/primitives/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/primitives/drawer.py` & `reflex-0.5.1a1/reflex/components/radix/primitives/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/primitives/drawer.pyi` & `reflex-0.5.1a1/reflex/components/radix/primitives/drawer.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/primitives/form.py` & `reflex-0.5.1a1/reflex/components/radix/primitives/form.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/primitives/form.pyi` & `reflex-0.5.1a1/reflex/components/radix/primitives/form.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/primitives/progress.py` & `reflex-0.5.1a1/reflex/components/radix/primitives/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/primitives/progress.pyi` & `reflex-0.5.1a1/reflex/components/radix/primitives/progress.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/primitives/slider.py` & `reflex-0.5.1a1/reflex/components/radix/primitives/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/primitives/slider.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/tabs.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,49 @@
-"""Stub file for reflex/components/radix/primitives/slider.py"""
+"""Stub file for reflex/components/radix/themes/components/tabs.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Any, Dict, List, Literal
 from reflex.components.component import Component, ComponentNamespace
-from reflex.components.radix.primitives.base import RadixPrimitiveComponentWithClassName
-from reflex.style import Style
+from reflex.constants import EventTriggers
 from reflex.vars import Var
+from ..base import LiteralAccentColor, RadixThemesComponent
 
-LiteralSliderOrientation = Literal["horizontal", "vertical"]
-LiteralSliderDir = Literal["ltr", "rtl"]
-
-class SliderComponent(RadixPrimitiveComponentWithClassName):
+class TabsRoot(RadixThemesComponent):
+    def get_event_triggers(self) -> Dict[str, Any]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        as_child: Optional[Union[Var[bool], bool]] = None,
+        default_value: Optional[Union[Var[str], str]] = None,
+        value: Optional[Union[Var[str], str]] = None,
+        orientation: Optional[
+            Union[
+                Var[Literal["horizontal", "vertical"]],
+                Literal["horizontal", "vertical"],
+            ]
+        ] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_change: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_context_menu: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_double_click: Optional[
@@ -71,58 +79,45 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "SliderComponent":
-        """Create the component.
+    ) -> "TabsRoot":
+        """Create a new component instance.
+
+        Will prepend "RadixThemes" to the component tag to avoid conflicts with
+        other UI libraries for common names, like Text and Button.
 
         Args:
-            *children: The children of the component.
-            as_child: Change the default rendered element for the one passed as a child.
+            *children: Child components.
+            default_value: The value of the tab that should be active when initially rendered. Use when you do not need to control the state of the tabs.
+            value: The controlled value of the tab that should be active. Use when you need to control the state of the tabs.
+            orientation: The orientation of the tabs.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: The props of the component.
+            **props: Component properties.
 
         Returns:
-            The component.
+            A new component instance.
         """
         ...
 
-class SliderRoot(SliderComponent):
-    def get_event_triggers(self) -> Dict[str, Any]: ...
-    def add_style(self) -> Style | None: ...
+class TabsList(RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        default_value: Optional[Union[Var[List[int]], List[int]]] = None,
-        value: Optional[Union[Var[List[int]], List[int]]] = None,
-        name: Optional[Union[Var[str], str]] = None,
-        disabled: Optional[Union[Var[bool], bool]] = None,
-        orientation: Optional[
-            Union[
-                Var[Literal["horizontal", "vertical"]],
-                Literal["horizontal", "vertical"],
-            ]
-        ] = None,
-        dir: Optional[Union[Var[Literal["ltr", "rtl"]], Literal["ltr", "rtl"]]] = None,
-        inverted: Optional[Union[Var[bool], bool]] = None,
-        min: Optional[Union[Var[int], int]] = None,
-        max: Optional[Union[Var[int], int]] = None,
-        step: Optional[Union[Var[int], int]] = None,
-        min_steps_between_thumbs: Optional[Union[Var[int], int]] = None,
-        as_child: Optional[Union[Var[bool], bool]] = None,
+        size: Optional[Union[Var[Literal["1", "2"]], Literal["1", "2"]]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -166,48 +161,107 @@
         ] = None,
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_value_change: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_value_commit: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         **props
-    ) -> "SliderRoot":
-        """Create the component.
+    ) -> "TabsList":
+        """Create a new component instance.
+
+        Will prepend "RadixThemes" to the component tag to avoid conflicts with
+        other UI libraries for common names, like Text and Button.
 
         Args:
-            *children: The children of the component.
-            as_child: Change the default rendered element for the one passed as a child.
+            *children: Child components.
+            size: Tabs size "1" - "2"
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: The props of the component.
+            **props: Component properties.
 
         Returns:
-            The component.
+            A new component instance.
         """
         ...
 
-class SliderTrack(SliderComponent):
-    def add_style(self) -> Style | None: ...
+class TabsTrigger(RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        as_child: Optional[Union[Var[bool], bool]] = None,
+        value: Optional[Union[Var[str], str]] = None,
+        disabled: Optional[Union[Var[bool], bool]] = None,
+        color_scheme: Optional[
+            Union[
+                Var[
+                    Literal[
+                        "tomato",
+                        "red",
+                        "ruby",
+                        "crimson",
+                        "pink",
+                        "plum",
+                        "purple",
+                        "violet",
+                        "iris",
+                        "indigo",
+                        "blue",
+                        "cyan",
+                        "teal",
+                        "jade",
+                        "green",
+                        "grass",
+                        "brown",
+                        "orange",
+                        "sky",
+                        "mint",
+                        "lime",
+                        "yellow",
+                        "amber",
+                        "gold",
+                        "bronze",
+                        "gray",
+                    ]
+                ],
+                Literal[
+                    "tomato",
+                    "red",
+                    "ruby",
+                    "crimson",
+                    "pink",
+                    "plum",
+                    "purple",
+                    "violet",
+                    "iris",
+                    "indigo",
+                    "blue",
+                    "cyan",
+                    "teal",
+                    "jade",
+                    "green",
+                    "grass",
+                    "brown",
+                    "orange",
+                    "sky",
+                    "mint",
+                    "lime",
+                    "yellow",
+                    "amber",
+                    "gold",
+                    "bronze",
+                    "gray",
+                ],
+            ]
+        ] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -252,41 +306,42 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "SliderTrack":
-        """Create the component.
+    ) -> "TabsTrigger":
+        """Create a TabsTrigger component.
 
         Args:
             *children: The children of the component.
-            as_child: Change the default rendered element for the one passed as a child.
+            value: The value of the tab. Must be unique for each tab.
+            disabled: Whether the tab is disabled
+            color_scheme: The color of the line under the tab when active.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: The props of the component.
+            **props: The properties of the component.
 
         Returns:
-            The component.
+            The TabsTrigger Component.
         """
         ...
 
-class SliderRange(SliderComponent):
-    def add_style(self) -> Style | None: ...
+class TabsContent(RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        as_child: Optional[Union[Var[bool], bool]] = None,
+        value: Optional[Union[Var[str], str]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -331,50 +386,65 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "SliderRange":
-        """Create the component.
+    ) -> "TabsContent":
+        """Create a new component instance.
+
+        Will prepend "RadixThemes" to the component tag to avoid conflicts with
+        other UI libraries for common names, like Text and Button.
 
         Args:
-            *children: The children of the component.
-            as_child: Change the default rendered element for the one passed as a child.
+            *children: Child components.
+            value: The value of the tab. Must be unique for each tab.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: The props of the component.
+            **props: Component properties.
 
         Returns:
-            The component.
+            A new component instance.
         """
         ...
 
-class SliderThumb(SliderComponent):
-    def add_style(self) -> Style | None: ...
-    @overload
-    @classmethod
-    def create(  # type: ignore
-        cls,
+class Tabs(ComponentNamespace):
+    root = staticmethod(TabsRoot.create)
+    list = staticmethod(TabsList.create)
+    trigger = staticmethod(TabsTrigger.create)
+    content = staticmethod(TabsContent.create)
+
+    @staticmethod
+    def __call__(
         *children,
-        as_child: Optional[Union[Var[bool], bool]] = None,
+        default_value: Optional[Union[Var[str], str]] = None,
+        value: Optional[Union[Var[str], str]] = None,
+        orientation: Optional[
+            Union[
+                Var[Literal["horizontal", "vertical"]],
+                Literal["horizontal", "vertical"],
+            ]
+        ] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_change: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_context_menu: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_double_click: Optional[
@@ -410,36 +480,32 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "SliderThumb":
-        """Create the component.
+    ) -> "TabsRoot":
+        """Create a new component instance.
+
+        Will prepend "RadixThemes" to the component tag to avoid conflicts with
+        other UI libraries for common names, like Text and Button.
 
         Args:
-            *children: The children of the component.
-            as_child: Change the default rendered element for the one passed as a child.
+            *children: Child components.
+            default_value: The value of the tab that should be active when initially rendered. Use when you do not need to control the state of the tabs.
+            value: The controlled value of the tab that should be active. Use when you need to control the state of the tabs.
+            orientation: The orientation of the tabs.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: The props of the component.
+            **props: Component properties.
 
         Returns:
-            The component.
+            A new component instance.
         """
         ...
 
-class Slider(ComponentNamespace):
-    root = staticmethod(SliderRoot.create)
-    track = staticmethod(SliderTrack.create)
-    range = staticmethod(SliderRange.create)
-    thumb = staticmethod(SliderThumb.create)
-
-    @staticmethod
-    def __call__(**props) -> Component: ...
-
-slider = Slider()
+tabs = Tabs()
```

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/base.py` & `reflex-0.5.1a1/reflex/components/radix/themes/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/base.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/color_mode.py` & `reflex-0.5.1a1/reflex/components/radix/themes/color_mode.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/color_mode.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/color_mode.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/__init__.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/alert_dialog.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/alert_dialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/alert_dialog.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/alert_dialog.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/aspect_ratio.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/aspect_ratio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/avatar.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/avatar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/avatar.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/avatar.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/badge.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/badge.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/badge.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/badge.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/button.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/button.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/button.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/callout.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/callout.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/callout.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/callout.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/card.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/card.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/card.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/checkbox.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/checkbox.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/checkbox.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/checkbox_cards.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/checkbox_cards.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/checkbox_cards.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/checkbox_cards.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/checkbox_group.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/checkbox_group.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/checkbox_group.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/checkbox_group.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/context_menu.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/context_menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/context_menu.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/context_menu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/data_list.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/data_list.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/data_list.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/data_list.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/dialog.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/dialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/dialog.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/dialog.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/dropdown_menu.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/dropdown_menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/dropdown_menu.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/dropdown_menu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/hover_card.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/hover_card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/hover_card.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/hover_card.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/icon_button.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/icon_button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/icon_button.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/icon_button.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/inset.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/inset.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/inset.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/inset.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/popover.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/popover.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/popover.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/popover.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/progress.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/progress.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/progress.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/radio.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/radio.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/radio.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/radio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/radio_cards.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/radio_cards.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/radio_cards.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/radio_cards.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/radio_group.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/radio_group.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/radio_group.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/radio_group.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/scroll_area.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/scroll_area.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/scroll_area.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/scroll_area.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/segmented_control.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/segmented_control.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/segmented_control.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/segmented_control.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/select.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/select.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/select.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/select.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/separator.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/separator.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/separator.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/separator.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/skeleton.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/skeleton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/skeleton.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/skeleton.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/slider.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/slider.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/slider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/spinner.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/spinner.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/switch.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/switch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/switch.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/switch.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/table.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/table.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/table.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/table.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/tabs.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/tabs.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
     # The color of the line under the tab when active.
     color_scheme: Var[LiteralAccentColor]
 
     _valid_parents: List[str] = ["TabsList"]
 
     @classmethod
-    def create(self, *children, **props) -> Component:
+    def create(cls, *children, **props) -> Component:
         """Create a TabsTrigger component.
 
         Args:
             *children: The children of the component.
             **props: The properties of the component.
 
         Returns:
```

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/tabs.pyi` & `reflex-0.5.1a1/reflex/components/recharts/general.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,50 @@
-"""Stub file for reflex/components/radix/themes/components/tabs.py"""
+"""Stub file for reflex/components/recharts/general.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Any, Dict, List, Literal
-from reflex.components.component import Component, ComponentNamespace
+from typing import Any, Dict, List, Union
+from reflex.components.component import MemoizationLeaf
 from reflex.constants import EventTriggers
 from reflex.vars import Var
-from ..base import LiteralAccentColor, RadixThemesComponent
+from .recharts import (
+    LiteralIconType,
+    LiteralLayout,
+    LiteralLegendAlign,
+    LiteralPosition,
+    LiteralVerticalAlign,
+    Recharts,
+)
 
-class TabsRoot(RadixThemesComponent):
-    def get_event_triggers(self) -> Dict[str, Any]: ...
+class ResponsiveContainer(Recharts, MemoizationLeaf):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        default_value: Optional[Union[Var[str], str]] = None,
-        value: Optional[Union[Var[str], str]] = None,
-        orientation: Optional[
-            Union[
-                Var[Literal["horizontal", "vertical"]],
-                Literal["horizontal", "vertical"],
-            ]
-        ] = None,
+        aspect: Optional[Union[Var[int], int]] = None,
+        width: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        height: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        min_width: Optional[Union[Var[int], int]] = None,
+        min_height: Optional[Union[Var[int], int]] = None,
+        debounce: Optional[Union[Var[int], int]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_change: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_context_menu: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_double_click: Optional[
@@ -79,72 +80,108 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "TabsRoot":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "ResponsiveContainer":
+        """Create a new memoization leaf component.
 
         Args:
-            *children: Child components.
-            default_value: The value of the tab that should be active when initially rendered. Use when you do not need to control the state of the tabs.
-            value: The controlled value of the tab that should be active. Use when you need to control the state of the tabs.
-            orientation: The orientation of the tabs.
+            *children: The children of the component.
+            aspect: The aspect ratio of the container. The final aspect ratio of the SVG element will be (width / height) * aspect. Number
+            width: The width of chart container. Can be a number or string
+            height: The height of chart container. Number
+            min_width: The minimum width of chart container.
+            min_height: The minimum height of chart container. Number
+            debounce: If specified a positive number, debounced function will be used to handle the resize event.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: The props of the component.
 
         Returns:
-            A new component instance.
+            The memoization leaf
         """
         ...
 
-class TabsList(RadixThemesComponent):
+class Legend(Recharts):
+    def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        size: Optional[Union[Var[Literal["1", "2"]], Literal["1", "2"]]] = None,
+        width: Optional[Union[Var[int], int]] = None,
+        height: Optional[Union[Var[int], int]] = None,
+        layout: Optional[
+            Union[
+                Var[Literal["horizontal", "vertical"]],
+                Literal["horizontal", "vertical"],
+            ]
+        ] = None,
+        align: Optional[
+            Union[
+                Var[Literal["left", "center", "right"]],
+                Literal["left", "center", "right"],
+            ]
+        ] = None,
+        vertical_align: Optional[
+            Union[
+                Var[Literal["top", "middle", "bottom"]],
+                Literal["top", "middle", "bottom"],
+            ]
+        ] = None,
+        icon_size: Optional[Union[Var[int], int]] = None,
+        icon_type: Optional[
+            Union[
+                Var[
+                    Literal[
+                        "line",
+                        "plainline",
+                        "square",
+                        "rect",
+                        "circle",
+                        "cross",
+                        "diamond",
+                        "star",
+                        "triangle",
+                        "wye",
+                    ]
+                ],
+                Literal[
+                    "line",
+                    "plainline",
+                    "square",
+                    "rect",
+                    "circle",
+                    "cross",
+                    "diamond",
+                    "star",
+                    "triangle",
+                    "wye",
+                ],
+            ]
+        ] = None,
+        chart_width: Optional[Union[Var[int], int]] = None,
+        chart_height: Optional[Union[Var[int], int]] = None,
+        margin: Optional[Union[Var[Dict[str, Any]], Dict[str, Any]]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
-        on_blur: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_context_menu: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_double_click: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_focus: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mount: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_down: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_mouse_enter: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_leave: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_move: Optional[
@@ -152,116 +189,57 @@
         ] = None,
         on_mouse_out: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_mouse_up: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_scroll: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_unmount: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         **props
-    ) -> "TabsList":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "Legend":
+        """Create the component.
 
         Args:
-            *children: Child components.
-            size: Tabs size "1" - "2"
+            *children: The children of the component.
+            width: The width of legend container. Number
+            height: The height of legend container. Number
+            layout: The layout of legend items. 'horizontal' | 'vertical'
+            align: The alignment of legend items in 'horizontal' direction, which can be 'left', 'center', 'right'.
+            vertical_align: The alignment of legend items in 'vertical' direction, which can be 'top', 'middle', 'bottom'.
+            icon_size: The size of icon in each legend item.
+            icon_type: The type of icon in each legend item. 'line' | 'plainline' | 'square' | 'rect' | 'circle' | 'cross' | 'diamond' | 'star' | 'triangle' | 'wye'
+            chart_width: The width of chart container, usually calculated internally.
+            chart_height: The height of chart container, usually calculated internally.
+            margin: The margin of chart container, usually calculated internally.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: The props of the component.
 
         Returns:
-            A new component instance.
+            The component.
         """
         ...
 
-class TabsTrigger(RadixThemesComponent):
+class GraphingTooltip(Recharts):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        value: Optional[Union[Var[str], str]] = None,
-        disabled: Optional[Union[Var[bool], bool]] = None,
-        color_scheme: Optional[
-            Union[
-                Var[
-                    Literal[
-                        "tomato",
-                        "red",
-                        "ruby",
-                        "crimson",
-                        "pink",
-                        "plum",
-                        "purple",
-                        "violet",
-                        "iris",
-                        "indigo",
-                        "blue",
-                        "cyan",
-                        "teal",
-                        "jade",
-                        "green",
-                        "grass",
-                        "brown",
-                        "orange",
-                        "sky",
-                        "mint",
-                        "lime",
-                        "yellow",
-                        "amber",
-                        "gold",
-                        "bronze",
-                        "gray",
-                    ]
-                ],
-                Literal[
-                    "tomato",
-                    "red",
-                    "ruby",
-                    "crimson",
-                    "pink",
-                    "plum",
-                    "purple",
-                    "violet",
-                    "iris",
-                    "indigo",
-                    "blue",
-                    "cyan",
-                    "teal",
-                    "jade",
-                    "green",
-                    "grass",
-                    "brown",
-                    "orange",
-                    "sky",
-                    "mint",
-                    "lime",
-                    "yellow",
-                    "amber",
-                    "gold",
-                    "bronze",
-                    "gray",
-                ],
-            ]
-        ] = None,
+        separator: Optional[Union[Var[str], str]] = None,
+        offset: Optional[Union[Var[int], int]] = None,
+        filter_null: Optional[Union[Var[bool], bool]] = None,
+        cursor: Optional[Union[Var[bool], bool]] = None,
+        view_box: Optional[Union[Var[Dict[str, Any]], Dict[str, Any]]] = None,
+        active: Optional[Union[Var[bool], bool]] = None,
+        position: Optional[Union[Var[Dict[str, Any]], Dict[str, Any]]] = None,
+        coordinate: Optional[Union[Var[Dict[str, Any]], Dict[str, Any]]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -306,42 +284,95 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "TabsTrigger":
-        """Create a TabsTrigger component.
+    ) -> "GraphingTooltip":
+        """Create the component.
 
         Args:
             *children: The children of the component.
-            value: The value of the tab. Must be unique for each tab.
-            disabled: Whether the tab is disabled
-            color_scheme: The color of the line under the tab when active.
+            separator: The separator between name and value.
+            offset: The offset size of tooltip. Number
+            filter_null: When an item of the payload has value null or undefined, this item won't be displayed.
+            cursor: If set false, no cursor will be drawn when tooltip is active.
+            view_box: The box of viewing area, which has the shape of {x: someVal, y: someVal, width: someVal, height: someVal}, usually calculated internally.
+            active: If set true, the tooltip is displayed. If set false, the tooltip is hidden, usually calculated internally.
+            position: If this field is set, the tooltip position will be fixed and will not move anymore.
+            coordinate: The coordinate of tooltip which is usually calculated internally.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: The properties of the component.
+            **props: The props of the component.
 
         Returns:
-            The TabsTrigger Component.
+            The component.
         """
         ...
 
-class TabsContent(RadixThemesComponent):
+class Label(Recharts):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
+        view_box: Optional[Union[Var[Dict[str, Any]], Dict[str, Any]]] = None,
         value: Optional[Union[Var[str], str]] = None,
+        offset: Optional[Union[Var[int], int]] = None,
+        position: Optional[
+            Union[
+                Var[
+                    Literal[
+                        "top",
+                        "left",
+                        "right",
+                        "bottom",
+                        "inside",
+                        "outside",
+                        "insideLeft",
+                        "insideRight",
+                        "insideTop",
+                        "insideBottom",
+                        "insideTopLeft",
+                        "insideBottomLeft",
+                        "insideTopRight",
+                        "insideBottomRight",
+                        "insideStart",
+                        "insideEnd",
+                        "end",
+                        "center",
+                    ]
+                ],
+                Literal[
+                    "top",
+                    "left",
+                    "right",
+                    "bottom",
+                    "inside",
+                    "outside",
+                    "insideLeft",
+                    "insideRight",
+                    "insideTop",
+                    "insideBottom",
+                    "insideTopLeft",
+                    "insideBottomLeft",
+                    "insideTopRight",
+                    "insideBottomRight",
+                    "insideStart",
+                    "insideEnd",
+                    "end",
+                    "center",
+                ],
+            ]
+        ] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -386,65 +417,101 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "TabsContent":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "Label":
+        """Create the component.
 
         Args:
-            *children: Child components.
-            value: The value of the tab. Must be unique for each tab.
+            *children: The children of the component.
+            view_box: The box of viewing area, which has the shape of {x: someVal, y: someVal, width: someVal, height: someVal}, usually calculated internally.
+            value: The value of label, which can be specified by this props or the children of <Label />
+            offset: The offset of label which can be specified by this props or the children of <Label />
+            position: The position of label which can be specified by this props or the children of <Label />
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: The props of the component.
 
         Returns:
-            A new component instance.
+            The component.
         """
         ...
 
-class Tabs(ComponentNamespace):
-    root = staticmethod(TabsRoot.create)
-    list = staticmethod(TabsList.create)
-    trigger = staticmethod(TabsTrigger.create)
-    content = staticmethod(TabsContent.create)
-
-    @staticmethod
-    def __call__(
+class LabelList(Recharts):
+    @overload
+    @classmethod
+    def create(  # type: ignore
+        cls,
         *children,
-        default_value: Optional[Union[Var[str], str]] = None,
-        value: Optional[Union[Var[str], str]] = None,
-        orientation: Optional[
+        data_key: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        position: Optional[
             Union[
-                Var[Literal["horizontal", "vertical"]],
-                Literal["horizontal", "vertical"],
+                Var[
+                    Literal[
+                        "top",
+                        "left",
+                        "right",
+                        "bottom",
+                        "inside",
+                        "outside",
+                        "insideLeft",
+                        "insideRight",
+                        "insideTop",
+                        "insideBottom",
+                        "insideTopLeft",
+                        "insideBottomLeft",
+                        "insideTopRight",
+                        "insideBottomRight",
+                        "insideStart",
+                        "insideEnd",
+                        "end",
+                        "center",
+                    ]
+                ],
+                Literal[
+                    "top",
+                    "left",
+                    "right",
+                    "bottom",
+                    "inside",
+                    "outside",
+                    "insideLeft",
+                    "insideRight",
+                    "insideTop",
+                    "insideBottom",
+                    "insideTopLeft",
+                    "insideBottomLeft",
+                    "insideTopRight",
+                    "insideBottomRight",
+                    "insideStart",
+                    "insideEnd",
+                    "end",
+                    "center",
+                ],
             ]
         ] = None,
+        offset: Optional[Union[Var[int], int]] = None,
+        fill: Optional[Union[Var[str], str]] = None,
+        stroke: Optional[Union[Var[str], str]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_change: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_context_menu: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_double_click: Optional[
@@ -480,32 +547,29 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "TabsRoot":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "LabelList":
+        """Create the component.
 
         Args:
-            *children: Child components.
-            default_value: The value of the tab that should be active when initially rendered. Use when you do not need to control the state of the tabs.
-            value: The controlled value of the tab that should be active. Use when you need to control the state of the tabs.
-            orientation: The orientation of the tabs.
+            *children: The children of the component.
+            data_key: The key of a group of label values in data.
+            position: The position of each label relative to it view box。"Top" | "left" | "right" | "bottom" | "inside" | "outside" | "insideLeft" | "insideRight" | "insideTop" | "insideBottom" | "insideTopLeft" | "insideBottomLeft" | "insideTopRight" | "insideBottomRight" | "insideStart" | "insideEnd" | "end" | "center"
+            offset: The offset to the specified "position"
+            fill: Color of the fill
+            stroke: Color of the stroke
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: The props of the component.
 
         Returns:
-            A new component instance.
+            The component.
         """
         ...
-
-tabs = Tabs()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/text_area.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/text_area.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/text_area.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/text_area.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/text_field.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/text_field.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/text_field.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/text_field.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/tooltip.py` & `reflex-0.5.1a1/reflex/components/radix/themes/components/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/components/tooltip.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/components/tooltip.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/layout/__init__.py` & `reflex-0.5.1a1/reflex/components/radix/themes/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/layout/base.py` & `reflex-0.5.1a1/reflex/components/radix/themes/layout/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/layout/base.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/layout/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/layout/box.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/layout/box.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/layout/center.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/layout/center.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/layout/container.py` & `reflex-0.5.1a1/reflex/components/radix/themes/layout/container.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/layout/container.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/layout/container.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/layout/flex.py` & `reflex-0.5.1a1/reflex/components/radix/themes/layout/flex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/layout/flex.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/layout/flex.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/layout/grid.py` & `reflex-0.5.1a1/reflex/components/radix/themes/layout/grid.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/layout/grid.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/layout/grid.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/layout/list.py` & `reflex-0.5.1a1/reflex/components/radix/themes/layout/list.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/layout/list.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/layout/list.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/layout/section.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/layout/section.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/layout/spacer.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/layout/spacer.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/layout/stack.py` & `reflex-0.5.1a1/reflex/components/radix/themes/layout/stack.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/layout/stack.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/layout/stack.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/typography/blockquote.py` & `reflex-0.5.1a1/reflex/components/radix/themes/typography/blockquote.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/typography/blockquote.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/typography/blockquote.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/typography/code.py` & `reflex-0.5.1a1/reflex/components/radix/themes/typography/code.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/typography/code.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/typography/code.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/typography/heading.py` & `reflex-0.5.1a1/reflex/components/radix/themes/typography/heading.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/typography/heading.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/typography/heading.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/typography/link.py` & `reflex-0.5.1a1/reflex/components/radix/themes/typography/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/typography/link.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/typography/link.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/typography/text.py` & `reflex-0.5.1a1/reflex/components/radix/themes/typography/text.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/radix/themes/typography/text.pyi` & `reflex-0.5.1a1/reflex/components/radix/themes/typography/text.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/react_player/audio.pyi` & `reflex-0.5.1a1/reflex/components/react_player/audio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/react_player/react_player.py` & `reflex-0.5.1a1/reflex/components/react_player/react_player.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/react_player/react_player.pyi` & `reflex-0.5.1a1/reflex/components/react_player/react_player.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/react_player/video.pyi` & `reflex-0.5.1a1/reflex/components/react_player/video.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/recharts/__init__.py` & `reflex-0.5.1a1/reflex/components/recharts/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/recharts/cartesian.py` & `reflex-0.5.1a1/reflex/components/recharts/cartesian.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/recharts/cartesian.pyi` & `reflex-0.5.1a1/reflex/components/recharts/cartesian.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/recharts/charts.py` & `reflex-0.5.1a1/reflex/components/recharts/charts.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/recharts/charts.pyi` & `reflex-0.5.1a1/reflex/components/recharts/charts.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/recharts/general.py` & `reflex-0.5.1a1/reflex/components/recharts/general.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/recharts/general.pyi` & `reflex-0.5.1a1/reflex/components/recharts/polar.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,131 @@
-"""Stub file for reflex/components/recharts/general.py"""
+"""Stub file for reflex/components/recharts/polar.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Any, Dict, List, Union
-from reflex.components.component import MemoizationLeaf
 from reflex.constants import EventTriggers
 from reflex.vars import Var
 from .recharts import (
-    LiteralIconType,
-    LiteralLayout,
-    LiteralLegendAlign,
-    LiteralPosition,
-    LiteralVerticalAlign,
+    LiteralAnimationEasing,
+    LiteralGridType,
+    LiteralPolarRadiusType,
+    LiteralScale,
     Recharts,
 )
 
-class ResponsiveContainer(Recharts, MemoizationLeaf):
+class Pie(Recharts):
+    def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        aspect: Optional[Union[Var[int], int]] = None,
-        width: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
-        height: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
-        min_width: Optional[Union[Var[int], int]] = None,
-        min_height: Optional[Union[Var[int], int]] = None,
-        debounce: Optional[Union[Var[int], int]] = None,
+        data: Optional[Union[Var[List[Dict[str, Any]]], List[Dict[str, Any]]]] = None,
+        data_key: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        cx: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        cy: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        inner_radius: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        outer_radius: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        start_angle: Optional[Union[Var[int], int]] = None,
+        end_angle: Optional[Union[Var[int], int]] = None,
+        min_angle: Optional[Union[Var[int], int]] = None,
+        padding_angle: Optional[Union[Var[int], int]] = None,
+        name_key: Optional[Union[Var[str], str]] = None,
+        legend_type: Optional[Union[Var[str], str]] = None,
+        label: Optional[Union[Var[bool], bool]] = None,
+        label_line: Optional[Union[Var[bool], bool]] = None,
+        fill: Optional[Union[Var[str], str]] = None,
+        stroke: Optional[Union[Var[str], str]] = None,
+        style: Optional[Style] = None,
+        key: Optional[Any] = None,
+        id: Optional[Any] = None,
+        class_name: Optional[Any] = None,
+        autofocus: Optional[bool] = None,
+        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
+        on_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_enter: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_leave: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_move: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_out: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_over: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        **props
+    ) -> "Pie":
+        """Create the component.
+
+        Args:
+            *children: The children of the component.
+            data: data
+            data_key: The key of each sector's value.
+            cx: The x-coordinate of center. If set a percentage, the final value is obtained by multiplying the percentage of container width.
+            cy: The y-coordinate of center. If set a percentage, the final value is obtained by multiplying the percentage of container height.
+            inner_radius: The inner radius of pie, which can be set to a percent value.
+            outer_radius: The outer radius of pie, which can be set to a percent value.
+            start_angle: The angle of first sector.
+            end_angle: The direction of sectors. 1 means clockwise and -1 means anticlockwise.
+            min_angle: The minimum angle of each unzero data.
+            padding_angle: The angle between two sectors.
+            name_key: The key of each sector's name.
+            legend_type: The type of icon in legend. If set to 'none', no legend item will be rendered.
+            label: If false set, labels will not be drawn.
+            label_line: If false set, label lines will not be drawn.
+            fill: fill color
+            stroke: stroke color
+            style: The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: The props of the component.
+
+        Returns:
+            The component.
+        """
+        ...
+
+class Radar(Recharts):
+    @overload
+    @classmethod
+    def create(  # type: ignore
+        cls,
+        *children,
+        data_key: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        points: Optional[Union[Var[List[Dict[str, Any]]], List[Dict[str, Any]]]] = None,
+        dot: Optional[Union[Var[bool], bool]] = None,
+        stroke: Optional[Union[Var[str], str]] = None,
+        fill: Optional[Union[Var[str], str]] = None,
+        fill_opacity: Optional[Union[Var[float], float]] = None,
+        legend_type: Optional[Union[Var[str], str]] = None,
+        label: Optional[Union[Var[bool], bool]] = None,
+        animation_begin: Optional[Union[Var[int], int]] = None,
+        animation_duration: Optional[Union[Var[int], int]] = None,
+        animation_easing: Optional[
+            Union[
+                Var[Literal["ease", "ease-in", "ease-out", "ease-in-out", "linear"]],
+                Literal["ease", "ease-in", "ease-out", "ease-in-out", "linear"],
+            ]
+        ] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -80,99 +170,55 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "ResponsiveContainer":
-        """Create a new memoization leaf component.
+    ) -> "Radar":
+        """Create the component.
 
         Args:
             *children: The children of the component.
-            aspect: The aspect ratio of the container. The final aspect ratio of the SVG element will be (width / height) * aspect. Number
-            width: The width of chart container. Can be a number or string
-            height: The height of chart container. Number
-            min_width: The minimum width of chart container.
-            min_height: The minimum height of chart container. Number
-            debounce: If specified a positive number, debounced function will be used to handle the resize event.
+            data_key: The key of a group of data which should be unique in a radar chart.
+            points: The coordinates of all the vertexes of the radar shape, like [{ x, y }].
+            dot: If false set, dots will not be drawn
+            stroke: Stoke color
+            fill: Fill color
+            fill_opacity: opacity
+            legend_type: The type of icon in legend. If set to 'none', no legend item will be rendered.
+            label: If false set, labels will not be drawn
+            animation_begin: Specifies when the animation should begin, the unit of this option is ms.
+            animation_duration: Specifies the duration of animation, the unit of this option is ms.
+            animation_easing: The type of easing function. 'ease' | 'ease-in' | 'ease-out' | 'ease-in-out' | 'linear'
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
-            The memoization leaf
+            The component.
         """
         ...
 
-class Legend(Recharts):
+class RadialBar(Recharts):
     def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        width: Optional[Union[Var[int], int]] = None,
-        height: Optional[Union[Var[int], int]] = None,
-        layout: Optional[
-            Union[
-                Var[Literal["horizontal", "vertical"]],
-                Literal["horizontal", "vertical"],
-            ]
-        ] = None,
-        align: Optional[
-            Union[
-                Var[Literal["left", "center", "right"]],
-                Literal["left", "center", "right"],
-            ]
-        ] = None,
-        vertical_align: Optional[
-            Union[
-                Var[Literal["top", "middle", "bottom"]],
-                Literal["top", "middle", "bottom"],
-            ]
-        ] = None,
-        icon_size: Optional[Union[Var[int], int]] = None,
-        icon_type: Optional[
-            Union[
-                Var[
-                    Literal[
-                        "line",
-                        "plainline",
-                        "square",
-                        "rect",
-                        "circle",
-                        "cross",
-                        "diamond",
-                        "star",
-                        "triangle",
-                        "wye",
-                    ]
-                ],
-                Literal[
-                    "line",
-                    "plainline",
-                    "square",
-                    "rect",
-                    "circle",
-                    "cross",
-                    "diamond",
-                    "star",
-                    "triangle",
-                    "wye",
-                ],
-            ]
-        ] = None,
-        chart_width: Optional[Union[Var[int], int]] = None,
-        chart_height: Optional[Union[Var[int], int]] = None,
-        margin: Optional[Union[Var[Dict[str, Any]], Dict[str, Any]]] = None,
+        data: Optional[Union[Var[List[Dict[str, Any]]], List[Dict[str, Any]]]] = None,
+        min_angle: Optional[Union[Var[int], int]] = None,
+        legend_type: Optional[Union[Var[str], str]] = None,
+        label: Optional[Union[Var[bool], bool]] = None,
+        background: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_click: Optional[
@@ -190,83 +236,68 @@
         on_mouse_out: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "Legend":
+    ) -> "RadialBar":
         """Create the component.
 
         Args:
             *children: The children of the component.
-            width: The width of legend container. Number
-            height: The height of legend container. Number
-            layout: The layout of legend items. 'horizontal' | 'vertical'
-            align: The alignment of legend items in 'horizontal' direction, which can be 'left', 'center', 'right'.
-            vertical_align: The alignment of legend items in 'vertical' direction, which can be 'top', 'middle', 'bottom'.
-            icon_size: The size of icon in each legend item.
-            icon_type: The type of icon in each legend item. 'line' | 'plainline' | 'square' | 'rect' | 'circle' | 'cross' | 'diamond' | 'star' | 'triangle' | 'wye'
-            chart_width: The width of chart container, usually calculated internally.
-            chart_height: The height of chart container, usually calculated internally.
-            margin: The margin of chart container, usually calculated internally.
+            data: The source data which each element is an object.
+            min_angle: Min angle of each bar. A positive value between 0 and 360.
+            legend_type: Type of legend
+            label: If false set, labels will not be drawn.
+            background: If false set, background sector will not be drawn.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
         """
         ...
 
-class GraphingTooltip(Recharts):
+class PolarAngleAxis(Recharts):
+    def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        separator: Optional[Union[Var[str], str]] = None,
-        offset: Optional[Union[Var[int], int]] = None,
-        filter_null: Optional[Union[Var[bool], bool]] = None,
-        cursor: Optional[Union[Var[bool], bool]] = None,
-        view_box: Optional[Union[Var[Dict[str, Any]], Dict[str, Any]]] = None,
-        active: Optional[Union[Var[bool], bool]] = None,
-        position: Optional[Union[Var[Dict[str, Any]], Dict[str, Any]]] = None,
-        coordinate: Optional[Union[Var[Dict[str, Any]], Dict[str, Any]]] = None,
+        data_key: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
+        cx: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        cy: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        radius: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        axis_line: Optional[
+            Union[Var[Union[bool, Dict[str, Any]]], Union[bool, Dict[str, Any]]]
+        ] = None,
+        axis_line_type: Optional[Union[Var[str], str]] = None,
+        tick_line: Optional[
+            Union[Var[Union[bool, Dict[str, Any]]], Union[bool, Dict[str, Any]]]
+        ] = None,
+        tick: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        ticks: Optional[Union[Var[List[Dict[str, Any]]], List[Dict[str, Any]]]] = None,
+        orient: Optional[Union[Var[str], str]] = None,
+        allow_duplicated_category: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
-        on_blur: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_context_menu: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_double_click: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_focus: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mount: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_down: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_mouse_enter: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_leave: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_move: Optional[
@@ -274,104 +305,58 @@
         ] = None,
         on_mouse_out: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_mouse_up: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_scroll: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_unmount: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         **props
-    ) -> "GraphingTooltip":
+    ) -> "PolarAngleAxis":
         """Create the component.
 
         Args:
             *children: The children of the component.
-            separator: The separator between name and value.
-            offset: The offset size of tooltip. Number
-            filter_null: When an item of the payload has value null or undefined, this item won't be displayed.
-            cursor: If set false, no cursor will be drawn when tooltip is active.
-            view_box: The box of viewing area, which has the shape of {x: someVal, y: someVal, width: someVal, height: someVal}, usually calculated internally.
-            active: If set true, the tooltip is displayed. If set false, the tooltip is hidden, usually calculated internally.
-            position: If this field is set, the tooltip position will be fixed and will not move anymore.
-            coordinate: The coordinate of tooltip which is usually calculated internally.
+            data_key: The key of a group of data which should be unique to show the meaning of angle axis.
+            cx: The x-coordinate of center. If set a percentage, the final value is obtained by multiplying the percentage of container width.
+            cy: The y-coordinate of center. If set a percentage, the final value is obtained by multiplying the percentage of container height.
+            radius: The outer radius of circle grid. If set a percentage, the final value is obtained by multiplying the percentage of maxRadius which is calculated by the width, height, cx, cy.
+            axis_line: If false set, axis line will not be drawn. If true set, axis line will be drawn which have the props calculated internally. If object set, axis line will be drawn which have the props mergered by the internal calculated props and the option.
+            axis_line_type: The type of axis line.
+            tick_line: If false set, tick lines will not be drawn. If true set, tick lines will be drawn which have the props calculated internally. If object set, tick lines will be drawn which have the props mergered by the internal calculated props and the option.
+            tick: The width or height of tick.
+            ticks: The array of every tick's value and angle.
+            orient: The orientation of axis text.
+            allow_duplicated_category: Allow the axis has duplicated categorys or not when the type of axis is "category".
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
         """
         ...
 
-class Label(Recharts):
+class PolarGrid(Recharts):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        view_box: Optional[Union[Var[Dict[str, Any]], Dict[str, Any]]] = None,
-        value: Optional[Union[Var[str], str]] = None,
-        offset: Optional[Union[Var[int], int]] = None,
-        position: Optional[
-            Union[
-                Var[
-                    Literal[
-                        "top",
-                        "left",
-                        "right",
-                        "bottom",
-                        "inside",
-                        "outside",
-                        "insideLeft",
-                        "insideRight",
-                        "insideTop",
-                        "insideBottom",
-                        "insideTopLeft",
-                        "insideBottomLeft",
-                        "insideTopRight",
-                        "insideBottomRight",
-                        "insideStart",
-                        "insideEnd",
-                        "end",
-                        "center",
-                    ]
-                ],
-                Literal[
-                    "top",
-                    "left",
-                    "right",
-                    "bottom",
-                    "inside",
-                    "outside",
-                    "insideLeft",
-                    "insideRight",
-                    "insideTop",
-                    "insideBottom",
-                    "insideTopLeft",
-                    "insideBottomLeft",
-                    "insideTopRight",
-                    "insideBottomRight",
-                    "insideStart",
-                    "insideEnd",
-                    "end",
-                    "center",
-                ],
-            ]
+        cx: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        cy: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        inner_radius: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        outer_radius: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        polar_angles: Optional[Union[Var[List[int]], List[int]]] = None,
+        polar_radius: Optional[Union[Var[List[int]], List[int]]] = None,
+        grid_type: Optional[
+            Union[Var[Literal["polygon", "circle"]], Literal["polygon", "circle"]]
         ] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
@@ -417,119 +402,109 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "Label":
+    ) -> "PolarGrid":
         """Create the component.
 
         Args:
             *children: The children of the component.
-            view_box: The box of viewing area, which has the shape of {x: someVal, y: someVal, width: someVal, height: someVal}, usually calculated internally.
-            value: The value of label, which can be specified by this props or the children of <Label />
-            offset: The offset of label which can be specified by this props or the children of <Label />
-            position: The position of label which can be specified by this props or the children of <Label />
+            cx: The x-coordinate of center. If set a percentage, the final value is obtained by multiplying the percentage of container width.
+            cy: The y-coordinate of center. If set a percentage, the final value is obtained by multiplying the percentage of container height.
+            inner_radius: The radius of the inner polar grid.
+            outer_radius: The radius of the outer polar grid.
+            polar_angles: The array of every line grid's angle.
+            polar_radius: The array of every line grid's radius.
+            grid_type: The type of polar grids. 'polygon' | 'circle'
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
         """
         ...
 
-class LabelList(Recharts):
+class PolarRadiusAxis(Recharts):
+    def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        data_key: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
-        position: Optional[
+        angle: Optional[Union[Var[int], int]] = None,
+        type_: Optional[
+            Union[Var[Literal["number", "category"]], Literal["number", "category"]]
+        ] = None,
+        allow_duplicated_category: Optional[Union[Var[bool], bool]] = None,
+        cx: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        cy: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        reversed: Optional[Union[Var[bool], bool]] = None,
+        orientation: Optional[Union[Var[str], str]] = None,
+        axis_line: Optional[
+            Union[Var[Union[bool, Dict[str, Any]]], Union[bool, Dict[str, Any]]]
+        ] = None,
+        tick: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
+        tick_count: Optional[Union[Var[int], int]] = None,
+        scale: Optional[
             Union[
                 Var[
                     Literal[
-                        "top",
-                        "left",
-                        "right",
-                        "bottom",
-                        "inside",
-                        "outside",
-                        "insideLeft",
-                        "insideRight",
-                        "insideTop",
-                        "insideBottom",
-                        "insideTopLeft",
-                        "insideBottomLeft",
-                        "insideTopRight",
-                        "insideBottomRight",
-                        "insideStart",
-                        "insideEnd",
-                        "end",
-                        "center",
+                        "auto",
+                        "linear",
+                        "pow",
+                        "sqrt",
+                        "log",
+                        "identity",
+                        "time",
+                        "band",
+                        "point",
+                        "ordinal",
+                        "quantile",
+                        "quantize",
+                        "utc",
+                        "sequential",
+                        "threshold",
                     ]
                 ],
                 Literal[
-                    "top",
-                    "left",
-                    "right",
-                    "bottom",
-                    "inside",
-                    "outside",
-                    "insideLeft",
-                    "insideRight",
-                    "insideTop",
-                    "insideBottom",
-                    "insideTopLeft",
-                    "insideBottomLeft",
-                    "insideTopRight",
-                    "insideBottomRight",
-                    "insideStart",
-                    "insideEnd",
-                    "end",
-                    "center",
+                    "auto",
+                    "linear",
+                    "pow",
+                    "sqrt",
+                    "log",
+                    "identity",
+                    "time",
+                    "band",
+                    "point",
+                    "ordinal",
+                    "quantile",
+                    "quantize",
+                    "utc",
+                    "sequential",
+                    "threshold",
                 ],
             ]
         ] = None,
-        offset: Optional[Union[Var[int], int]] = None,
-        fill: Optional[Union[Var[str], str]] = None,
-        stroke: Optional[Union[Var[str], str]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
-        on_blur: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_context_menu: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_double_click: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_focus: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mount: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_mouse_down: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         on_mouse_enter: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_leave: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_move: Optional[
@@ -537,34 +512,31 @@
         ] = None,
         on_mouse_out: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        on_mouse_up: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_scroll: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_unmount: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
         **props
-    ) -> "LabelList":
+    ) -> "PolarRadiusAxis":
         """Create the component.
 
         Args:
             *children: The children of the component.
-            data_key: The key of a group of label values in data.
-            position: The position of each label relative to it view box。"Top" | "left" | "right" | "bottom" | "inside" | "outside" | "insideLeft" | "insideRight" | "insideTop" | "insideBottom" | "insideTopLeft" | "insideBottomLeft" | "insideTopRight" | "insideBottomRight" | "insideStart" | "insideEnd" | "end" | "center"
-            offset: The offset to the specified "position"
-            fill: Color of the fill
-            stroke: Color of the stroke
+            angle: The angle of radial direction line to display axis text.
+            type_: The type of axis line. 'number' | 'category'
+            allow_duplicated_category: Allow the axis has duplicated categorys or not when the type of axis is "category".
+            cx: The x-coordinate of center.
+            cy: The y-coordinate of center.
+            reversed: If set to true, the ticks of this axis are reversed.
+            orientation: The orientation of axis text.
+            axis_line: If false set, axis line will not be drawn. If true set, axis line will be drawn which have the props calculated internally. If object set, axis line will be drawn which have the props mergered by the internal calculated props and the option.
+            tick: The width or height of tick.
+            tick_count: The count of ticks.
+            scale: If 'auto' set, the scale funtion is linear scale. 'auto' | 'linear' | 'pow' | 'sqrt' | 'log' | 'identity' | 'time' | 'band' | 'point' | 'ordinal' | 'quantile' | 'quantize' | 'utc' | 'sequential' | 'threshold'
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `reflex-0.5.0a3/reflex/components/recharts/polar.py` & `reflex-0.5.1a1/reflex/components/recharts/polar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/recharts/polar.pyi` & `reflex-0.5.1a1/reflex/components/core/banner.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,77 @@
-"""Stub file for reflex/components/recharts/polar.py"""
+"""Stub file for reflex/components/core/banner.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Any, Dict, List, Union
-from reflex.constants import EventTriggers
-from reflex.vars import Var
-from .recharts import (
-    LiteralAnimationEasing,
-    LiteralGridType,
-    LiteralPolarRadiusType,
-    LiteralScale,
-    Recharts,
+from typing import Optional
+from reflex.components.base.bare import Bare
+from reflex.components.component import Component
+from reflex.components.core.cond import cond
+from reflex.components.el.elements.typography import Div
+from reflex.components.lucide.icon import Icon
+from reflex.components.radix.themes.components.dialog import (
+    DialogContent,
+    DialogRoot,
+    DialogTitle,
 )
+from reflex.components.radix.themes.layout import Flex
+from reflex.components.radix.themes.typography.text import Text
+from reflex.components.sonner.toast import Toaster, ToastProps
+from reflex.constants import Dirs, Hooks, Imports
+from reflex.constants.compiler import CompileVars
+from reflex.utils import imports
+from reflex.utils.serializers import serialize
+from reflex.vars import Var, VarData
+
+connect_error_var_data: VarData
+connect_errors: Var
+connection_error: Var
+connection_errors_count: Var
+has_connection_errors: Var
+has_too_many_connection_errors: Var
 
-class Pie(Recharts):
-    def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
+class WebsocketTargetURL(Bare):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        data: Optional[Union[Var[List[Dict[str, Any]]], List[Dict[str, Any]]]] = None,
-        data_key: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
-        cx: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
-        cy: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
-        inner_radius: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
-        outer_radius: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
-        start_angle: Optional[Union[Var[int], int]] = None,
-        end_angle: Optional[Union[Var[int], int]] = None,
-        min_angle: Optional[Union[Var[int], int]] = None,
-        padding_angle: Optional[Union[Var[int], int]] = None,
-        name_key: Optional[Union[Var[str], str]] = None,
-        legend_type: Optional[Union[Var[str], str]] = None,
-        label: Optional[Union[Var[bool], bool]] = None,
-        label_line: Optional[Union[Var[bool], bool]] = None,
-        fill: Optional[Union[Var[str], str]] = None,
-        stroke: Optional[Union[Var[str], str]] = None,
+        contents: Optional[Union[Var[str], str]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
+        on_blur: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_context_menu: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_double_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_focus: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mount: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_down: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_mouse_enter: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_leave: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_move: Optional[
@@ -61,71 +79,76 @@
         ] = None,
         on_mouse_out: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_mouse_up: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_scroll: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_unmount: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         **props
-    ) -> "Pie":
-        """Create the component.
-
-        Args:
-            *children: The children of the component.
-            data: data
-            data_key: The key of each sector's value.
-            cx: The x-coordinate of center. If set a percentage, the final value is obtained by multiplying the percentage of container width.
-            cy: The y-coordinate of center. If set a percentage, the final value is obtained by multiplying the percentage of container height.
-            inner_radius: The inner radius of pie, which can be set to a percent value.
-            outer_radius: The outer radius of pie, which can be set to a percent value.
-            start_angle: The angle of first sector.
-            end_angle: The direction of sectors. 1 means clockwise and -1 means anticlockwise.
-            min_angle: The minimum angle of each unzero data.
-            padding_angle: The angle between two sectors.
-            name_key: The key of each sector's name.
-            legend_type: The type of icon in legend. If set to 'none', no legend item will be rendered.
-            label: If false set, labels will not be drawn.
-            label_line: If false set, label lines will not be drawn.
-            fill: fill color
-            stroke: stroke color
-            style: The style of the component.
-            key: A unique key for the component.
-            id: The id for the component.
-            class_name: The class name for the component.
-            autofocus: Whether the component should take the focus once the page is loaded
-            custom_attrs: custom attribute
-            **props: The props of the component.
+    ) -> "WebsocketTargetURL":
+        """Create a websocket target URL component.
 
         Returns:
-            The component.
+            The websocket target URL component.
         """
         ...
 
-class Radar(Recharts):
+def default_connection_error() -> list[str | Var | Component]: ...
+
+class ConnectionToaster(Toaster):
+    def add_hooks(self) -> list[str]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        data_key: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
-        points: Optional[Union[Var[List[Dict[str, Any]]], List[Dict[str, Any]]]] = None,
-        dot: Optional[Union[Var[bool], bool]] = None,
-        stroke: Optional[Union[Var[str], str]] = None,
-        fill: Optional[Union[Var[str], str]] = None,
-        fill_opacity: Optional[Union[Var[float], float]] = None,
-        legend_type: Optional[Union[Var[str], str]] = None,
-        label: Optional[Union[Var[bool], bool]] = None,
-        animation_begin: Optional[Union[Var[int], int]] = None,
-        animation_duration: Optional[Union[Var[int], int]] = None,
-        animation_easing: Optional[
+        theme: Optional[Union[Var[str], str]] = None,
+        rich_colors: Optional[Union[Var[bool], bool]] = None,
+        expand: Optional[Union[Var[bool], bool]] = None,
+        visible_toasts: Optional[Union[Var[int], int]] = None,
+        position: Optional[
             Union[
-                Var[Literal["ease", "ease-in", "ease-out", "ease-in-out", "linear"]],
-                Literal["ease", "ease-in", "ease-out", "ease-in-out", "linear"],
+                Var[
+                    Literal[
+                        "top-left",
+                        "top-center",
+                        "top-right",
+                        "bottom-left",
+                        "bottom-center",
+                        "bottom-right",
+                    ]
+                ],
+                Literal[
+                    "top-left",
+                    "top-center",
+                    "top-right",
+                    "bottom-left",
+                    "bottom-center",
+                    "bottom-right",
+                ],
             ]
         ] = None,
+        close_button: Optional[Union[Var[bool], bool]] = None,
+        offset: Optional[Union[Var[str], str]] = None,
+        dir: Optional[Union[Var[str], str]] = None,
+        hotkey: Optional[Union[Var[str], str]] = None,
+        invert: Optional[Union[Var[bool], bool]] = None,
+        toast_options: Optional[Union[Var[ToastProps], ToastProps]] = None,
+        gap: Optional[Union[Var[int], int]] = None,
+        loading_icon: Optional[Union[Var[Icon], Icon]] = None,
+        pause_when_page_is_hidden: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -170,64 +193,79 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "Radar":
+    ) -> "ConnectionToaster":
         """Create the component.
 
         Args:
             *children: The children of the component.
-            data_key: The key of a group of data which should be unique in a radar chart.
-            points: The coordinates of all the vertexes of the radar shape, like [{ x, y }].
-            dot: If false set, dots will not be drawn
-            stroke: Stoke color
-            fill: Fill color
-            fill_opacity: opacity
-            legend_type: The type of icon in legend. If set to 'none', no legend item will be rendered.
-            label: If false set, labels will not be drawn
-            animation_begin: Specifies when the animation should begin, the unit of this option is ms.
-            animation_duration: Specifies the duration of animation, the unit of this option is ms.
-            animation_easing: The type of easing function. 'ease' | 'ease-in' | 'ease-out' | 'ease-in-out' | 'linear'
+            theme: the theme of the toast
+            rich_colors: whether to show rich colors
+            expand: whether to expand the toast
+            visible_toasts: the number of toasts that are currently visible
+            position: the position of the toast
+            close_button: whether to show the close button
+            offset: offset of the toast
+            dir: directionality of the toast (default: ltr)
+            hotkey: Keyboard shortcut that will move focus to the toaster area.
+            invert: Dark toasts in light mode and vice versa.
+            toast_options: These will act as default options for all toasts. See toast() for all available options.
+            gap: Gap between toasts when expanded
+            loading_icon: Changes the default loading icon
+            pause_when_page_is_hidden: Pauses toast timers when the page is hidden, e.g., when the tab is backgrounded, the browser is minimized, or the OS is locked.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
         """
         ...
 
-class RadialBar(Recharts):
-    def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
+class ConnectionBanner(Component):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        data: Optional[Union[Var[List[Dict[str, Any]]], List[Dict[str, Any]]]] = None,
-        min_angle: Optional[Union[Var[int], int]] = None,
-        legend_type: Optional[Union[Var[str], str]] = None,
-        label: Optional[Union[Var[bool], bool]] = None,
-        background: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
+        on_blur: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_context_menu: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_double_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_focus: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mount: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_down: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_mouse_enter: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_leave: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_move: Optional[
@@ -235,69 +273,68 @@
         ] = None,
         on_mouse_out: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_mouse_up: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_scroll: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_unmount: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         **props
-    ) -> "RadialBar":
-        """Create the component.
+    ) -> "ConnectionBanner":
+        """Create a connection banner component.
 
         Args:
-            *children: The children of the component.
-            data: The source data which each element is an object.
-            min_angle: Min angle of each bar. A positive value between 0 and 360.
-            legend_type: Type of legend
-            label: If false set, labels will not be drawn.
-            background: If false set, background sector will not be drawn.
-            style: The style of the component.
-            key: A unique key for the component.
-            id: The id for the component.
-            class_name: The class name for the component.
-            autofocus: Whether the component should take the focus once the page is loaded
-            custom_attrs: custom attribute
-            **props: The props of the component.
+            comp: The component to render when there's a server connection error.
 
         Returns:
-            The component.
+            The connection banner component.
         """
         ...
 
-class PolarAngleAxis(Recharts):
-    def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
+class ConnectionModal(Component):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        data_key: Optional[Union[Var[Union[str, int]], Union[str, int]]] = None,
-        cx: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
-        cy: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
-        radius: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
-        axis_line: Optional[
-            Union[Var[Union[bool, Dict[str, Any]]], Union[bool, Dict[str, Any]]]
-        ] = None,
-        axis_line_type: Optional[Union[Var[str], str]] = None,
-        tick_line: Optional[
-            Union[Var[Union[bool, Dict[str, Any]]], Union[bool, Dict[str, Any]]]
-        ] = None,
-        tick: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
-        ticks: Optional[Union[Var[List[Dict[str, Any]]], List[Dict[str, Any]]]] = None,
-        orient: Optional[Union[Var[str], str]] = None,
-        allow_duplicated_category: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
+        on_blur: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_context_menu: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_double_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_focus: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mount: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_down: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_mouse_enter: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_leave: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_move: Optional[
@@ -305,59 +342,42 @@
         ] = None,
         on_mouse_out: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_mouse_up: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_scroll: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_unmount: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         **props
-    ) -> "PolarAngleAxis":
-        """Create the component.
+    ) -> "ConnectionModal":
+        """Create a connection banner component.
 
         Args:
-            *children: The children of the component.
-            data_key: The key of a group of data which should be unique to show the meaning of angle axis.
-            cx: The x-coordinate of center. If set a percentage, the final value is obtained by multiplying the percentage of container width.
-            cy: The y-coordinate of center. If set a percentage, the final value is obtained by multiplying the percentage of container height.
-            radius: The outer radius of circle grid. If set a percentage, the final value is obtained by multiplying the percentage of maxRadius which is calculated by the width, height, cx, cy.
-            axis_line: If false set, axis line will not be drawn. If true set, axis line will be drawn which have the props calculated internally. If object set, axis line will be drawn which have the props mergered by the internal calculated props and the option.
-            axis_line_type: The type of axis line.
-            tick_line: If false set, tick lines will not be drawn. If true set, tick lines will be drawn which have the props calculated internally. If object set, tick lines will be drawn which have the props mergered by the internal calculated props and the option.
-            tick: The width or height of tick.
-            ticks: The array of every tick's value and angle.
-            orient: The orientation of axis text.
-            allow_duplicated_category: Allow the axis has duplicated categorys or not when the type of axis is "category".
-            style: The style of the component.
-            key: A unique key for the component.
-            id: The id for the component.
-            class_name: The class name for the component.
-            autofocus: Whether the component should take the focus once the page is loaded
-            custom_attrs: custom attribute
-            **props: The props of the component.
+            comp: The component to render when there's a server connection error.
 
         Returns:
-            The component.
+            The connection banner component.
         """
         ...
 
-class PolarGrid(Recharts):
+class WifiOffPulse(Icon):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        cx: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
-        cy: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
-        inner_radius: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
-        outer_radius: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
-        polar_angles: Optional[Union[Var[List[int]], List[int]]] = None,
-        polar_radius: Optional[Union[Var[List[int]], List[int]]] = None,
-        grid_type: Optional[
-            Union[Var[Literal["polygon", "circle"]], Literal["polygon", "circle"]]
-        ] = None,
+        size: Optional[Union[Var[int], int]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -402,109 +422,105 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "PolarGrid":
-        """Create the component.
+    ) -> "WifiOffPulse":
+        """Create a wifi_off icon with an animated opacity pulse.
 
         Args:
-            *children: The children of the component.
-            cx: The x-coordinate of center. If set a percentage, the final value is obtained by multiplying the percentage of container width.
-            cy: The y-coordinate of center. If set a percentage, the final value is obtained by multiplying the percentage of container height.
-            inner_radius: The radius of the inner polar grid.
-            outer_radius: The radius of the outer polar grid.
-            polar_angles: The array of every line grid's angle.
-            polar_radius: The array of every line grid's radius.
-            grid_type: The type of polar grids. 'polygon' | 'circle'
+            size: The size of the icon in pixels.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: The props of the component.
+            **props: The properties of the component.
 
         Returns:
-            The component.
+            The icon component with default props applied.
         """
         ...
 
-class PolarRadiusAxis(Recharts):
-    def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
+class ConnectionPulser(Div):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        angle: Optional[Union[Var[int], int]] = None,
-        type_: Optional[
-            Union[Var[Literal["number", "category"]], Literal["number", "category"]]
-        ] = None,
-        allow_duplicated_category: Optional[Union[Var[bool], bool]] = None,
-        cx: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
-        cy: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
-        reversed: Optional[Union[Var[bool], bool]] = None,
-        orientation: Optional[Union[Var[str], str]] = None,
-        axis_line: Optional[
-            Union[Var[Union[bool, Dict[str, Any]]], Union[bool, Dict[str, Any]]]
-        ] = None,
-        tick: Optional[Union[Var[Union[int, str]], Union[int, str]]] = None,
-        tick_count: Optional[Union[Var[int], int]] = None,
-        scale: Optional[
-            Union[
-                Var[
-                    Literal[
-                        "auto",
-                        "linear",
-                        "pow",
-                        "sqrt",
-                        "log",
-                        "identity",
-                        "time",
-                        "band",
-                        "point",
-                        "ordinal",
-                        "quantile",
-                        "quantize",
-                        "utc",
-                        "sequential",
-                        "threshold",
-                    ]
-                ],
-                Literal[
-                    "auto",
-                    "linear",
-                    "pow",
-                    "sqrt",
-                    "log",
-                    "identity",
-                    "time",
-                    "band",
-                    "point",
-                    "ordinal",
-                    "quantile",
-                    "quantize",
-                    "utc",
-                    "sequential",
-                    "threshold",
-                ],
-            ]
+        access_key: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        auto_capitalize: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        content_editable: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        context_menu: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        dir: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        draggable: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        enter_key_hint: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        hidden: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        input_mode: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        item_prop: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        lang: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        role: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        slot: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        spell_check: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        tab_index: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        ] = None,
+        title: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
+        on_blur: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_context_menu: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_double_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_focus: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mount: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_down: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_mouse_enter: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_leave: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_move: Optional[
@@ -512,36 +528,49 @@
         ] = None,
         on_mouse_out: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_mouse_up: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_scroll: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_unmount: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         **props
-    ) -> "PolarRadiusAxis":
-        """Create the component.
+    ) -> "ConnectionPulser":
+        """Create a connection pulser component.
 
         Args:
-            *children: The children of the component.
-            angle: The angle of radial direction line to display axis text.
-            type_: The type of axis line. 'number' | 'category'
-            allow_duplicated_category: Allow the axis has duplicated categorys or not when the type of axis is "category".
-            cx: The x-coordinate of center.
-            cy: The y-coordinate of center.
-            reversed: If set to true, the ticks of this axis are reversed.
-            orientation: The orientation of axis text.
-            axis_line: If false set, axis line will not be drawn. If true set, axis line will be drawn which have the props calculated internally. If object set, axis line will be drawn which have the props mergered by the internal calculated props and the option.
-            tick: The width or height of tick.
-            tick_count: The count of ticks.
-            scale: If 'auto' set, the scale funtion is linear scale. 'auto' | 'linear' | 'pow' | 'sqrt' | 'log' | 'identity' | 'time' | 'band' | 'point' | 'ordinal' | 'quantile' | 'quantize' | 'utc' | 'sequential' | 'threshold'
+            access_key:  Provides a hint for generating a keyboard shortcut for the current element.
+            auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
+            content_editable: Indicates whether the element's content is editable.
+            context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
+            dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
+            draggable: Defines whether the element can be dragged.
+            enter_key_hint: Hints what media types the media element is able to play.
+            hidden: Defines whether the element is hidden.
+            input_mode: Defines the type of the element.
+            item_prop: Defines the name of the element for metadata purposes.
+            lang: Defines the language used in the element.
+            role: Defines the role of the element.
+            slot: Assigns a slot in a shadow DOM shadow tree to an element.
+            spell_check: Defines whether the element may be checked for spelling errors.
+            tab_index: Defines the position of the current element in the tabbing order.
+            title: Defines a tooltip for the element.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: The props of the component.
+            **props: The properties of the component.
 
         Returns:
-            The component.
+            The connection pulser component.
         """
         ...
```

### Comparing `reflex-0.5.0a3/reflex/components/recharts/recharts.py` & `reflex-0.5.1a1/reflex/components/recharts/recharts.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/recharts/recharts.pyi` & `reflex-0.5.1a1/reflex/components/recharts/recharts.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/sonner/toast.py` & `reflex-0.5.1a1/reflex/components/sonner/toast.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 """Sonner toast component."""
 
 from __future__ import annotations
 
-from typing import Literal
+from typing import Any, Literal, Optional, Union
 
 from reflex.base import Base
 from reflex.components.component import Component, ComponentNamespace
 from reflex.components.lucide.icon import Icon
-from reflex.event import EventSpec, call_script
+from reflex.components.props import PropsBase
+from reflex.event import (
+    EventSpec,
+    call_script,
+)
 from reflex.style import Style, color_mode
 from reflex.utils import format
 from reflex.utils.imports import ImportVar
-from reflex.utils.serializers import serialize
+from reflex.utils.serializers import serialize, serializer
 from reflex.vars import Var, VarData
 
 LiteralPosition = Literal[
     "top-left",
     "top-center",
     "top-right",
     "bottom-left",
@@ -23,86 +27,146 @@
     "bottom-right",
 ]
 
 
 toast_ref = Var.create_safe("refs['__toast']")
 
 
-class PropsBase(Base):
-    """Base class for all props classes."""
+class ToastAction(Base):
+    """A toast action that render a button in the toast."""
 
-    def json(self) -> str:
-        """Convert the object to a json string.
+    label: str
+    on_click: Any
 
-        Returns:
-            The object as a json string.
-        """
-        from reflex.utils.serializers import serialize
 
-        return self.__config__.json_dumps(
-            {format.to_camel_case(key): value for key, value in self.dict().items()},
-            default=serialize,
+@serializer
+def serialize_action(action: ToastAction) -> dict:
+    """Serialize a toast action.
+
+    Args:
+        action: The toast action to serialize.
+
+    Returns:
+        The serialized toast action with on_click formatted to queue the given event.
+    """
+    return {
+        "label": action.label,
+        "onClick": format.format_queue_events(action.on_click),
+    }
+
+
+def _toast_callback_signature(toast: Var) -> list[Var]:
+    """The signature for the toast callback, stripping out unserializable keys.
+
+    Args:
+        toast: The toast variable.
+
+    Returns:
+        A function call stripping non-serializable members of the toast object.
+    """
+    return [
+        Var.create_safe(
+            f"(() => {{let {{action, cancel, onDismiss, onAutoClose, ...rest}} = {toast}; return rest}})()"
         )
+    ]
 
 
 class ToastProps(PropsBase):
     """Props for the toast component."""
 
     # Toast's description, renders underneath the title.
-    description: str = ""
+    description: Optional[Union[str, Var]]
 
     # Whether to show the close button.
-    close_button: bool = False
+    close_button: Optional[bool]
 
     # Dark toast in light mode and vice versa.
-    invert: bool = False
+    invert: Optional[bool]
 
     # Control the sensitivity of the toast for screen readers
-    important: bool = False
+    important: Optional[bool]
 
     # Time in milliseconds that should elapse before automatically closing the toast.
-    duration: int = 4000
+    duration: Optional[int]
 
     # Position of the toast.
-    position: LiteralPosition = "bottom-right"
+    position: Optional[LiteralPosition]
 
     # If false, it'll prevent the user from dismissing the toast.
-    dismissible: bool = True
+    dismissible: Optional[bool]
 
     # TODO: fix serialization of icons for toast? (might not be possible yet)
     # Icon displayed in front of toast's text, aligned vertically.
     # icon: Optional[Icon] = None
 
     # TODO: fix implementation for action / cancel buttons
     # Renders a primary button, clicking it will close the toast.
-    # action: str = ""
+    action: Optional[ToastAction]
 
     # Renders a secondary button, clicking it will close the toast.
-    # cancel: str = ""
+    cancel: Optional[ToastAction]
 
     # Custom id for the toast.
-    id: str = ""
+    id: Optional[str]
 
     # Removes the default styling, which allows for easier customization.
-    unstyled: bool = False
+    unstyled: Optional[bool]
 
     # Custom style for the toast.
-    style: Style = Style()
+    style: Optional[Style]
 
+    # XXX: These still do not seem to work
     # Custom style for the toast primary button.
-    # action_button_styles: Style = Style()
+    action_button_styles: Optional[Style]
 
     # Custom style for the toast secondary button.
-    # cancel_button_styles: Style = Style()
+    cancel_button_styles: Optional[Style]
+
+    # The function gets called when either the close button is clicked, or the toast is swiped.
+    on_dismiss: Optional[Any]
+
+    # Function that gets called when the toast disappears automatically after it's timeout (duration` prop).
+    on_auto_close: Optional[Any]
+
+    def dict(self, *args, **kwargs) -> dict:
+        """Convert the object to a dictionary.
+
+        Args:
+            *args: The arguments to pass to the base class.
+            **kwargs: The keyword arguments to pass to the base
+
+        Returns:
+            The object as a dictionary with ToastAction fields intact.
+        """
+        kwargs.setdefault("exclude_none", True)
+        d = super().dict(*args, **kwargs)
+        # Keep these fields as ToastAction so they can be serialized specially
+        if "action" in d:
+            d["action"] = self.action
+            if isinstance(self.action, dict):
+                d["action"] = ToastAction(**self.action)
+        if "cancel" in d:
+            d["cancel"] = self.cancel
+            if isinstance(self.cancel, dict):
+                d["cancel"] = ToastAction(**self.cancel)
+        if "on_dismiss" in d:
+            d["on_dismiss"] = format.format_queue_events(
+                self.on_dismiss, _toast_callback_signature
+            )
+        if "on_auto_close" in d:
+            d["on_auto_close"] = format.format_queue_events(
+                self.on_auto_close, _toast_callback_signature
+            )
+        return d
 
 
 class Toaster(Component):
     """A Toaster Component for displaying toast notifications."""
 
-    library = "sonner@1.4.41"
+    library: str = "sonner@1.4.41"
 
     tag = "Toaster"
 
     # the theme of the toast
     theme: Var[str] = color_mode
 
     # whether to show rich colors
@@ -141,20 +205,23 @@
     # Changes the default loading icon
     loading_icon: Var[Icon]
 
     # Pauses toast timers when the page is hidden, e.g., when the tab is backgrounded, the browser is minimized, or the OS is locked.
     pause_when_page_is_hidden: Var[bool]
 
     def _get_hooks(self) -> Var[str]:
-        hook = Var.create_safe(f"{toast_ref} = toast", _var_is_local=True)
-        hook._var_data = VarData(  # type: ignore
-            imports={
-                "/utils/state": [ImportVar(tag="refs")],
-                self.library: [ImportVar(tag="toast", install=False)],
-            }
+        hook = Var.create_safe(
+            f"{toast_ref} = toast",
+            _var_is_local=True,
+            _var_data=VarData(
+                imports={
+                    "/utils/state": [ImportVar(tag="refs")],
+                    self.library: [ImportVar(tag="toast", install=False)],
+                }
+            ),
         )
         return hook
 
     @staticmethod
     def send_toast(message: str, level: str | None = None, **props) -> EventSpec:
         """Send a toast message.
```

### Comparing `reflex-0.5.0a3/reflex/components/sonner/toast.pyi` & `reflex-0.5.1a1/reflex/components/sonner/toast.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -3,49 +3,62 @@
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Literal
+from typing import Any, Literal, Optional, Union
 from reflex.base import Base
 from reflex.components.component import Component, ComponentNamespace
 from reflex.components.lucide.icon import Icon
+from reflex.components.props import PropsBase
 from reflex.event import EventSpec, call_script
 from reflex.style import Style, color_mode
 from reflex.utils import format
 from reflex.utils.imports import ImportVar
-from reflex.utils.serializers import serialize
+from reflex.utils.serializers import serialize, serializer
 from reflex.vars import Var, VarData
 
 LiteralPosition = Literal[
     "top-left",
     "top-center",
     "top-right",
     "bottom-left",
     "bottom-center",
     "bottom-right",
 ]
 toast_ref = Var.create_safe("refs['__toast']")
 
-class PropsBase(Base):
-    def json(self) -> str: ...
+class ToastAction(Base):
+    label: str
+    on_click: Any
+
+@serializer
+def serialize_action(action: ToastAction) -> dict: ...
 
 class ToastProps(PropsBase):
-    description: str
-    close_button: bool
-    invert: bool
-    important: bool
-    duration: int
-    position: LiteralPosition
-    dismissible: bool
-    id: str
-    unstyled: bool
-    style: Style
+    description: Optional[Union[str, Var]]
+    close_button: Optional[bool]
+    invert: Optional[bool]
+    important: Optional[bool]
+    duration: Optional[int]
+    position: Optional[LiteralPosition]
+    dismissible: Optional[bool]
+    action: Optional[ToastAction]
+    cancel: Optional[ToastAction]
+    id: Optional[str]
+    unstyled: Optional[bool]
+    style: Optional[Style]
+    action_button_styles: Optional[Style]
+    cancel_button_styles: Optional[Style]
+    on_dismiss: Optional[Any]
+    on_auto_close: Optional[Any]
+
+    def dict(self, *args, **kwargs) -> dict: ...
 
 class Toaster(Component):
     @staticmethod
     def send_toast(message: str, level: str | None = None, **props) -> EventSpec: ...
     @staticmethod
     def toast_info(message: str, **kwargs): ...
     @staticmethod
```

### Comparing `reflex-0.5.0a3/reflex/components/suneditor/editor.py` & `reflex-0.5.1a1/reflex/components/suneditor/editor.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/suneditor/editor.pyi` & `reflex-0.5.1a1/reflex/components/suneditor/editor.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/tags/iter_tag.py` & `reflex-0.5.1a1/reflex/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/tags/tag.py` & `reflex-0.5.1a1/reflex/components/tags/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/components/tags/tagless.py` & `reflex-0.5.1a1/reflex/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/config.py` & `reflex-0.5.1a1/reflex/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,16 +247,18 @@
     def update_from_env(self) -> dict[str, Any]:
         """Update the config values based on set environment variables.
 
         Returns:
             The updated config values.
 
         Raises:
-            ValueError: If an environment variable is set to an invalid type.
+            EnvVarValueError: If an environment variable is set to an invalid type.
         """
+        from reflex.utils.exceptions import EnvVarValueError
+
         updated_values = {}
         # Iterate over the fields.
         for key, field in self.__fields__.items():
             # The env var name is the key in uppercase.
             env_var = os.environ.get(key.upper())
 
             # If the env var is set, override the config value.
@@ -269,19 +271,19 @@
                 # Convert the env var to the expected type.
                 try:
                     if issubclass(field.type_, bool):
                         # special handling for bool values
                         env_var = env_var.lower() in ["true", "1", "yes"]
                     else:
                         env_var = field.type_(env_var)
-                except ValueError:
+                except ValueError as ve:
                     console.error(
                         f"Could not convert {key.upper()}={env_var} to type {field.type_}"
                     )
-                    raise
+                    raise EnvVarValueError from ve
 
                 # Set the value.
                 updated_values[key] = env_var
 
         return updated_values
 
     def get_event_namespace(self) -> str:
```

### Comparing `reflex-0.5.0a3/reflex/config.pyi` & `reflex-0.5.1a1/reflex/config.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/constants/__init__.py` & `reflex-0.5.1a1/reflex/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/constants/base.py` & `reflex-0.5.1a1/reflex/constants/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/constants/base.pyi` & `reflex-0.5.1a1/reflex/constants/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/constants/colors.py` & `reflex-0.5.1a1/reflex/constants/colors.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/constants/compiler.py` & `reflex-0.5.1a1/reflex/constants/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,17 +99,17 @@
         return self.value.lower() + Ext.ZIP
 
 
 class Imports(SimpleNamespace):
     """Common sets of import vars."""
 
     EVENTS = {
-        "react": {ImportVar(tag="useContext")},
-        f"/{Dirs.CONTEXTS_PATH}": {ImportVar(tag="EventLoopContext")},
-        f"/{Dirs.STATE_PATH}": {ImportVar(tag=CompileVars.TO_EVENT)},
+        "react": [ImportVar(tag="useContext")],
+        f"/{Dirs.CONTEXTS_PATH}": [ImportVar(tag="EventLoopContext")],
+        f"/{Dirs.STATE_PATH}": [ImportVar(tag=CompileVars.TO_EVENT)],
     }
 
 
 class Hooks(SimpleNamespace):
     """Common sets of hook declarations."""
 
     EVENTS = f"const [{CompileVars.ADD_EVENTS}, {CompileVars.CONNECT_ERROR}] = useContext(EventLoopContext);"
```

### Comparing `reflex-0.5.0a3/reflex/constants/config.py` & `reflex-0.5.1a1/reflex/constants/config.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/constants/custom_components.py` & `reflex-0.5.1a1/reflex/constants/custom_components.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/constants/event.py` & `reflex-0.5.1a1/reflex/constants/event.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/constants/installer.py` & `reflex-0.5.1a1/reflex/constants/installer.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 # Bun config.
 class Bun(SimpleNamespace):
     """Bun constants."""
 
     # The Bun version.
-    VERSION = "1.1.6"
+    VERSION = "1.1.8"
     # Min Bun Version
     MIN_VERSION = "0.7.0"
     # The directory to store the bun.
     ROOT_PATH = os.path.join(Reflex.DIR, "bun")
     # Default bun path.
     DEFAULT_PATH = os.path.join(
         ROOT_PATH, "bin", "bun" if not IS_WINDOWS else "bun.exe"
```

### Comparing `reflex-0.5.0a3/reflex/constants/route.py` & `reflex-0.5.1a1/reflex/constants/route.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/constants/style.py` & `reflex-0.5.1a1/reflex/constants/style.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/custom_components/custom_components.py` & `reflex-0.5.1a1/reflex/custom_components/custom_components.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/event.py` & `reflex-0.5.1a1/reflex/event.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Define event classes to connect the frontend and backend."""
 
 from __future__ import annotations
 
 import inspect
 from base64 import b64encode
-from types import FunctionType
 from typing import (
     Any,
     Callable,
     Dict,
     List,
     Optional,
     Tuple,
@@ -176,16 +175,18 @@
         Args:
             *args: The arguments to pass to the handler.
 
         Returns:
             The event spec, containing both the function and args.
 
         Raises:
-            TypeError: If the arguments are invalid.
+            EventHandlerTypeError: If the arguments are invalid.
         """
+        from reflex.utils.exceptions import EventHandlerTypeError
+
         # Get the function args.
         fn_args = inspect.getfullargspec(self.fn).args[1:]
         fn_args = (Var.create_safe(arg) for arg in fn_args)
 
         # Construct the payload.
         values = []
         for arg in args:
@@ -193,15 +194,15 @@
             if isinstance(arg, FileUpload):
                 return arg.as_event_spec(handler=self)
 
             # Otherwise, convert to JSON.
             try:
                 values.append(Var.create(arg, _var_is_string=isinstance(arg, str)))
             except TypeError as e:
-                raise TypeError(
+                raise EventHandlerTypeError(
                     f"Arguments to event handlers must be Vars or JSON-serializable. Got {arg} of type {type(arg)}."
                 ) from e
         payload = tuple(zip(fn_args, values))
 
         # Return the event spec.
         return EventSpec(
             handler=self, args=payload, event_actions=self.event_actions.copy()
@@ -252,27 +253,29 @@
         Args:
             *args: The arguments to add positionally.
 
         Returns:
             The event spec with the new arguments.
 
         Raises:
-            TypeError: If the arguments are invalid.
+            EventHandlerTypeError: If the arguments are invalid.
         """
+        from reflex.utils.exceptions import EventHandlerTypeError
+
         # Get the remaining unfilled function args.
         fn_args = inspect.getfullargspec(self.handler.fn).args[1 + len(self.args) :]
         fn_args = (Var.create_safe(arg) for arg in fn_args)
 
         # Construct the payload.
         values = []
         for arg in args:
             try:
                 values.append(Var.create(arg, _var_is_string=isinstance(arg, str)))
             except TypeError as e:
-                raise TypeError(
+                raise EventHandlerTypeError(
                     f"Arguments to event handlers must be Vars or JSON-serializable. Got {arg} of type {type(arg)}."
                 ) from e
         new_payload = tuple(zip(fn_args, values))
         return self.with_args(self.args + new_payload)
 
 
 class CallableEventSpec(EventSpec):
@@ -308,18 +311,20 @@
             *args: The args to pass to the function.
             **kwargs: The kwargs to pass to the function.
 
         Returns:
             The EventSpec returned from calling the function.
 
         Raises:
-            TypeError: If the CallableEventSpec has no associated function.
+            EventHandlerTypeError: If the CallableEventSpec has no associated function.
         """
+        from reflex.utils.exceptions import EventHandlerTypeError
+
         if self.fn is None:
-            raise TypeError("CallableEventSpec has no associated function.")
+            raise EventHandlerTypeError("CallableEventSpec has no associated function.")
         return self.fn(*args, **kwargs)
 
 
 class EventChain(EventActionsMixin):
     """Container for a chain of events that will be executed in order."""
 
     events: List[EventSpec]
@@ -458,26 +463,35 @@
         args=tuple(
             (Var.create_safe(k), Var.create_safe(v, _var_is_string=isinstance(v, str)))
             for k, v in kwargs.items()
         ),
     )
 
 
-def redirect(path: str | Var[str], external: Optional[bool] = False) -> EventSpec:
+def redirect(
+    path: str | Var[str],
+    external: Optional[bool] = False,
+    replace: Optional[bool] = False,
+) -> EventSpec:
     """Redirect to a new path.
 
     Args:
         path: The path to redirect to.
         external: Whether to open in new tab or not.
+        replace: If True, the current page will not create a new history entry.
 
     Returns:
         An event to redirect to the path.
     """
     return server_side(
-        "_redirect", get_fn_signature(redirect), path=path, external=external
+        "_redirect",
+        get_fn_signature(redirect),
+        path=path,
+        external=external,
+        replace=replace,
     )
 
 
 def console_log(message: str | Var[str]) -> EventSpec:
     """Do a console.log on the browser.
 
     Args:
@@ -696,39 +710,36 @@
         Args for the callback function
     """
     return [eval_result]
 
 
 def call_script(
     javascript_code: str,
-    callback: EventHandler | Callable | None = None,
+    callback: EventSpec
+    | EventHandler
+    | Callable
+    | List[EventSpec | EventHandler | Callable]
+    | None = None,
 ) -> EventSpec:
     """Create an event handler that executes arbitrary javascript code.
 
     Args:
         javascript_code: The code to execute.
         callback: EventHandler that will receive the result of evaluating the javascript code.
 
     Returns:
         EventSpec: An event that will execute the client side javascript.
-
-    Raises:
-        ValueError: If the callback is not a valid event handler.
     """
     callback_kwargs = {}
     if callback is not None:
-        arg_name = parse_args_spec(_callback_arg_spec)[0]._var_name
-        if isinstance(callback, EventHandler):
-            event_spec = call_event_handler(callback, _callback_arg_spec)
-        elif isinstance(callback, FunctionType):
-            event_spec = call_event_fn(callback, _callback_arg_spec)[0]
-        else:
-            raise ValueError("Cannot use {callback!r} as a call_script callback.")
         callback_kwargs = {
-            "callback": f"({arg_name}) => queueEvents([{format.format_event(event_spec)}], {constants.CompileVars.SOCKET})"
+            "callback": format.format_queue_events(
+                callback,
+                args_spec=lambda result: [result],
+            )
         }
     return server_side(
         "_call_script",
         get_fn_signature(call_script),
         javascript_code=javascript_code,
         **callback_kwargs,
     )
@@ -830,32 +841,33 @@
         fn: The function to call.
         arg: The argument to pass to the function.
 
     Returns:
         The event specs from calling the function.
 
     Raises:
-        ValueError: If the lambda has an invalid signature.
+        EventHandlerValueError: If the lambda has an invalid signature.
     """
     # Import here to avoid circular imports.
     from reflex.event import EventHandler, EventSpec
+    from reflex.utils.exceptions import EventHandlerValueError
 
     # Get the args of the lambda.
     args = inspect.getfullargspec(fn).args
 
     if isinstance(arg, ArgsSpec):
         out = fn(*parse_args_spec(arg))  # type: ignore
     else:
         # Call the lambda.
         if len(args) == 0:
             out = fn()
         elif len(args) == 1:
             out = fn(arg)
         else:
-            raise ValueError(f"Lambda {fn} must have 0 or 1 arguments.")
+            raise EventHandlerValueError(f"Lambda {fn} must have 0 or 1 arguments.")
 
     # Convert the output to a list.
     if not isinstance(out, List):
         out = [out]
 
     # Convert any event specs to event specs.
     events = []
@@ -865,15 +877,17 @@
             if len(args) == 0:
                 e = e()
             elif len(args) == 1:
                 e = e(arg)  # type: ignore
 
         # Make sure the event spec is valid.
         if not isinstance(e, EventSpec):
-            raise ValueError(f"Lambda {fn} returned an invalid event spec: {e}.")
+            raise EventHandlerValueError(
+                f"Lambda {fn} returned an invalid event spec: {e}."
+            )
 
         # Add the event spec to the chain.
         events.append(e)
 
     # Return the events.
     return events
```

### Comparing `reflex-0.5.0a3/reflex/experimental/__init__.py` & `reflex-0.5.1a1/reflex/experimental/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 """Namespace for experimental features."""
 
 from types import SimpleNamespace
 
+from reflex.components.props import PropsBase
 from reflex.components.radix.themes.components.progress import progress as progress
 from reflex.components.sonner.toast import toast as toast
 
 from ..utils.console import warn
 from . import hooks as hooks
+from .client_state import ClientStateVar as ClientStateVar
 from .layout import layout as layout
 from .misc import run_in_thread as run_in_thread
 
 warn(
     "`rx._x` contains experimental features and might be removed at any time in the future .",
 )
 
 _x = SimpleNamespace(
+    client_state=ClientStateVar.create,
     hooks=hooks,
     layout=layout,
     progress=progress,
+    PropsBase=PropsBase,
     run_in_thread=run_in_thread,
     toast=toast,
 )
```

### Comparing `reflex-0.5.0a3/reflex/experimental/hooks.py` & `reflex-0.5.1a1/reflex/experimental/hooks.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/experimental/layout.py` & `reflex-0.5.1a1/reflex/experimental/layout.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/middleware/hydrate_middleware.py` & `reflex-0.5.1a1/reflex/middleware/hydrate_middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/middleware/middleware.py` & `reflex-0.5.1a1/reflex/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/model.py` & `reflex-0.5.1a1/reflex/model.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/page.py` & `reflex-0.5.1a1/reflex/page.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/reflex.py` & `reflex-0.5.1a1/reflex/reflex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/route.py` & `reflex-0.5.1a1/reflex/route.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/state.py` & `reflex-0.5.1a1/reflex/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -275,19 +275,21 @@
             *args: The event args.
 
         Returns:
             The (partial) EventSpec that will be used to create the event to setvar.
 
         Raises:
             AttributeError: If the given Var name does not exist on the state.
-            ValueError: If the given Var name is not a str
+            EventHandlerValueError: If the given Var name is not a str
         """
+        from reflex.utils.exceptions import EventHandlerValueError
+
         if args:
             if not isinstance(args[0], str):
-                raise ValueError(
+                raise EventHandlerValueError(
                     f"Var name must be passed as a string, got {args[0]!r}"
                 )
             # Check that the requested Var setter exists on the State at compile time.
             if getattr(self.state_cls, constants.SETTER_PREFIX + args[0], None) is None:
                 raise AttributeError(
                     f"Variable `{args[0]}` cannot be set on `{self.state_cls.get_full_name()}`"
                 )
@@ -353,14 +355,17 @@
 
     # The router data for the current page
     router: RouterData = RouterData()
 
     # Whether the state has ever been touched since instantiation.
     _was_touched: bool = False
 
+    # Whether this state class is a mixin and should not be instantiated.
+    _mixin: ClassVar[bool] = False
+
     # A special event handler for setting base vars.
     setvar: ClassVar[EventHandler]
 
     def __init__(
         self,
         *args,
         parent_state: BaseState | None = None,
@@ -376,18 +381,20 @@
             *args: The args to pass to the Pydantic init method.
             parent_state: The parent state.
             init_substates: Whether to initialize the substates in this instance.
             _reflex_internal_init: A flag to indicate that the state is being initialized by the framework.
             **kwargs: The kwargs to pass to the Pydantic init method.
 
         Raises:
-            RuntimeError: If the state is instantiated directly by end user.
+            ReflexRuntimeError: If the state is instantiated directly by end user.
         """
+        from reflex.utils.exceptions import ReflexRuntimeError
+
         if not _reflex_internal_init and not is_testing_env():
-            raise RuntimeError(
+            raise ReflexRuntimeError(
                 "State classes should not be instantiated directly in a Reflex app. "
                 "See https://reflex.dev/docs/state/ for further information."
             )
         kwargs["parent_state"] = parent_state
         super().__init__(*args, **kwargs)
 
         # Setup the substates (for memory state manager only).
@@ -420,31 +427,38 @@
         """Helper function to get all computed vars of a instance.
 
         Returns:
             A list of computed vars.
         """
         return [
             v
-            for mixin in cls.__mro__
-            if mixin is cls or not issubclass(mixin, (BaseState, ABC))
+            for mixin in cls._mixins() + [cls]
             for v in mixin.__dict__.values()
             if isinstance(v, ComputedVar)
         ]
 
     @classmethod
-    def __init_subclass__(cls, **kwargs):
+    def __init_subclass__(cls, mixin: bool = False, **kwargs):
         """Do some magic for the subclass initialization.
 
         Args:
+            mixin: Whether the subclass is a mixin and should not be initialized.
             **kwargs: The kwargs to pass to the pydantic init_subclass method.
 
         Raises:
-            ValueError: If a substate class shadows another.
+            StateValueError: If a substate class shadows another.
         """
+        from reflex.utils.exceptions import StateValueError
+
         super().__init_subclass__(**kwargs)
+
+        cls._mixin = mixin
+        if mixin:
+            return
+
         # Event handlers should not shadow builtin state methods.
         cls._check_overridden_methods()
         # Computed vars should not shadow builtin state props.
         cls._check_overriden_basevars()
 
         # Reset subclass tracking for this class.
         cls.class_subclasses = set()
@@ -467,15 +481,15 @@
                         c
                         for c in parent_state.class_subclasses
                         if c.__name__ != cls.__name__
                     )
                 else:
                     # During normal operation, subclasses cannot have the same name, even if they are
                     # defined in different modules.
-                    raise ValueError(
+                    raise StateValueError(
                         f"The substate class '{cls.__name__}' has been defined multiple times. "
                         "Shadowing substate classes is not allowed."
                     )
             # Track this new subclass in the parent state's subclasses set.
             parent_state.class_subclasses.add(cls)
 
         # Get computed vars.
@@ -532,15 +546,17 @@
             if cls._item_is_event_handler(name, fn)
         }
 
         for mixin in cls._mixins():
             for name, value in mixin.__dict__.items():
                 if isinstance(value, ComputedVar):
                     fget = cls._copy_fn(value.fget)
-                    newcv = ComputedVar(fget=fget, _var_name=value._var_name)
+                    newcv = value._replace(fget=fget)
+                    # cleanup refs to mixin cls in var_data
+                    newcv._var_data = None
                     newcv._var_set_state(cls)
                     setattr(cls, name, newcv)
                     cls.computed_vars[newcv._var_name] = newcv
                     cls.vars[newcv._var_name] = newcv
                     continue
                 if events.get(name) is not None:
                     continue
@@ -608,16 +624,19 @@
 
         Returns:
             The mixin classes of the state.
         """
         return [
             mixin
             for mixin in cls.__mro__
-            if not issubclass(mixin, (BaseState, ABC))
-            and mixin not in [pydantic.BaseModel, Base]
+            if (
+                mixin not in [pydantic.BaseModel, Base, cls]
+                and issubclass(mixin, BaseState)
+                and mixin._mixin is True
+            )
         ]
 
     @classmethod
     def _init_var_dependency_dicts(cls):
         """Initialize the var dependency tracking dicts.
 
         Allows the state to know which vars each ComputedVar depends on and
@@ -732,15 +751,15 @@
 
         Returns:
             The parent state.
         """
         parent_states = [
             base
             for base in cls.__bases__
-            if types._issubclass(base, BaseState) and base is not BaseState
+            if issubclass(base, BaseState) and base is not BaseState and not base._mixin
         ]
         assert len(parent_states) < 2, "Only one parent state is allowed."
         return parent_states[0] if len(parent_states) == 1 else None  # type: ignore
 
     @classmethod
     def get_substates(cls) -> set[Type[BaseState]]:
         """Get the substates of the state.
@@ -825,18 +844,20 @@
     def _init_var(cls, prop: BaseVar):
         """Initialize a variable.
 
         Args:
             prop: The variable to initialize
 
         Raises:
-            TypeError: if the variable has an incorrect type
+            VarTypeError: if the variable has an incorrect type
         """
+        from reflex.utils.exceptions import VarTypeError
+
         if not types.is_valid_var_type(prop._var_type):
-            raise TypeError(
+            raise VarTypeError(
                 "State vars must be primitive Python types, "
                 "Plotly figures, Pandas dataframes, "
                 "or subclasses of rx.Base. "
                 f'Found var "{prop._var_name}" with type {prop._var_type}.'
             )
         cls._set_var(prop)
         cls._create_setter(prop)
@@ -1450,14 +1471,17 @@
             handler: EventHandler to process.
             state: State to process the handler.
             payload: The event payload.
 
         Yields:
             StateUpdate object
         """
+        from reflex.utils import telemetry
+        from reflex.utils.exceptions import ReflexError
+
         # Get the function to process the event.
         fn = functools.partial(handler.fn, state)
 
         # Wrap the function in a try/except block.
         try:
             # Handle async functions.
             if asyncio.iscoroutinefunction(fn.func):
@@ -1485,17 +1509,19 @@
                 yield state._as_state_update(handler, events=None, final=True)
 
             # Handle regular event chains.
             else:
                 yield state._as_state_update(handler, events, final=True)
 
         # If an error occurs, throw a window alert.
-        except Exception:
+        except Exception as ex:
             error = traceback.format_exc()
             print(error)
+            if isinstance(ex, ReflexError):
+                telemetry.send("error", context="backend", detail=str(ex))
             yield state._as_state_update(
                 handler,
                 window_alert("An error occurred. See logs for details."),
                 final=True,
             )
 
     def _mark_dirty_computed_vars(self) -> None:
@@ -1684,18 +1710,20 @@
         base_vars = {
             prop_name: self.get_value(getattr(self, prop_name))
             for prop_name in self.base_vars
         }
         if initial:
             computed_vars = {
                 # Include initial computed vars.
-                prop_name: cv._initial_value
-                if isinstance(cv, ComputedVar)
-                and not isinstance(cv._initial_value, types.Unset)
-                else self.get_value(getattr(self, prop_name))
+                prop_name: (
+                    cv._initial_value
+                    if isinstance(cv, ComputedVar)
+                    and not isinstance(cv._initial_value, types.Unset)
+                    else self.get_value(getattr(self, prop_name))
+                )
                 for prop_name, cv in self.computed_vars.items()
             }
         elif include_computed:
             computed_vars = {
                 # Include the computed vars.
                 prop_name: self.get_value(getattr(self, prop_name))
                 for prop_name in self.computed_vars
@@ -1814,15 +1842,15 @@
                 self.router.session.client_token,
                 router_data=self.router_data,
             ),
             State.set_is_hydrated(True),  # type: ignore
         ]
 
 
-class ComponentState(Base):
+class ComponentState(State, mixin=True):
     """Base class to allow for the creation of a state instance per component.
 
     This allows for the bundling of UI and state logic into a single class,
     where each instance has a separate instance of the state.
 
     Subclass this class and define vars and event handlers in the traditional way.
     Then define a `get_component` method that returns the UI for the component instance.
@@ -1857,14 +1885,26 @@
     ```
     """
 
     # The number of components created from this class.
     _per_component_state_instance_count: ClassVar[int] = 0
 
     @classmethod
+    def __init_subclass__(cls, mixin: bool = False, **kwargs):
+        """Overwrite mixin default to True.
+
+        Args:
+            mixin: Whether the subclass is a mixin and should not be initialized.
+            **kwargs: The kwargs to pass to the pydantic init_subclass method.
+        """
+        if ComponentState in cls.__bases__:
+            mixin = True
+        super().__init_subclass__(mixin=mixin, **kwargs)
+
+    @classmethod
     def get_component(cls, *children, **props) -> "Component":
         """Get the component instance.
 
         Args:
             children: The children of the component.
             props: The props of the component.
```

### Comparing `reflex-0.5.0a3/reflex/style.py` & `reflex-0.5.1a1/reflex/style.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 
 VarData.update_forward_refs()  # Ensure all type definitions are resolved
 
 LIGHT_COLOR_MODE: str = "light"
 DARK_COLOR_MODE: str = "dark"
 
 # Reference the global ColorModeContext
-color_mode_var_data = VarData(  # type: ignore
+color_mode_var_data = VarData(
     imports={
-        f"/{constants.Dirs.CONTEXTS_PATH}": {ImportVar(tag="ColorModeContext")},
-        "react": {ImportVar(tag="useContext")},
+        f"/{constants.Dirs.CONTEXTS_PATH}": [ImportVar(tag="ColorModeContext")],
+        "react": [ImportVar(tag="useContext")],
     },
     hooks={
         f"const [ {constants.ColorMode.NAME}, {constants.ColorMode.TOGGLE} ] = useContext(ColorModeContext)": None,
     },
 )
 # Var resolves to the current color mode for the app ("light" or "dark")
 color_mode = BaseVar(
```

### Comparing `reflex-0.5.0a3/reflex/testing.py` & `reflex-0.5.1a1/reflex/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from http.server import SimpleHTTPRequestHandler
 from typing import (
     TYPE_CHECKING,
     Any,
     AsyncIterator,
     Callable,
     Coroutine,
+    List,
     Optional,
     Type,
     TypeVar,
     Union,
 )
 
 import psutil
@@ -509,20 +510,27 @@
         if not self._poll_for(
             target=lambda: getattr(backend.servers[0], "sockets", False),
             timeout=timeout,
         ):
             raise TimeoutError("Backend is not listening.")
         return backend.servers[0].sockets[0]
 
-    def frontend(self, driver_clz: Optional[Type["WebDriver"]] = None) -> "WebDriver":
+    def frontend(
+        self,
+        driver_clz: Optional[Type["WebDriver"]] = None,
+        driver_kwargs: dict[str, Any] | None = None,
+        driver_option_args: List[str] | None = None,
+    ) -> "WebDriver":
         """Get a selenium webdriver instance pointed at the app.
 
         Args:
             driver_clz: webdriver.Chrome (default), webdriver.Firefox, webdriver.Safari,
                 webdriver.Edge, etc
+            driver_kwargs: additional keyword arguments to pass to the webdriver constructor
+            driver_option_args: additional arguments for the webdriver options
 
         Returns:
             Instance of the given webdriver navigated to the frontend url of the app.
 
         Raises:
             RuntimeError: when selenium is not importable or frontend is not running
         """
@@ -537,27 +545,38 @@
         options: ArgOptions | None = None
         if os.environ.get("APP_HARNESS_HEADLESS"):
             want_headless = True
         if driver_clz is None:
             requested_driver = os.environ.get("APP_HARNESS_DRIVER", "Chrome")
             driver_clz = getattr(webdriver, requested_driver)
             options = getattr(webdriver, f"{requested_driver}Options")()
-        if driver_clz is webdriver.Chrome and want_headless:
+        if driver_clz is webdriver.Chrome:
             options = webdriver.ChromeOptions()
-            options.add_argument("--headless=new")
-        elif driver_clz is webdriver.Firefox and want_headless:
+            options.add_argument("--class=AppHarness")
+            if want_headless:
+                options.add_argument("--headless=new")
+        elif driver_clz is webdriver.Firefox:
             options = webdriver.FirefoxOptions()
-            options.add_argument("-headless")
-        elif driver_clz is webdriver.Edge and want_headless:
+            if want_headless:
+                options.add_argument("-headless")
+        elif driver_clz is webdriver.Edge:
             options = webdriver.EdgeOptions()
-            options.add_argument("headless")
-        if options and (args := os.environ.get("APP_HARNESS_DRIVER_ARGS")):
+            if want_headless:
+                options.add_argument("headless")
+        if options is None:
+            raise RuntimeError(f"Could not determine options for {driver_clz}")
+        if args := os.environ.get("APP_HARNESS_DRIVER_ARGS"):
             for arg in args.split(","):
                 options.add_argument(arg)
-        driver = driver_clz(options=options)  # type: ignore
+        if driver_option_args is not None:
+            for arg in driver_option_args:
+                options.add_argument(arg)
+        if driver_kwargs is None:
+            driver_kwargs = {}
+        driver = driver_clz(options=options, **driver_kwargs)  # type: ignore
         driver.get(self.frontend_url)
         self._frontends.append(driver)
         return driver
 
     async def get_state(self, token: str) -> BaseState:
         """Get the state associated with the given token.
```

### Comparing `reflex-0.5.0a3/reflex/utils/build.py` & `reflex-0.5.1a1/reflex/utils/build.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/utils/compat.py` & `reflex-0.5.1a1/reflex/utils/compat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/utils/console.py` & `reflex-0.5.1a1/reflex/utils/console.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/utils/exec.py` & `reflex-0.5.1a1/reflex/utils/exec.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/utils/export.py` & `reflex-0.5.1a1/reflex/utils/export.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/utils/format.py` & `reflex-0.5.1a1/reflex/utils/format.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 from __future__ import annotations
 
 import inspect
 import json
 import os
 import re
-from typing import TYPE_CHECKING, Any, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Callable, List, Optional, Union
 
 from reflex import constants
 from reflex.utils import exceptions, serializers, types
 from reflex.utils.serializers import serialize
 from reflex.vars import BaseVar, Var
 
 if TYPE_CHECKING:
     from reflex.components.component import ComponentStyle
-    from reflex.event import EventChain, EventHandler, EventSpec
+    from reflex.event import ArgsSpec, EventChain, EventHandler, EventSpec
 
 WRAP_MAP = {
     "{": "}",
     "(": ")",
     "[": "]",
     "<": ">",
     '"': '"',
@@ -586,14 +586,85 @@
             f"addEvents([{chain}]",
             f", {format_var(event_arg)}" if event_arg else "",
             ")",
         ]
     )
 
 
+def format_queue_events(
+    events: EventSpec
+    | EventHandler
+    | Callable
+    | List[EventSpec | EventHandler | Callable]
+    | None = None,
+    args_spec: Optional[ArgsSpec] = None,
+) -> Var[EventChain]:
+    """Format a list of event handler / event spec as a javascript callback.
+
+    The resulting code can be passed to interfaces that expect a callback
+    function and when triggered it will directly call queueEvents.
+
+    It is intended to be executed in the rx.call_script context, where some
+    existing API needs a callback to trigger a backend event handler.
+
+    Args:
+        events: The events to queue.
+        args_spec: The argument spec for the callback.
+
+    Returns:
+        The compiled javascript callback to queue the given events on the frontend.
+    """
+    from reflex.event import (
+        EventChain,
+        EventHandler,
+        EventSpec,
+        call_event_fn,
+        call_event_handler,
+    )
+
+    if not events:
+        return Var.create_safe(
+            "() => null", _var_is_string=False, _var_is_local=False
+        ).to(EventChain)
+
+    # If no spec is provided, the function will take no arguments.
+    def _default_args_spec():
+        return []
+
+    # Construct the arguments that the function accepts.
+    sig = inspect.signature(args_spec or _default_args_spec)  # type: ignore
+    if sig.parameters:
+        arg_def = ",".join(f"_{p}" for p in sig.parameters)
+        arg_def = f"({arg_def})"
+    else:
+        arg_def = "()"
+
+    payloads = []
+    if not isinstance(events, list):
+        events = [events]
+
+    # Process each event/spec/lambda (similar to Component._create_event_chain).
+    for spec in events:
+        specs: list[EventSpec] = []
+        if isinstance(spec, (EventHandler, EventSpec)):
+            specs = [call_event_handler(spec, args_spec or _default_args_spec)]
+        elif isinstance(spec, type(lambda: None)):
+            specs = call_event_fn(spec, args_spec or _default_args_spec)
+        payloads.extend(format_event(s) for s in specs)
+
+    # Return the final code snippet, expecting queueEvents, processEvent, and socket to be in scope.
+    # Typically this snippet will _only_ run from within an rx.call_script eval context.
+    return Var.create_safe(
+        f"{arg_def} => {{queueEvents([{','.join(payloads)}], {constants.CompileVars.SOCKET}); "
+        f"processEvent({constants.CompileVars.SOCKET})}}",
+        _var_is_string=False,
+        _var_is_local=False,
+    ).to(EventChain)
+
+
 def format_query_params(router_data: dict[str, Any]) -> dict[str, str]:
     """Convert back query params name to python-friendly case.
 
     Args:
         router_data: the router_data dict containing the query params
 
     Returns:
```

### Comparing `reflex-0.5.0a3/reflex/utils/imports.py` & `reflex-0.5.1a1/reflex/utils/imports.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/utils/path_ops.py` & `reflex-0.5.1a1/reflex/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/utils/prerequisites.py` & `reflex-0.5.1a1/reflex/utils/prerequisites.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,15 +177,20 @@
 def get_install_package_manager() -> str | None:
     """Get the package manager executable for installation.
       Currently, bun is used for installation only.
 
     Returns:
         The path to the package manager.
     """
-    if constants.IS_WINDOWS and not is_windows_bun_supported():
+    if (
+        constants.IS_WINDOWS
+        and not is_windows_bun_supported()
+        or windows_check_onedrive_in_path()
+        or windows_npm_escape_hatch()
+    ):
         return get_package_manager()
     return get_config().bun_path
 
 
 def get_package_manager() -> str | None:
     """Get the package manager executable for running app.
       Currently on unix systems, npm is used for running the app only.
@@ -195,47 +200,72 @@
     """
     npm_path = path_ops.get_npm_path()
     if npm_path is not None:
         npm_path = str(Path(npm_path).resolve())
     return npm_path
 
 
+def windows_check_onedrive_in_path() -> bool:
+    """For windows, check if oneDrive is present in the project dir path.
+
+    Returns:
+        If oneDrive is in the path of the project directory.
+    """
+    return "onedrive" in str(Path.cwd()).lower()
+
+
+def windows_npm_escape_hatch() -> bool:
+    """For windows, if the user sets REFLEX_USE_NPM, use npm instead of bun.
+
+    Returns:
+        If the user has set REFLEX_USE_NPM.
+    """
+    return os.environ.get("REFLEX_USE_NPM", "").lower() in ["true", "1", "yes"]
+
+
 def get_app(reload: bool = False) -> ModuleType:
     """Get the app module based on the default config.
 
     Args:
         reload: Re-import the app module from disk
 
     Returns:
         The app based on the default config.
 
     Raises:
         RuntimeError: If the app name is not set in the config.
+        exceptions.ReflexError: Reflex specific errors.
     """
-    os.environ[constants.RELOAD_CONFIG] = str(reload)
-    config = get_config()
-    if not config.app_name:
-        raise RuntimeError(
-            "Cannot get the app module because `app_name` is not set in rxconfig! "
-            "If this error occurs in a reflex test case, ensure that `get_app` is mocked."
-        )
-    module = config.module
-    sys.path.insert(0, os.getcwd())
-    app = __import__(module, fromlist=(constants.CompileVars.APP,))
-
-    if reload:
-        from reflex.state import reload_state_module
+    from reflex.utils import exceptions, telemetry
 
-        # Reset rx.State subclasses to avoid conflict when reloading.
-        reload_state_module(module=module)
-
-        # Reload the app module.
-        importlib.reload(app)
-
-    return app
+    try:
+        os.environ[constants.RELOAD_CONFIG] = str(reload)
+        config = get_config()
+        if not config.app_name:
+            raise RuntimeError(
+                "Cannot get the app module because `app_name` is not set in rxconfig! "
+                "If this error occurs in a reflex test case, ensure that `get_app` is mocked."
+            )
+        module = config.module
+        sys.path.insert(0, os.getcwd())
+        app = __import__(module, fromlist=(constants.CompileVars.APP,))
+
+        if reload:
+            from reflex.state import reload_state_module
+
+            # Reset rx.State subclasses to avoid conflict when reloading.
+            reload_state_module(module=module)
+
+            # Reload the app module.
+            importlib.reload(app)
+
+        return app
+    except exceptions.ReflexError as ex:
+        telemetry.send("error", context="frontend", detail=str(ex))
+        raise
 
 
 def get_compiled_app(reload: bool = False, export: bool = False) -> ModuleType:
     """Get the app module based on the default config after first compiling it.
 
     Args:
         reload: Re-import the app module from disk
@@ -379,15 +409,15 @@
     if os.path.exists(gitignore_file):
         with open(gitignore_file, "r") as f:
             files_to_ignore |= set([line.strip() for line in f.readlines()])
 
     # Write files to the .gitignore file.
     with open(gitignore_file, "w", newline="\n") as f:
         console.debug(f"Creating {gitignore_file}")
-        f.write(f"{(path_ops.join(sorted(files_to_ignore))).lstrip()}")
+        f.write(f"{(path_ops.join(sorted(files_to_ignore))).lstrip()}\n")
 
 
 def initialize_requirements_txt():
     """Initialize the requirements.txt file.
     If absent, generate one for the user.
     If the requirements.txt does not have reflex as dependency,
     generate a requirement pinning current version and append to
@@ -733,18 +763,25 @@
 
 def install_bun():
     """Install bun onto the user's system.
 
     Raises:
         FileNotFoundError: If required packages are not found.
     """
-    if constants.IS_WINDOWS and not is_windows_bun_supported():
-        console.warn(
-            "Bun for Windows is currently only available for x86 64-bit Windows. Installation will fall back on npm."
-        )
+    win_supported = is_windows_bun_supported()
+    one_drive_in_path = windows_check_onedrive_in_path()
+    if constants.IS_WINDOWS and not win_supported or one_drive_in_path:
+        if not win_supported:
+            console.warn(
+                "Bun for Windows is currently only available for x86 64-bit Windows. Installation will fall back on npm."
+            )
+        if one_drive_in_path:
+            console.warn(
+                "Creating project directories in OneDrive is not recommended for bun usage on windows. This will fallback to npm."
+            )
 
     # Skip if bun is already installed.
     if os.path.exists(get_config().bun_path) and get_bun_version() == version.parse(
         constants.Bun.VERSION
     ):
         console.debug("Skipping bun installation as it is already installed.")
         return
@@ -839,19 +876,21 @@
     """
     # unsupported archs(arm and 32bit machines) will use npm anyway. so we dont have to run npm twice
     fallback_command = (
         get_package_manager()
         if not constants.IS_WINDOWS
         or constants.IS_WINDOWS
         and is_windows_bun_supported()
+        and not windows_check_onedrive_in_path()
         else None
     )
     processes.run_process_with_fallback(
         [get_install_package_manager(), "install"],  # type: ignore
         fallback=fallback_command,
+        analytics_enabled=True,
         show_status_message="Installing base frontend packages",
         cwd=constants.Dirs.WEB,
         shell=constants.IS_WINDOWS,
     )
 
     if config.tailwind is not None:
         processes.run_process_with_fallback(
@@ -859,24 +898,26 @@
                 get_install_package_manager(),
                 "add",
                 "-d",
                 constants.Tailwind.VERSION,
                 *((config.tailwind or {}).get("plugins", [])),
             ],
             fallback=fallback_command,
+            analytics_enabled=True,
             show_status_message="Installing tailwind",
             cwd=constants.Dirs.WEB,
             shell=constants.IS_WINDOWS,
         )
 
     # Install custom packages defined in frontend_packages
     if len(packages) > 0:
         processes.run_process_with_fallback(
             [get_install_package_manager(), "add", *packages],
             fallback=fallback_command,
+            analytics_enabled=True,
             show_status_message="Installing frontend packages from config and components",
             cwd=constants.Dirs.WEB,
             shell=constants.IS_WINDOWS,
         )
 
 
 def needs_reinit(frontend: bool = True) -> bool:
@@ -925,14 +966,19 @@
                 f"""On Python 3.12, `uvicorn==0.24.0.post1` is recommended for improved hot reload times. Found {uvi_ver} instead."""
             )
 
         if sys.version_info < (3, 12) and uvi_ver != "0.20.0":
             console.warn(
                 f"""On Python < 3.12, `uvicorn==0.20.0` is recommended for improved hot reload times.  Found {uvi_ver} instead."""
             )
+
+        if windows_check_onedrive_in_path():
+            console.warn(
+                "Creating project directories in OneDrive may lead to performance issues. For optimal performance, It is recommended to avoid using OneDrive for your reflex app."
+            )
     # No need to reinitialize if the app is already initialized.
     return False
 
 
 def is_latest_template() -> bool:
     """Whether the app is using the latest template.
```

### Comparing `reflex-0.5.0a3/reflex/utils/processes.py` & `reflex-0.5.1a1/reflex/utils/processes.py`

 * *Files 18% similar despite different names*

```diff
@@ -207,29 +207,33 @@
 
 
 def stream_logs(
     message: str,
     process: subprocess.Popen,
     progress=None,
     suppress_errors: bool = False,
+    analytics_enabled: bool = False,
 ):
     """Stream the logs for a process.
 
     Args:
         message: The message to display.
         process: The process.
         progress: The ongoing progress bar if one is being used.
         suppress_errors: If True, do not exit if errors are encountered (for fallback).
+        analytics_enabled: Whether analytics are enabled for this command.
 
     Yields:
         The lines of the process output.
 
     Raises:
         Exit: If the process failed.
     """
+    from reflex.utils import telemetry
+
     # Store the tail of the logs.
     logs = collections.deque(maxlen=512)
     with process:
         console.debug(message, progress=progress)
         if process.stdout is None:
             return
         for line in process.stdout:
@@ -242,14 +246,16 @@
     # Windows uvicorn bug
     # https://github.com/reflex-dev/reflex/issues/2335
     accepted_return_codes = [0, -2, 15] if constants.IS_WINDOWS else [0, -2]
     if process.returncode not in accepted_return_codes and not suppress_errors:
         console.error(f"{message} failed with exit code {process.returncode}")
         for line in logs:
             console.error(line, end="")
+        if analytics_enabled:
+            telemetry.send("error", context=message)
         console.error("Run with [bold]--loglevel debug [/bold] for the full log.")
         raise typer.Exit(1)
 
 
 def show_logs(message: str, process: subprocess.Popen):
     """Show the logs for a process.
 
@@ -257,24 +263,35 @@
         message: The message to display.
         process: The process.
     """
     for _ in stream_logs(message, process):
         pass
 
 
-def show_status(message: str, process: subprocess.Popen, suppress_errors: bool = False):
+def show_status(
+    message: str,
+    process: subprocess.Popen,
+    suppress_errors: bool = False,
+    analytics_enabled: bool = False,
+):
     """Show the status of a process.
 
     Args:
         message: The initial message to display.
         process: The process.
         suppress_errors: If True, do not exit if errors are encountered (for fallback).
+        analytics_enabled: Whether analytics are enabled for this command.
     """
     with console.status(message) as status:
-        for line in stream_logs(message, process, suppress_errors=suppress_errors):
+        for line in stream_logs(
+            message,
+            process,
+            suppress_errors=suppress_errors,
+            analytics_enabled=analytics_enabled,
+        ):
             status.update(f"{message} {line}")
 
 
 def show_progress(message: str, process: subprocess.Popen, checkpoints: List[str]):
     """Show a progress bar for a process.
 
     Args:
@@ -315,40 +332,53 @@
     npm_path = str(Path(npm_path).resolve()) if npm_path else npm_path
 
     if command[0] == npm_path:
         return command + ["--loglevel", "silly"]
     return command
 
 
-def run_process_with_fallback(args, *, show_status_message, fallback=None, **kwargs):
+def run_process_with_fallback(
+    args,
+    *,
+    show_status_message,
+    fallback=None,
+    analytics_enabled: bool = False,
+    **kwargs,
+):
     """Run subprocess and retry using fallback command if initial command fails.
 
     Args:
         args: A string, or a sequence of program arguments.
         show_status_message: The status message to be displayed in the console.
         fallback: The fallback command to run.
+        analytics_enabled: Whether analytics are enabled for this command.
         kwargs: Kwargs to pass to new_process function.
     """
     process = new_process(get_command_with_loglevel(args), **kwargs)
     if fallback is None:
         # No fallback given, or this _is_ the fallback command.
-        show_status(show_status_message, process)
+        show_status(
+            show_status_message,
+            process,
+            analytics_enabled=analytics_enabled,
+        )
     else:
         # Suppress errors for initial command, because we will try to fallback
         show_status(show_status_message, process, suppress_errors=True)
         if process.returncode != 0:
             # retry with fallback command.
             fallback_args = [fallback, *args[1:]]
             console.warn(
                 f"There was an error running command: {args}. Falling back to: {fallback_args}."
             )
             run_process_with_fallback(
                 fallback_args,
                 show_status_message=show_status_message,
                 fallback=None,
+                analytics_enabled=analytics_enabled,
                 **kwargs,
             )
 
 
 def execute_command_and_return_output(command) -> str | None:
     """Execute a command and return the output.
```

### Comparing `reflex-0.5.0a3/reflex/utils/pyi_generator.py` & `reflex-0.5.1a1/reflex/utils/pyi_generator.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/utils/serializers.py` & `reflex-0.5.1a1/reflex/utils/serializers.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/utils/telemetry.py` & `reflex-0.5.1a1/reflex/utils/telemetry.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,32 +122,32 @@
         stamp = datetime.utcnow().isoformat()
     else:
         # for python 3.11 & 3.12
         stamp = datetime.now(UTC).isoformat()
 
     cpuinfo = get_cpu_info()
 
+    additional_keys = ["template", "context", "detail"]
+    additional_fields = {
+        key: value for key in additional_keys if (value := kwargs.get(key)) is not None
+    }
     return {
         "api_key": "phc_JoMo0fOyi0GQAooY3UyO9k0hebGkMyFJrrCw1Gt5SGb",
         "event": event,
         "properties": {
             "distinct_id": installation_id,
             "distinct_app_id": project_hash,
             "user_os": get_os(),
             "user_os_detail": get_detailed_platform_str(),
             "reflex_version": get_reflex_version(),
             "python_version": get_python_version(),
             "cpu_count": get_cpu_count(),
             "memory": get_memory(),
             "cpu_info": dict(cpuinfo) if cpuinfo else {},
-            **(
-                {"template": template}
-                if (template := kwargs.get("template")) is not None
-                else {}
-            ),
+            **additional_fields,
         },
         "timestamp": stamp,
     }
 
 
 def _send_event(event_data: dict) -> bool:
     try:
```

### Comparing `reflex-0.5.0a3/reflex/utils/types.py` & `reflex-0.5.1a1/reflex/utils/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,30 @@
     Relationship,
 )
 
 from reflex import constants
 from reflex.base import Base
 from reflex.utils import console, serializers
 
+if sys.version_info >= (3, 12):
+    from typing import override
+else:
+
+    def override(func: Callable) -> Callable:
+        """Fallback for @override decorator.
+
+        Args:
+            func: The function to decorate.
+
+        Returns:
+            The unmodified function.
+        """
+        return func
+
+
 # Potential GenericAlias types for isinstance checks.
 GenericAliasTypes = [_GenericAlias]
 
 with contextlib.suppress(ImportError):
     # For newer versions of Python.
     from types import GenericAlias  # type: ignore
```

### Comparing `reflex-0.5.0a3/reflex/utils/watch.py` & `reflex-0.5.1a1/reflex/utils/watch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.0a3/reflex/vars.py` & `reflex-0.5.1a1/reflex/vars.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,21 +31,24 @@
     get_origin,
     get_type_hints,
 )
 
 from reflex import constants
 from reflex.base import Base
 from reflex.utils import console, format, imports, serializers, types
+from reflex.utils.exceptions import VarAttributeError, VarTypeError, VarValueError
 
 # This module used to export ImportVar itself, so we still import it for export here
 from reflex.utils.imports import ImportDict, ImportVar
+from reflex.utils.types import override
 
 if TYPE_CHECKING:
     from reflex.state import BaseState
 
+
 # Set of unique variable names.
 USED_VARIABLES = set()
 
 # Supported operators for all types.
 ALL_OPS = ["==", "!=", "!==", "===", "&&", "||"]
 # Delimiters used between function args or operands.
 DELIMITERS = [","]
@@ -336,77 +339,87 @@
     _var_full_name_needs_state_prefix: bool
 
     # Extra metadata associated with the Var
     _var_data: Optional[VarData]
 
     @classmethod
     def create(
-        cls, value: Any, _var_is_local: bool = True, _var_is_string: bool = False
+        cls,
+        value: Any,
+        _var_is_local: bool = True,
+        _var_is_string: bool = False,
+        _var_data: Optional[VarData] = None,
     ) -> Var | None:
         """Create a var from a value.
 
         Args:
             value: The value to create the var from.
             _var_is_local: Whether the var is local.
             _var_is_string: Whether the var is a string literal.
+            _var_data: Additional hooks and imports associated with the Var.
 
         Returns:
             The var.
 
         Raises:
-            TypeError: If the value is JSON-unserializable.
+            VarTypeError: If the value is JSON-unserializable.
         """
         # Check for none values.
         if value is None:
             return None
 
         # If the value is already a var, do nothing.
         if isinstance(value, Var):
             return value
 
         # Try to pull the imports and hooks from contained values.
-        _var_data = None
         if not isinstance(value, str):
-            _var_data = VarData.merge(*_extract_var_data(value))
+            _var_data = VarData.merge(*_extract_var_data(value), _var_data)
 
         # Try to serialize the value.
         type_ = type(value)
         name = value if type_ in types.JSONType else serializers.serialize(value)
         if name is None:
-            raise TypeError(
+            raise VarTypeError(
                 f"No JSON serializer found for var {value} of type {type_}."
             )
         name = name if isinstance(name, str) else format.json_dumps(name)
 
         return BaseVar(
             _var_name=name,
             _var_type=type_,
             _var_is_local=_var_is_local,
             _var_is_string=_var_is_string,
             _var_data=_var_data,
         )
 
     @classmethod
     def create_safe(
-        cls, value: Any, _var_is_local: bool = True, _var_is_string: bool = False
+        cls,
+        value: Any,
+        _var_is_local: bool = True,
+        _var_is_string: bool = False,
+        _var_data: Optional[VarData] = None,
     ) -> Var:
         """Create a var from a value, asserting that it is not None.
 
         Args:
             value: The value to create the var from.
             _var_is_local: Whether the var is local.
             _var_is_string: Whether the var is a string literal.
+            _var_data: Additional hooks and imports associated with the Var.
 
         Returns:
             The var.
         """
         var = cls.create(
             value,
             _var_is_local=_var_is_local,
             _var_is_string=_var_is_string,
+            _var_data=_var_data,
         )
         assert var is not None
         return var
 
     @classmethod
     def __class_getitem__(cls, type_: str) -> _GenericAlias:
         """Get a typed var.
@@ -538,28 +551,28 @@
             out = format.format_string(out)
         return out
 
     def __bool__(self) -> bool:
         """Raise exception if using Var in a boolean context.
 
         Raises:
-            TypeError: when attempting to bool-ify the Var.
+            VarTypeError: when attempting to bool-ify the Var.
         """
-        raise TypeError(
+        raise VarTypeError(
             f"Cannot convert Var {self._var_full_name!r} to bool for use with `if`, `and`, `or`, and `not`. "
             "Instead use `rx.cond` and bitwise operators `&` (and), `|` (or), `~` (invert)."
         )
 
     def __iter__(self) -> Any:
         """Raise exception if using Var in an iterable context.
 
         Raises:
-            TypeError: when attempting to iterate over the Var.
+            VarTypeError: when attempting to iterate over the Var.
         """
-        raise TypeError(
+        raise VarTypeError(
             f"Cannot iterate over Var {self._var_full_name!r}. Instead use `rx.foreach`."
         )
 
     def __format__(self, format_spec: str) -> str:
         """Format the var into a Javascript equivalent to an f-string.
 
         Args:
@@ -580,27 +593,27 @@
         Args:
             i: The index to index into.
 
         Returns:
             The indexed var.
 
         Raises:
-            TypeError: If the var is not indexable.
+            VarTypeError: If the var is not indexable.
         """
         # Indexing is only supported for strings, lists, tuples, dicts, and dataframes.
         if not (
             types._issubclass(self._var_type, Union[List, Dict, Tuple, str])
             or types.is_dataframe(self._var_type)
         ):
             if self._var_type == Any:
-                raise TypeError(
+                raise VarTypeError(
                     "Could not index into var of type Any. (If you are trying to index into a state var, "
                     "add the correct type annotation to the var.)"
                 )
-            raise TypeError(
+            raise VarTypeError(
                 f"Var {self._var_name} of type {self._var_type} does not support indexing."
             )
 
         # The type of the indexed var.
         type_ = Any
 
         # Convert any vars to local vars.
@@ -611,15 +624,15 @@
         if types._issubclass(self._var_type, Union[List, Tuple, str]):
             # List/Tuple/String indices must be ints, slices, or vars.
             if (
                 not isinstance(i, types.get_args(Union[int, slice, Var]))
                 or isinstance(i, Var)
                 and not i._var_type == int
             ):
-                raise TypeError("Index must be an integer or an integer var.")
+                raise VarTypeError("Index must be an integer or an integer var.")
 
             # Handle slices first.
             if isinstance(i, slice):
                 # Get the start and stop indices.
                 start = i.start or 0
                 stop = i.stop or "undefined"
 
@@ -654,15 +667,15 @@
             and not isinstance(i, types.get_args(Union[int, str, float, Var]))
         ) or (
             isinstance(i, Var)
             and not types._issubclass(
                 i._var_type, types.get_args(Union[int, str, float])
             )
         ):
-            raise TypeError(
+            raise VarTypeError(
                 "Index must be one of the following types: int, str, int or str Var"
             )
         # Get the type of the indexed var.
         if isinstance(i, str):
             i = format.wrap(i, '"')
         type_ = (
             types.get_args(self._var_type)[1]
@@ -683,71 +696,73 @@
         Args:
             name: The name of the attribute.
 
         Returns:
             The var attribute.
 
         Raises:
-            AttributeError: If the attribute cannot be found, or if __getattr__ fallback should be used.
+            VarAttributeError: If the attribute cannot be found, or if __getattr__ fallback should be used.
         """
         try:
             var_attribute = super().__getattribute__(name)
             if not name.startswith("_"):
                 # Check if the attribute should be accessed through the Var instead of
                 # accessing one of the Var operations
                 type_ = types.get_attribute_access_type(
                     super().__getattribute__("_var_type"), name
                 )
                 if type_ is not None:
-                    raise AttributeError(f"{name} is being accessed through the Var.")
+                    raise VarAttributeError(
+                        f"{name} is being accessed through the Var."
+                    )
             # Return the attribute as-is.
             return var_attribute
-        except AttributeError:
+        except VarAttributeError:
             raise  # fall back to __getattr__ anyway
 
     def __getattr__(self, name: str) -> Var:
         """Get a var attribute.
 
         Args:
             name: The name of the attribute.
 
         Returns:
             The var attribute.
 
         Raises:
-            AttributeError: If the var is wrongly annotated or can't find attribute.
-            TypeError: If an annotation to the var isn't provided.
+            VarAttributeError: If the var is wrongly annotated or can't find attribute.
+            VarTypeError: If an annotation to the var isn't provided.
         """
         # Check if the attribute is one of the class fields.
         if not name.startswith("_"):
             if self._var_type == Any:
-                raise TypeError(
+                raise VarTypeError(
                     f"You must provide an annotation for the state var `{self._var_full_name}`. Annotation cannot be `{self._var_type}`"
                 ) from None
             is_optional = types.is_optional(self._var_type)
             type_ = types.get_attribute_access_type(self._var_type, name)
 
             if type_ is not None:
                 return self._replace(
                     _var_name=f"{self._var_name}{'?' if is_optional else ''}.{name}",
                     _var_type=type_,
                     _var_is_string=False,
                 )
 
             if name in REPLACED_NAMES:
-                raise AttributeError(
+                raise VarAttributeError(
                     f"Field {name!r} was renamed to {REPLACED_NAMES[name]!r}"
                 )
 
-            raise AttributeError(
+            raise VarAttributeError(
                 f"The State var `{self._var_full_name}` has no attribute '{name}' or may have been annotated "
                 f"wrongly."
             )
 
-        raise AttributeError(
+        raise VarAttributeError(
             f"The State var has no attribute '{name}' or may have been annotated wrongly.",
         )
 
     def operation(
         self,
         op: str = "",
         other: Var | None = None,
@@ -766,26 +781,26 @@
             fn: A function to apply to the operation.
             invoke_fn: Whether to invoke the function.
 
         Returns:
             The operation result.
 
         Raises:
-            TypeError: If the operation between two operands is invalid.
-            ValueError: If flip is set to true and value of operand is not provided
+            VarTypeError: If the operation between two operands is invalid.
+            VarValueError: If flip is set to true and value of operand is not provided
         """
         if isinstance(other, str):
             other = Var.create(json.dumps(other))
         else:
             other = Var.create(other)
 
         type_ = type_ or self._var_type
 
         if other is None and flip:
-            raise ValueError(
+            raise VarValueError(
                 "flip_operands cannot be set to True if the value of 'other' operand is not provided"
             )
 
         left_operand, right_operand = (other, self) if flip else (self, other)
 
         def get_operand_full_name(operand):
             # operand vars that are string literals need to be wrapped in back ticks.
@@ -800,42 +815,42 @@
         if other is not None:
             # check if the operation between operands is valid.
             if op and not self.is_valid_operation(
                 types.get_base_class(left_operand._var_type),  # type: ignore
                 types.get_base_class(right_operand._var_type),  # type: ignore
                 op,
             ):
-                raise TypeError(
+                raise VarTypeError(
                     f"Unsupported Operand type(s) for {op}: `{left_operand._var_full_name}` of type {left_operand._var_type.__name__} and `{right_operand._var_full_name}` of type {right_operand._var_type.__name__}"  # type: ignore
                 )
 
             left_operand_full_name = get_operand_full_name(left_operand)
             right_operand_full_name = get_operand_full_name(right_operand)
 
             left_operand_full_name = format.wrap(left_operand_full_name, "(")
             right_operand_full_name = format.wrap(right_operand_full_name, "(")
 
             # apply function to operands
             if fn is not None:
                 if invoke_fn:
                     # invoke the function on left operand.
                     operation_name = (
-                        f"{left_operand_full_name}.{fn}({right_operand_full_name})"
-                    )  # type: ignore
+                        f"{left_operand_full_name}.{fn}({right_operand_full_name})"  # type: ignore
+                    )
                 else:
                     # pass the operands as arguments to the function.
                     operation_name = (
-                        f"{left_operand_full_name} {op} {right_operand_full_name}"
-                    )  # type: ignore
+                        f"{left_operand_full_name} {op} {right_operand_full_name}"  # type: ignore
+                    )
                     operation_name = f"{fn}({operation_name})"
             else:
                 # apply operator to operands (left operand <operator> right_operand)
                 operation_name = (
-                    f"{left_operand_full_name} {op} {right_operand_full_name}"
-                )  # type: ignore
+                    f"{left_operand_full_name} {op} {right_operand_full_name}"  # type: ignore
+                )
                 operation_name = format.wrap(operation_name, "(")
         else:
             # apply operator to left operand (<operator> left_operand)
             operation_name = f"{op}{get_operand_full_name(self)}"
             # apply function to operands
             if fn is not None:
                 operation_name = (
@@ -921,18 +936,18 @@
     def length(self) -> Var:
         """Get the length of a list var.
 
         Returns:
             A var with the absolute value.
 
         Raises:
-            TypeError: If the var is not a list.
+            VarTypeError: If the var is not a list.
         """
         if not types._issubclass(self._var_type, List):
-            raise TypeError(f"Cannot get length of non-list var {self}.")
+            raise VarTypeError(f"Cannot get length of non-list var {self}.")
         return self._replace(
             _var_name=f"{self._var_name}.length",
             _var_type=int,
             _var_is_string=False,
         )
 
     def _type(self) -> Var:
@@ -1324,34 +1339,34 @@
         """
         return self.operation("||", other, type_=bool, flip=True)
 
     def __contains__(self, _: Any) -> Var:
         """Override the 'in' operator to alert the user that it is not supported.
 
         Raises:
-            TypeError: the operation is not supported
+            VarTypeError: the operation is not supported
         """
-        raise TypeError(
+        raise VarTypeError(
             "'in' operator not supported for Var types, use Var.contains() instead."
         )
 
     def contains(self, other: Any) -> Var:
         """Check if a var contains the object `other`.
 
         Args:
             other: The object to check.
 
         Raises:
-            TypeError: If the var is not a valid type: dict, list, tuple or str.
+            VarTypeError: If the var is not a valid type: dict, list, tuple or str.
 
         Returns:
             A var representing the contain check.
         """
         if not (types._issubclass(self._var_type, Union[dict, list, tuple, str, set])):
-            raise TypeError(
+            raise VarTypeError(
                 f"Var {self._var_full_name} of type {self._var_type} does not support contains check."
             )
         method = (
             "hasOwnProperty"
             if types.get_base_class(self._var_type) == dict
             else "includes"
         )
@@ -1367,53 +1382,53 @@
                 merge_var_data=other._var_data,
             )
         else:  # str, list, tuple
             # For strings, the left operand must be a string.
             if types._issubclass(self._var_type, str) and not types._issubclass(
                 other._var_type, str
             ):
-                raise TypeError(
+                raise VarTypeError(
                     f"'in <string>' requires string as left operand, not {other._var_type}"
                 )
             return self._replace(
                 _var_name=f"{self._var_name}.includes({other._var_full_name})",
                 _var_type=bool,
                 _var_is_string=False,
                 merge_var_data=other._var_data,
             )
 
     def reverse(self) -> Var:
         """Reverse a list var.
 
         Raises:
-            TypeError: If the var is not a list.
+            VarTypeError: If the var is not a list.
 
         Returns:
             A var with the reversed list.
         """
         if not types._issubclass(self._var_type, list):
-            raise TypeError(f"Cannot reverse non-list var {self._var_full_name}.")
+            raise VarTypeError(f"Cannot reverse non-list var {self._var_full_name}.")
 
         return self._replace(
             _var_name=f"[...{self._var_full_name}].reverse()",
             _var_is_string=False,
             _var_full_name_needs_state_prefix=False,
         )
 
     def lower(self) -> Var:
         """Convert a string var to lowercase.
 
         Returns:
             A var with the lowercase string.
 
         Raises:
-            TypeError: If the var is not a string.
+            VarTypeError: If the var is not a string.
         """
         if not types._issubclass(self._var_type, str):
-            raise TypeError(
+            raise VarTypeError(
                 f"Cannot convert non-string var {self._var_full_name} to lowercase."
             )
 
         return self._replace(
             _var_name=f"{self._var_name}.toLowerCase()",
             _var_is_string=False,
             _var_type=str,
@@ -1422,18 +1437,18 @@
     def upper(self) -> Var:
         """Convert a string var to uppercase.
 
         Returns:
             A var with the uppercase string.
 
         Raises:
-            TypeError: If the var is not a string.
+            VarTypeError: If the var is not a string.
         """
         if not types._issubclass(self._var_type, str):
-            raise TypeError(
+            raise VarTypeError(
                 f"Cannot convert non-string var {self._var_full_name} to uppercase."
             )
 
         return self._replace(
             _var_name=f"{self._var_name}.toUpperCase()",
             _var_is_string=False,
             _var_type=str,
@@ -1445,18 +1460,18 @@
         Args:
             other: The string to strip the var with.
 
         Returns:
             A var with the stripped string.
 
         Raises:
-            TypeError: If the var is not a string.
+            VarTypeError: If the var is not a string.
         """
         if not types._issubclass(self._var_type, str):
-            raise TypeError(f"Cannot strip non-string var {self._var_full_name}.")
+            raise VarTypeError(f"Cannot strip non-string var {self._var_full_name}.")
 
         other = Var.create_safe(json.dumps(other)) if isinstance(other, str) else other
 
         return self._replace(
             _var_name=f"{self._var_name}.replace(/^${other._var_full_name}|${other._var_full_name}$/g, '')",
             _var_is_string=False,
             merge_var_data=other._var_data,
@@ -1468,18 +1483,18 @@
         Args:
             other: The string to split the var with.
 
         Returns:
             A var with the list.
 
         Raises:
-            TypeError: If the var is not a string.
+            VarTypeError: If the var is not a string.
         """
         if not types._issubclass(self._var_type, str):
-            raise TypeError(f"Cannot split non-string var {self._var_full_name}.")
+            raise VarTypeError(f"Cannot split non-string var {self._var_full_name}.")
 
         other = Var.create_safe(json.dumps(other)) if isinstance(other, str) else other
 
         return self._replace(
             _var_name=f"{self._var_name}.split({other._var_full_name})",
             _var_is_string=False,
             _var_type=List[str],
@@ -1492,18 +1507,18 @@
         Args:
             other: The string to join the list with.
 
         Returns:
             A var with the string.
 
         Raises:
-            TypeError: If the var is not a list.
+            VarTypeError: If the var is not a list.
         """
         if not types._issubclass(self._var_type, list):
-            raise TypeError(f"Cannot join non-list var {self._var_full_name}.")
+            raise VarTypeError(f"Cannot join non-list var {self._var_full_name}.")
 
         if other is None:
             other = Var.create_safe('""')
         if isinstance(other, str):
             other = Var.create_safe(json.dumps(other))
         else:
             other = Var.create_safe(other)
@@ -1521,19 +1536,19 @@
         Args:
             fn: The function to call on each component.
 
         Returns:
             A var representing foreach operation.
 
         Raises:
-            TypeError: If the var is not a list.
+            VarTypeError: If the var is not a list.
         """
         inner_types = get_args(self._var_type)
         if not inner_types:
-            raise TypeError(
+            raise VarTypeError(
                 f"Cannot foreach over non-sequence var {self._var_full_name} of type {self._var_type}."
             )
         arg = BaseVar(
             _var_name=get_unique_variable_name(),
             _var_type=inner_types[0],
         )
         index = BaseVar(
@@ -1562,33 +1577,35 @@
             v2: The end of the range.
             step: The number of numbers between each item.
 
         Returns:
             A var representing range operation.
 
         Raises:
-            TypeError: If the var is not an int.
+            VarTypeError: If the var is not an int.
         """
         if not isinstance(v1, Var):
             v1 = Var.create_safe(v1)
         if v1._var_type != int:
-            raise TypeError(f"Cannot get range on non-int var {v1._var_full_name}.")
+            raise VarTypeError(f"Cannot get range on non-int var {v1._var_full_name}.")
         if not isinstance(v2, Var):
             v2 = Var.create(v2)
         if v2 is None:
             v2 = Var.create_safe("undefined")
         elif v2._var_type != int:
-            raise TypeError(f"Cannot get range on non-int var {v2._var_full_name}.")
+            raise VarTypeError(f"Cannot get range on non-int var {v2._var_full_name}.")
 
         if not isinstance(step, Var):
             step = Var.create(step)
         if step is None:
             step = Var.create_safe(1)
         elif step._var_type != int:
-            raise TypeError(f"Cannot get range on non-int var {step._var_full_name}.")
+            raise VarTypeError(
+                f"Cannot get range on non-int var {step._var_full_name}."
+            )
 
         return BaseVar(
             _var_name=f"Array.from(range({v1._var_full_name}, {v2._var_full_name}, {step._var_name}))",
             _var_type=List[int],
             _var_is_local=False,
             _var_data=VarData.merge(
                 v1._var_data,
@@ -1863,14 +1880,40 @@
         self._initial_value = initial_value
         self._cache = cache
         property.__init__(self, fget)
         kwargs["_var_name"] = kwargs.pop("_var_name", fget.__name__)
         kwargs["_var_type"] = kwargs.pop("_var_type", self._determine_var_type())
         BaseVar.__init__(self, **kwargs)  # type: ignore
 
+    @override
+    def _replace(self, merge_var_data=None, **kwargs: Any) -> ComputedVar:
+        """Replace the attributes of the ComputedVar.
+
+        Args:
+            merge_var_data: VarData to merge into the existing VarData.
+            **kwargs: Var fields to update.
+
+        Returns:
+            The new ComputedVar instance.
+        """
+        return ComputedVar(
+            fget=kwargs.get("fget", self.fget),
+            initial_value=kwargs.get("initial_value", self._initial_value),
+            cache=kwargs.get("cache", self._cache),
+            _var_name=kwargs.get("_var_name", self._var_name),
+            _var_type=kwargs.get("_var_type", self._var_type),
+            _var_is_local=kwargs.get("_var_is_local", self._var_is_local),
+            _var_is_string=kwargs.get("_var_is_string", self._var_is_string),
+            _var_full_name_needs_state_prefix=kwargs.get(
+                "_var_full_name_needs_state_prefix",
+                self._var_full_name_needs_state_prefix,
+            ),
+            _var_data=VarData.merge(self._var_data, merge_var_data),
+        )
+
     @property
     def _cache_attr(self) -> str:
         """Get the attribute used to cache the value on the instance.
 
         Returns:
             An attribute name.
         """
@@ -1915,15 +1958,15 @@
             obj: the object to disassemble (defaults to the fget function).
             self_name: if specified, look for this name in LOAD_FAST and LOAD_DEREF instructions.
 
         Returns:
             A set of variable names accessed by the given obj.
 
         Raises:
-            ValueError: if the function references the get_state, parent_state, or substates attributes
+            VarValueError: if the function references the get_state, parent_state, or substates attributes
                 (cannot track deps in a related state, only implicitly via parent state).
         """
         d = set()
         if obj is None:
             fget = property.__getattribute__(self, "fget")
             if fget is not None:
                 obj = cast(FunctionType, fget)
@@ -1962,15 +2005,15 @@
                 "LOAD_METHOD",
             ):
                 try:
                     ref_obj = getattr(objclass, instruction.argval)
                 except Exception:
                     ref_obj = None
                 if instruction.argval in invalid_names:
-                    raise ValueError(
+                    raise VarValueError(
                         f"Cached var {self._var_full_name} cannot access arbitrary state via `{instruction.argval}`."
                     )
                 if callable(ref_obj):
                     # recurse into callable attributes
                     d.update(
                         self._deps(
                             objclass=objclass,
```

### Comparing `reflex-0.5.0a3/reflex/vars.pyi` & `reflex-0.5.1a1/reflex/vars.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -30,35 +30,35 @@
 
 def get_unique_variable_name() -> str: ...
 def _encode_var(value: Var) -> str: ...
 def _decode_var(value: str) -> tuple[VarData, str]: ...
 def _extract_var_data(value: Iterable) -> list[VarData | None]: ...
 
 class VarData(Base):
-    state: str
-    imports: dict[str, set[ImportVar]]
-    hooks: Dict[str, None]
-    interpolations: List[Tuple[int, int]]
+    state: str = ""
+    imports: dict[str, List[ImportVar]] = {}
+    hooks: Dict[str, None] = {}
+    interpolations: List[Tuple[int, int]] = []
     @classmethod
     def merge(cls, *others: VarData | None) -> VarData | None: ...
 
 class Var:
     _var_name: str
     _var_type: Type
     _var_is_local: bool = False
     _var_is_string: bool = False
     _var_full_name_needs_state_prefix: bool = False
     _var_data: VarData | None = None
     @classmethod
     def create(
-        cls, value: Any, _var_is_local: bool = False, _var_is_string: bool = False
+        cls, value: Any, _var_is_local: bool = False, _var_is_string: bool = False, _var_data: VarData | None = None,
     ) -> Optional[Var]: ...
     @classmethod
     def create_safe(
-        cls, value: Any, _var_is_local: bool = False, _var_is_string: bool = False
+        cls, value: Any, _var_is_local: bool = False, _var_is_string: bool = False, _var_data: VarData | None = None,
     ) -> Var: ...
     @classmethod
     def __class_getitem__(cls, type_: Type) -> _GenericAlias: ...
     def _replace(self, merge_var_data=None, **kwargs: Any) -> Var: ...
     def equals(self, other: Var) -> bool: ...
     def to_string(self) -> Var: ...
     def __hash__(self) -> int: ...
@@ -135,14 +135,15 @@
 class ComputedVar(Var):
     _var_cache: bool
     fget: FunctionType
     @property
     def _cache_attr(self) -> str: ...
     def __get__(self, instance, owner): ...
     def _deps(self, objclass: Type, obj: Optional[FunctionType] = ...) -> Set[str]: ...
+    def _replace(self, merge_var_data=None, **kwargs: Any) -> ComputedVar: ...
     def mark_dirty(self, instance) -> None: ...
     def _determine_var_type(self) -> Type: ...
     @overload
     def __init__(
         self,
         fget: Callable[[BaseState], Any],
         **kwargs,
```

### Comparing `reflex-0.5.0a3/PKG-INFO` & `reflex-0.5.1a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex
-Version: 0.5.0a3
+Version: 0.5.1a1
 Summary: Web apps in pure Python.
 Home-page: https://reflex.dev
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@reflex.dev
 Requires-Python: >=3.8,<4.0
```

