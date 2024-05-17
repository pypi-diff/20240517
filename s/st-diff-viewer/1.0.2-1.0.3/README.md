# Comparing `tmp/st_diff_viewer-1.0.2.tar.gz` & `tmp/st_diff_viewer-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_diff_viewer-1.0.2.tar", max compression
+gzip compressed data, was "st_diff_viewer-1.0.3.tar", max compression
```

## Comparing `st_diff_viewer-1.0.2.tar` & `st_diff_viewer-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1063 2024-05-17 07:07:34.851441 st_diff_viewer-1.0.2/LICENSE
--rw-r--r--   0        0        0      675 2024-05-17 12:13:27.315638 st_diff_viewer-1.0.2/README.md
--rw-r--r--   0        0        0    10730 2024-05-17 10:20:33.150645 st_diff_viewer-1.0.2/docs/head.png
--rw-r--r--   0        0        0    37586 2024-05-17 09:21:13.808831 st_diff_viewer-1.0.2/docs/img.png
--rw-r--r--   0        0        0      699 2024-05-17 12:22:21.681384 st_diff_viewer-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2470 2024-05-17 12:21:04.651220 st_diff_viewer-1.0.2/st_diff_viewer/__init__.py
--rw-r--r--   0        0        0     2626 2024-05-17 12:22:18.692725 st_diff_viewer-1.0.2/st_diff_viewer/frontend/out/404.html
--rw-r--r--   0        0        0      321 2024-05-17 12:22:18.365720 st_diff_viewer-1.0.2/st_diff_viewer/frontend/out/_next/static/_AHG4uWRwYU17O4FvaGOj/_buildManifest.js
--rw-r--r--   0        0        0       77 2024-05-17 12:22:18.365967 st_diff_viewer-1.0.2/st_diff_viewer/frontend/out/_next/static/_AHG4uWRwYU17O4FvaGOj/_ssgManifest.js
--rw-r--r--   0        0        0   233887 2024-05-17 12:22:18.366198 st_diff_viewer-1.0.2/st_diff_viewer/frontend/out/_next/static/chunks/92-bf787e1cee9c20db.js
--rw-r--r--   0        0        0   140973 2024-05-17 12:22:18.366378 st_diff_viewer-1.0.2/st_diff_viewer/frontend/out/_next/static/chunks/framework-c0663f0e1a0e4372.js
--rw-r--r--   0        0        0    95990 2024-05-17 12:22:18.366433 st_diff_viewer-1.0.2/st_diff_viewer/frontend/out/_next/static/chunks/main-49701d22161bf8f9.js
--rw-r--r--   0        0        0      442 2024-05-17 12:22:18.367400 st_diff_viewer-1.0.2/st_diff_viewer/frontend/out/_next/static/chunks/pages/_app-2ddf65715eee6393.js
--rw-r--r--   0        0        0      247 2024-05-17 12:22:18.367116 st_diff_viewer-1.0.2/st_diff_viewer/frontend/out/_next/static/chunks/pages/_error-54de1933a164a1ff.js
--rw-r--r--   0        0        0     1085 2024-05-17 12:22:18.367649 st_diff_viewer-1.0.2/st_diff_viewer/frontend/out/_next/static/chunks/pages/index-08087b43971404a5.js
--rw-r--r--   0        0        0    91381 2024-05-17 12:22:18.367089 st_diff_viewer-1.0.2/st_diff_viewer/frontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js
--rw-r--r--   0        0        0     1485 2024-05-17 12:22:18.366671 st_diff_viewer-1.0.2/st_diff_viewer/frontend/out/_next/static/chunks/webpack-88e841e08c00aeb1.js
--rw-r--r--   0        0        0     4386 2024-05-17 12:22:18.366854 st_diff_viewer-1.0.2/st_diff_viewer/frontend/out/_next/static/css/34e82990737d7da2.css
--rw-r--r--   0        0        0    25931 2024-05-17 12:22:18.369770 st_diff_viewer-1.0.2/st_diff_viewer/frontend/out/favicon.ico
--rw-r--r--   0        0        0     1986 2024-05-17 12:22:18.645270 st_diff_viewer-1.0.2/st_diff_viewer/frontend/out/index.html
--rw-r--r--   0        0        0     1101 2024-05-17 12:22:18.369736 st_diff_viewer-1.0.2/st_diff_viewer/frontend/out/vercel.svg
--rw-r--r--   0        0        0     1406 1970-01-01 00:00:00.000000 st_diff_viewer-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-17 07:07:34.851441 st_diff_viewer-1.0.3/LICENSE
+-rw-r--r--   0        0        0      735 2024-05-17 12:26:32.281665 st_diff_viewer-1.0.3/README.md
+-rw-r--r--   0        0        0    10730 2024-05-17 10:20:33.150645 st_diff_viewer-1.0.3/docs/head.png
+-rw-r--r--   0        0        0    37586 2024-05-17 09:21:13.808831 st_diff_viewer-1.0.3/docs/img.png
+-rw-r--r--   0        0        0      699 2024-05-17 12:27:10.945701 st_diff_viewer-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2470 2024-05-17 12:21:04.651220 st_diff_viewer-1.0.3/st_diff_viewer/__init__.py
+-rw-r--r--   0        0        0     2626 2024-05-17 12:27:08.021802 st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/404.html
+-rw-r--r--   0        0        0   233887 2024-05-17 12:27:07.664157 st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/chunks/92-bf787e1cee9c20db.js
+-rw-r--r--   0        0        0   140973 2024-05-17 12:27:07.664280 st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/chunks/framework-c0663f0e1a0e4372.js
+-rw-r--r--   0        0        0    95990 2024-05-17 12:27:07.664418 st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/chunks/main-49701d22161bf8f9.js
+-rw-r--r--   0        0        0      442 2024-05-17 12:27:07.665217 st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/chunks/pages/_app-2ddf65715eee6393.js
+-rw-r--r--   0        0        0      247 2024-05-17 12:27:07.665441 st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/chunks/pages/_error-54de1933a164a1ff.js
+-rw-r--r--   0        0        0     1085 2024-05-17 12:27:07.665652 st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/chunks/pages/index-08087b43971404a5.js
+-rw-r--r--   0        0        0    91381 2024-05-17 12:27:07.665179 st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js
+-rw-r--r--   0        0        0     1485 2024-05-17 12:27:07.664694 st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/chunks/webpack-88e841e08c00aeb1.js
+-rw-r--r--   0        0        0     4386 2024-05-17 12:27:07.664845 st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/css/34e82990737d7da2.css
+-rw-r--r--   0        0        0      321 2024-05-17 12:27:07.664951 st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/eevQmOyAWWKyTH0eX_1RU/_buildManifest.js
+-rw-r--r--   0        0        0       77 2024-05-17 12:27:07.665232 st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/eevQmOyAWWKyTH0eX_1RU/_ssgManifest.js
+-rw-r--r--   0        0        0    25931 2024-05-17 12:27:07.667905 st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/favicon.ico
+-rw-r--r--   0        0        0     1986 2024-05-17 12:27:07.953071 st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/index.html
+-rw-r--r--   0        0        0     1101 2024-05-17 12:27:07.667296 st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/vercel.svg
+-rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 st_diff_viewer-1.0.3/PKG-INFO
```

### Comparing `st_diff_viewer-1.0.2/LICENSE` & `st_diff_viewer-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `st_diff_viewer-1.0.2/README.md` & `st_diff_viewer-1.0.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# streamlit-diff-viewer
+# [streamlit-diff-viewer](https://github.com/LinXueyuanStdio/streamlit-diff-viewer)
 git-like diff viewer for streamlit webapp
 
 ![](docs/head.png)
 
 ## Installation
 
 ```bash
```

### Comparing `st_diff_viewer-1.0.2/docs/head.png` & `st_diff_viewer-1.0.3/docs/head.png`

 * *Files identical despite different names*

### Comparing `st_diff_viewer-1.0.2/docs/img.png` & `st_diff_viewer-1.0.3/docs/img.png`

 * *Files identical despite different names*

### Comparing `st_diff_viewer-1.0.2/pyproject.toml` & `st_diff_viewer-1.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "st-diff-viewer"
-version = "1.0.2"
+version = "1.0.3"
 description = "A Streamlit component to display diff betoween two strings"
 authors = ["Xueyuan Lin <linxy59@mail2.sysu.eud.cn>"]
 readme = "README.md"
 packages = [{ include = "st_diff_viewer"}]
 
 license = "MIT"
```

### Comparing `st_diff_viewer-1.0.2/st_diff_viewer/__init__.py` & `st_diff_viewer-1.0.3/st_diff_viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `st_diff_viewer-1.0.2/st_diff_viewer/frontend/out/404.html` & `st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/404.html`

 * *Files 7% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><title>404: This page could not be found</title><meta name="next-head-count" content="3"/><link rel="preload" href="/component/st_diff_viewer.st_diff_viewer/_next/static/css/34e82990737d7da2.css" as="style"/><link rel="stylesheet" href="/component/st_diff_viewer.st_diff_viewer/_next/static/css/34e82990737d7da2.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/webpack-88e841e08c00aeb1.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/framework-c0663f0e1a0e4372.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/main-49701d22161bf8f9.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/pages/_app-2ddf65715eee6393.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/pages/_error-54de1933a164a1ff.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/_AHG4uWRwYU17O4FvaGOj/_buildManifest.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/_AHG4uWRwYU17O4FvaGOj/_ssgManifest.js" defer=""></script></head><body><div id="__next"><div style="font-family:system-ui,&quot;Segoe UI&quot;,Roboto,Helvetica,Arial,sans-serif,&quot;Apple Color Emoji&quot;,&quot;Segoe UI Emoji&quot;;height:100vh;text-align:center;display:flex;flex-direction:column;align-items:center;justify-content:center"><div style="line-height:48px"><style>body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}</style><h1 class="next-error-h1" style="display:inline-block;margin:0 20px 0 0;padding-right:23px;font-size:24px;font-weight:500;vertical-align:top">404</h1><div style="display:inline-block"><h2 style="font-size:14px;font-weight:400;line-height:28px">This page could not be found<!-- -->.</h2></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"statusCode":404}},"page":"/_error","query":{},"buildId":"_AHG4uWRwYU17O4FvaGOj","assetPrefix":"/component/st_diff_viewer.st_diff_viewer","nextExport":true,"isFallback":false,"gip":true,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><title>404: This page could not be found</title><meta name="next-head-count" content="3"/><link rel="preload" href="/component/st_diff_viewer.st_diff_viewer/_next/static/css/34e82990737d7da2.css" as="style"/><link rel="stylesheet" href="/component/st_diff_viewer.st_diff_viewer/_next/static/css/34e82990737d7da2.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/webpack-88e841e08c00aeb1.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/framework-c0663f0e1a0e4372.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/main-49701d22161bf8f9.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/pages/_app-2ddf65715eee6393.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/pages/_error-54de1933a164a1ff.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/eevQmOyAWWKyTH0eX_1RU/_buildManifest.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/eevQmOyAWWKyTH0eX_1RU/_ssgManifest.js" defer=""></script></head><body><div id="__next"><div style="font-family:system-ui,&quot;Segoe UI&quot;,Roboto,Helvetica,Arial,sans-serif,&quot;Apple Color Emoji&quot;,&quot;Segoe UI Emoji&quot;;height:100vh;text-align:center;display:flex;flex-direction:column;align-items:center;justify-content:center"><div style="line-height:48px"><style>body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}</style><h1 class="next-error-h1" style="display:inline-block;margin:0 20px 0 0;padding-right:23px;font-size:24px;font-weight:500;vertical-align:top">404</h1><div style="display:inline-block"><h2 style="font-size:14px;font-weight:400;line-height:28px">This page could not be found<!-- -->.</h2></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"statusCode":404}},"page":"/_error","query":{},"buildId":"eevQmOyAWWKyTH0eX_1RU","assetPrefix":"/component/st_diff_viewer.st_diff_viewer","nextExport":true,"isFallback":false,"gip":true,"scriptLoader":[]}</script></body></html>
```

### Comparing `st_diff_viewer-1.0.2/st_diff_viewer/frontend/out/_next/static/chunks/92-bf787e1cee9c20db.js` & `st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/chunks/92-bf787e1cee9c20db.js`

 * *Files identical despite different names*

### Comparing `st_diff_viewer-1.0.2/st_diff_viewer/frontend/out/_next/static/chunks/framework-c0663f0e1a0e4372.js` & `st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/chunks/framework-c0663f0e1a0e4372.js`

 * *Files identical despite different names*

### Comparing `st_diff_viewer-1.0.2/st_diff_viewer/frontend/out/_next/static/chunks/main-49701d22161bf8f9.js` & `st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/chunks/main-49701d22161bf8f9.js`

 * *Files identical despite different names*

### Comparing `st_diff_viewer-1.0.2/st_diff_viewer/frontend/out/_next/static/chunks/pages/index-08087b43971404a5.js` & `st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/chunks/pages/index-08087b43971404a5.js`

 * *Files identical despite different names*

### Comparing `st_diff_viewer-1.0.2/st_diff_viewer/frontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js` & `st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js`

 * *Files identical despite different names*

### Comparing `st_diff_viewer-1.0.2/st_diff_viewer/frontend/out/_next/static/chunks/webpack-88e841e08c00aeb1.js` & `st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/chunks/webpack-88e841e08c00aeb1.js`

 * *Files identical despite different names*

### Comparing `st_diff_viewer-1.0.2/st_diff_viewer/frontend/out/_next/static/css/34e82990737d7da2.css` & `st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/css/34e82990737d7da2.css`

 * *Files identical despite different names*

### Comparing `st_diff_viewer-1.0.2/st_diff_viewer/frontend/out/favicon.ico` & `st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/favicon.ico`

 * *Files identical despite different names*

### Comparing `st_diff_viewer-1.0.2/st_diff_viewer/frontend/out/index.html` & `st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/index.html`

 * *Files 8% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><title>Create Next App</title><meta name="description" content="Generated by create next app"/><link rel="icon" href="/favicon.ico"/><meta name="next-head-count" content="5"/><link rel="preload" href="/component/st_diff_viewer.st_diff_viewer/_next/static/css/34e82990737d7da2.css" as="style"/><link rel="stylesheet" href="/component/st_diff_viewer.st_diff_viewer/_next/static/css/34e82990737d7da2.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/webpack-88e841e08c00aeb1.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/framework-c0663f0e1a0e4372.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/main-49701d22161bf8f9.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/pages/_app-2ddf65715eee6393.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/92-bf787e1cee9c20db.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/pages/index-08087b43971404a5.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/_AHG4uWRwYU17O4FvaGOj/_buildManifest.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/_AHG4uWRwYU17O4FvaGOj/_ssgManifest.js" defer=""></script></head><body><div id="__next"></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"_AHG4uWRwYU17O4FvaGOj","assetPrefix":"/component/st_diff_viewer.st_diff_viewer","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><title>Create Next App</title><meta name="description" content="Generated by create next app"/><link rel="icon" href="/favicon.ico"/><meta name="next-head-count" content="5"/><link rel="preload" href="/component/st_diff_viewer.st_diff_viewer/_next/static/css/34e82990737d7da2.css" as="style"/><link rel="stylesheet" href="/component/st_diff_viewer.st_diff_viewer/_next/static/css/34e82990737d7da2.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/webpack-88e841e08c00aeb1.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/framework-c0663f0e1a0e4372.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/main-49701d22161bf8f9.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/pages/_app-2ddf65715eee6393.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/92-bf787e1cee9c20db.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/pages/index-08087b43971404a5.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/eevQmOyAWWKyTH0eX_1RU/_buildManifest.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/eevQmOyAWWKyTH0eX_1RU/_ssgManifest.js" defer=""></script></head><body><div id="__next"></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"eevQmOyAWWKyTH0eX_1RU","assetPrefix":"/component/st_diff_viewer.st_diff_viewer","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `st_diff_viewer-1.0.2/st_diff_viewer/frontend/out/vercel.svg` & `st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/vercel.svg`

 * *Files identical despite different names*

### Comparing `st_diff_viewer-1.0.2/PKG-INFO` & `st_diff_viewer-1.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-diff-viewer
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Streamlit component to display diff betoween two strings
 License: MIT
 Author: Xueyuan Lin
 Author-email: linxy59@mail2.sysu.eud.cn
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: streamlit (>=0.63)
 Description-Content-Type: text/markdown
 
-# streamlit-diff-viewer
+# [streamlit-diff-viewer](https://github.com/LinXueyuanStdio/streamlit-diff-viewer)
 git-like diff viewer for streamlit webapp
 
 ![](docs/head.png)
 
 ## Installation
 
 ```bash
```

