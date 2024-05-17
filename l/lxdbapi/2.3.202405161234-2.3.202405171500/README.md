# Comparing `tmp/lxdbapi-2.3.202405161234.tar.gz` & `tmp/lxdbapi-2.3.202405171500.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lxdbapi-2.3.202405161234.tar", last modified: Thu May 16 12:35:13 2024, max compression
+gzip compressed data, was "lxdbapi-2.3.202405171500.tar", last modified: Fri May 17 13:00:30 2024, max compression
```

## Comparing `lxdbapi-2.3.202405161234.tar` & `lxdbapi-2.3.202405171500.tar`

### file list

```diff
@@ -1,365 +1,365 @@
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.596176 lxdbapi-2.3.202405161234/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     3519 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/LICENSE
--rw-r--r--   0 leandata  (1133) leandata  (1129)     4461 2024-05-16 12:35:13.596176 lxdbapi-2.3.202405161234/PKG-INFO
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      104 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/README.md
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      633 2024-05-16 12:34:59.000000 lxdbapi-2.3.202405161234/pyproject.toml
--rw-rw-r--   0 leandata  (1133) leandata  (1129)       38 2024-05-16 12:35:13.596176 lxdbapi-2.3.202405161234/setup.cfg
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.536179 lxdbapi-2.3.202405161234/src/
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.544178 lxdbapi-2.3.202405161234/src/lxdbapi/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     2026 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/__init__.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.544178 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)        0 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/__init__.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.544178 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     2991 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/__init__.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.544178 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      533 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    16215 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/_markupbase.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    75573 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/datetime.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.548178 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     2289 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     8463 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/_encoded_words.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)   104712 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/_header_value_parser.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    17393 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/_parseaddr.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    14671 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/_policybase.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     3737 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/base64mime.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    17459 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/charset.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     2804 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/encoders.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     3684 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/errors.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    22756 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/feedparser.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    19549 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/generator.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    24477 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/header.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    20661 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/headerregistry.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     2348 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/iterators.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    35273 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/message.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.552178 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/mime/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)        0 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/mime/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1411 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/mime/application.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     2825 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/mime/audio.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      880 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/mime/base.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1917 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/mime/image.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1439 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/mime/message.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1704 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/mime/multipart.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      842 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/mime/nonmultipart.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1562 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/mime/text.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     5324 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/parser.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     8839 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/policy.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    10927 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/quoprimime.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    14310 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/utils.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.552178 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/html/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      924 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/html/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    75432 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/html/entities.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    19782 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/html/parser.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.552178 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/http/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)        0 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/http/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    47626 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/http/client.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    76575 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/http/cookiejar.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    21589 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/http/cookies.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    45547 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/http/server.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    32685 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/misc.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    15666 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/socket.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    24286 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/socketserver.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.552178 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/test/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      264 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/test/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     7427 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/test/pystone.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     7229 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/test/ssl_servers.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    70893 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/test/support.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1929 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/total_ordering.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.556178 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/urllib/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)        0 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/urllib/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     2723 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/urllib/error.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    35800 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/urllib/parse.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    96323 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/urllib/request.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     3184 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/urllib/response.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     6877 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/urllib/robotparser.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.556178 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/xmlrpc/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)       38 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/xmlrpc/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    48149 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/xmlrpc/client.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    37310 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/xmlrpc/server.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.556178 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/builtins/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1702 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/builtins/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     2112 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/builtins/disabled.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1402 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/builtins/iterators.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     4577 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/builtins/misc.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1760 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/builtins/new_min_max.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     2009 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/builtins/newnext.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     3184 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/builtins/newround.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     4149 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/builtins/newsuper.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.560178 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      223 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      178 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/_dummy_thread.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      174 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/_markupbase.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      166 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/_thread.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      287 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/builtins.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      426 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/collections.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      149 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/configparser.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      441 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/copyreg.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.560178 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/dbm/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      496 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/dbm/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      170 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/dbm/dumb.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      166 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/dbm/gnu.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      166 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/dbm/ndbm.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.560178 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/html/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1020 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/html/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      181 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/html/entities.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      171 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/html/parser.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.560178 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/http/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)       75 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/http/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      169 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/http/client.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      177 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/http/cookiejar.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      237 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/http/cookies.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      610 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/http/server.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      158 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/itertools.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      232 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/pickle.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      163 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/queue.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      164 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/reprlib.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      177 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/socketserver.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      257 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/subprocess.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      135 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/sys.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.560178 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/test/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      114 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/test/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      267 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/test/support.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.564178 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/tkinter/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      624 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/tkinter/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      337 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/tkinter/colorchooser.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      337 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/tkinter/commondialog.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      328 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/tkinter/constants.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      315 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/tkinter/dialog.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      310 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/tkinter/dnd.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      327 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/tkinter/filedialog.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      313 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/tkinter/font.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      331 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/tkinter/messagebox.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      333 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/tkinter/scrolledtext.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      333 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/tkinter/simpledialog.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      306 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/tkinter/tix.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      306 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/tkinter/ttk.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.564178 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/urllib/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      114 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/urllib/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      487 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/urllib/error.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1053 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/urllib/parse.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     3504 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/urllib/request.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      350 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/urllib/response.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      183 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/urllib/robotparser.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      166 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/winreg.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.564178 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/xmlrpc/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)        0 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/xmlrpc/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      147 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/xmlrpc/client.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      147 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/xmlrpc/server.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.564178 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/standard_library/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    27773 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/standard_library/__init__.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.564178 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/tests/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)        0 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/tests/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    19962 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/tests/base.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.568177 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/types/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     6834 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/types/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    16318 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/types/newbytes.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     3106 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/types/newdict.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    13295 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/types/newint.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     2290 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/types/newlist.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      718 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/types/newmemoryview.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     3358 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/types/newobject.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      810 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/types/newopen.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     5300 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/types/newrange.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    15770 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/types/newstr.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.568177 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/utils/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    21843 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/utils/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     6100 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/utils/surrogateescape.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.536179 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.572177 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1705 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1551 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/any_pb2.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     3350 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/api_pb2.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.572177 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/compiler/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)        0 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/compiler/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     4359 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/compiler/plugin_pb2.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    45158 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/descriptor.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     6819 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/descriptor_database.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)   119790 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/descriptor_pb2.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    46961 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/descriptor_pool.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1661 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/duration_pb2.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1529 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/empty_pb2.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1639 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/field_mask_pb2.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.576177 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/internal/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)        0 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/internal/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     4570 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/internal/api_implementation.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    21560 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/internal/containers.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    37583 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/internal/decoder.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    28660 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/internal/encoder.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     4469 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/internal/enum_type_wrapper.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     8451 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/internal/extension_dict.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     3367 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/internal/message_listener.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    58202 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/internal/python_message.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    16268 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/internal/type_checkers.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    29379 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/internal/well_known_types.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     8452 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/internal/wire_format.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    32699 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/json_format.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    14456 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/message.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     7497 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/message_factory.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     5515 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/proto_builder.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.576177 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/pyext/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)        0 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/pyext/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     2855 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/pyext/cpp_message.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     3785 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/reflection.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     9146 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/service.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    11072 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/service_reflection.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1682 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/source_context_pb2.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     3903 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/struct_pb2.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     6953 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/symbol_database.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     4728 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/text_encoding.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    60024 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/text_format.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1677 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/timestamp_pb2.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     6176 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/type_pb2.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.576177 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/util/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)        0 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/util/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    14148 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/util/json_format_pb2.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    27137 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/util/json_format_proto3_pb2.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     5404 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/wrappers_pb2.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.576177 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)       31 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    17494 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixer_util.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.580177 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     5236 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     3840 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_UserDict.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     3143 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_absolute_import.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      665 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_add__future__imports_except_unicode_literals.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      397 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_basestring.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      685 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_bytes.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      704 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_cmp.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      231 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_division.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     3295 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_division_safe.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      924 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_execfile.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     2030 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_future_builtins.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      736 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_future_standard_library.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1004 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_future_standard_library_urllib.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      687 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_input.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     9568 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_metaclass.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     3158 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_next_call.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      410 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_object.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1217 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_oldstr_wrap.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      832 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_order___future__imports.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     3384 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_print.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      741 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_print_with_import.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     3887 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_raise.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      854 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_remove_old__future__imports.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      779 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_unicode_keep_u.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      370 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_unicode_literals_import.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      482 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_xrange_with_import.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    13816 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/main.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.580177 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)       31 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/__init__.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.584177 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     3719 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1723 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/feature_base.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      679 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_add_all__future__imports.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1272 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_add_all_future_builtins.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      666 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_add_future_standard_library_import.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1581 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_annotations.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      907 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_division.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     2675 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_features.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      438 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_fullargspec.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1453 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_future_builtins.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      873 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_getcwd.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     4947 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_imports.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     8583 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_imports2.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     5994 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_kwargs.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      551 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_memoryview.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     3263 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_metaclass.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      891 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_newstyle.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1233 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_next.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      404 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_printfunction.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1099 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_raise.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1225 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_raise_.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      835 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_throw.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     5949 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_unpacking.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     8190 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/main.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.584177 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/past/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     2920 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/past/__init__.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.584177 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/past/builtins/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1820 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/past/builtins/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     2633 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/past/builtins/misc.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     9376 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/past/builtins/noniterators.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.584177 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/past/translation/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    17649 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/past/translation/__init__.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.588177 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/past/types/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      882 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/past/types/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      731 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/past/types/basestring.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     2724 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/past/types/olddict.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     4335 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/past/types/oldstr.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.588177 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/past/utils/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     2633 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/past/utils/__init__.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.540179 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.588177 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     3535 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     4372 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/_compat.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1059 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/_flatten.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    36239 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/adapter.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     3890 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/advice.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.592177 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    10481 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     3043 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/builtins.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     6800 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/collections.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    20866 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/idatetime.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     5375 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/interfaces.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1245 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/io.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     4685 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/mapping.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1690 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/numbers.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     5533 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/sequence.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.592177 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/tests/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     5345 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/tests/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     3906 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/tests/basemapping.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1350 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/tests/test_builtins.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     5739 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/tests/test_collections.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1619 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/tests/test_idatetime.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      822 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/tests/test_import_interfaces.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1602 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/tests/test_io.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1399 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/tests/test_numbers.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    42861 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/declarations.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     4148 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/document.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     8635 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/exceptions.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    38870 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/interface.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    50134 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/interfaces.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    25876 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/registry.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    24155 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/ro.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.596176 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     3969 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/__init__.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      901 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/advisory_testing.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      919 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/dummy.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      893 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/idummy.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      816 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/m1.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     3015 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/odd.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    79784 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/test_adapter.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     5990 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/test_advice.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1324 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/test_compile_flags.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    83080 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/test_declarations.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    17023 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/test_document.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1122 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/test_element.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     6439 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/test_exceptions.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    92261 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/test_interface.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     4489 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/test_interfaces.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     7601 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/test_odd_declarations.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)   113667 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/test_registry.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    14201 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/test_ro.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     1941 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/test_sorting.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    19562 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/test_verify.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     7172 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/verify.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     8489 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/balanced_connection_manager.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    24150 2024-05-14 00:03:14.000000 lxdbapi-2.3.202405161234/src/lxdbapi/client.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    19006 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/common_pb2.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     8231 2024-03-15 13:01:38.000000 lxdbapi-2.3.202405161234/src/lxdbapi/connection.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     5806 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/connection_manager.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    21788 2024-03-15 13:01:38.000000 lxdbapi-2.3.202405161234/src/lxdbapi/cursor.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     3055 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/errors.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     2852 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/errorsOld.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    20576 2024-05-14 00:03:14.000000 lxdbapi-2.3.202405161234/src/lxdbapi/multi_connection.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     3696 2024-05-14 00:03:14.000000 lxdbapi-2.3.202405161234/src/lxdbapi/network_avatica_connection.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    19548 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/requests_pb2.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    14485 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/responses_pb2.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    11707 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/sqlalchemy_leanxcale.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    23869 2024-03-20 10:28:12.000000 lxdbapi-2.3.202405161234/src/lxdbapi/types.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)     6507 2024-03-15 13:01:36.000000 lxdbapi-2.3.202405161234/src/lxdbapi/typessOld.py
--rw-rw-r--   0 leandata  (1133) leandata  (1129)      103 2024-05-16 12:34:59.000000 lxdbapi-2.3.202405161234/src/lxdbapi/versions.py
-drwxrwxr-x   0 leandata  (1133) leandata  (1129)        0 2024-05-16 12:35:13.596176 lxdbapi-2.3.202405161234/src/lxdbapi.egg-info/
--rw-r--r--   0 leandata  (1133) leandata  (1129)     4461 2024-05-16 12:35:13.000000 lxdbapi-2.3.202405161234/src/lxdbapi.egg-info/PKG-INFO
--rw-rw-r--   0 leandata  (1133) leandata  (1129)    16216 2024-05-16 12:35:13.000000 lxdbapi-2.3.202405161234/src/lxdbapi.egg-info/SOURCES.txt
--rw-rw-r--   0 leandata  (1133) leandata  (1129)        1 2024-05-16 12:35:13.000000 lxdbapi-2.3.202405161234/src/lxdbapi.egg-info/dependency_links.txt
--rw-rw-r--   0 leandata  (1133) leandata  (1129)       80 2024-05-16 12:35:13.000000 lxdbapi-2.3.202405161234/src/lxdbapi.egg-info/entry_points.txt
--rw-rw-r--   0 leandata  (1133) leandata  (1129)        8 2024-05-16 12:35:13.000000 lxdbapi-2.3.202405161234/src/lxdbapi.egg-info/top_level.txt
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.249731 lxdbapi-2.3.202405171500/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     3519 2023-09-29 11:09:58.000000 lxdbapi-2.3.202405171500/LICENSE
+-rw-r--r--   0 rogelio   (1001) rogelio   (1001)     4461 2024-05-17 13:00:30.249731 lxdbapi-2.3.202405171500/PKG-INFO
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      104 2023-09-20 09:24:46.000000 lxdbapi-2.3.202405171500/README.md
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      633 2024-05-17 13:00:25.000000 lxdbapi-2.3.202405171500/pyproject.toml
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)       38 2024-05-17 13:00:30.249731 lxdbapi-2.3.202405171500/setup.cfg
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.189731 lxdbapi-2.3.202405171500/src/
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.197731 lxdbapi-2.3.202405171500/src/lxdbapi/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     2026 2023-11-28 15:28:25.000000 lxdbapi-2.3.202405171500/src/lxdbapi/__init__.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.197731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)        0 2023-11-29 10:06:54.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/__init__.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.197731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     2991 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/__init__.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.201731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      533 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    16215 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/_markupbase.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    75573 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/datetime.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.201731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     2289 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     8463 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/_encoded_words.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)   104712 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/_header_value_parser.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    17393 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/_parseaddr.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    14671 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/_policybase.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     3737 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/base64mime.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    17459 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/charset.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     2804 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/encoders.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     3684 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/errors.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    22756 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/feedparser.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    19549 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/generator.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    24477 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/header.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    20661 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/headerregistry.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     2348 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/iterators.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    35273 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/message.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.205731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/mime/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)        0 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/mime/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1411 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/mime/application.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     2825 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/mime/audio.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      880 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/mime/base.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1917 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/mime/image.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1439 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/mime/message.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1704 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/mime/multipart.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      842 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/mime/nonmultipart.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1562 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/mime/text.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     5324 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/parser.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     8839 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/policy.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    10927 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/quoprimime.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    14310 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/utils.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.205731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/html/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      924 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/html/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    75432 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/html/entities.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    19782 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/html/parser.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.205731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/http/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)        0 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/http/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    47626 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/http/client.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    76575 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/http/cookiejar.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    21589 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/http/cookies.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    45547 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/http/server.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    32685 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/misc.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    15666 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/socket.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    24286 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/socketserver.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.205731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/test/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      264 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/test/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     7427 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/test/pystone.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     7229 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/test/ssl_servers.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    70893 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/test/support.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1929 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/total_ordering.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.205731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/urllib/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)        0 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/urllib/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     2723 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/urllib/error.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    35800 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/urllib/parse.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    96323 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/urllib/request.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     3184 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/urllib/response.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     6877 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/urllib/robotparser.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.209731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/xmlrpc/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)       38 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/xmlrpc/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    48149 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/xmlrpc/client.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    37310 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/xmlrpc/server.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.209731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/builtins/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1702 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/builtins/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     2112 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/builtins/disabled.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1402 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/builtins/iterators.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     4577 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/builtins/misc.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1760 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/builtins/new_min_max.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     2009 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/builtins/newnext.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     3184 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/builtins/newround.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     4149 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/builtins/newsuper.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.213731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      223 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      178 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/_dummy_thread.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      174 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/_markupbase.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      166 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/_thread.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      287 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/builtins.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      426 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/collections.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      149 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/configparser.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      441 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/copyreg.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.213731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/dbm/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      496 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/dbm/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      170 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/dbm/dumb.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      166 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/dbm/gnu.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      166 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/dbm/ndbm.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.213731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/html/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1020 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/html/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      181 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/html/entities.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      171 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/html/parser.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.213731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/http/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)       75 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/http/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      169 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/http/client.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      177 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/http/cookiejar.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      237 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/http/cookies.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      610 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/http/server.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      158 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/itertools.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      232 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/pickle.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      163 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/queue.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      164 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/reprlib.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      177 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/socketserver.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      257 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/subprocess.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      135 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/sys.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.213731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/test/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      114 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/test/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      267 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/test/support.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.217731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/tkinter/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      624 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/tkinter/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      337 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/tkinter/colorchooser.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      337 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/tkinter/commondialog.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      328 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/tkinter/constants.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      315 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/tkinter/dialog.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      310 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/tkinter/dnd.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      327 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/tkinter/filedialog.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      313 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/tkinter/font.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      331 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/tkinter/messagebox.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      333 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/tkinter/scrolledtext.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      333 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/tkinter/simpledialog.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      306 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/tkinter/tix.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      306 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/tkinter/ttk.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.217731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/urllib/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      114 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/urllib/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      487 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/urllib/error.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1053 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/urllib/parse.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     3504 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/urllib/request.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      350 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/urllib/response.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      183 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/urllib/robotparser.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      166 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/winreg.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.217731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/xmlrpc/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)        0 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/xmlrpc/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      147 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/xmlrpc/client.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      147 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/xmlrpc/server.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.217731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/standard_library/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    27773 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/standard_library/__init__.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.217731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/tests/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)        0 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/tests/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    19962 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/tests/base.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.217731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/types/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     6834 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/types/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    16318 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/types/newbytes.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     3106 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/types/newdict.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    13295 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/types/newint.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     2290 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/types/newlist.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      718 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/types/newmemoryview.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     3358 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/types/newobject.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      810 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/types/newopen.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     5300 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/types/newrange.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    15770 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/types/newstr.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.221731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/utils/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    21843 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/utils/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     6100 2023-11-29 10:06:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/utils/surrogateescape.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.193731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.225731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1705 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1551 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/any_pb2.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     3350 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/api_pb2.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.225731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/compiler/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)        0 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/compiler/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     4359 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/compiler/plugin_pb2.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    45158 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/descriptor.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     6819 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/descriptor_database.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)   119790 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/descriptor_pb2.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    46961 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/descriptor_pool.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1661 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/duration_pb2.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1529 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/empty_pb2.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1639 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/field_mask_pb2.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.229731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/internal/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)        0 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/internal/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     4570 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/internal/api_implementation.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    21560 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/internal/containers.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    37583 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/internal/decoder.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    28660 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/internal/encoder.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     4469 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/internal/enum_type_wrapper.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     8451 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/internal/extension_dict.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     3367 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/internal/message_listener.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    58202 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/internal/python_message.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    16268 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/internal/type_checkers.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    29379 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/internal/well_known_types.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     8452 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/internal/wire_format.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    32699 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/json_format.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    14456 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/message.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     7497 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/message_factory.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     5515 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/proto_builder.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.229731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/pyext/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)        0 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/pyext/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     2855 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/pyext/cpp_message.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     3785 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/reflection.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     9146 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/service.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    11072 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/service_reflection.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1682 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/source_context_pb2.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     3903 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/struct_pb2.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     6953 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/symbol_database.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     4728 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/text_encoding.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    60024 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/text_format.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1677 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/timestamp_pb2.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     6176 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/type_pb2.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.229731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/util/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)        0 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/util/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    14148 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/util/json_format_pb2.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    27137 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/util/json_format_proto3_pb2.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     5404 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/wrappers_pb2.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.229731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)       31 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    17494 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixer_util.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.233731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     5236 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     3840 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_UserDict.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     3143 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_absolute_import.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      665 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_add__future__imports_except_unicode_literals.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      397 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_basestring.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      685 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_bytes.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      704 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_cmp.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      231 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_division.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     3295 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_division_safe.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      924 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_execfile.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     2030 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_future_builtins.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      736 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_future_standard_library.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1004 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_future_standard_library_urllib.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      687 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_input.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     9568 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_metaclass.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     3158 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_next_call.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      410 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_object.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1217 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_oldstr_wrap.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      832 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_order___future__imports.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     3384 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_print.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      741 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_print_with_import.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     3887 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_raise.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      854 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_remove_old__future__imports.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      779 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_unicode_keep_u.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      370 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_unicode_literals_import.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      482 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_xrange_with_import.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    13816 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/main.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.233731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)       31 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/__init__.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.237731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     3719 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1723 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/feature_base.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      679 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_add_all__future__imports.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1272 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_add_all_future_builtins.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      666 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_add_future_standard_library_import.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1581 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_annotations.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      907 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_division.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     2675 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_features.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      438 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_fullargspec.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1453 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_future_builtins.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      873 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_getcwd.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     4947 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_imports.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     8583 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_imports2.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     5994 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_kwargs.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      551 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_memoryview.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     3263 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_metaclass.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      891 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_newstyle.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1233 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_next.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      404 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_printfunction.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1099 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_raise.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1225 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_raise_.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      835 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_throw.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     5949 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_unpacking.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     8190 2023-11-29 10:06:59.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/main.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.237731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/past/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     2920 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/past/__init__.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.237731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/past/builtins/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1820 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/past/builtins/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     2633 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/past/builtins/misc.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     9376 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/past/builtins/noniterators.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.237731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/past/translation/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    17649 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/past/translation/__init__.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.241731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/past/types/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      882 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/past/types/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      731 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/past/types/basestring.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     2724 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/past/types/olddict.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     4335 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/past/types/oldstr.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.241731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/past/utils/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     2633 2023-11-29 10:06:57.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/past/utils/__init__.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.193731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.245731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     3535 2023-12-21 14:41:36.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     4372 2023-12-21 14:41:36.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/_compat.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1059 2023-12-21 14:41:36.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/_flatten.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    36239 2023-12-21 14:41:36.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/adapter.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     3890 2023-12-21 14:41:36.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/advice.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.245731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    10481 2023-12-21 14:41:36.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     3043 2023-12-21 14:41:36.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/builtins.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     6800 2023-12-21 14:41:36.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/collections.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    20866 2023-12-21 14:41:36.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/idatetime.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     5375 2023-12-21 14:41:36.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/interfaces.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1245 2023-12-21 14:41:36.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/io.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     4685 2023-12-21 14:41:36.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/mapping.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1690 2023-12-21 14:41:36.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/numbers.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     5533 2023-12-21 14:41:36.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/sequence.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.245731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/tests/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     5345 2023-12-21 14:41:36.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/tests/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     3906 2023-12-21 14:41:36.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/tests/basemapping.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1350 2023-12-21 14:41:37.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/tests/test_builtins.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     5739 2023-12-21 14:41:37.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/tests/test_collections.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1619 2023-12-21 14:41:37.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/tests/test_idatetime.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      822 2024-03-15 11:25:18.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/tests/test_import_interfaces.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1602 2023-12-21 14:41:37.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/tests/test_io.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1399 2023-12-21 14:41:37.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/tests/test_numbers.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    42861 2023-12-21 14:41:37.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/declarations.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     4148 2023-12-21 14:41:37.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/document.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     8635 2023-12-21 14:41:37.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/exceptions.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    38870 2023-12-21 14:41:37.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/interface.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    50134 2023-12-21 14:41:37.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/interfaces.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    25876 2023-12-21 14:41:37.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/registry.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    24155 2023-12-21 14:41:37.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/ro.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.249731 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     3969 2023-12-21 14:41:37.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/__init__.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      901 2023-12-21 14:41:37.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/advisory_testing.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      919 2023-12-21 14:41:37.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/dummy.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      893 2023-12-21 14:41:37.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/idummy.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      816 2024-03-15 11:25:18.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/m1.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     3015 2023-12-21 14:41:37.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/odd.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    79784 2023-12-21 14:41:37.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/test_adapter.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     5990 2023-12-21 14:41:37.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/test_advice.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1324 2023-12-21 14:41:37.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/test_compile_flags.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    83080 2023-12-21 14:41:37.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/test_declarations.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    17023 2023-12-21 14:41:37.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/test_document.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1122 2023-12-21 14:41:37.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/test_element.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     6439 2023-12-21 14:41:37.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/test_exceptions.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    92261 2023-12-21 14:41:37.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/test_interface.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     4489 2023-12-21 14:41:37.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/test_interfaces.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     7601 2023-12-21 14:41:37.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/test_odd_declarations.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)   113667 2023-12-21 14:41:37.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/test_registry.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    14201 2023-12-21 14:41:37.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/test_ro.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     1941 2023-12-21 14:41:37.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/test_sorting.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    19562 2023-12-21 14:41:37.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/test_verify.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     7172 2023-12-21 14:41:37.000000 lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/verify.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     8489 2023-09-29 11:09:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/balanced_connection_manager.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    24150 2024-05-07 08:59:44.000000 lxdbapi-2.3.202405171500/src/lxdbapi/client.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    19006 2024-03-19 13:33:50.000000 lxdbapi-2.3.202405171500/src/lxdbapi/common_pb2.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     8231 2024-03-19 13:33:50.000000 lxdbapi-2.3.202405171500/src/lxdbapi/connection.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     5806 2023-09-29 11:09:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/connection_manager.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    21788 2024-03-19 13:33:50.000000 lxdbapi-2.3.202405171500/src/lxdbapi/cursor.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     3055 2024-01-17 11:13:44.000000 lxdbapi-2.3.202405171500/src/lxdbapi/errors.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     2852 2023-09-29 11:09:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/errorsOld.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    20576 2024-05-07 08:59:44.000000 lxdbapi-2.3.202405171500/src/lxdbapi/multi_connection.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     5073 2024-05-17 13:00:19.000000 lxdbapi-2.3.202405171500/src/lxdbapi/network_avatica_connection.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    19548 2024-03-19 13:33:50.000000 lxdbapi-2.3.202405171500/src/lxdbapi/requests_pb2.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    14485 2024-03-19 13:33:50.000000 lxdbapi-2.3.202405171500/src/lxdbapi/responses_pb2.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    11707 2024-03-08 11:52:33.000000 lxdbapi-2.3.202405171500/src/lxdbapi/sqlalchemy_leanxcale.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    23869 2024-03-20 09:52:00.000000 lxdbapi-2.3.202405171500/src/lxdbapi/types.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)     6507 2023-09-29 11:09:58.000000 lxdbapi-2.3.202405171500/src/lxdbapi/typessOld.py
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)      103 2024-05-17 13:00:25.000000 lxdbapi-2.3.202405171500/src/lxdbapi/versions.py
+drwxrwxr-x   0 rogelio   (1001) rogelio   (1001)        0 2024-05-17 13:00:30.249731 lxdbapi-2.3.202405171500/src/lxdbapi.egg-info/
+-rw-r--r--   0 rogelio   (1001) rogelio   (1001)     4461 2024-05-17 13:00:30.000000 lxdbapi-2.3.202405171500/src/lxdbapi.egg-info/PKG-INFO
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)    16216 2024-05-17 13:00:30.000000 lxdbapi-2.3.202405171500/src/lxdbapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)        1 2024-05-17 13:00:30.000000 lxdbapi-2.3.202405171500/src/lxdbapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)       80 2024-05-17 13:00:30.000000 lxdbapi-2.3.202405171500/src/lxdbapi.egg-info/entry_points.txt
+-rw-rw-r--   0 rogelio   (1001) rogelio   (1001)        8 2024-05-17 13:00:30.000000 lxdbapi-2.3.202405171500/src/lxdbapi.egg-info/top_level.txt
```

### Comparing `lxdbapi-2.3.202405161234/LICENSE` & `lxdbapi-2.3.202405171500/LICENSE`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/PKG-INFO` & `lxdbapi-2.3.202405171500/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lxdbapi
-Version: 2.3.202405161234
+Version: 2.3.202405171500
 Summary: LeanXcale implementation for Python Database API Specification v2.0
 Author-email: leanXcale <support@leanxcale.com>
 License: Copyright <2023> <LEANXCALE S.L.>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lxdbapi-2.3.202405161234/pyproject.toml` & `lxdbapi-2.3.202405171500/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lxdbapi"
-version = "2.3.202405161234"
+version = "2.3.202405171500"
 authors = [
   { name="leanXcale", email="support@leanxcale.com" },
 ]
 description = "LeanXcale implementation for Python Database API Specification v2.0"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
```

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/__init__.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/__init__.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/__init__.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/__init__.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/__init__.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/_markupbase.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/_markupbase.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/datetime.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/datetime.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/__init__.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/__init__.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/_encoded_words.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/_encoded_words.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/_header_value_parser.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/_header_value_parser.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/_parseaddr.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/_parseaddr.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/_policybase.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/_policybase.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/base64mime.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/base64mime.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/charset.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/charset.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/encoders.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/encoders.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/errors.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/errors.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/feedparser.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/feedparser.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/generator.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/generator.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/header.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/header.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/headerregistry.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/headerregistry.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/iterators.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/iterators.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/message.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/message.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/mime/application.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/mime/application.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/mime/audio.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/mime/audio.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/mime/base.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/mime/base.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/mime/image.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/mime/image.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/mime/message.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/mime/message.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/mime/multipart.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/mime/multipart.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/mime/nonmultipart.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/mime/nonmultipart.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/mime/text.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/mime/text.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/parser.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/parser.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/policy.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/policy.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/quoprimime.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/quoprimime.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/email/utils.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/email/utils.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/html/__init__.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/html/__init__.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/html/entities.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/html/entities.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/html/parser.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/html/parser.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/http/client.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/http/client.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/http/cookiejar.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/http/cookiejar.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/http/cookies.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/http/cookies.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/http/server.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/http/server.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/misc.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/misc.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/socket.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/socket.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/socketserver.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/socketserver.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/test/pystone.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/test/pystone.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/test/ssl_servers.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/test/ssl_servers.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/test/support.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/test/support.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/total_ordering.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/total_ordering.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/urllib/error.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/urllib/error.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/urllib/parse.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/urllib/parse.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/urllib/request.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/urllib/request.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/urllib/response.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/urllib/response.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/urllib/robotparser.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/urllib/robotparser.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/xmlrpc/client.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/xmlrpc/client.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/backports/xmlrpc/server.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/backports/xmlrpc/server.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/builtins/__init__.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/builtins/__init__.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/builtins/disabled.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/builtins/disabled.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/builtins/iterators.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/builtins/iterators.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/builtins/misc.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/builtins/misc.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/builtins/new_min_max.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/builtins/new_min_max.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/builtins/newnext.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/builtins/newnext.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/builtins/newround.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/builtins/newround.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/builtins/newsuper.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/builtins/newsuper.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/html/__init__.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/html/__init__.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/http/server.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/http/server.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/tkinter/__init__.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/tkinter/__init__.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/urllib/parse.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/urllib/parse.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/moves/urllib/request.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/moves/urllib/request.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/standard_library/__init__.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/standard_library/__init__.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/tests/base.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/tests/base.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/types/__init__.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/types/__init__.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/types/newbytes.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/types/newbytes.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/types/newdict.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/types/newdict.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/types/newint.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/types/newint.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/types/newlist.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/types/newlist.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/types/newmemoryview.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/types/newmemoryview.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/types/newobject.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/types/newobject.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/types/newopen.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/types/newopen.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/types/newrange.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/types/newrange.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/types/newstr.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/types/newstr.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/utils/__init__.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/future/utils/surrogateescape.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/future/utils/surrogateescape.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/__init__.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/any_pb2.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/any_pb2.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/api_pb2.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/api_pb2.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/compiler/plugin_pb2.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/compiler/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/descriptor.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/descriptor.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/descriptor_database.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/descriptor_database.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/descriptor_pb2.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/descriptor_pb2.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/descriptor_pool.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/descriptor_pool.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/duration_pb2.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/duration_pb2.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/empty_pb2.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/empty_pb2.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/field_mask_pb2.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/field_mask_pb2.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/internal/api_implementation.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/internal/api_implementation.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/internal/containers.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/internal/containers.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/internal/decoder.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/internal/decoder.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/internal/encoder.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/internal/encoder.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/internal/enum_type_wrapper.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/internal/enum_type_wrapper.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/internal/extension_dict.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/internal/extension_dict.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/internal/message_listener.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/internal/message_listener.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/internal/python_message.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/internal/python_message.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/internal/type_checkers.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/internal/type_checkers.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/internal/well_known_types.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/internal/well_known_types.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/internal/wire_format.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/internal/wire_format.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/json_format.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/json_format.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/message.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/message.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/message_factory.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/message_factory.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/proto_builder.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/proto_builder.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/pyext/cpp_message.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/pyext/cpp_message.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/reflection.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/reflection.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/service.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/service.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/service_reflection.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/service_reflection.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/source_context_pb2.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/source_context_pb2.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/struct_pb2.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/struct_pb2.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/symbol_database.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/symbol_database.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/text_encoding.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/text_encoding.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/text_format.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/text_format.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/timestamp_pb2.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/timestamp_pb2.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/type_pb2.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/type_pb2.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/util/json_format_pb2.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/util/json_format_pb2.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/util/json_format_proto3_pb2.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/util/json_format_proto3_pb2.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/google/protobuf/wrappers_pb2.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/google/protobuf/wrappers_pb2.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixer_util.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixer_util.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/__init__.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/__init__.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_UserDict.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_UserDict.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_absolute_import.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_absolute_import.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_add__future__imports_except_unicode_literals.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_add__future__imports_except_unicode_literals.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_bytes.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_bytes.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_cmp.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_cmp.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_division_safe.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_division_safe.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_execfile.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_execfile.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_future_builtins.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_future_builtins.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_future_standard_library.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_future_standard_library.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_future_standard_library_urllib.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_future_standard_library_urllib.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_input.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_input.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_metaclass.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_metaclass.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_next_call.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_next_call.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_oldstr_wrap.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_oldstr_wrap.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_order___future__imports.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_order___future__imports.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_print.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_print.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_print_with_import.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_print_with_import.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_raise.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_raise.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_remove_old__future__imports.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_remove_old__future__imports.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/fixes/fix_unicode_keep_u.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/fixes/fix_unicode_keep_u.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libfuturize/main.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libfuturize/main.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/__init__.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/__init__.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/feature_base.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/feature_base.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_add_all__future__imports.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_add_all__future__imports.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_add_all_future_builtins.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_add_all_future_builtins.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_add_future_standard_library_import.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_add_future_standard_library_import.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_annotations.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_annotations.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_division.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_division.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_features.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_features.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_future_builtins.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_future_builtins.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_getcwd.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_getcwd.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_imports.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_imports.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_imports2.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_imports2.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_kwargs.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_kwargs.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_memoryview.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_memoryview.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_metaclass.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_metaclass.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_newstyle.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_newstyle.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_next.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_next.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_raise.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_raise.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_raise_.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_raise_.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_throw.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_throw.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/fixes/fix_unpacking.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/fixes/fix_unpacking.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/libpasteurize/main.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/libpasteurize/main.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/past/__init__.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/past/__init__.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/past/builtins/__init__.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/past/builtins/__init__.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/past/builtins/misc.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/past/builtins/misc.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/past/builtins/noniterators.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/past/builtins/noniterators.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/past/translation/__init__.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/past/translation/__init__.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/past/types/__init__.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/past/types/__init__.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/past/types/basestring.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/past/types/basestring.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/past/types/olddict.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/past/types/olddict.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/past/types/oldstr.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/past/types/oldstr.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/past/utils/__init__.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/past/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/__init__.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/_compat.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/_compat.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/_flatten.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/_flatten.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/adapter.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/adapter.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/advice.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/advice.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/__init__.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/__init__.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/builtins.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/builtins.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/collections.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/collections.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/idatetime.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/idatetime.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/interfaces.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/interfaces.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/io.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/io.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/mapping.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/mapping.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/numbers.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/numbers.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/sequence.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/sequence.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/tests/__init__.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/tests/basemapping.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/tests/basemapping.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/tests/test_builtins.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/tests/test_builtins.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/tests/test_collections.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/tests/test_idatetime.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/tests/test_idatetime.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/tests/test_import_interfaces.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/tests/test_import_interfaces.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/tests/test_io.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/common/tests/test_numbers.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/common/tests/test_numbers.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/declarations.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/declarations.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/document.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/document.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/exceptions.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/exceptions.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/interface.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/interface.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/interfaces.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/interfaces.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/registry.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/registry.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/ro.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/ro.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/__init__.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/advisory_testing.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/advisory_testing.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/dummy.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/dummy.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/idummy.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/idummy.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/m1.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/m1.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/odd.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/odd.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/test_adapter.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/test_adapter.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/test_advice.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/test_advice.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/test_compile_flags.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/test_compile_flags.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/test_declarations.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/test_declarations.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/test_document.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/test_element.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/test_exceptions.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/test_interface.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/test_interfaces.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/test_odd_declarations.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/test_odd_declarations.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/test_registry.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/test_ro.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/test_ro.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/test_sorting.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/test_sorting.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/tests/test_verify.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/tests/test_verify.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/_vendor/zope/interface/verify.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/_vendor/zope/interface/verify.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/balanced_connection_manager.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/balanced_connection_manager.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/client.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/client.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/common_pb2.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/common_pb2.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/connection.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/connection.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/connection_manager.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/connection_manager.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/cursor.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/cursor.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/errors.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/errors.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/errorsOld.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/errorsOld.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/multi_connection.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/multi_connection.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/requests_pb2.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/requests_pb2.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/responses_pb2.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/responses_pb2.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/sqlalchemy_leanxcale.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/sqlalchemy_leanxcale.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/types.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/types.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi/typessOld.py` & `lxdbapi-2.3.202405171500/src/lxdbapi/typessOld.py`

 * *Files identical despite different names*

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi.egg-info/PKG-INFO` & `lxdbapi-2.3.202405171500/src/lxdbapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lxdbapi
-Version: 2.3.202405161234
+Version: 2.3.202405171500
 Summary: LeanXcale implementation for Python Database API Specification v2.0
 Author-email: leanXcale <support@leanxcale.com>
 License: Copyright <2023> <LEANXCALE S.L.>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lxdbapi-2.3.202405161234/src/lxdbapi.egg-info/SOURCES.txt` & `lxdbapi-2.3.202405171500/src/lxdbapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

