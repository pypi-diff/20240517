# Comparing `tmp/django_persian_pdf-0.1.2.tar.gz` & `tmp/django_persian_pdf-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_persian_pdf-0.1.2.tar", last modified: Fri Apr 19 09:14:18 2024, max compression
+gzip compressed data, was "django_persian_pdf-0.1.3.tar", last modified: Fri May 17 14:29:46 2024, max compression
```

## Comparing `django_persian_pdf-0.1.2.tar` & `django_persian_pdf-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 druid     (1000) druid     (1000)        0 2024-04-19 09:14:18.906850 django_persian_pdf-0.1.2/
--rw-rw-r--   0 druid     (1000) druid     (1000)      285 2024-04-19 07:35:17.000000 django_persian_pdf-0.1.2/CHANGELOG.rst
--rw-rw-r--   0 druid     (1000) druid     (1000)     1090 2024-03-14 12:36:31.000000 django_persian_pdf-0.1.2/LICENSE
--rw-rw-r--   0 druid     (1000) druid     (1000)      115 2024-03-08 22:52:06.000000 django_persian_pdf-0.1.2/MANIFEST.in
--rw-r--r--   0 druid     (1000) druid     (1000)     5843 2024-04-19 09:14:18.902850 django_persian_pdf-0.1.2/PKG-INFO
--rw-rw-r--   0 druid     (1000) druid     (1000)     4456 2024-04-19 09:03:37.000000 django_persian_pdf-0.1.2/README.rst
--rw-rw-r--   0 druid     (1000) druid     (1000)     1977 2024-04-19 09:03:54.000000 django_persian_pdf-0.1.2/pyproject.toml
--rw-rw-r--   0 druid     (1000) druid     (1000)       38 2024-04-19 09:14:18.906850 django_persian_pdf-0.1.2/setup.cfg
-drwxrwxr-x   0 druid     (1000) druid     (1000)        0 2024-04-19 09:14:18.898851 django_persian_pdf-0.1.2/src/
-drwxrwxr-x   0 druid     (1000) druid     (1000)        0 2024-04-19 09:14:18.902850 django_persian_pdf-0.1.2/src/django_persian_pdf/
--rw-rw-r--   0 druid     (1000) druid     (1000)      108 2024-04-19 07:20:34.000000 django_persian_pdf-0.1.2/src/django_persian_pdf/__init__.py
--rw-rw-r--   0 druid     (1000) druid     (1000)      179 2024-04-19 09:04:40.000000 django_persian_pdf-0.1.2/src/django_persian_pdf/apps.py
--rw-rw-r--   0 druid     (1000) druid     (1000)     2948 2024-01-12 14:26:45.000000 django_persian_pdf-0.1.2/src/django_persian_pdf/compilers.py
--rw-rw-r--   0 druid     (1000) druid     (1000)        0 2024-03-08 22:52:06.000000 django_persian_pdf-0.1.2/src/django_persian_pdf/py.typed
--rw-rw-r--   0 druid     (1000) druid     (1000)      236 2024-01-08 10:03:12.000000 django_persian_pdf-0.1.2/src/django_persian_pdf/responses.py
--rw-rw-r--   0 druid     (1000) druid     (1000)     1812 2024-04-19 07:20:34.000000 django_persian_pdf-0.1.2/src/django_persian_pdf/views.py
-drwxrwxr-x   0 druid     (1000) druid     (1000)        0 2024-04-19 09:14:18.902850 django_persian_pdf-0.1.2/src/django_persian_pdf.egg-info/
--rw-r--r--   0 druid     (1000) druid     (1000)     5843 2024-04-19 09:14:18.000000 django_persian_pdf-0.1.2/src/django_persian_pdf.egg-info/PKG-INFO
--rw-rw-r--   0 druid     (1000) druid     (1000)      490 2024-04-19 09:14:18.000000 django_persian_pdf-0.1.2/src/django_persian_pdf.egg-info/SOURCES.txt
--rw-rw-r--   0 druid     (1000) druid     (1000)        1 2024-04-19 09:14:18.000000 django_persian_pdf-0.1.2/src/django_persian_pdf.egg-info/dependency_links.txt
--rw-rw-r--   0 druid     (1000) druid     (1000)       12 2024-04-19 09:14:18.000000 django_persian_pdf-0.1.2/src/django_persian_pdf.egg-info/requires.txt
--rw-rw-r--   0 druid     (1000) druid     (1000)       19 2024-04-19 09:14:18.000000 django_persian_pdf-0.1.2/src/django_persian_pdf.egg-info/top_level.txt
+drwxrwxr-x   0 druid     (1000) druid     (1000)        0 2024-05-17 14:29:46.760231 django_persian_pdf-0.1.3/
+-rw-rw-r--   0 druid     (1000) druid     (1000)      285 2024-04-19 07:35:17.000000 django_persian_pdf-0.1.3/CHANGELOG.rst
+-rw-rw-r--   0 druid     (1000) druid     (1000)     1090 2024-03-14 12:36:31.000000 django_persian_pdf-0.1.3/LICENSE
+-rw-rw-r--   0 druid     (1000) druid     (1000)      115 2024-03-08 22:52:06.000000 django_persian_pdf-0.1.3/MANIFEST.in
+-rw-r--r--   0 druid     (1000) druid     (1000)     5866 2024-05-17 14:29:46.760231 django_persian_pdf-0.1.3/PKG-INFO
+-rw-rw-r--   0 druid     (1000) druid     (1000)     4479 2024-05-17 14:27:48.000000 django_persian_pdf-0.1.3/README.rst
+-rw-rw-r--   0 druid     (1000) druid     (1000)     2546 2024-05-17 14:27:48.000000 django_persian_pdf-0.1.3/pyproject.toml
+-rw-rw-r--   0 druid     (1000) druid     (1000)       38 2024-05-17 14:29:46.764231 django_persian_pdf-0.1.3/setup.cfg
+drwxrwxr-x   0 druid     (1000) druid     (1000)        0 2024-05-17 14:29:46.752231 django_persian_pdf-0.1.3/src/
+drwxrwxr-x   0 druid     (1000) druid     (1000)        0 2024-05-17 14:29:46.756231 django_persian_pdf-0.1.3/src/django_persian_pdf/
+-rw-rw-r--   0 druid     (1000) druid     (1000)      108 2024-05-17 14:27:48.000000 django_persian_pdf-0.1.3/src/django_persian_pdf/__init__.py
+-rw-rw-r--   0 druid     (1000) druid     (1000)      179 2024-05-17 14:27:48.000000 django_persian_pdf-0.1.3/src/django_persian_pdf/apps.py
+-rw-rw-r--   0 druid     (1000) druid     (1000)     2931 2024-05-17 14:27:48.000000 django_persian_pdf-0.1.3/src/django_persian_pdf/compilers.py
+-rw-rw-r--   0 druid     (1000) druid     (1000)        0 2024-03-08 22:52:06.000000 django_persian_pdf-0.1.3/src/django_persian_pdf/py.typed
+-rw-rw-r--   0 druid     (1000) druid     (1000)      236 2024-05-17 14:27:48.000000 django_persian_pdf-0.1.3/src/django_persian_pdf/responses.py
+-rw-rw-r--   0 druid     (1000) druid     (1000)     1811 2024-05-17 14:27:48.000000 django_persian_pdf-0.1.3/src/django_persian_pdf/views.py
+drwxrwxr-x   0 druid     (1000) druid     (1000)        0 2024-05-17 14:29:46.760231 django_persian_pdf-0.1.3/src/django_persian_pdf.egg-info/
+-rw-r--r--   0 druid     (1000) druid     (1000)     5866 2024-05-17 14:29:46.000000 django_persian_pdf-0.1.3/src/django_persian_pdf.egg-info/PKG-INFO
+-rw-rw-r--   0 druid     (1000) druid     (1000)      490 2024-05-17 14:29:46.000000 django_persian_pdf-0.1.3/src/django_persian_pdf.egg-info/SOURCES.txt
+-rw-rw-r--   0 druid     (1000) druid     (1000)        1 2024-05-17 14:29:46.000000 django_persian_pdf-0.1.3/src/django_persian_pdf.egg-info/dependency_links.txt
+-rw-rw-r--   0 druid     (1000) druid     (1000)       12 2024-05-17 14:29:46.000000 django_persian_pdf-0.1.3/src/django_persian_pdf.egg-info/requires.txt
+-rw-rw-r--   0 druid     (1000) druid     (1000)       19 2024-05-17 14:29:46.000000 django_persian_pdf-0.1.3/src/django_persian_pdf.egg-info/top_level.txt
```

### Comparing `django_persian_pdf-0.1.2/LICENSE` & `django_persian_pdf-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_persian_pdf-0.1.2/PKG-INFO` & `django_persian_pdf-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-persian-pdf
-Version: 0.1.2
+Version: 0.1.3
 Summary: Django class based views to generate pdf files using html or latex template.
 Author-email: Ali Abharya <abharya.dev@gmail.com>
 Maintainer-email: Ali Abharya <abharya.dev@gmail.com>
 License: MIT
 Project-URL: Changelog, https://github.com/bindruid/django-persian-pdf/blob/master/CHANGELOG.rst
 Project-URL: Repository, https://github.com/bindruid/django-persian-pdf
 Keywords: pdf,django,persian,xelatex
@@ -53,15 +53,15 @@
 -  ``HTMLToPDFDetailView`` is an extension of django ``DetailView`` using ``.html`` template  to generate pdf file.
 -  ``LatexToPDFTemplateView`` is an extension of django ``TemplateView`` using ``.tex`` template to generate pdf file.
 -  ``LatexToPDFDetailView`` is an extension of django ``DetailView`` using ``.tex`` template to generate pdf file.
 
 Status
 ------
 
-.. image:: https://github.com/bindruid/django-persian-pdf/workflows/Test/badge.svg?branch=master
+.. image:: https://img.shields.io/github/actions/workflow/status/bindruid/django-persian-pdf/test.yml.svg?branch=master
    :target: https://github.com/bindruid/django-persian-pdf/actions?workflow=Test
 
 .. image:: https://img.shields.io/pypi/v/django-persian-pdf.svg
    :target: https://pypi.python.org/pypi/django-persian-pdf
 
 .. image:: https://img.shields.io/pypi/pyversions/django-persian-pdf.svg
    :target: https://pypi.org/project/django-persian-pdf
```

### Comparing `django_persian_pdf-0.1.2/README.rst` & `django_persian_pdf-0.1.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 -  ``HTMLToPDFDetailView`` is an extension of django ``DetailView`` using ``.html`` template  to generate pdf file.
 -  ``LatexToPDFTemplateView`` is an extension of django ``TemplateView`` using ``.tex`` template to generate pdf file.
 -  ``LatexToPDFDetailView`` is an extension of django ``DetailView`` using ``.tex`` template to generate pdf file.
 
 Status
 ------
 
-.. image:: https://github.com/bindruid/django-persian-pdf/workflows/Test/badge.svg?branch=master
+.. image:: https://img.shields.io/github/actions/workflow/status/bindruid/django-persian-pdf/test.yml.svg?branch=master
    :target: https://github.com/bindruid/django-persian-pdf/actions?workflow=Test
 
 .. image:: https://img.shields.io/pypi/v/django-persian-pdf.svg
    :target: https://pypi.python.org/pypi/django-persian-pdf
 
 .. image:: https://img.shields.io/pypi/pyversions/django-persian-pdf.svg
    :target: https://pypi.org/project/django-persian-pdf
```

### Comparing `django_persian_pdf-0.1.2/src/django_persian_pdf/compilers.py` & `django_persian_pdf-0.1.3/src/django_persian_pdf/compilers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 import logging
 import os
-from subprocess import PIPE, run, CalledProcessError
-from tempfile import mkdtemp, NamedTemporaryFile, mkstemp
 from abc import ABC, abstractmethod
+from subprocess import PIPE, CalledProcessError, run
+from tempfile import NamedTemporaryFile, mkdtemp, mkstemp
 
 logger = logging.getLogger(__name__)
 
 
 class BaseCompiler(ABC):
     build_engine: str = None
     template_file_suffix: str = None
 
     def __init__(self, template_string: str):
         self.template_string = template_string
         self.temporary_build_folder = None
         self.temporary_build_file = None
-        self.pdf_file = NamedTemporaryFile(suffix=".pdf")
+        self.pdf_file = NamedTemporaryFile(suffix='.pdf')
         self.pdf_file.close()
 
     def clean_string(self) -> str:
         return self.template_string
 
     @abstractmethod
     def get_compile_command(self) -> str:
         pass
 
     def build(self):
         clean_string = self.clean_string()
         self.temporary_build_folder = mkdtemp()
-        temp_file, self.temporary_build_file = mkstemp(suffix=self.template_file_suffix,
-                                                       dir=self.temporary_build_folder)
+        temp_file, self.temporary_build_file = mkstemp(
+            suffix=self.template_file_suffix, dir=self.temporary_build_folder
+        )
         os.write(temp_file, str.encode(clean_string))
         os.close(temp_file)
 
     def compile(self):
         self.build()
 
         cmd = self.get_compile_command()
         try:
-            run(cmd, shell=True, stdout=PIPE, stderr=PIPE, check=True)
+            run(cmd, shell=True, stdout=PIPE, stderr=PIPE, check=True)  # noqa
 
         except CalledProcessError as called_process_error:
             logger.error(f'Failed compiling the pdf with error: {called_process_error.output}')
 
         return self.read()
 
     def read(self):
@@ -56,28 +57,28 @@
         return pdf_contents
 
 
 class LatexCompiler(BaseCompiler):
     build_engine = 'xelatex'
 
     def clean_string(self):
-        clean_string = self.template_string.replace("ـ", "-")
+        clean_string = self.template_string.replace('ـ', '-')
         clean_string = clean_string.replace('"', '\\"')
         clean_string = clean_string.replace("'", "\\'")
         clean_string = clean_string.replace('ي', 'ی')
         return clean_string
 
     def get_compile_command(self) -> str:
         cmd = f'{self.build_engine} -halt-on-error -output-directory={self.temporary_build_folder} {self.temporary_build_file}'
         return cmd
 
     def read(self):
         pdf_contents = ''
         try:
-            f = open(self.temporary_build_file + '.pdf', 'rb')
+            f = open(self.temporary_build_file + '.pdf', 'rb')  # noqa
             pdf_contents = f.read()
             f.close()
         except FileNotFoundError as err:
             logger.error(f'Failed reading pdf file: {err}')
         return pdf_contents
```

### Comparing `django_persian_pdf-0.1.2/src/django_persian_pdf/views.py` & `django_persian_pdf-0.1.3/src/django_persian_pdf/views.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from django.template import Template, Context
+from django.template import Context, Template
 from django.template.loader import get_template
 from django.utils.encoding import smart_str
 from django.views.generic.base import TemplateView
 from django.views.generic.detail import SingleObjectMixin
 
-from .compilers import LatexCompiler, ChromeCompiler
+from .compilers import ChromeCompiler, LatexCompiler
 from .responses import PDFResponse
 
 
 class PDFTemplateView(TemplateView):
     response_class = PDFResponse
     compiler_class = None
 
@@ -31,15 +31,14 @@
         template_path = template.origin.name
         with open(template_path) as f:
             content = f.read()
             return content
 
 
 class PDFDetailView(SingleObjectMixin, PDFTemplateView):
-
     def get(self, request, *args, **kwargs):
         self.object = self.get_object()
         context = self.get_context_data(object=self.object)
         return self.render_to_response(context)
 
 
 class LatexToPDFTemplateView(PDFTemplateView):
```

### Comparing `django_persian_pdf-0.1.2/src/django_persian_pdf.egg-info/PKG-INFO` & `django_persian_pdf-0.1.3/src/django_persian_pdf.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-persian-pdf
-Version: 0.1.2
+Version: 0.1.3
 Summary: Django class based views to generate pdf files using html or latex template.
 Author-email: Ali Abharya <abharya.dev@gmail.com>
 Maintainer-email: Ali Abharya <abharya.dev@gmail.com>
 License: MIT
 Project-URL: Changelog, https://github.com/bindruid/django-persian-pdf/blob/master/CHANGELOG.rst
 Project-URL: Repository, https://github.com/bindruid/django-persian-pdf
 Keywords: pdf,django,persian,xelatex
@@ -53,15 +53,15 @@
 -  ``HTMLToPDFDetailView`` is an extension of django ``DetailView`` using ``.html`` template  to generate pdf file.
 -  ``LatexToPDFTemplateView`` is an extension of django ``TemplateView`` using ``.tex`` template to generate pdf file.
 -  ``LatexToPDFDetailView`` is an extension of django ``DetailView`` using ``.tex`` template to generate pdf file.
 
 Status
 ------
 
-.. image:: https://github.com/bindruid/django-persian-pdf/workflows/Test/badge.svg?branch=master
+.. image:: https://img.shields.io/github/actions/workflow/status/bindruid/django-persian-pdf/test.yml.svg?branch=master
    :target: https://github.com/bindruid/django-persian-pdf/actions?workflow=Test
 
 .. image:: https://img.shields.io/pypi/v/django-persian-pdf.svg
    :target: https://pypi.python.org/pypi/django-persian-pdf
 
 .. image:: https://img.shields.io/pypi/pyversions/django-persian-pdf.svg
    :target: https://pypi.org/project/django-persian-pdf
```

