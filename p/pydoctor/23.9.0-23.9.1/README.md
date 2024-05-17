# Comparing `tmp/pydoctor-23.9.0.tar.gz` & `tmp/pydoctor-23.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydoctor-23.9.0.tar", last modified: Sun Sep 24 14:00:24 2023, max compression
+gzip compressed data, was "pydoctor-23.9.1.tar", last modified: Sat Nov  4 23:43:25 2023, max compression
```

## Comparing `pydoctor-23.9.0.tar` & `pydoctor-23.9.1.tar`

### file list

```diff
@@ -1,333 +1,333 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.356934 pydoctor-23.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2023-09-24 14:00:18.000000 pydoctor-23.9.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-09-24 14:00:18.000000 pydoctor-23.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    22121 2023-09-24 14:00:24.356934 pydoctor-23.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19753 2023-09-24 14:00:18.000000 pydoctor-23.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.328933 pydoctor-23.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.328933 pydoctor-23.9.0/docs/epytext_demo/
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/epytext_demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/epytext_demo/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5428 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/epytext_demo/demo_epytext_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.328933 pydoctor-23.9.0/docs/google_demo/
--rw-r--r--   0 runner    (1001) docker     (127)     9329 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/google_demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.328933 pydoctor-23.9.0/docs/numpy_demo/
--rw-r--r--   0 runner    (1001) docker     (127)     9516 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/numpy_demo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.328933 pydoctor-23.9.0/docs/restructuredtext_demo/
--rw-r--r--   0 runner    (1001) docker     (127)     6840 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/restructuredtext_demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/restructuredtext_demo/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5859 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/restructuredtext_demo/demo_restructuredtext_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.328933 pydoctor-23.9.0/docs/sample_template/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/sample_template/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)      729 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/sample_template/header.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.328933 pydoctor-23.9.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.328933 pydoctor-23.9.0/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/source/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    14427 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/source/codedoc.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6169 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8419 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/source/contrib.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.328933 pydoctor-23.9.0/docs/source/custom_template_demo/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/source/custom_template_demo/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      404 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/source/custom_template_demo/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     9284 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/source/customize.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.332933 pydoctor-23.9.0/docs/source/docformat/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/source/docformat/epytext.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.332933 pydoctor-23.9.0/docs/source/docformat/epytext_demo/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/source/docformat/epytext_demo/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/source/docformat/google-numpy.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.332933 pydoctor-23.9.0/docs/source/docformat/google_demo/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/source/docformat/google_demo/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/source/docformat/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7304 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/source/docformat/list-restructuredtext-support.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.332933 pydoctor-23.9.0/docs/source/docformat/numpy_demo/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/source/docformat/numpy_demo/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/source/docformat/restructuredtext.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.332933 pydoctor-23.9.0/docs/source/docformat/restructuredtext_demo/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/source/docformat/restructuredtext_demo/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/source/help.rst
--rw-r--r--   0 runner    (1001) docker     (127)      412 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/source/publish-github-action.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/source/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/source/sphinx-integration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      845 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/source/transition.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.332933 pydoctor-23.9.0/docs/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/tests/test-search.html
--rw-r--r--   0 runner    (1001) docker     (127)     9932 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/tests/test_python_igraph_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/tests/test_standard_library_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2023-09-24 14:00:18.000000 pydoctor-23.9.0/docs/tests/test_twisted_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.332933 pydoctor-23.9.0/pydoctor/
--rw-r--r--   0 runner    (1001) docker     (127)      543 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18979 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/_configparser.py
--rw-r--r--   0 runner    (1001) docker     (127)    52141 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/astbuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)    16856 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/astutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6539 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.336933 pydoctor-23.9.0/pydoctor/epydoc/
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/epydoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7391 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/epydoc/doctest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5866 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/epydoc/docutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.336933 pydoctor-23.9.0/pydoctor/epydoc/markup/
--rw-r--r--   0 runner    (1001) docker     (127)    18076 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/epydoc/markup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/epydoc/markup/_napoleon.py
--rw-r--r--   0 runner    (1001) docker     (127)    45239 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/epydoc/markup/_pyval_repr.py
--rw-r--r--   0 runner    (1001) docker     (127)     8171 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/epydoc/markup/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    56006 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/epydoc/markup/epytext.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/epydoc/markup/google.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/epydoc/markup/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/epydoc/markup/plaintext.py
--rw-r--r--   0 runner    (1001) docker     (127)    20001 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/epydoc/markup/restructuredtext.py
--rw-r--r--   0 runner    (1001) docker     (127)     6924 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/epydoc/sre_constants36.py
--rw-r--r--   0 runner    (1001) docker     (127)    38153 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/epydoc/sre_parse36.py
--rw-r--r--   0 runner    (1001) docker     (127)    43492 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/epydoc2stan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.336933 pydoctor-23.9.0/pydoctor/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)     6562 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6484 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/extensions/attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/extensions/deprecate.py
--rw-r--r--   0 runner    (1001) docker     (127)    14017 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/extensions/zopeinterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    10847 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/linker.py
--rw-r--r--   0 runner    (1001) docker     (127)    62319 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/mro.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.336933 pydoctor-23.9.0/pydoctor/napoleon/
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/napoleon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59464 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/napoleon/docstring.py
--rw-r--r--   0 runner    (1001) docker     (127)     8808 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/napoleon/iterators.py
--rw-r--r--   0 runner    (1001) docker     (127)    11099 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/node2stan.py
--rw-r--r--   0 runner    (1001) docker     (127)    19315 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/qnmatch.py
--rw-r--r--   0 runner    (1001) docker     (127)    12913 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/sphinx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.336933 pydoctor-23.9.0/pydoctor/sphinx_ext/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/sphinx_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5618 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/sphinx_ext/build_apidocs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/stanutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.336933 pydoctor-23.9.0/pydoctor/templatewriter/
--rw-r--r--   0 runner    (1001) docker     (127)    16888 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/templatewriter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.336933 pydoctor-23.9.0/pydoctor/templatewriter/pages/
--rw-r--r--   0 runner    (1001) docker     (127)    22630 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/templatewriter/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/templatewriter/pages/attributechild.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/templatewriter/pages/functionchild.py
--rw-r--r--   0 runner    (1001) docker     (127)    16423 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/templatewriter/pages/sidebar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/templatewriter/pages/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     6639 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/templatewriter/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    12964 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/templatewriter/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     7627 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/templatewriter/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6010 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/templatewriter/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.340933 pydoctor-23.9.0/pydoctor/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.340933 pydoctor-23.9.0/pydoctor/test/epydoc/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/epydoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/epydoc/epytext.doctest
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/epydoc/restructuredtext.doctest
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/epydoc/test_epytext.py
--rw-r--r--   0 runner    (1001) docker     (127)    11254 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/epydoc/test_epytext2html.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/epydoc/test_epytext2node.py
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/epydoc/test_google_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/epydoc/test_parsed_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (127)    43455 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/epydoc/test_pyval_repr.py
--rw-r--r--   0 runner    (1001) docker     (127)    11641 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/epydoc/test_restructuredtext.py
--rw-r--r--   0 runner    (1001) docker     (127)    90196 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/test_astbuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/test_attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/test_colorize.py
--rw-r--r--   0 runner    (1001) docker     (127)     8968 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/test_commandline.py
--rw-r--r--   0 runner    (1001) docker     (127)    25534 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/test_configparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/test_cyclic_imports_base_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    70217 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/test_epydoc2stan.py
--rw-r--r--   0 runner    (1001) docker     (127)    17068 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8883 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/test_mro.py
--rw-r--r--   0 runner    (1001) docker     (127)    85527 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/test_napoleon_docstring.py
--rw-r--r--   0 runner    (1001) docker     (127)    11945 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/test_napoleon_iterators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4559 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/test_node2stan.py
--rw-r--r--   0 runner    (1001) docker     (127)     9007 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/test_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     7016 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/test_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/test_pydantic_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     5052 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/test_qnmatch.py
--rw-r--r--   0 runner    (1001) docker     (127)    22037 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/test_sphinx.py
--rw-r--r--   0 runner    (1001) docker     (127)    31453 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/test_templatewriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7512 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/test_twisted_python_deprecate.py
--rw-r--r--   0 runner    (1001) docker     (127)    16016 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/test_type_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/test_visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    21531 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/test_zopeinterface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.324932 pydoctor-23.9.0/pydoctor/test/testcustomtemplates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.340933 pydoctor-23.9.0/pydoctor/test/testcustomtemplates/allok/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testcustomtemplates/allok/nav.html
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testcustomtemplates/allok/pydoctor.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.324932 pydoctor-23.9.0/pydoctor/test/testcustomtemplates/casing/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.340933 pydoctor-23.9.0/pydoctor/test/testcustomtemplates/casing/test1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testcustomtemplates/casing/test1/nav.HTML
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.340933 pydoctor-23.9.0/pydoctor/test/testcustomtemplates/casing/test2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testcustomtemplates/casing/test2/nav.Html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.340933 pydoctor-23.9.0/pydoctor/test/testcustomtemplates/casing/test3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testcustomtemplates/casing/test3/nav.htmL
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.344934 pydoctor-23.9.0/pydoctor/test/testcustomtemplates/faketemplate/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testcustomtemplates/faketemplate/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testcustomtemplates/faketemplate/header.html
--rw-r--r--   0 runner    (1001) docker     (127)      615 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testcustomtemplates/faketemplate/nav.html
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testcustomtemplates/faketemplate/pydoctor.js
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testcustomtemplates/faketemplate/random.html
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testcustomtemplates/faketemplate/subheader.html
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testcustomtemplates/faketemplate/summary.html
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testcustomtemplates/faketemplate/table.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.324932 pydoctor-23.9.0/pydoctor/test/testcustomtemplates/overridesubfolders/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.324932 pydoctor-23.9.0/pydoctor/test/testcustomtemplates/overridesubfolders/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.344934 pydoctor-23.9.0/pydoctor/test/testcustomtemplates/overridesubfolders/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testcustomtemplates/overridesubfolders/static/fonts/foo.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.344934 pydoctor-23.9.0/pydoctor/test/testcustomtemplates/subfolders/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testcustomtemplates/subfolders/atemplate.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.344934 pydoctor-23.9.0/pydoctor/test/testcustomtemplates/subfolders/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.344934 pydoctor-23.9.0/pydoctor/test/testcustomtemplates/subfolders/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testcustomtemplates/subfolders/static/fonts/bar.svg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testcustomtemplates/subfolders/static/fonts/foo.svg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testcustomtemplates/subfolders/static/info.svg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testcustomtemplates/subfolders/static/lol.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.324932 pydoctor-23.9.0/pydoctor/test/testpackages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.344934 pydoctor-23.9.0/pydoctor/test/testpackages/allgames/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/allgames/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/allgames/mod1.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/allgames/mod2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.344934 pydoctor-23.9.0/pydoctor/test/testpackages/basic/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/basic/_private_mod.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/basic/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.344934 pydoctor-23.9.0/pydoctor/test/testpackages/c_module_invalid_text_signature/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.344934 pydoctor-23.9.0/pydoctor/test/testpackages/c_module_invalid_text_signature/mymod/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/c_module_invalid_text_signature/mymod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/c_module_invalid_text_signature/mymod/base.c
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/c_module_invalid_text_signature/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.344934 pydoctor-23.9.0/pydoctor/test/testpackages/c_module_python_module_name_clash/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.344934 pydoctor-23.9.0/pydoctor/test/testpackages/c_module_python_module_name_clash/mymod/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/c_module_python_module_name_clash/mymod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/c_module_python_module_name_clash/mymod/base.c
--rw-r--r--   0 runner    (1001) docker     (127)      590 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/c_module_python_module_name_clash/mymod/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/c_module_python_module_name_clash/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.344934 pydoctor-23.9.0/pydoctor/test/testpackages/codeininit/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/codeininit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.344934 pydoctor-23.9.0/pydoctor/test/testpackages/cyclic_imports/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/cyclic_imports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/cyclic_imports/a.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/cyclic_imports/b.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.344934 pydoctor-23.9.0/pydoctor/test/testpackages/cyclic_imports_base_classes/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/cyclic_imports_base_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/cyclic_imports_base_classes/a.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/cyclic_imports_base_classes/b.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.344934 pydoctor-23.9.0/pydoctor/test/testpackages/importingfrompackage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/importingfrompackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/importingfrompackage/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.344934 pydoctor-23.9.0/pydoctor/test/testpackages/importingfrompackage/subpack/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/importingfrompackage/subpack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        2 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/importingfrompackage/subpack/submod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.344934 pydoctor-23.9.0/pydoctor/test/testpackages/interfaceallgames/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/interfaceallgames/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/interfaceallgames/_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/interfaceallgames/implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/interfaceallgames/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.344934 pydoctor-23.9.0/pydoctor/test/testpackages/interfaceclass/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/interfaceclass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/interfaceclass/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.344934 pydoctor-23.9.0/pydoctor/test/testpackages/liveobject/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/liveobject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/liveobject/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.348934 pydoctor-23.9.0/pydoctor/test/testpackages/modnamedafterbuiltin/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/modnamedafterbuiltin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/modnamedafterbuiltin/dict.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/modnamedafterbuiltin/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.348934 pydoctor-23.9.0/pydoctor/test/testpackages/multipleinheritance/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/multipleinheritance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/multipleinheritance/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.348934 pydoctor-23.9.0/pydoctor/test/testpackages/nestedconfusion/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/nestedconfusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/nestedconfusion/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.348934 pydoctor-23.9.0/pydoctor/test/testpackages/package_module_name_clash/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/package_module_name_clash/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.348934 pydoctor-23.9.0/pydoctor/test/testpackages/package_module_name_clash/pack/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/package_module_name_clash/pack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/package_module_name_clash/pack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.348934 pydoctor-23.9.0/pydoctor/test/testpackages/relativeimporttest/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/relativeimporttest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/relativeimporttest/mod1.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/relativeimporttest/mod2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.348934 pydoctor-23.9.0/pydoctor/test/testpackages/reparented_module/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/reparented_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/reparented_module/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.348934 pydoctor-23.9.0/pydoctor/test/testpackages/reparenting_crash/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/reparenting_crash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/reparenting_crash/reparenting_crash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.348934 pydoctor-23.9.0/pydoctor/test/testpackages/reparenting_crash_alt/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/reparenting_crash_alt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/reparenting_crash_alt/_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/reparenting_crash_alt/reparenting_crash_alt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.348934 pydoctor-23.9.0/pydoctor/test/testpackages/reparenting_follows_aliases/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/reparenting_follows_aliases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/reparenting_follows_aliases/_myotherthing.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/reparenting_follows_aliases/_mything.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/reparenting_follows_aliases/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.348934 pydoctor-23.9.0/pydoctor/test/testpackages/report_trigger/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/report_trigger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/report_trigger/report_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.348934 pydoctor-23.9.0/pydoctor/test/testpackages/syntax_error/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/test/testpackages/syntax_error/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.348934 pydoctor-23.9.0/pydoctor/themes/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.352934 pydoctor-23.9.0/pydoctor/themes/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/base/ajax.js
--rw-r--r--   0 runner    (1001) docker     (127)      943 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/base/all-documents.html
--rw-r--r--   0 runner    (1001) docker     (127)    22329 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/base/apidocs.css
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/base/attribute-child.html
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/base/common.html
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/base/extra.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.352934 pydoctor-23.9.0/pydoctor/themes/base/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)      474 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/base/fonts/info.svg
--rw-r--r--   0 runner    (1001) docker     (127)      423 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/base/fonts/x-circle.svg
--rw-r--r--   0 runner    (1001) docker     (127)      746 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/base/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)      994 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/base/function-child.html
--rw-r--r--   0 runner    (1001) docker     (127)      657 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/base/head.html
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/base/header.html
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/base/index.html
--rw-r--r--   0 runner    (1001) docker     (127)   113673 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/base/lunr.js
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/base/nameIndex.html
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/base/nav.html
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/base/pydoctor.js
--rw-r--r--   0 runner    (1001) docker     (127)    14286 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/base/search.js
--rw-r--r--   0 runner    (1001) docker     (127)    15394 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/base/searchlib.js
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/base/sidebar-list.html
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/base/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/base/sidebartoggle.js
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/base/subheader.html
--rw-r--r--   0 runner    (1001) docker     (127)      809 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/base/summary.html
--rw-r--r--   0 runner    (1001) docker     (127)      423 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/base/table.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.352934 pydoctor-23.9.0/pydoctor/themes/classic/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/classic/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)   117305 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/classic/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      728 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/classic/head.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.352934 pydoctor-23.9.0/pydoctor/themes/readthedocs/
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/readthedocs/common.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.352934 pydoctor-23.9.0/pydoctor/themes/readthedocs/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    67312 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/readthedocs/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    66444 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/readthedocs/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (127)      963 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/readthedocs/fonts/book.svg
--rw-r--r--   0 runner    (1001) docker     (127)      479 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/readthedocs/fonts/home.svg
--rw-r--r--   0 runner    (1001) docker     (127)   184912 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/readthedocs/fonts/lato-bold.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   182708 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/readthedocs/fonts/lato-normal.woff2
--rw-r--r--   0 runner    (1001) docker     (127)      485 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/readthedocs/fonts/minus-square-o.svg
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/readthedocs/fonts/plus-square-o.svg
--rw-r--r--   0 runner    (1001) docker     (127)      649 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/readthedocs/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)      731 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/readthedocs/head.html
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/readthedocs/nav.html
--rw-r--r--   0 runner    (1001) docker     (127)    16297 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/themes/readthedocs/readthedocstheme.css
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10818 2023-09-24 14:00:18.000000 pydoctor-23.9.0/pydoctor/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:00:24.332933 pydoctor-23.9.0/pydoctor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22121 2023-09-24 14:00:24.000000 pydoctor-23.9.0/pydoctor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10618 2023-09-24 14:00:24.000000 pydoctor-23.9.0/pydoctor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-24 14:00:24.000000 pydoctor-23.9.0/pydoctor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-09-24 14:00:24.000000 pydoctor-23.9.0/pydoctor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      412 2023-09-24 14:00:24.000000 pydoctor-23.9.0/pydoctor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-09-24 14:00:24.000000 pydoctor-23.9.0/pydoctor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2023-09-24 14:00:24.356934 pydoctor-23.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-09-24 14:00:18.000000 pydoctor-23.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.396241 pydoctor-23.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2023-11-04 23:43:21.000000 pydoctor-23.9.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2023-11-04 23:43:21.000000 pydoctor-23.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    22177 2023-11-04 23:43:25.396241 pydoctor-23.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19809 2023-11-04 23:43:21.000000 pydoctor-23.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.368241 pydoctor-23.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.368241 pydoctor-23.9.1/docs/epytext_demo/
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/epytext_demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/epytext_demo/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5428 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/epytext_demo/demo_epytext_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.368241 pydoctor-23.9.1/docs/google_demo/
+-rw-r--r--   0 runner    (1001) docker     (127)     9329 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/google_demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.368241 pydoctor-23.9.1/docs/numpy_demo/
+-rw-r--r--   0 runner    (1001) docker     (127)     9516 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/numpy_demo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.368241 pydoctor-23.9.1/docs/restructuredtext_demo/
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/restructuredtext_demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/restructuredtext_demo/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5859 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/restructuredtext_demo/demo_restructuredtext_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.368241 pydoctor-23.9.1/docs/sample_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/sample_template/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/sample_template/header.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.368241 pydoctor-23.9.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.368241 pydoctor-23.9.1/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/source/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14427 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/source/codedoc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6169 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8419 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/source/contrib.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.368241 pydoctor-23.9.1/docs/source/custom_template_demo/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/source/custom_template_demo/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/source/custom_template_demo/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     9284 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/source/customize.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.368241 pydoctor-23.9.1/docs/source/docformat/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/source/docformat/epytext.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.368241 pydoctor-23.9.1/docs/source/docformat/epytext_demo/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/source/docformat/epytext_demo/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/source/docformat/google-numpy.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.368241 pydoctor-23.9.1/docs/source/docformat/google_demo/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/source/docformat/google_demo/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/source/docformat/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7304 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/source/docformat/list-restructuredtext-support.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.368241 pydoctor-23.9.1/docs/source/docformat/numpy_demo/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/source/docformat/numpy_demo/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/source/docformat/restructuredtext.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.368241 pydoctor-23.9.1/docs/source/docformat/restructuredtext_demo/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/source/docformat/restructuredtext_demo/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/source/help.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/source/publish-github-action.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/source/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/source/sphinx-integration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/source/transition.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.372241 pydoctor-23.9.1/docs/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/tests/test-search.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9932 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/tests/test_python_igraph_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/tests/test_standard_library_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2023-11-04 23:43:21.000000 pydoctor-23.9.1/docs/tests/test_twisted_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.372241 pydoctor-23.9.1/pydoctor/
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18979 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/_configparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52141 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/astbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16856 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/astutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6539 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.372241 pydoctor-23.9.1/pydoctor/epydoc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/epydoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7391 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/epydoc/doctest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5866 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/epydoc/docutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.376241 pydoctor-23.9.1/pydoctor/epydoc/markup/
+-rw-r--r--   0 runner    (1001) docker     (127)    18076 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/epydoc/markup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/epydoc/markup/_napoleon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45239 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/epydoc/markup/_pyval_repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8171 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/epydoc/markup/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56006 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/epydoc/markup/epytext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/epydoc/markup/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/epydoc/markup/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/epydoc/markup/plaintext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20001 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/epydoc/markup/restructuredtext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6924 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/epydoc/sre_constants36.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38153 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/epydoc/sre_parse36.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43492 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/epydoc2stan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.376241 pydoctor-23.9.1/pydoctor/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6484 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/extensions/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6998 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/extensions/deprecate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14017 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/extensions/zopeinterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10923 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/linker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62319 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/mro.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.376241 pydoctor-23.9.1/pydoctor/napoleon/
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/napoleon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59464 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/napoleon/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8808 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/napoleon/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11099 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/node2stan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19315 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/qnmatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12913 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/sphinx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.376241 pydoctor-23.9.1/pydoctor/sphinx_ext/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/sphinx_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5618 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/sphinx_ext/build_apidocs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/stanutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.376241 pydoctor-23.9.1/pydoctor/templatewriter/
+-rw-r--r--   0 runner    (1001) docker     (127)    16888 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/templatewriter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.376241 pydoctor-23.9.1/pydoctor/templatewriter/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)    22630 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/templatewriter/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/templatewriter/pages/attributechild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/templatewriter/pages/functionchild.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16423 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/templatewriter/pages/sidebar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/templatewriter/pages/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6639 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/templatewriter/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12964 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/templatewriter/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7627 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/templatewriter/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6010 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/templatewriter/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.380241 pydoctor-23.9.1/pydoctor/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.380241 pydoctor-23.9.1/pydoctor/test/epydoc/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/epydoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/epydoc/epytext.doctest
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/epydoc/restructuredtext.doctest
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/epydoc/test_epytext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11254 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/epydoc/test_epytext2html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/epydoc/test_epytext2node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/epydoc/test_google_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/epydoc/test_parsed_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43455 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/epydoc/test_pyval_repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11641 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/epydoc/test_restructuredtext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90196 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/test_astbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/test_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/test_colorize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/test_commandline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25534 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/test_configparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/test_cyclic_imports_base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71360 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/test_epydoc2stan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17068 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8883 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/test_mro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85527 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/test_napoleon_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11945 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/test_napoleon_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4559 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/test_node2stan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9007 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7016 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/test_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/test_pydantic_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5052 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/test_qnmatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22037 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/test_sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31453 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/test_templatewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7512 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/test_twisted_python_deprecate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16016 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/test_type_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/test_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21531 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/test_zopeinterface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.364241 pydoctor-23.9.1/pydoctor/test/testcustomtemplates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.380241 pydoctor-23.9.1/pydoctor/test/testcustomtemplates/allok/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testcustomtemplates/allok/nav.html
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testcustomtemplates/allok/pydoctor.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.364241 pydoctor-23.9.1/pydoctor/test/testcustomtemplates/casing/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.380241 pydoctor-23.9.1/pydoctor/test/testcustomtemplates/casing/test1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testcustomtemplates/casing/test1/nav.HTML
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.380241 pydoctor-23.9.1/pydoctor/test/testcustomtemplates/casing/test2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testcustomtemplates/casing/test2/nav.Html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.380241 pydoctor-23.9.1/pydoctor/test/testcustomtemplates/casing/test3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testcustomtemplates/casing/test3/nav.htmL
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.380241 pydoctor-23.9.1/pydoctor/test/testcustomtemplates/faketemplate/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testcustomtemplates/faketemplate/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testcustomtemplates/faketemplate/header.html
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testcustomtemplates/faketemplate/nav.html
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testcustomtemplates/faketemplate/pydoctor.js
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testcustomtemplates/faketemplate/random.html
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testcustomtemplates/faketemplate/subheader.html
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testcustomtemplates/faketemplate/summary.html
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testcustomtemplates/faketemplate/table.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.364241 pydoctor-23.9.1/pydoctor/test/testcustomtemplates/overridesubfolders/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.364241 pydoctor-23.9.1/pydoctor/test/testcustomtemplates/overridesubfolders/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.380241 pydoctor-23.9.1/pydoctor/test/testcustomtemplates/overridesubfolders/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testcustomtemplates/overridesubfolders/static/fonts/foo.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.380241 pydoctor-23.9.1/pydoctor/test/testcustomtemplates/subfolders/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testcustomtemplates/subfolders/atemplate.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.384241 pydoctor-23.9.1/pydoctor/test/testcustomtemplates/subfolders/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.384241 pydoctor-23.9.1/pydoctor/test/testcustomtemplates/subfolders/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testcustomtemplates/subfolders/static/fonts/bar.svg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testcustomtemplates/subfolders/static/fonts/foo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testcustomtemplates/subfolders/static/info.svg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testcustomtemplates/subfolders/static/lol.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.364241 pydoctor-23.9.1/pydoctor/test/testpackages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.384241 pydoctor-23.9.1/pydoctor/test/testpackages/allgames/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/allgames/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/allgames/mod1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/allgames/mod2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.384241 pydoctor-23.9.1/pydoctor/test/testpackages/basic/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/basic/_private_mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/basic/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.384241 pydoctor-23.9.1/pydoctor/test/testpackages/c_module_invalid_text_signature/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.384241 pydoctor-23.9.1/pydoctor/test/testpackages/c_module_invalid_text_signature/mymod/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/c_module_invalid_text_signature/mymod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/c_module_invalid_text_signature/mymod/base.c
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/c_module_invalid_text_signature/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.384241 pydoctor-23.9.1/pydoctor/test/testpackages/c_module_python_module_name_clash/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.384241 pydoctor-23.9.1/pydoctor/test/testpackages/c_module_python_module_name_clash/mymod/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/c_module_python_module_name_clash/mymod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/c_module_python_module_name_clash/mymod/base.c
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/c_module_python_module_name_clash/mymod/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/c_module_python_module_name_clash/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.384241 pydoctor-23.9.1/pydoctor/test/testpackages/codeininit/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/codeininit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.384241 pydoctor-23.9.1/pydoctor/test/testpackages/cyclic_imports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/cyclic_imports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/cyclic_imports/a.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/cyclic_imports/b.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.384241 pydoctor-23.9.1/pydoctor/test/testpackages/cyclic_imports_base_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/cyclic_imports_base_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/cyclic_imports_base_classes/a.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/cyclic_imports_base_classes/b.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.384241 pydoctor-23.9.1/pydoctor/test/testpackages/importingfrompackage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/importingfrompackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/importingfrompackage/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.384241 pydoctor-23.9.1/pydoctor/test/testpackages/importingfrompackage/subpack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/importingfrompackage/subpack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/importingfrompackage/subpack/submod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.384241 pydoctor-23.9.1/pydoctor/test/testpackages/interfaceallgames/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/interfaceallgames/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/interfaceallgames/_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/interfaceallgames/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/interfaceallgames/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.384241 pydoctor-23.9.1/pydoctor/test/testpackages/interfaceclass/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/interfaceclass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/interfaceclass/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.384241 pydoctor-23.9.1/pydoctor/test/testpackages/liveobject/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/liveobject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/liveobject/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.384241 pydoctor-23.9.1/pydoctor/test/testpackages/modnamedafterbuiltin/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/modnamedafterbuiltin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/modnamedafterbuiltin/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/modnamedafterbuiltin/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.384241 pydoctor-23.9.1/pydoctor/test/testpackages/multipleinheritance/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/multipleinheritance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/multipleinheritance/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.384241 pydoctor-23.9.1/pydoctor/test/testpackages/nestedconfusion/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/nestedconfusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/nestedconfusion/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.388241 pydoctor-23.9.1/pydoctor/test/testpackages/package_module_name_clash/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/package_module_name_clash/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.388241 pydoctor-23.9.1/pydoctor/test/testpackages/package_module_name_clash/pack/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/package_module_name_clash/pack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/package_module_name_clash/pack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.388241 pydoctor-23.9.1/pydoctor/test/testpackages/relativeimporttest/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/relativeimporttest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/relativeimporttest/mod1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/relativeimporttest/mod2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.388241 pydoctor-23.9.1/pydoctor/test/testpackages/reparented_module/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/reparented_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/reparented_module/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.388241 pydoctor-23.9.1/pydoctor/test/testpackages/reparenting_crash/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/reparenting_crash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/reparenting_crash/reparenting_crash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.388241 pydoctor-23.9.1/pydoctor/test/testpackages/reparenting_crash_alt/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/reparenting_crash_alt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/reparenting_crash_alt/_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/reparenting_crash_alt/reparenting_crash_alt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.388241 pydoctor-23.9.1/pydoctor/test/testpackages/reparenting_follows_aliases/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/reparenting_follows_aliases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/reparenting_follows_aliases/_myotherthing.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/reparenting_follows_aliases/_mything.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/reparenting_follows_aliases/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.388241 pydoctor-23.9.1/pydoctor/test/testpackages/report_trigger/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/report_trigger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/report_trigger/report_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.388241 pydoctor-23.9.1/pydoctor/test/testpackages/syntax_error/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/test/testpackages/syntax_error/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.388241 pydoctor-23.9.1/pydoctor/themes/
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.392241 pydoctor-23.9.1/pydoctor/themes/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/base/ajax.js
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/base/all-documents.html
+-rw-r--r--   0 runner    (1001) docker     (127)    22329 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/base/apidocs.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/base/attribute-child.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/base/common.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/base/extra.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.392241 pydoctor-23.9.1/pydoctor/themes/base/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/base/fonts/info.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/base/fonts/x-circle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/base/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/base/function-child.html
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/base/head.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/base/header.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/base/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)   113673 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/base/lunr.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/base/nameIndex.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/base/nav.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/base/pydoctor.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14286 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/base/search.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15394 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/base/searchlib.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/base/sidebar-list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/base/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/base/sidebartoggle.js
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/base/subheader.html
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/base/summary.html
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/base/table.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.392241 pydoctor-23.9.1/pydoctor/themes/classic/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/classic/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)   117305 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/classic/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/classic/head.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.392241 pydoctor-23.9.1/pydoctor/themes/readthedocs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/readthedocs/common.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.392241 pydoctor-23.9.1/pydoctor/themes/readthedocs/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    67312 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/readthedocs/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    66444 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/readthedocs/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/readthedocs/fonts/book.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/readthedocs/fonts/home.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   184912 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/readthedocs/fonts/lato-bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   182708 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/readthedocs/fonts/lato-normal.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/readthedocs/fonts/minus-square-o.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/readthedocs/fonts/plus-square-o.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/readthedocs/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/readthedocs/head.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/readthedocs/nav.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16297 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/themes/readthedocs/readthedocstheme.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10818 2023-11-04 23:43:21.000000 pydoctor-23.9.1/pydoctor/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 23:43:25.372241 pydoctor-23.9.1/pydoctor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22177 2023-11-04 23:43:25.000000 pydoctor-23.9.1/pydoctor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10618 2023-11-04 23:43:25.000000 pydoctor-23.9.1/pydoctor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-04 23:43:25.000000 pydoctor-23.9.1/pydoctor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2023-11-04 23:43:25.000000 pydoctor-23.9.1/pydoctor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2023-11-04 23:43:25.000000 pydoctor-23.9.1/pydoctor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-04 23:43:25.000000 pydoctor-23.9.1/pydoctor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2023-11-04 23:43:25.396241 pydoctor-23.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2023-11-04 23:43:21.000000 pydoctor-23.9.1/setup.py
```

### Comparing `pydoctor-23.9.0/LICENSE.txt` & `pydoctor-23.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/PKG-INFO` & `pydoctor-23.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoctor
-Version: 23.9.0
+Version: 23.9.1
 Summary: API doc generator.
 Home-page: https://github.com/twisted/pydoctor
 Author: Michael Hudson-Doyle
 Author-email: micahel@gmail.com
 Maintainer: Maarten ter Huurne
 Maintainer-email: maarten@boxingbeetle.com
 License: MIT/X11
@@ -130,16 +130,18 @@
 __ https://numpydoc.readthedocs.io/en/latest/format.html#docstring-standard
 
 You can select a different format using the ``--docformat`` option or the ``__docformat__`` module variable. 
 
 What's New?
 ~~~~~~~~~~~
 
-.. in development
-.. ^^^^^^^^^^^^^^
+pydoctor 23.9.1
+^^^^^^^^^^^^^^^
+
+* Fix regression in link not found warnings' line numbers.
 
 pydoctor 23.9.0
 ^^^^^^^^^^^^^^^
 
 This is the last major release to support Python 3.6.
 
 * Do not show `**kwargs` when keywords are specifically documented with the `keyword` field
```

### Comparing `pydoctor-23.9.0/README.rst` & `pydoctor-23.9.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -69,16 +69,18 @@
 __ https://numpydoc.readthedocs.io/en/latest/format.html#docstring-standard
 
 You can select a different format using the ``--docformat`` option or the ``__docformat__`` module variable. 
 
 What's New?
 ~~~~~~~~~~~
 
-.. in development
-.. ^^^^^^^^^^^^^^
+pydoctor 23.9.1
+^^^^^^^^^^^^^^^
+
+* Fix regression in link not found warnings' line numbers.
 
 pydoctor 23.9.0
 ^^^^^^^^^^^^^^^
 
 This is the last major release to support Python 3.6.
 
 * Do not show `**kwargs` when keywords are specifically documented with the `keyword` field
```

### Comparing `pydoctor-23.9.0/docs/Makefile` & `pydoctor-23.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/docs/epytext_demo/__init__.py` & `pydoctor-23.9.1/docs/epytext_demo/__init__.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/docs/epytext_demo/constants.py` & `pydoctor-23.9.1/docs/epytext_demo/constants.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/docs/epytext_demo/demo_epytext_module.py` & `pydoctor-23.9.1/docs/epytext_demo/demo_epytext_module.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/docs/google_demo/__init__.py` & `pydoctor-23.9.1/docs/google_demo/__init__.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/docs/make.bat` & `pydoctor-23.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/docs/numpy_demo/__init__.py` & `pydoctor-23.9.1/docs/numpy_demo/__init__.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/docs/restructuredtext_demo/__init__.py` & `pydoctor-23.9.1/docs/restructuredtext_demo/__init__.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/docs/restructuredtext_demo/constants.py` & `pydoctor-23.9.1/docs/restructuredtext_demo/constants.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/docs/restructuredtext_demo/demo_restructuredtext_module.py` & `pydoctor-23.9.1/docs/restructuredtext_demo/demo_restructuredtext_module.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/docs/sample_template/header.html` & `pydoctor-23.9.1/docs/sample_template/header.html`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/docs/source/codedoc.rst` & `pydoctor-23.9.1/docs/source/codedoc.rst`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/docs/source/conf.py` & `pydoctor-23.9.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/docs/source/contrib.rst` & `pydoctor-23.9.1/docs/source/contrib.rst`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/docs/source/customize.rst` & `pydoctor-23.9.1/docs/source/customize.rst`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/docs/source/docformat/epytext.rst` & `pydoctor-23.9.1/docs/source/docformat/epytext.rst`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/docs/source/docformat/google-numpy.rst` & `pydoctor-23.9.1/docs/source/docformat/google-numpy.rst`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/docs/source/docformat/index.rst` & `pydoctor-23.9.1/docs/source/docformat/index.rst`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/docs/source/docformat/list-restructuredtext-support.rst` & `pydoctor-23.9.1/docs/source/docformat/list-restructuredtext-support.rst`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/docs/source/docformat/restructuredtext.rst` & `pydoctor-23.9.1/docs/source/docformat/restructuredtext.rst`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/docs/source/faq.rst` & `pydoctor-23.9.1/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/docs/source/help.rst` & `pydoctor-23.9.1/docs/source/help.rst`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/docs/source/publish-github-action.rst` & `pydoctor-23.9.1/docs/source/publish-github-action.rst`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/docs/source/quickstart.rst` & `pydoctor-23.9.1/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/docs/source/sphinx-integration.rst` & `pydoctor-23.9.1/docs/source/sphinx-integration.rst`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/docs/source/transition.rst` & `pydoctor-23.9.1/docs/source/transition.rst`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/docs/tests/test-search.html` & `pydoctor-23.9.1/docs/tests/test-search.html`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/docs/tests/test.py` & `pydoctor-23.9.1/docs/tests/test.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/docs/tests/test_python_igraph_docs.py` & `pydoctor-23.9.1/docs/tests/test_python_igraph_docs.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/docs/tests/test_standard_library_docs.py` & `pydoctor-23.9.1/docs/tests/test_standard_library_docs.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/docs/tests/test_twisted_docs.py` & `pydoctor-23.9.1/docs/tests/test_twisted_docs.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/__init__.py` & `pydoctor-23.9.1/pydoctor/__init__.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/_configparser.py` & `pydoctor-23.9.1/pydoctor/_configparser.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/astbuilder.py` & `pydoctor-23.9.1/pydoctor/astbuilder.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/astutils.py` & `pydoctor-23.9.1/pydoctor/astutils.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/driver.py` & `pydoctor-23.9.1/pydoctor/driver.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/epydoc/__init__.py` & `pydoctor-23.9.1/pydoctor/epydoc/__init__.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/epydoc/doctest.py` & `pydoctor-23.9.1/pydoctor/epydoc/doctest.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/epydoc/docutils.py` & `pydoctor-23.9.1/pydoctor/epydoc/docutils.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/epydoc/markup/__init__.py` & `pydoctor-23.9.1/pydoctor/epydoc/markup/__init__.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/epydoc/markup/_napoleon.py` & `pydoctor-23.9.1/pydoctor/epydoc/markup/_napoleon.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/epydoc/markup/_pyval_repr.py` & `pydoctor-23.9.1/pydoctor/epydoc/markup/_pyval_repr.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/epydoc/markup/_types.py` & `pydoctor-23.9.1/pydoctor/epydoc/markup/_types.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/epydoc/markup/epytext.py` & `pydoctor-23.9.1/pydoctor/epydoc/markup/epytext.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/epydoc/markup/google.py` & `pydoctor-23.9.1/pydoctor/epydoc/markup/google.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/epydoc/markup/numpy.py` & `pydoctor-23.9.1/pydoctor/epydoc/markup/numpy.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/epydoc/markup/plaintext.py` & `pydoctor-23.9.1/pydoctor/epydoc/markup/plaintext.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/epydoc/markup/restructuredtext.py` & `pydoctor-23.9.1/pydoctor/epydoc/markup/restructuredtext.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/epydoc/sre_constants36.py` & `pydoctor-23.9.1/pydoctor/epydoc/sre_constants36.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/epydoc/sre_parse36.py` & `pydoctor-23.9.1/pydoctor/epydoc/sre_parse36.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/epydoc2stan.py` & `pydoctor-23.9.1/pydoctor/epydoc2stan.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/extensions/__init__.py` & `pydoctor-23.9.1/pydoctor/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/extensions/attrs.py` & `pydoctor-23.9.1/pydoctor/extensions/attrs.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/extensions/deprecate.py` & `pydoctor-23.9.1/pydoctor/extensions/deprecate.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/extensions/zopeinterface.py` & `pydoctor-23.9.1/pydoctor/extensions/zopeinterface.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/factory.py` & `pydoctor-23.9.1/pydoctor/factory.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/linker.py` & `pydoctor-23.9.1/pydoctor/linker.py`

 * *Files 5% similar despite different names*

```diff
@@ -247,16 +247,14 @@
     """
     def __init__(self, obj:'model.Documentable') -> None:
         self._obj = obj
         self._module = obj.module
         self._scope = obj.parent or obj
         self._module_linker = self._module.docstring_linker
         self._scope_linker = self._scope.docstring_linker
-
-        self.switch_context(obj).__enter__()
     
     @property
     def obj(self) -> 'model.Documentable':
         return self._obj
 
     def warn_ambiguous_annotation(self, target:str) -> None:
         # report a low-level message about ambiguous annotation
@@ -266,23 +264,25 @@
             self.obj.report(
                 f'ambiguous annotation {target!r}, could be interpreted as '
                 f'{obj_ann!r} instead of {mod_ann!r}', section='annotation',
                 thresh=1
             )
     
     def link_to(self, target: str, label: "Flattenable") -> Tag:
-        if self._module.isNameDefined(target):
-            self.warn_ambiguous_annotation(target)
-            return self._module_linker.link_to(target, label)
-        elif self._scope.isNameDefined(target):
-            return self._scope_linker.link_to(target, label)
-        else:
-            return self._module_linker.link_to(target, label)
+        with self.switch_context(self._obj):
+            if self._module.isNameDefined(target):
+                self.warn_ambiguous_annotation(target)
+                return self._module_linker.link_to(target, label)
+            elif self._scope.isNameDefined(target):
+                return self._scope_linker.link_to(target, label)
+            else:
+                return self._module_linker.link_to(target, label)
     
     def link_xref(self, target: str, label: "Flattenable", lineno: int) -> Tag:
-        return self.obj.docstring_linker.link_xref(target, label, lineno)
+        with self.switch_context(self._obj):
+            return self.obj.docstring_linker.link_xref(target, label, lineno)
 
     @contextlib.contextmanager
     def switch_context(self, ob:Optional['model.Documentable']) -> Iterator[None]:
         with self._module_linker.switch_context(ob):
             with self._scope_linker.switch_context(ob):
                 yield
```

### Comparing `pydoctor-23.9.0/pydoctor/model.py` & `pydoctor-23.9.1/pydoctor/model.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/mro.py` & `pydoctor-23.9.1/pydoctor/mro.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/napoleon/__init__.py` & `pydoctor-23.9.1/pydoctor/napoleon/__init__.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/napoleon/docstring.py` & `pydoctor-23.9.1/pydoctor/napoleon/docstring.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/napoleon/iterators.py` & `pydoctor-23.9.1/pydoctor/napoleon/iterators.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/node2stan.py` & `pydoctor-23.9.1/pydoctor/node2stan.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/options.py` & `pydoctor-23.9.1/pydoctor/options.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/qnmatch.py` & `pydoctor-23.9.1/pydoctor/qnmatch.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/sphinx.py` & `pydoctor-23.9.1/pydoctor/sphinx.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/sphinx_ext/build_apidocs.py` & `pydoctor-23.9.1/pydoctor/sphinx_ext/build_apidocs.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/stanutils.py` & `pydoctor-23.9.1/pydoctor/stanutils.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/templatewriter/__init__.py` & `pydoctor-23.9.1/pydoctor/templatewriter/__init__.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/templatewriter/pages/__init__.py` & `pydoctor-23.9.1/pydoctor/templatewriter/pages/__init__.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/templatewriter/pages/attributechild.py` & `pydoctor-23.9.1/pydoctor/templatewriter/pages/attributechild.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/templatewriter/pages/functionchild.py` & `pydoctor-23.9.1/pydoctor/templatewriter/pages/functionchild.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/templatewriter/pages/sidebar.py` & `pydoctor-23.9.1/pydoctor/templatewriter/pages/sidebar.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/templatewriter/pages/table.py` & `pydoctor-23.9.1/pydoctor/templatewriter/pages/table.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/templatewriter/search.py` & `pydoctor-23.9.1/pydoctor/templatewriter/search.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/templatewriter/summary.py` & `pydoctor-23.9.1/pydoctor/templatewriter/summary.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/templatewriter/util.py` & `pydoctor-23.9.1/pydoctor/templatewriter/util.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/templatewriter/writer.py` & `pydoctor-23.9.1/pydoctor/templatewriter/writer.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/__init__.py` & `pydoctor-23.9.1/pydoctor/test/__init__.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/epydoc/__init__.py` & `pydoctor-23.9.1/pydoctor/test/epydoc/__init__.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/epydoc/epytext.doctest` & `pydoctor-23.9.1/pydoctor/test/epydoc/epytext.doctest`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/epydoc/restructuredtext.doctest` & `pydoctor-23.9.1/pydoctor/test/epydoc/restructuredtext.doctest`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/epydoc/test_epytext.py` & `pydoctor-23.9.1/pydoctor/test/epydoc/test_epytext.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/epydoc/test_epytext2html.py` & `pydoctor-23.9.1/pydoctor/test/epydoc/test_epytext2html.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/epydoc/test_epytext2node.py` & `pydoctor-23.9.1/pydoctor/test/epydoc/test_epytext2node.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/epydoc/test_google_numpy.py` & `pydoctor-23.9.1/pydoctor/test/epydoc/test_google_numpy.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/epydoc/test_parsed_docstrings.py` & `pydoctor-23.9.1/pydoctor/test/epydoc/test_parsed_docstrings.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/epydoc/test_pyval_repr.py` & `pydoctor-23.9.1/pydoctor/test/epydoc/test_pyval_repr.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/epydoc/test_restructuredtext.py` & `pydoctor-23.9.1/pydoctor/test/epydoc/test_restructuredtext.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/test_astbuilder.py` & `pydoctor-23.9.1/pydoctor/test/test_astbuilder.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/test_attrs.py` & `pydoctor-23.9.1/pydoctor/test/test_attrs.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/test_colorize.py` & `pydoctor-23.9.1/pydoctor/test/test_colorize.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/test_commandline.py` & `pydoctor-23.9.1/pydoctor/test/test_commandline.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/test_configparser.py` & `pydoctor-23.9.1/pydoctor/test/test_configparser.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/test_cyclic_imports_base_classes.py` & `pydoctor-23.9.1/pydoctor/test/test_cyclic_imports_base_classes.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/test_epydoc2stan.py` & `pydoctor-23.9.1/pydoctor/test/test_epydoc2stan.py`

 * *Files 1% similar despite different names*

```diff
@@ -2102,7 +2102,50 @@
     assert captured == ('invalid:4: bad docstring: Wrong underline character for heading.\n'
                         'invalid:8: bad docstring: Wrong underline character for heading.\n')
     assert actual  == expected
 
     assert docstring2html(mod.contents['func'], docformat='plaintext') == expected
     captured = capsys.readouterr().out
     assert captured == ''
+
+def test_regression_not_found_linenumbers(capsys: CapSys) -> None:
+    """
+    Test for issue https://github.com/twisted/pydoctor/issues/745
+    """
+    code = '''
+    __docformat__ = 'restructuredtext'
+    class Settings:
+        """
+        Object that manages the configuration for Twine.
+
+        This object can only be instantiated with keyword arguments.
+
+        For example,
+
+        .. code-block:: python
+
+            Settings(True, username='fakeusername')
+
+        Will raise a :class:`TypeError`. Instead, you would want
+
+        .. code-block:: python
+
+            Settings(sign=True, username='fakeusername')
+        """
+
+        def check_repository_url(self) -> None:
+            """
+            Verify we are not using legacy PyPI.
+            """
+            ...
+
+        def create_repository(self) -> repository.Repository:
+            """
+            Create a new repository for uploading.
+            """
+            ...
+    '''
+
+    mod = fromText(code, )
+    docstring2html(mod.contents['Settings'])
+    captured = capsys.readouterr().out
+    assert captured == '<test>:15: Cannot find link target for "TypeError"\n'
```

### Comparing `pydoctor-23.9.0/pydoctor/test/test_model.py` & `pydoctor-23.9.1/pydoctor/test/test_model.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/test_mro.py` & `pydoctor-23.9.1/pydoctor/test/test_mro.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/test_napoleon_docstring.py` & `pydoctor-23.9.1/pydoctor/test/test_napoleon_docstring.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/test_napoleon_iterators.py` & `pydoctor-23.9.1/pydoctor/test/test_napoleon_iterators.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/test_node2stan.py` & `pydoctor-23.9.1/pydoctor/test/test_node2stan.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/test_options.py` & `pydoctor-23.9.1/pydoctor/test/test_options.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/test_packages.py` & `pydoctor-23.9.1/pydoctor/test/test_packages.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/test_pydantic_fields.py` & `pydoctor-23.9.1/pydoctor/test/test_pydantic_fields.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/test_qnmatch.py` & `pydoctor-23.9.1/pydoctor/test/test_qnmatch.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/test_sphinx.py` & `pydoctor-23.9.1/pydoctor/test/test_sphinx.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/test_templatewriter.py` & `pydoctor-23.9.1/pydoctor/test/test_templatewriter.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/test_twisted_python_deprecate.py` & `pydoctor-23.9.1/pydoctor/test/test_twisted_python_deprecate.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/test_type_fields.py` & `pydoctor-23.9.1/pydoctor/test/test_type_fields.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/test_utils.py` & `pydoctor-23.9.1/pydoctor/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/test_visitor.py` & `pydoctor-23.9.1/pydoctor/test/test_visitor.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/test_zopeinterface.py` & `pydoctor-23.9.1/pydoctor/test/test_zopeinterface.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/testcustomtemplates/allok/nav.html` & `pydoctor-23.9.1/pydoctor/test/testcustomtemplates/allok/nav.html`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/testcustomtemplates/faketemplate/nav.html` & `pydoctor-23.9.1/pydoctor/test/testcustomtemplates/faketemplate/nav.html`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/testpackages/basic/mod.py` & `pydoctor-23.9.1/pydoctor/test/testpackages/basic/mod.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/testpackages/c_module_invalid_text_signature/mymod/base.c` & `pydoctor-23.9.1/pydoctor/test/testpackages/c_module_invalid_text_signature/mymod/base.c`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/testpackages/c_module_python_module_name_clash/mymod/base.c` & `pydoctor-23.9.1/pydoctor/test/testpackages/c_module_python_module_name_clash/mymod/base.c`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/testpackages/c_module_python_module_name_clash/mymod/base.py` & `pydoctor-23.9.1/pydoctor/test/testpackages/c_module_python_module_name_clash/mymod/base.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/test/testpackages/multipleinheritance/mod.py` & `pydoctor-23.9.1/pydoctor/test/testpackages/multipleinheritance/mod.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/__init__.py` & `pydoctor-23.9.1/pydoctor/themes/__init__.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/base/ajax.js` & `pydoctor-23.9.1/pydoctor/themes/base/ajax.js`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/base/all-documents.html` & `pydoctor-23.9.1/pydoctor/themes/base/all-documents.html`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/base/apidocs.css` & `pydoctor-23.9.1/pydoctor/themes/base/apidocs.css`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/base/attribute-child.html` & `pydoctor-23.9.1/pydoctor/themes/base/attribute-child.html`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/base/common.html` & `pydoctor-23.9.1/pydoctor/themes/base/common.html`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/base/footer.html` & `pydoctor-23.9.1/pydoctor/themes/base/footer.html`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/base/function-child.html` & `pydoctor-23.9.1/pydoctor/themes/base/function-child.html`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/base/head.html` & `pydoctor-23.9.1/pydoctor/themes/base/head.html`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/base/index.html` & `pydoctor-23.9.1/pydoctor/themes/base/index.html`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/base/lunr.js` & `pydoctor-23.9.1/pydoctor/themes/base/lunr.js`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/base/nameIndex.html` & `pydoctor-23.9.1/pydoctor/themes/base/nameIndex.html`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/base/nav.html` & `pydoctor-23.9.1/pydoctor/themes/base/nav.html`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/base/pydoctor.js` & `pydoctor-23.9.1/pydoctor/themes/base/pydoctor.js`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/base/search.js` & `pydoctor-23.9.1/pydoctor/themes/base/search.js`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/base/searchlib.js` & `pydoctor-23.9.1/pydoctor/themes/base/searchlib.js`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/base/sidebar-list.html` & `pydoctor-23.9.1/pydoctor/themes/base/sidebar-list.html`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/base/sidebar.html` & `pydoctor-23.9.1/pydoctor/themes/base/sidebar.html`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/base/sidebartoggle.js` & `pydoctor-23.9.1/pydoctor/themes/base/sidebartoggle.js`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/base/summary.html` & `pydoctor-23.9.1/pydoctor/themes/base/summary.html`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/classic/bootstrap.min.css` & `pydoctor-23.9.1/pydoctor/themes/classic/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/classic/head.html` & `pydoctor-23.9.1/pydoctor/themes/classic/head.html`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/readthedocs/common.html` & `pydoctor-23.9.1/pydoctor/themes/readthedocs/common.html`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/readthedocs/fonts/Roboto-Slab-Bold.woff2` & `pydoctor-23.9.1/pydoctor/themes/readthedocs/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/readthedocs/fonts/Roboto-Slab-Regular.woff2` & `pydoctor-23.9.1/pydoctor/themes/readthedocs/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/readthedocs/fonts/book.svg` & `pydoctor-23.9.1/pydoctor/themes/readthedocs/fonts/book.svg`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/readthedocs/fonts/lato-bold.woff2` & `pydoctor-23.9.1/pydoctor/themes/readthedocs/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/readthedocs/fonts/lato-normal.woff2` & `pydoctor-23.9.1/pydoctor/themes/readthedocs/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/readthedocs/fonts/plus-square-o.svg` & `pydoctor-23.9.1/pydoctor/themes/readthedocs/fonts/plus-square-o.svg`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/readthedocs/footer.html` & `pydoctor-23.9.1/pydoctor/themes/readthedocs/footer.html`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/readthedocs/head.html` & `pydoctor-23.9.1/pydoctor/themes/readthedocs/head.html`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/readthedocs/nav.html` & `pydoctor-23.9.1/pydoctor/themes/readthedocs/nav.html`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/themes/readthedocs/readthedocstheme.css` & `pydoctor-23.9.1/pydoctor/themes/readthedocs/readthedocstheme.css`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/utils.py` & `pydoctor-23.9.1/pydoctor/utils.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor/visitor.py` & `pydoctor-23.9.1/pydoctor/visitor.py`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/pydoctor.egg-info/PKG-INFO` & `pydoctor-23.9.1/pydoctor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoctor
-Version: 23.9.0
+Version: 23.9.1
 Summary: API doc generator.
 Home-page: https://github.com/twisted/pydoctor
 Author: Michael Hudson-Doyle
 Author-email: micahel@gmail.com
 Maintainer: Maarten ter Huurne
 Maintainer-email: maarten@boxingbeetle.com
 License: MIT/X11
@@ -130,16 +130,18 @@
 __ https://numpydoc.readthedocs.io/en/latest/format.html#docstring-standard
 
 You can select a different format using the ``--docformat`` option or the ``__docformat__`` module variable. 
 
 What's New?
 ~~~~~~~~~~~
 
-.. in development
-.. ^^^^^^^^^^^^^^
+pydoctor 23.9.1
+^^^^^^^^^^^^^^^
+
+* Fix regression in link not found warnings' line numbers.
 
 pydoctor 23.9.0
 ^^^^^^^^^^^^^^^
 
 This is the last major release to support Python 3.6.
 
 * Do not show `**kwargs` when keywords are specifically documented with the `keyword` field
```

### Comparing `pydoctor-23.9.0/pydoctor.egg-info/SOURCES.txt` & `pydoctor-23.9.1/pydoctor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydoctor-23.9.0/setup.cfg` & `pydoctor-23.9.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pydoctor
-version = 23.9.0
+version = 23.9.1
 author = Michael Hudson-Doyle
 author_email = micahel@gmail.com
 maintainer = Maarten ter Huurne
 maintainer_email = maarten@boxingbeetle.com
 description = API doc generator.
 long_description_content_type = text/x-rst
 license = MIT/X11
```

