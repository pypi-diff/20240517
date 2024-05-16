# Comparing `tmp/sphinx_mdinclude-0.6.0.tar.gz` & `tmp/sphinx_mdinclude-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_mdinclude-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sphinx_mdinclude-0.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinx_mdinclude-0.6.0.tar` & `sphinx_mdinclude-0.6.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      180 2024-04-21 05:12:02.608182 sphinx_mdinclude-0.6.0/.flake8
--rw-r--r--   0        0        0      207 2024-04-21 05:13:19.859896 sphinx_mdinclude-0.6.0/.github/dependabot.yml
--rw-r--r--   0        0        0      139 2024-04-21 05:12:02.608456 sphinx_mdinclude-0.6.0/.github/issue_template.md
--rw-r--r--   0        0        0       61 2024-04-21 05:12:02.608551 sphinx_mdinclude-0.6.0/.github/pull_request_template.md
--rw-r--r--   0        0        0      682 2024-04-22 03:04:23.203972 sphinx_mdinclude-0.6.0/.github/workflows/build.yml
--rw-r--r--   0        0        0     1091 2024-04-21 05:12:02.608833 sphinx_mdinclude-0.6.0/.gitignore
--rw-r--r--   0        0        0       50 2024-04-21 05:13:19.860138 sphinx_mdinclude-0.6.0/.mailmap
--rw-r--r--   0        0        0      194 2024-04-21 05:13:19.860231 sphinx_mdinclude-0.6.0/.readthedocs.yml
--rw-r--r--   0        0        0     7240 2024-04-22 04:15:31.799081 sphinx_mdinclude-0.6.0/CHANGELOG.md
--rw-r--r--   0        0        0     1082 2024-04-21 05:12:02.609184 sphinx_mdinclude-0.6.0/LICENSE
--rw-r--r--   0        0        0     3026 2024-04-21 05:13:19.860494 sphinx_mdinclude-0.6.0/README.md
--rw-r--r--   0        0        0      598 2024-04-21 05:13:19.860593 sphinx_mdinclude-0.6.0/docs/_static/custom.css
--rw-r--r--   0        0        0    42080 2024-04-21 05:13:19.860779 sphinx_mdinclude-0.6.0/docs/_static/omnilib.png
--rw-r--r--   0        0        0      342 2024-04-21 05:12:02.609680 sphinx_mdinclude-0.6.0/docs/_templates/badges.html
--rw-r--r--   0        0        0     1145 2024-04-21 05:13:19.860912 sphinx_mdinclude-0.6.0/docs/_templates/omnilib.html
--rw-r--r--   0        0        0       71 2024-04-21 05:12:02.609868 sphinx_mdinclude-0.6.0/docs/changelog.rst
--rw-r--r--   0        0        0     2703 2024-04-21 05:13:19.861006 sphinx_mdinclude-0.6.0/docs/conf.py
--rw-r--r--   0        0        0     2991 2024-04-22 03:04:23.205071 sphinx_mdinclude-0.6.0/docs/example.md
--rw-r--r--   0        0        0       51 2024-04-21 05:12:02.610170 sphinx_mdinclude-0.6.0/docs/included.md
--rw-r--r--   0        0        0       99 2024-04-21 05:12:02.610262 sphinx_mdinclude-0.6.0/docs/index.md
--rw-r--r--   0        0        0      812 2024-04-22 03:04:23.205541 sphinx_mdinclude-0.6.0/makefile
--rw-r--r--   0        0        0     1841 2024-04-22 04:13:12.002236 sphinx_mdinclude-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      310 2024-04-21 05:12:02.610809 sphinx_mdinclude-0.6.0/sphinx_mdinclude/__init__.py
--rw-r--r--   0        0        0      156 2024-04-22 04:15:31.808781 sphinx_mdinclude-0.6.0/sphinx_mdinclude/__version__.py
--rw-r--r--   0        0        0     3473 2024-04-22 04:13:12.002541 sphinx_mdinclude-0.6.0/sphinx_mdinclude/parse.py
--rw-r--r--   0        0        0    12736 2024-04-22 04:13:12.003277 sphinx_mdinclude-0.6.0/sphinx_mdinclude/render.py
--rw-r--r--   0        0        0     5144 2024-04-22 04:13:12.003530 sphinx_mdinclude-0.6.0/sphinx_mdinclude/sphinx.py
--rw-r--r--   0        0        0      280 2024-04-22 03:04:23.207825 sphinx_mdinclude-0.6.0/sphinx_mdinclude/tests/__init__.py
--rw-r--r--   0        0        0      167 2024-04-22 03:04:23.208071 sphinx_mdinclude-0.6.0/sphinx_mdinclude/tests/__main__.py
--rw-r--r--   0        0        0      357 2024-04-22 03:04:23.208341 sphinx_mdinclude-0.6.0/sphinx_mdinclude/tests/test.md
--rw-r--r--   0        0        0      419 2024-04-22 03:04:23.208723 sphinx_mdinclude-0.6.0/sphinx_mdinclude/tests/test.rst
--rw-r--r--   0        0        0    24025 2024-04-22 04:13:12.003836 sphinx_mdinclude-0.6.0/sphinx_mdinclude/tests/test_renderer.py
--rw-r--r--   0        0        0     2121 2024-04-22 04:13:12.004172 sphinx_mdinclude-0.6.0/sphinx_mdinclude/tests/test_smoke.py
--rw-r--r--   0        0        0     4594 1970-01-01 00:00:00.000000 sphinx_mdinclude-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      189 2024-05-16 21:42:29.179638 sphinx_mdinclude-0.6.1/.flake8
+-rw-r--r--   0        0        0      207 2024-04-21 05:13:19.859896 sphinx_mdinclude-0.6.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      139 2024-04-21 05:12:02.608456 sphinx_mdinclude-0.6.1/.github/issue_template.md
+-rw-r--r--   0        0        0       61 2024-04-21 05:12:02.608551 sphinx_mdinclude-0.6.1/.github/pull_request_template.md
+-rw-r--r--   0        0        0      682 2024-04-22 03:04:23.203972 sphinx_mdinclude-0.6.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1091 2024-04-21 05:12:02.608833 sphinx_mdinclude-0.6.1/.gitignore
+-rw-r--r--   0        0        0       50 2024-04-21 05:13:19.860138 sphinx_mdinclude-0.6.1/.mailmap
+-rw-r--r--   0        0        0      194 2024-04-21 05:13:19.860231 sphinx_mdinclude-0.6.1/.readthedocs.yml
+-rw-r--r--   0        0        0     7480 2024-05-16 22:29:39.366307 sphinx_mdinclude-0.6.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1082 2024-04-21 05:12:02.609184 sphinx_mdinclude-0.6.1/LICENSE
+-rw-r--r--   0        0        0     3026 2024-04-21 05:13:19.860494 sphinx_mdinclude-0.6.1/README.md
+-rw-r--r--   0        0        0      598 2024-04-21 05:13:19.860593 sphinx_mdinclude-0.6.1/docs/_static/custom.css
+-rw-r--r--   0        0        0    42080 2024-04-21 05:13:19.860779 sphinx_mdinclude-0.6.1/docs/_static/omnilib.png
+-rw-r--r--   0        0        0      342 2024-04-21 05:12:02.609680 sphinx_mdinclude-0.6.1/docs/_templates/badges.html
+-rw-r--r--   0        0        0     1145 2024-04-21 05:13:19.860912 sphinx_mdinclude-0.6.1/docs/_templates/omnilib.html
+-rw-r--r--   0        0        0       71 2024-04-21 05:12:02.609868 sphinx_mdinclude-0.6.1/docs/changelog.rst
+-rw-r--r--   0        0        0     2703 2024-04-21 05:13:19.861006 sphinx_mdinclude-0.6.1/docs/conf.py
+-rw-r--r--   0        0        0     2991 2024-04-22 03:04:23.205071 sphinx_mdinclude-0.6.1/docs/example.md
+-rw-r--r--   0        0        0       51 2024-04-21 05:12:02.610170 sphinx_mdinclude-0.6.1/docs/included.md
+-rw-r--r--   0        0        0       99 2024-04-21 05:12:02.610262 sphinx_mdinclude-0.6.1/docs/index.md
+-rw-r--r--   0        0        0      812 2024-04-22 03:04:23.205541 sphinx_mdinclude-0.6.1/makefile
+-rw-r--r--   0        0        0     1861 2024-05-16 21:34:41.613348 sphinx_mdinclude-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      310 2024-04-21 05:12:02.610809 sphinx_mdinclude-0.6.1/sphinx_mdinclude/__init__.py
+-rw-r--r--   0        0        0      156 2024-05-16 22:29:39.377636 sphinx_mdinclude-0.6.1/sphinx_mdinclude/__version__.py
+-rw-r--r--   0        0        0     3473 2024-04-22 04:13:12.002541 sphinx_mdinclude-0.6.1/sphinx_mdinclude/parse.py
+-rw-r--r--   0        0        0    13161 2024-05-16 21:42:29.179923 sphinx_mdinclude-0.6.1/sphinx_mdinclude/render.py
+-rw-r--r--   0        0        0     5144 2024-04-22 04:13:12.003530 sphinx_mdinclude-0.6.1/sphinx_mdinclude/sphinx.py
+-rw-r--r--   0        0        0      280 2024-04-22 03:04:23.207825 sphinx_mdinclude-0.6.1/sphinx_mdinclude/tests/__init__.py
+-rw-r--r--   0        0        0      167 2024-04-22 03:04:23.208071 sphinx_mdinclude-0.6.1/sphinx_mdinclude/tests/__main__.py
+-rw-r--r--   0        0        0      357 2024-04-22 03:04:23.208341 sphinx_mdinclude-0.6.1/sphinx_mdinclude/tests/test.md
+-rw-r--r--   0        0        0      419 2024-04-22 03:04:23.208723 sphinx_mdinclude-0.6.1/sphinx_mdinclude/tests/test.rst
+-rw-r--r--   0        0        0    24445 2024-05-16 21:42:29.180203 sphinx_mdinclude-0.6.1/sphinx_mdinclude/tests/test_renderer.py
+-rw-r--r--   0        0        0     2121 2024-04-22 04:13:12.004172 sphinx_mdinclude-0.6.1/sphinx_mdinclude/tests/test_smoke.py
+-rw-r--r--   0        0        0     4622 1970-01-01 00:00:00.000000 sphinx_mdinclude-0.6.1/PKG-INFO
```

### Comparing `sphinx_mdinclude-0.6.0/.github/workflows/build.yml` & `sphinx_mdinclude-0.6.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.6.0/.gitignore` & `sphinx_mdinclude-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.6.0/CHANGELOG.md` & `sphinx_mdinclude-0.6.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,29 @@
 sphinx-mdinclude
 ================
 
 [![Generated by attribution][attribution-badge]][attribution-url]
 
 
+v0.6.1
+------
+
+Bugfix release
+
+- Fix rendering of codespans within link text (#68)
+- Added explicit dependency on Sphinx (#70)
+
+```text
+$ git shortlog -s v0.6.0...v0.6.1
+     2	Amethyst Reese
+     1	Peter Sobot
+     5	dependabot[bot]
+```
+
+
 v0.6.0
 ------
 
 Feature release
 
 - Added support for mistune v3, dropped support for mistune v2 (#22, #46)
 - Added strict type annotations and type checking (#62)
```

### Comparing `sphinx_mdinclude-0.6.0/LICENSE` & `sphinx_mdinclude-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.6.0/README.md` & `sphinx_mdinclude-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.6.0/docs/_static/custom.css` & `sphinx_mdinclude-0.6.1/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.6.0/docs/_static/omnilib.png` & `sphinx_mdinclude-0.6.1/docs/_static/omnilib.png`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.6.0/docs/_templates/omnilib.html` & `sphinx_mdinclude-0.6.1/docs/_templates/omnilib.html`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.6.0/docs/conf.py` & `sphinx_mdinclude-0.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.6.0/docs/example.md` & `sphinx_mdinclude-0.6.1/docs/example.md`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.6.0/makefile` & `sphinx_mdinclude-0.6.1/makefile`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.6.0/pyproject.toml` & `sphinx_mdinclude-0.6.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -24,28 +24,29 @@
 keywords = ["Markdown", "reStructuredText", "sphinx-extension"]
 dynamic = ["version", "description"]
 requires-python = ">=3.8"
 dependencies = [
     "mistune >=3.0,<4.0",
     "docutils >=0.16,<1.0",
     "pygments >= 2.8",
+    "sphinx >= 6",
 ]
 
 [project.optional-dependencies]
 dev = [
     "docutils==0.20.1; python_version < '3.9'",
-    "docutils==0.21.1; python_version >= '3.9'",
+    "docutils==0.21.2; python_version >= '3.9'",
     "mistune==3.0.2",
 
     "attribution==1.7.1",
-    "black==24.4.0",
-    "coverage==7.4.4",
+    "black==24.4.2",
+    "coverage==7.5.1",
     "flake8==7.0.0",
     "flit==3.9.0",
-    "mypy==1.9.0",
+    "mypy==1.10.0",
     "sphinx==7.1.2; python_version < '3.9'",
     "sphinx==7.3.7; python_version >= '3.9'",
     "ufmt==2.5.1",
     "usort==1.0.8.post1",
 ]
 
 [project.urls]
```

### Comparing `sphinx_mdinclude-0.6.0/sphinx_mdinclude/parse.py` & `sphinx_mdinclude-0.6.1/sphinx_mdinclude/parse.py`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.6.0/sphinx_mdinclude/render.py` & `sphinx_mdinclude-0.6.1/sphinx_mdinclude/render.py`

 * *Files 4% similar despite different names*

```diff
@@ -237,14 +237,25 @@
         :param url: URL for ``<a>`` tag.
         :param title: title content for `title` attribute.
         """
         if text.startswith("\n.. image::"):
             text = re.sub(r":target: (.*)\n", f":target: {url}\n", text)
             return text
 
+        if text.startswith("``") and text.endswith("``"):
+            # Return raw HTML for inline code:
+            html = (
+                '<code class="docutils literal">'
+                '<span class="pre">{}</span>'
+                "</code>".format(text[2:-2].replace("`", "&#96;"))
+            )
+            return self._raw_html(
+                '<a href="{url}">{text}</a>'.format(url=url, text=html)
+            )
+
         underscore = "_"
         if title:
             return self._raw_html(
                 '<a href="{url}" title="{title}">{text}</a>'.format(
                     url=url, title=title, text=text
                 )
             )
```

### Comparing `sphinx_mdinclude-0.6.0/sphinx_mdinclude/sphinx.py` & `sphinx_mdinclude-0.6.1/sphinx_mdinclude/sphinx.py`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.6.0/sphinx_mdinclude/tests/test_renderer.py` & `sphinx_mdinclude-0.6.1/sphinx_mdinclude/tests/test_renderer.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,14 +143,25 @@
             out.strip(),
             ".. role:: raw-html-md(raw)\n"
             "   :format: html\n\n\n"
             ':raw-html-md:`<code class="docutils literal">'
             '<span class="pre">&#96;a&#96;</span></code>`',
         )
 
+    def test_inline_code_within_link(self) -> None:
+        src = "[`foobar`](https://example.com)"
+        out = self.conv(src)
+        self.assertEqual(
+            out.strip(),
+            ".. role:: raw-html-md(raw)\n"
+            "   :format: html\n\n\n"
+            ':raw-html-md:`<a href="https://example.com"><code class="docutils literal">'
+            '<span class="pre">foobar</span></code></a>`',
+        )
+
     def test_strikethrough(self) -> None:
         src = "~~a~~"
         self.conv(src)
 
     def test_emphasis(self) -> None:
         src = "*a*"
         out = self.conv(src)
```

### Comparing `sphinx_mdinclude-0.6.0/sphinx_mdinclude/tests/test_smoke.py` & `sphinx_mdinclude-0.6.1/sphinx_mdinclude/tests/test_smoke.py`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.6.0/PKG-INFO` & `sphinx_mdinclude-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx_mdinclude
-Version: 0.6.0
+Version: 0.6.1
 Summary: Markdown extension for Sphinx
 Keywords: Markdown,reStructuredText,sphinx-extension
 Author-email: Hiroyuki Takagi <miyako.dev@gmail.com>, CrossNox <ijmermet+m2r2@gmail.com>, Amethyst Reese <amy@noswap.com>
 Maintainer-email: Amethyst Reese <amy@noswap.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
@@ -12,23 +12,24 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Topic :: Text Processing
 Requires-Dist: mistune >=3.0,<4.0
 Requires-Dist: docutils >=0.16,<1.0
 Requires-Dist: pygments >= 2.8
+Requires-Dist: sphinx >= 6
 Requires-Dist: docutils==0.20.1 ; extra == "dev" and ( python_version < '3.9')
-Requires-Dist: docutils==0.21.1 ; extra == "dev" and ( python_version >= '3.9')
+Requires-Dist: docutils==0.21.2 ; extra == "dev" and ( python_version >= '3.9')
 Requires-Dist: mistune==3.0.2 ; extra == "dev"
 Requires-Dist: attribution==1.7.1 ; extra == "dev"
-Requires-Dist: black==24.4.0 ; extra == "dev"
-Requires-Dist: coverage==7.4.4 ; extra == "dev"
+Requires-Dist: black==24.4.2 ; extra == "dev"
+Requires-Dist: coverage==7.5.1 ; extra == "dev"
 Requires-Dist: flake8==7.0.0 ; extra == "dev"
 Requires-Dist: flit==3.9.0 ; extra == "dev"
-Requires-Dist: mypy==1.9.0 ; extra == "dev"
+Requires-Dist: mypy==1.10.0 ; extra == "dev"
 Requires-Dist: sphinx==7.1.2 ; extra == "dev" and ( python_version < '3.9')
 Requires-Dist: sphinx==7.3.7 ; extra == "dev" and ( python_version >= '3.9')
 Requires-Dist: ufmt==2.5.1 ; extra == "dev"
 Requires-Dist: usort==1.0.8.post1 ; extra == "dev"
 Project-URL: Github, https://github.com/omnilib/sphinx-mdinclude
 Provides-Extra: dev
```

