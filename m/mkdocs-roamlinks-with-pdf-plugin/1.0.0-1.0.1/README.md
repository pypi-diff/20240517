# Comparing `tmp/mkdocs-roamlinks-with-pdf-plugin-1.0.0.tar.gz` & `tmp/mkdocs-roamlinks-with-pdf-plugin-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-roamlinks-with-pdf-plugin-1.0.0.tar", last modified: Fri May 17 07:50:10 2024, max compression
+gzip compressed data, was "mkdocs-roamlinks-with-pdf-plugin-1.0.1.tar", last modified: Fri May 17 09:13:08 2024, max compression
```

## Comparing `mkdocs-roamlinks-with-pdf-plugin-1.0.0.tar` & `mkdocs-roamlinks-with-pdf-plugin-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-17 07:50:10.172442 mkdocs-roamlinks-with-pdf-plugin-1.0.0/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1055 2024-05-17 07:39:54.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.0/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)      870 2024-05-17 07:50:10.172442 mkdocs-roamlinks-with-pdf-plugin-1.0.0/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1598 2024-05-17 07:41:28.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.0/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-17 07:50:10.168442 mkdocs-roamlinks-with-pdf-plugin-1.0.0/mkdocs_roamlinks_with_pdf_plugin/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-17 07:37:28.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.0/mkdocs_roamlinks_with_pdf_plugin/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7707 2024-05-17 07:38:29.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.0/mkdocs_roamlinks_with_pdf_plugin/plugin.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-17 07:50:10.168442 mkdocs-roamlinks-with-pdf-plugin-1.0.0/mkdocs_roamlinks_with_pdf_plugin.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)      870 2024-05-17 07:50:10.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.0/mkdocs_roamlinks_with_pdf_plugin.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      491 2024-05-17 07:50:10.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.0/mkdocs_roamlinks_with_pdf_plugin.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-17 07:50:10.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.0/mkdocs_roamlinks_with_pdf_plugin.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       94 2024-05-17 07:50:10.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.0/mkdocs_roamlinks_with_pdf_plugin.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       28 2024-05-17 07:50:10.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.0/mkdocs_roamlinks_with_pdf_plugin.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       39 2024-05-17 07:50:10.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.0/mkdocs_roamlinks_with_pdf_plugin.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-17 07:50:10.172442 mkdocs-roamlinks-with-pdf-plugin-1.0.0/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1181 2024-05-17 07:43:34.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.0/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-17 07:50:10.168442 mkdocs-roamlinks-with-pdf-plugin-1.0.0/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-17 07:37:28.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.0/tests/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5273 2024-05-17 07:37:28.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.0/tests/test_plugin.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-17 09:13:08.232968 mkdocs-roamlinks-with-pdf-plugin-1.0.1/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1055 2024-05-17 07:39:54.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.1/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)      870 2024-05-17 09:13:08.232968 mkdocs-roamlinks-with-pdf-plugin-1.0.1/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1598 2024-05-17 07:41:28.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.1/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-17 09:13:08.228968 mkdocs-roamlinks-with-pdf-plugin-1.0.1/mkdocs_roamlinks_with_pdf_plugin/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-17 07:37:28.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.1/mkdocs_roamlinks_with_pdf_plugin/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10672 2024-05-17 09:08:28.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.1/mkdocs_roamlinks_with_pdf_plugin/plugin.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-17 09:13:08.232968 mkdocs-roamlinks-with-pdf-plugin-1.0.1/mkdocs_roamlinks_with_pdf_plugin.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)      870 2024-05-17 09:13:08.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.1/mkdocs_roamlinks_with_pdf_plugin.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      491 2024-05-17 09:13:08.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.1/mkdocs_roamlinks_with_pdf_plugin.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-17 09:13:08.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.1/mkdocs_roamlinks_with_pdf_plugin.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       94 2024-05-17 09:13:08.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.1/mkdocs_roamlinks_with_pdf_plugin.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       28 2024-05-17 09:13:08.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.1/mkdocs_roamlinks_with_pdf_plugin.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       39 2024-05-17 09:13:08.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.1/mkdocs_roamlinks_with_pdf_plugin.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-17 09:13:08.232968 mkdocs-roamlinks-with-pdf-plugin-1.0.1/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1181 2024-05-17 09:09:39.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.1/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-17 09:13:08.232968 mkdocs-roamlinks-with-pdf-plugin-1.0.1/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-17 07:37:28.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.1/tests/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5273 2024-05-17 07:37:28.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.1/tests/test_plugin.py
```

### Comparing `mkdocs-roamlinks-with-pdf-plugin-1.0.0/LICENSE` & `mkdocs-roamlinks-with-pdf-plugin-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-roamlinks-with-pdf-plugin-1.0.0/PKG-INFO` & `mkdocs-roamlinks-with-pdf-plugin-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-roamlinks-with-pdf-plugin
-Version: 1.0.0
+Version: 1.0.1
 Summary: An MkDocs plugin
 Home-page: https://github.com/jokulab/mkdocs-roamlinks-plugin
 Author: jokulab
 Author-email: 166611085+jokudev@users.noreply.github.com
 License: MIT
 Keywords: mkdocs
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mkdocs-roamlinks-with-pdf-plugin-1.0.0/README.md` & `mkdocs-roamlinks-with-pdf-plugin-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-roamlinks-with-pdf-plugin-1.0.0/mkdocs_roamlinks_with_pdf_plugin/plugin.py` & `mkdocs-roamlinks-with-pdf-plugin-1.0.1/mkdocs_roamlinks_with_pdf_plugin/plugin.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,24 +12,30 @@
 # For Regex, match groups are:
 #       0: Whole markdown link e.g. [Alt-text](url)
 #       1: Alt text
 #       2: Full URL e.g. url + hash anchor
 #       3: Filename e.g. filename.md
 #       4: File extension e.g. .md, .png, etc.
 #       5. hash anchor e.g. #my-sub-heading-link
-AUTOLINK_RE = r'\[([^\]]+)\]\((([^)/]+\.(md|png|jpg|pdf))(#.*)*)\)'
+AUTOLINK_RE = r'\[([^\]]+)\]\((([^)/]+\.(md|png|jpg))(#.*)*)\)'
 
 # For Regex, match groups are:
 #       0: Whole roamlike link e.g. [[filename#title|alias|widthxheight]]
 #       1: Filename e.g. filename.md
 #       2: #title
 #       3: alias
 #       4: width
 #       5: height
-ROAMLINK_RE = r"""\[\[(.*?)(\#.*?)?(?:\|([\D][^\|\]]+[\d]*))?(?:\|(\d+)(?:x(\d+))?)?\]\]"""
+ROAMLINK_RE = r"""\[\[(?!.*\.pdf)(.*?)(\#.*?)?(?:\|([\D][^\|\]]+[\d]*))?(?:\|(\d+)(?:x(\d+))?)?\]\]"""
+
+# For Regex, match groups are:
+#       0: Whole roamlike link e.g. [[filename.pdf#height=100]]
+#       1: Filename e.g. filename.pdf
+#       2: #height=<number> e.g. #height=100
+ROAMLINK_PDF_RE = r"""\[\[(.*?\.pdf)(\#height=\d+)?\]\]"""
 
 class AutoLinkReplacer:
     def __init__(self, base_docs_url, page_url):
         self.base_docs_url = base_docs_url
         self.page_url = page_url
 
     def __call__(self, match):
@@ -161,14 +167,69 @@
             link = f'{link}{{ height="{height}" }}'
         elif width and height:
             link = f'{link}{{ width="{width}"; height="{height}" }}'
 
         return link
 
 
+class RoamLinkPDFReplacer:
+    def __init__(self, base_docs_url, page_url):
+        self.base_docs_url = base_docs_url
+        self.page_url = page_url
+
+    def __call__(self, match):
+        # Name of the markdown file
+        whole_link = match.group(0)
+        filename = match.group(1).strip() if match.group(1) else ""
+        height = match.group(2).strip() if match.group(2) else ""
+
+        # Absolute URL of the linker
+        abs_linker_url = os.path.dirname(
+            os.path.join(self.base_docs_url, self.page_url))
+
+        # Find directory URL to target link
+        rel_link_url = ''
+        # Walk through all files in docs directory to find a matching file
+        if filename:
+            if '/' in filename:
+                if 'http' in filename: # http or https
+                    rel_link_url = filename
+                else:
+                    rel_file = filename
+
+                    abs_link_url = os.path.dirname(os.path.join(
+                        self.base_docs_url, rel_file))
+                    # Constructing relative path from the linker to the link
+                    rel_link_url = os.path.join(
+                            os.path.relpath(abs_link_url, abs_linker_url), os.path.basename(rel_file))
+                    if height:
+                        rel_link_url = rel_link_url + height
+            else:
+                for root, dirs, files in os.walk(self.base_docs_url, followlinks=True):
+                    for name in files:
+                        # If we have a match, create the relative path from linker to the link
+                        if self.simplify(name) == self.simplify(filename):
+                            # Absolute path to the file we want to link to
+                            abs_link_url = os.path.dirname(os.path.join(
+                                root, name))
+                            # Constructing relative path from the linker to the link
+                            rel_link_url = os.path.join(
+                                    os.path.relpath(abs_link_url, abs_linker_url), name)
+                            if height:
+                                rel_link_url = rel_link_url + height
+            if rel_link_url == '':
+                log.warning(f"RoamLinksPlugin unable to find {filename} in directory {self.base_docs_url}")
+                return whole_link
+
+        # Construct the return link
+        # Windows escapes "\" unintentionally, and it creates incorrect links, so need to replace with "/"
+        rel_link_url = rel_link_url.replace("\\", "/")
+
+        return f'[[{rel_link_url}]]'
+
 class RoamLinksPlugin(BasePlugin):
     def on_page_markdown(self,
                          markdown,
                          page,
                          config,
                          site_navigation=None,
                          **kwargs):
@@ -180,9 +241,11 @@
         page_url = page.file.src_path
 
         # Look for matches and replace
         markdown = re.sub(AUTOLINK_RE,
                           AutoLinkReplacer(base_docs_url, page_url), markdown)
         markdown = re.sub(ROAMLINK_RE,
                           RoamLinkReplacer(base_docs_url, page_url), markdown)
+        markdown = re.sub(ROAMLINK_PDF_RE,
+                          RoamLinkPDFReplacer(base_docs_url, page_url), markdown)
 
         return markdown
```

### Comparing `mkdocs-roamlinks-with-pdf-plugin-1.0.0/mkdocs_roamlinks_with_pdf_plugin.egg-info/PKG-INFO` & `mkdocs-roamlinks-with-pdf-plugin-1.0.1/mkdocs_roamlinks_with_pdf_plugin.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-roamlinks-with-pdf-plugin
-Version: 1.0.0
+Version: 1.0.1
 Summary: An MkDocs plugin
 Home-page: https://github.com/jokulab/mkdocs-roamlinks-plugin
 Author: jokulab
 Author-email: 166611085+jokudev@users.noreply.github.com
 License: MIT
 Keywords: mkdocs
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mkdocs-roamlinks-with-pdf-plugin-1.0.0/setup.py` & `mkdocs-roamlinks-with-pdf-plugin-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mkdocs-roamlinks-with-pdf-plugin',
-    version='1.0.0',
+    version='1.0.1',
     description='An MkDocs plugin',
     long_description='An MkDocs plugin that automagically generates relative links and convert roamlike links for foam and obsidian between markdown pages',
     keywords='mkdocs',
     url= 'https://github.com/jokulab/mkdocs-roamlinks-plugin',
     author='jokulab',
     author_email='166611085+jokudev@users.noreply.github.com',
     license='MIT',
```

### Comparing `mkdocs-roamlinks-with-pdf-plugin-1.0.0/tests/test_plugin.py` & `mkdocs-roamlinks-with-pdf-plugin-1.0.1/tests/test_plugin.py`

 * *Files identical despite different names*

