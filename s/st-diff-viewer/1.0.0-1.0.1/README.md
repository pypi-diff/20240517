# Comparing `tmp/st_diff_viewer-1.0.0.tar.gz` & `tmp/st_diff_viewer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_diff_viewer-1.0.0.tar", max compression
+gzip compressed data, was "st_diff_viewer-1.0.1.tar", max compression
```

## Comparing `st_diff_viewer-1.0.0.tar` & `st_diff_viewer-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0     1063 2024-05-17 07:07:34.851441 st_diff_viewer-1.0.0/LICENSE
--rw-r--r--   0        0        0      675 2024-05-17 12:07:47.336589 st_diff_viewer-1.0.0/README.md
--rw-r--r--   0        0        0      688 2024-05-17 12:07:20.970206 st_diff_viewer-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2470 2024-05-17 12:08:04.428074 st_diff_viewer-1.0.0/st-diff-viewer/__init__.py
--rw-r--r--   0        0        0     2780 2024-05-17 10:22:44.024972 st_diff_viewer-1.0.0/st-diff-viewer/frontend/out/404.html
--rw-r--r--   0        0        0   233887 2024-05-17 10:22:43.698292 st_diff_viewer-1.0.0/st-diff-viewer/frontend/out/_next/static/chunks/92-bf787e1cee9c20db.js
--rw-r--r--   0        0        0   140973 2024-05-17 10:22:43.698381 st_diff_viewer-1.0.0/st-diff-viewer/frontend/out/_next/static/chunks/framework-c0663f0e1a0e4372.js
--rw-r--r--   0        0        0    96046 2024-05-17 10:22:43.698560 st_diff_viewer-1.0.0/st-diff-viewer/frontend/out/_next/static/chunks/main-78a4b523a4dbe3d5.js
--rw-r--r--   0        0        0      442 2024-05-17 10:22:43.699389 st_diff_viewer-1.0.0/st-diff-viewer/frontend/out/_next/static/chunks/pages/_app-2ddf65715eee6393.js
--rw-r--r--   0        0        0      247 2024-05-17 10:22:43.699625 st_diff_viewer-1.0.0/st-diff-viewer/frontend/out/_next/static/chunks/pages/_error-54de1933a164a1ff.js
--rw-r--r--   0        0        0     1085 2024-05-17 10:22:43.699850 st_diff_viewer-1.0.0/st-diff-viewer/frontend/out/_next/static/chunks/pages/index-08087b43971404a5.js
--rw-r--r--   0        0        0    91381 2024-05-17 10:22:43.699543 st_diff_viewer-1.0.0/st-diff-viewer/frontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js
--rw-r--r--   0        0        0     1499 2024-05-17 10:22:43.698825 st_diff_viewer-1.0.0/st-diff-viewer/frontend/out/_next/static/chunks/webpack-545f75f9c7fe06d9.js
--rw-r--r--   0        0        0     4386 2024-05-17 10:22:43.699013 st_diff_viewer-1.0.0/st-diff-viewer/frontend/out/_next/static/css/34e82990737d7da2.css
--rw-r--r--   0        0        0      321 2024-05-17 10:22:43.699160 st_diff_viewer-1.0.0/st-diff-viewer/frontend/out/_next/static/nIcdbMRjqlcHjjesGgyOg/_buildManifest.js
--rw-r--r--   0        0        0       77 2024-05-17 10:22:43.699377 st_diff_viewer-1.0.0/st-diff-viewer/frontend/out/_next/static/nIcdbMRjqlcHjjesGgyOg/_ssgManifest.js
--rw-r--r--   0        0        0    25931 2024-05-17 10:22:43.702153 st_diff_viewer-1.0.0/st-diff-viewer/frontend/out/favicon.ico
--rw-r--r--   0        0        0     2154 2024-05-17 10:22:43.969627 st_diff_viewer-1.0.0/st-diff-viewer/frontend/out/index.html
--rw-r--r--   0        0        0     1101 2024-05-17 10:22:43.702001 st_diff_viewer-1.0.0/st-diff-viewer/frontend/out/vercel.svg
--rw-r--r--   0        0        0     1406 1970-01-01 00:00:00.000000 st_diff_viewer-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-17 07:07:34.851441 st_diff_viewer-1.0.1/LICENSE
+-rw-r--r--   0        0        0      675 2024-05-17 12:13:27.315638 st_diff_viewer-1.0.1/README.md
+-rw-r--r--   0        0        0    10730 2024-05-17 10:20:33.150645 st_diff_viewer-1.0.1/docs/head.png
+-rw-r--r--   0        0        0    37586 2024-05-17 09:21:13.808831 st_diff_viewer-1.0.1/docs/img.png
+-rw-r--r--   0        0        0      699 2024-05-17 12:17:08.205637 st_diff_viewer-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2470 2024-05-17 12:08:04.428074 st_diff_viewer-1.0.1/st-diff-viewer/__init__.py
+-rw-r--r--   0        0        0     2626 2024-05-17 12:17:04.950117 st_diff_viewer-1.0.1/st-diff-viewer/frontend/out/404.html
+-rw-r--r--   0        0        0   233887 2024-05-17 12:17:04.589682 st_diff_viewer-1.0.1/st-diff-viewer/frontend/out/_next/static/chunks/92-bf787e1cee9c20db.js
+-rw-r--r--   0        0        0   140973 2024-05-17 12:17:04.589742 st_diff_viewer-1.0.1/st-diff-viewer/frontend/out/_next/static/chunks/framework-c0663f0e1a0e4372.js
+-rw-r--r--   0        0        0    95990 2024-05-17 12:17:04.589898 st_diff_viewer-1.0.1/st-diff-viewer/frontend/out/_next/static/chunks/main-7a1f841e500a3672.js
+-rw-r--r--   0        0        0      442 2024-05-17 12:17:04.590932 st_diff_viewer-1.0.1/st-diff-viewer/frontend/out/_next/static/chunks/pages/_app-2ddf65715eee6393.js
+-rw-r--r--   0        0        0      247 2024-05-17 12:17:04.591136 st_diff_viewer-1.0.1/st-diff-viewer/frontend/out/_next/static/chunks/pages/_error-54de1933a164a1ff.js
+-rw-r--r--   0        0        0     1085 2024-05-17 12:17:04.591435 st_diff_viewer-1.0.1/st-diff-viewer/frontend/out/_next/static/chunks/pages/index-08087b43971404a5.js
+-rw-r--r--   0        0        0    91381 2024-05-17 12:17:04.590542 st_diff_viewer-1.0.1/st-diff-viewer/frontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js
+-rw-r--r--   0        0        0     1485 2024-05-17 12:17:04.590151 st_diff_viewer-1.0.1/st-diff-viewer/frontend/out/_next/static/chunks/webpack-e057b7ebab7de5e1.js
+-rw-r--r--   0        0        0     4386 2024-05-17 12:17:04.590519 st_diff_viewer-1.0.1/st-diff-viewer/frontend/out/_next/static/css/34e82990737d7da2.css
+-rw-r--r--   0        0        0      321 2024-05-17 12:17:04.590626 st_diff_viewer-1.0.1/st-diff-viewer/frontend/out/_next/static/xI7DBa1wGxt2ZHYitxVGK/_buildManifest.js
+-rw-r--r--   0        0        0       77 2024-05-17 12:17:04.590850 st_diff_viewer-1.0.1/st-diff-viewer/frontend/out/_next/static/xI7DBa1wGxt2ZHYitxVGK/_ssgManifest.js
+-rw-r--r--   0        0        0    25931 2024-05-17 12:17:04.604347 st_diff_viewer-1.0.1/st-diff-viewer/frontend/out/favicon.ico
+-rw-r--r--   0        0        0     1986 2024-05-17 12:17:04.882333 st_diff_viewer-1.0.1/st-diff-viewer/frontend/out/index.html
+-rw-r--r--   0        0        0     1101 2024-05-17 12:17:04.604390 st_diff_viewer-1.0.1/st-diff-viewer/frontend/out/vercel.svg
+-rw-r--r--   0        0        0     1406 1970-01-01 00:00:00.000000 st_diff_viewer-1.0.1/PKG-INFO
```

### Comparing `st_diff_viewer-1.0.0/LICENSE` & `st_diff_viewer-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `st_diff_viewer-1.0.0/README.md` & `st_diff_viewer-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `st_diff_viewer-1.0.0/pyproject.toml` & `st_diff_viewer-1.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "st-diff-viewer"
-version = "1.0.0"
+version = "1.0.1"
 description = "A Streamlit component to display diff betoween two strings"
 authors = ["Xueyuan Lin <linxy59@mail2.sysu.eud.cn>"]
 readme = "README.md"
 packages = [{ include = "st-diff-viewer"}]
 
 license = "MIT"
 
 # Only include the out directory of the frontend
 # The order of the include/exclude lists is important!
-include = ["st-diff-viewer/frontend/out/**"]
+include = ["st-diff-viewer/frontend/out/**", "docs/**"]
 exclude = ["st-diff-viewer/frontend/*"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.9.7 || >3.9.7,<4.0"
 streamlit = ">=0.63"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `st_diff_viewer-1.0.0/st-diff-viewer/__init__.py` & `st_diff_viewer-1.0.1/st-diff-viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `st_diff_viewer-1.0.0/st-diff-viewer/frontend/out/404.html` & `st_diff_viewer-1.0.1/st-diff-viewer/frontend/out/404.html`

 * *Files 21% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><title>404: This page could not be found</title><meta name="next-head-count" content="3"/><link rel="preload" href="/component/streamlit_diff_viewer.streamlit_diff_viewer/_next/static/css/34e82990737d7da2.css" as="style"/><link rel="stylesheet" href="/component/streamlit_diff_viewer.streamlit_diff_viewer/_next/static/css/34e82990737d7da2.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/component/streamlit_diff_viewer.streamlit_diff_viewer/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/component/streamlit_diff_viewer.streamlit_diff_viewer/_next/static/chunks/webpack-545f75f9c7fe06d9.js" defer=""></script><script src="/component/streamlit_diff_viewer.streamlit_diff_viewer/_next/static/chunks/framework-c0663f0e1a0e4372.js" defer=""></script><script src="/component/streamlit_diff_viewer.streamlit_diff_viewer/_next/static/chunks/main-78a4b523a4dbe3d5.js" defer=""></script><script src="/component/streamlit_diff_viewer.streamlit_diff_viewer/_next/static/chunks/pages/_app-2ddf65715eee6393.js" defer=""></script><script src="/component/streamlit_diff_viewer.streamlit_diff_viewer/_next/static/chunks/pages/_error-54de1933a164a1ff.js" defer=""></script><script src="/component/streamlit_diff_viewer.streamlit_diff_viewer/_next/static/nIcdbMRjqlcHjjesGgyOg/_buildManifest.js" defer=""></script><script src="/component/streamlit_diff_viewer.streamlit_diff_viewer/_next/static/nIcdbMRjqlcHjjesGgyOg/_ssgManifest.js" defer=""></script></head><body><div id="__next"><div style="font-family:system-ui,&quot;Segoe UI&quot;,Roboto,Helvetica,Arial,sans-serif,&quot;Apple Color Emoji&quot;,&quot;Segoe UI Emoji&quot;;height:100vh;text-align:center;display:flex;flex-direction:column;align-items:center;justify-content:center"><div style="line-height:48px"><style>body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}</style><h1 class="next-error-h1" style="display:inline-block;margin:0 20px 0 0;padding-right:23px;font-size:24px;font-weight:500;vertical-align:top">404</h1><div style="display:inline-block"><h2 style="font-size:14px;font-weight:400;line-height:28px">This page could not be found<!-- -->.</h2></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"statusCode":404}},"page":"/_error","query":{},"buildId":"nIcdbMRjqlcHjjesGgyOg","assetPrefix":"/component/streamlit_diff_viewer.streamlit_diff_viewer","nextExport":true,"isFallback":false,"gip":true,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><title>404: This page could not be found</title><meta name="next-head-count" content="3"/><link rel="preload" href="/component/st-diff-viewer.st-diff-viewer/_next/static/css/34e82990737d7da2.css" as="style"/><link rel="stylesheet" href="/component/st-diff-viewer.st-diff-viewer/_next/static/css/34e82990737d7da2.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/component/st-diff-viewer.st-diff-viewer/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/component/st-diff-viewer.st-diff-viewer/_next/static/chunks/webpack-e057b7ebab7de5e1.js" defer=""></script><script src="/component/st-diff-viewer.st-diff-viewer/_next/static/chunks/framework-c0663f0e1a0e4372.js" defer=""></script><script src="/component/st-diff-viewer.st-diff-viewer/_next/static/chunks/main-7a1f841e500a3672.js" defer=""></script><script src="/component/st-diff-viewer.st-diff-viewer/_next/static/chunks/pages/_app-2ddf65715eee6393.js" defer=""></script><script src="/component/st-diff-viewer.st-diff-viewer/_next/static/chunks/pages/_error-54de1933a164a1ff.js" defer=""></script><script src="/component/st-diff-viewer.st-diff-viewer/_next/static/xI7DBa1wGxt2ZHYitxVGK/_buildManifest.js" defer=""></script><script src="/component/st-diff-viewer.st-diff-viewer/_next/static/xI7DBa1wGxt2ZHYitxVGK/_ssgManifest.js" defer=""></script></head><body><div id="__next"><div style="font-family:system-ui,&quot;Segoe UI&quot;,Roboto,Helvetica,Arial,sans-serif,&quot;Apple Color Emoji&quot;,&quot;Segoe UI Emoji&quot;;height:100vh;text-align:center;display:flex;flex-direction:column;align-items:center;justify-content:center"><div style="line-height:48px"><style>body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}</style><h1 class="next-error-h1" style="display:inline-block;margin:0 20px 0 0;padding-right:23px;font-size:24px;font-weight:500;vertical-align:top">404</h1><div style="display:inline-block"><h2 style="font-size:14px;font-weight:400;line-height:28px">This page could not be found<!-- -->.</h2></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"statusCode":404}},"page":"/_error","query":{},"buildId":"xI7DBa1wGxt2ZHYitxVGK","assetPrefix":"/component/st-diff-viewer.st-diff-viewer","nextExport":true,"isFallback":false,"gip":true,"scriptLoader":[]}</script></body></html>
```

### Comparing `st_diff_viewer-1.0.0/st-diff-viewer/frontend/out/_next/static/chunks/92-bf787e1cee9c20db.js` & `st_diff_viewer-1.0.1/st-diff-viewer/frontend/out/_next/static/chunks/92-bf787e1cee9c20db.js`

 * *Files identical despite different names*

### Comparing `st_diff_viewer-1.0.0/st-diff-viewer/frontend/out/_next/static/chunks/framework-c0663f0e1a0e4372.js` & `st_diff_viewer-1.0.1/st-diff-viewer/frontend/out/_next/static/chunks/framework-c0663f0e1a0e4372.js`

 * *Files identical despite different names*

### Comparing `st_diff_viewer-1.0.0/st-diff-viewer/frontend/out/_next/static/chunks/main-78a4b523a4dbe3d5.js` & `st_diff_viewer-1.0.1/st-diff-viewer/frontend/out/_next/static/chunks/main-7a1f841e500a3672.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -39,15 +39,15 @@
                     return o
                 }
             });
             let n = r(5246),
                 a = r(2387);
 
             function o(e, t) {
-                return (0, a.normalizePathTrailingSlash)((0, n.addPathPrefix)(e, "/component/streamlit_diff_viewer.streamlit_diff_viewer"))
+                return (0, a.normalizePathTrailingSlash)((0, n.addPathPrefix)(e, "/component/st-diff-viewer.st-diff-viewer"))
             }("function" == typeof t.default || "object" == typeof t.default && null !== t.default) && void 0 === t.default.__esModule && (Object.defineProperty(t.default, "__esModule", {
                 value: !0
             }), Object.assign(t.default, t), e.exports = t.default)
         },
         370: function(e, t, r) {
             "use strict";
             Object.defineProperty(t, "__esModule", {
@@ -92,15 +92,15 @@
                 get: function() {
                     return a
                 }
             });
             let n = r(6325);
 
             function a(e) {
-                return (0, n.pathHasPrefix)(e, "/component/streamlit_diff_viewer.streamlit_diff_viewer")
+                return (0, n.pathHasPrefix)(e, "/component/st-diff-viewer.st-diff-viewer")
             }("function" == typeof t.default || "object" == typeof t.default && null !== t.default) && void 0 === t.default.__esModule && (Object.defineProperty(t.default, "__esModule", {
                 value: !0
             }), Object.assign(t.default, t), e.exports = t.default)
         },
         9623: function(e, t) {
             "use strict";
             let r;
@@ -354,15 +354,15 @@
                     value: (0, L.makePublicRouterInstance)(n)
                 }, y.default.createElement(b.HeadManagerContext.Provider, {
                     value: u
                 }, y.default.createElement(I.ImageConfigContext.Provider, {
                     value: {
                         deviceSizes: [640, 750, 828, 1080, 1200, 1920, 2048, 3840],
                         imageSizes: [16, 32, 48, 64, 96, 128, 256, 384],
-                        path: "/component/streamlit_diff_viewer.streamlit_diff_viewer/_next/image",
+                        path: "/component/st-diff-viewer.st-diff-viewer/_next/image",
                         loader: "default",
                         dangerouslyAllowSVG: !1,
                         unoptimized: !0
                     }
                 }, r)))))))
             }
             let Z = e => t => {
@@ -822,15 +822,15 @@
                 value: !0
             }), Object.assign(t.default, t), e.exports = t.default)
         },
         9577: function(e, t, r) {
             "use strict";
 
             function n(e) {
-                return (e = e.slice(54)).startsWith("/") || (e = "/" + e), e
+                return (e = e.slice(40)).startsWith("/") || (e = "/" + e), e
             }
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), Object.defineProperty(t, "removeBasePath", {
                 enumerable: !0,
                 get: function() {
                     return n
@@ -3147,15 +3147,15 @@
                             numHashes: null,
                             bitArray: []
                         };
                         (null == t ? void 0 : t.numHashes) && (this._bfl_s = new e(t.numItems, t.errorRate), this._bfl_s.import(t)), (null == n ? void 0 : n.numHashes) && (this._bfl_d = new e(n.numItems, n.errorRate), this._bfl_d.import(n))
                     }
                     this.events = V.events, this.pageLoader = i;
                     let j = (0, h.isDynamicRoute)(e) && self.__NEXT_DATA__.autoExport;
-                    if (this.basePath = "/component/streamlit_diff_viewer.streamlit_diff_viewer", this.sub = f, this.clc = null, this._wrapApp = u, this.isSsr = !0, this.isLocaleDomain = !1, this.isReady = !!(self.__NEXT_DATA__.gssp || self.__NEXT_DATA__.gip || self.__NEXT_DATA__.appGip && !self.__NEXT_DATA__.gsp || !j && !self.location.search), this.state = {
+                    if (this.basePath = "/component/st-diff-viewer.st-diff-viewer", this.sub = f, this.clc = null, this._wrapApp = u, this.isSsr = !0, this.isLocaleDomain = !1, this.isReady = !!(self.__NEXT_DATA__.gssp || self.__NEXT_DATA__.gip || self.__NEXT_DATA__.appGip && !self.__NEXT_DATA__.gsp || !j && !self.location.search), this.state = {
                             route: S,
                             pathname: e,
                             query: t,
                             asPath: j ? e : n,
                             isPreview: !!P,
                             locale: void 0,
                             isFallback: m
```

### Comparing `st_diff_viewer-1.0.0/st-diff-viewer/frontend/out/_next/static/chunks/pages/index-08087b43971404a5.js` & `st_diff_viewer-1.0.1/st-diff-viewer/frontend/out/_next/static/chunks/pages/index-08087b43971404a5.js`

 * *Files identical despite different names*

### Comparing `st_diff_viewer-1.0.0/st-diff-viewer/frontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js` & `st_diff_viewer-1.0.1/st-diff-viewer/frontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js`

 * *Files identical despite different names*

### Comparing `st_diff_viewer-1.0.0/st-diff-viewer/frontend/out/_next/static/css/34e82990737d7da2.css` & `st_diff_viewer-1.0.1/st-diff-viewer/frontend/out/_next/static/css/34e82990737d7da2.css`

 * *Files identical despite different names*

### Comparing `st_diff_viewer-1.0.0/st-diff-viewer/frontend/out/favicon.ico` & `st_diff_viewer-1.0.1/st-diff-viewer/frontend/out/favicon.ico`

 * *Files identical despite different names*

### Comparing `st_diff_viewer-1.0.0/st-diff-viewer/frontend/out/index.html` & `st_diff_viewer-1.0.1/st-diff-viewer/frontend/out/index.html`

 * *Files 20% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><title>Create Next App</title><meta name="description" content="Generated by create next app"/><link rel="icon" href="/favicon.ico"/><meta name="next-head-count" content="5"/><link rel="preload" href="/component/streamlit_diff_viewer.streamlit_diff_viewer/_next/static/css/34e82990737d7da2.css" as="style"/><link rel="stylesheet" href="/component/streamlit_diff_viewer.streamlit_diff_viewer/_next/static/css/34e82990737d7da2.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/component/streamlit_diff_viewer.streamlit_diff_viewer/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/component/streamlit_diff_viewer.streamlit_diff_viewer/_next/static/chunks/webpack-545f75f9c7fe06d9.js" defer=""></script><script src="/component/streamlit_diff_viewer.streamlit_diff_viewer/_next/static/chunks/framework-c0663f0e1a0e4372.js" defer=""></script><script src="/component/streamlit_diff_viewer.streamlit_diff_viewer/_next/static/chunks/main-78a4b523a4dbe3d5.js" defer=""></script><script src="/component/streamlit_diff_viewer.streamlit_diff_viewer/_next/static/chunks/pages/_app-2ddf65715eee6393.js" defer=""></script><script src="/component/streamlit_diff_viewer.streamlit_diff_viewer/_next/static/chunks/92-bf787e1cee9c20db.js" defer=""></script><script src="/component/streamlit_diff_viewer.streamlit_diff_viewer/_next/static/chunks/pages/index-08087b43971404a5.js" defer=""></script><script src="/component/streamlit_diff_viewer.streamlit_diff_viewer/_next/static/nIcdbMRjqlcHjjesGgyOg/_buildManifest.js" defer=""></script><script src="/component/streamlit_diff_viewer.streamlit_diff_viewer/_next/static/nIcdbMRjqlcHjjesGgyOg/_ssgManifest.js" defer=""></script></head><body><div id="__next"></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"nIcdbMRjqlcHjjesGgyOg","assetPrefix":"/component/streamlit_diff_viewer.streamlit_diff_viewer","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><title>Create Next App</title><meta name="description" content="Generated by create next app"/><link rel="icon" href="/favicon.ico"/><meta name="next-head-count" content="5"/><link rel="preload" href="/component/st-diff-viewer.st-diff-viewer/_next/static/css/34e82990737d7da2.css" as="style"/><link rel="stylesheet" href="/component/st-diff-viewer.st-diff-viewer/_next/static/css/34e82990737d7da2.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/component/st-diff-viewer.st-diff-viewer/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/component/st-diff-viewer.st-diff-viewer/_next/static/chunks/webpack-e057b7ebab7de5e1.js" defer=""></script><script src="/component/st-diff-viewer.st-diff-viewer/_next/static/chunks/framework-c0663f0e1a0e4372.js" defer=""></script><script src="/component/st-diff-viewer.st-diff-viewer/_next/static/chunks/main-7a1f841e500a3672.js" defer=""></script><script src="/component/st-diff-viewer.st-diff-viewer/_next/static/chunks/pages/_app-2ddf65715eee6393.js" defer=""></script><script src="/component/st-diff-viewer.st-diff-viewer/_next/static/chunks/92-bf787e1cee9c20db.js" defer=""></script><script src="/component/st-diff-viewer.st-diff-viewer/_next/static/chunks/pages/index-08087b43971404a5.js" defer=""></script><script src="/component/st-diff-viewer.st-diff-viewer/_next/static/xI7DBa1wGxt2ZHYitxVGK/_buildManifest.js" defer=""></script><script src="/component/st-diff-viewer.st-diff-viewer/_next/static/xI7DBa1wGxt2ZHYitxVGK/_ssgManifest.js" defer=""></script></head><body><div id="__next"></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"xI7DBa1wGxt2ZHYitxVGK","assetPrefix":"/component/st-diff-viewer.st-diff-viewer","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `st_diff_viewer-1.0.0/st-diff-viewer/frontend/out/vercel.svg` & `st_diff_viewer-1.0.1/st-diff-viewer/frontend/out/vercel.svg`

 * *Files identical despite different names*

### Comparing `st_diff_viewer-1.0.0/PKG-INFO` & `st_diff_viewer-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-diff-viewer
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Streamlit component to display diff betoween two strings
 License: MIT
 Author: Xueyuan Lin
 Author-email: linxy59@mail2.sysu.eud.cn
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

