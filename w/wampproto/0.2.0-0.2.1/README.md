# Comparing `tmp/wampproto-0.2.0.tar.gz` & `tmp/wampproto-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wampproto-0.2.0.tar", last modified: Mon May 13 12:56:20 2024, max compression
+gzip compressed data, was "wampproto-0.2.1.tar", last modified: Thu May 16 22:12:41 2024, max compression
```

## Comparing `wampproto-0.2.0.tar` & `wampproto-0.2.1.tar`

### file list

```diff
@@ -1,65 +1,67 @@
-drwxr-xr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-13 12:56:20.062290 wampproto-0.2.0/
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1107 2024-05-10 20:22:04.000000 wampproto-0.2.0/LICENSE
--rw-r--r--   0 om26er    (1000) om26er    (1000)     2320 2024-05-13 12:56:20.062290 wampproto-0.2.0/PKG-INFO
--rw-r--r--   0 om26er    (1000) om26er    (1000)       73 2024-05-13 12:47:17.000000 wampproto-0.2.0/README.md
--rw-r--r--   0 om26er    (1000) om26er    (1000)     2405 2024-05-13 12:49:31.000000 wampproto-0.2.0/pyproject.toml
--rw-r--r--   0 om26er    (1000) om26er    (1000)       38 2024-05-13 12:56:20.062290 wampproto-0.2.0/setup.cfg
-drwxr-xr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-13 12:56:20.058290 wampproto-0.2.0/tests/
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      574 2024-05-08 19:53:09.000000 wampproto-0.2.0/tests/test_session.py
-drwxr-xr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-13 12:56:20.058290 wampproto-0.2.0/wampproto/
--rw-rw-r--   0 om26er    (1000) om26er    (1000)       69 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/__init__.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     6939 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/acceptor.py
-drwxr-xr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-13 12:56:20.058290 wampproto-0.2.0/wampproto/auth/
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1105 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/auth/__init__.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      384 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/auth/anonymous.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     2537 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/auth/auth.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1616 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/auth/cryptosign.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      437 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/auth/ticket.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1551 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/auth/wampcra.py
--rw-r--r--   0 om26er    (1000) om26er    (1000)     4140 2024-05-13 12:47:17.000000 wampproto-0.2.0/wampproto/broker.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     5216 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/dealer.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      327 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/idgen.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     2723 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/joiner.py
-drwxr-xr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-13 12:56:20.062290 wampproto-0.2.0/wampproto/messages/
--rw-r--r--   0 om26er    (1000) om26er    (1000)     1641 2024-05-13 12:47:17.000000 wampproto-0.2.0/wampproto/messages/__init__.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      725 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/abort.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      958 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/authenticate.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1776 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/call.py
--rw-r--r--   0 om26er    (1000) om26er    (1000)      923 2024-05-13 12:47:17.000000 wampproto-0.2.0/wampproto/messages/cancel.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      940 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/challenge.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1978 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/error.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1628 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/event.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1167 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/exceptions.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      743 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/goodbye.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     3286 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/hello.py
--rw-r--r--   0 om26er    (1000) om26er    (1000)      958 2024-05-13 12:47:17.000000 wampproto-0.2.0/wampproto/messages/interrupt.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1946 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/invocation.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      244 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/message.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1522 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/publish.py
--rw-r--r--   0 om26er    (1000) om26er    (1000)      868 2024-05-13 12:47:17.000000 wampproto-0.2.0/wampproto/messages/published.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      927 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/register.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      850 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/registered.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1682 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/result.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      932 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/subscribe.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      850 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/subscribed.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      850 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/unregister.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      654 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/unregistered.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      859 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/unsubscribe.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      654 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/unsubscribed.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     2750 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/util.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     3136 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/welcome.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1671 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/yield_.py
-drwxr-xr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-13 12:56:20.062290 wampproto-0.2.0/wampproto/serializers/
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      326 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/serializers/__init__.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      411 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/serializers/cbor.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      534 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/serializers/json.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      420 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/serializers/msgpack.py
--rw-r--r--   0 om26er    (1000) om26er    (1000)     2814 2024-05-13 12:47:17.000000 wampproto-0.2.0/wampproto/serializers/serializer.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     6723 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/session.py
--rw-r--r--   0 om26er    (1000) om26er    (1000)     1210 2024-05-13 12:47:17.000000 wampproto-0.2.0/wampproto/types.py
-drwxr-xr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-13 12:56:20.062290 wampproto-0.2.0/wampproto.egg-info/
--rw-r--r--   0 om26er    (1000) om26er    (1000)     2320 2024-05-13 12:56:20.000000 wampproto-0.2.0/wampproto.egg-info/PKG-INFO
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1569 2024-05-13 12:56:20.000000 wampproto-0.2.0/wampproto.egg-info/SOURCES.txt
--rw-rw-r--   0 om26er    (1000) om26er    (1000)        1 2024-05-13 12:56:20.000000 wampproto-0.2.0/wampproto.egg-info/dependency_links.txt
--rw-rw-r--   0 om26er    (1000) om26er    (1000)       73 2024-05-13 12:56:20.000000 wampproto-0.2.0/wampproto.egg-info/requires.txt
--rw-rw-r--   0 om26er    (1000) om26er    (1000)       10 2024-05-13 12:56:20.000000 wampproto-0.2.0/wampproto.egg-info/top_level.txt
+drwxrwxr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-16 22:12:41.073400 wampproto-0.2.1/
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1107 2024-05-14 23:27:14.000000 wampproto-0.2.1/LICENSE
+-rw-r--r--   0 om26er    (1000) om26er    (1000)     2320 2024-05-16 22:12:41.069400 wampproto-0.2.1/PKG-INFO
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)       73 2024-05-14 23:27:14.000000 wampproto-0.2.1/README.md
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     2459 2024-05-16 22:11:56.000000 wampproto-0.2.1/pyproject.toml
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)       38 2024-05-16 22:12:41.073400 wampproto-0.2.1/setup.cfg
+drwxrwxr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-16 22:12:41.065400 wampproto-0.2.1/tests/
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     9137 2024-05-16 22:10:07.000000 wampproto-0.2.1/tests/test_session.py
+drwxrwxr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-16 22:12:41.065400 wampproto-0.2.1/wampproto/
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)       69 2024-05-14 23:27:14.000000 wampproto-0.2.1/wampproto/__init__.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     7102 2024-05-14 23:27:14.000000 wampproto-0.2.1/wampproto/acceptor.py
+drwxrwxr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-16 22:12:41.065400 wampproto-0.2.1/wampproto/auth/
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1105 2024-05-14 23:27:14.000000 wampproto-0.2.1/wampproto/auth/__init__.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      384 2024-05-14 23:27:14.000000 wampproto-0.2.1/wampproto/auth/anonymous.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     2537 2024-05-14 23:27:14.000000 wampproto-0.2.1/wampproto/auth/auth.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1616 2024-05-14 23:27:14.000000 wampproto-0.2.1/wampproto/auth/cryptosign.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      437 2024-05-14 23:27:14.000000 wampproto-0.2.1/wampproto/auth/ticket.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1551 2024-05-14 23:27:14.000000 wampproto-0.2.1/wampproto/auth/wampcra.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     4332 2024-05-14 23:27:14.000000 wampproto-0.2.1/wampproto/broker.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     7346 2024-05-14 23:27:14.000000 wampproto-0.2.1/wampproto/dealer.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      327 2024-05-14 23:27:14.000000 wampproto-0.2.1/wampproto/idgen.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     2829 2024-05-14 23:27:14.000000 wampproto-0.2.1/wampproto/joiner.py
+drwxrwxr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-16 22:12:41.069400 wampproto-0.2.1/wampproto/messages/
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1641 2024-05-14 23:27:14.000000 wampproto-0.2.1/wampproto/messages/__init__.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      720 2024-05-16 21:37:40.000000 wampproto-0.2.1/wampproto/messages/abort.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      918 2024-05-16 21:37:40.000000 wampproto-0.2.1/wampproto/messages/authenticate.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1566 2024-05-16 21:37:40.000000 wampproto-0.2.1/wampproto/messages/call.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      907 2024-05-16 21:37:40.000000 wampproto-0.2.1/wampproto/messages/cancel.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      915 2024-05-16 21:37:40.000000 wampproto-0.2.1/wampproto/messages/challenge.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1965 2024-05-16 21:37:40.000000 wampproto-0.2.1/wampproto/messages/error.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1621 2024-05-16 21:37:40.000000 wampproto-0.2.1/wampproto/messages/event.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1167 2024-05-14 23:27:14.000000 wampproto-0.2.1/wampproto/messages/exceptions.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      728 2024-05-16 21:37:40.000000 wampproto-0.2.1/wampproto/messages/goodbye.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     3266 2024-05-16 21:37:40.000000 wampproto-0.2.1/wampproto/messages/hello.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      921 2024-05-16 21:37:40.000000 wampproto-0.2.1/wampproto/messages/interrupt.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1895 2024-05-16 21:37:40.000000 wampproto-0.2.1/wampproto/messages/invocation.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      282 2024-05-16 21:37:40.000000 wampproto-0.2.1/wampproto/messages/message.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1503 2024-05-16 21:37:40.000000 wampproto-0.2.1/wampproto/messages/publish.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      843 2024-05-16 21:37:40.000000 wampproto-0.2.1/wampproto/messages/published.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      902 2024-05-16 21:37:40.000000 wampproto-0.2.1/wampproto/messages/register.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      854 2024-05-16 21:37:40.000000 wampproto-0.2.1/wampproto/messages/registered.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1666 2024-05-16 21:37:40.000000 wampproto-0.2.1/wampproto/messages/result.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      941 2024-05-16 21:37:40.000000 wampproto-0.2.1/wampproto/messages/subscribe.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      854 2024-05-16 21:37:40.000000 wampproto-0.2.1/wampproto/messages/subscribed.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      854 2024-05-16 21:37:40.000000 wampproto-0.2.1/wampproto/messages/unregister.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      657 2024-05-16 21:37:40.000000 wampproto-0.2.1/wampproto/messages/unregistered.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      858 2024-05-16 21:37:40.000000 wampproto-0.2.1/wampproto/messages/unsubscribe.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      657 2024-05-16 21:37:40.000000 wampproto-0.2.1/wampproto/messages/unsubscribed.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     5136 2024-05-14 23:27:14.000000 wampproto-0.2.1/wampproto/messages/util.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      244 2024-05-14 23:27:14.000000 wampproto-0.2.1/wampproto/messages/validation_spec.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     3100 2024-05-16 21:37:40.000000 wampproto-0.2.1/wampproto/messages/welcome.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1662 2024-05-16 21:37:40.000000 wampproto-0.2.1/wampproto/messages/yield_.py
+drwxrwxr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-16 22:12:41.069400 wampproto-0.2.1/wampproto/serializers/
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      326 2024-05-14 23:27:14.000000 wampproto-0.2.1/wampproto/serializers/__init__.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      411 2024-05-14 23:27:14.000000 wampproto-0.2.1/wampproto/serializers/cbor.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      404 2024-05-16 22:10:07.000000 wampproto-0.2.1/wampproto/serializers/json.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      420 2024-05-14 23:27:14.000000 wampproto-0.2.1/wampproto/serializers/msgpack.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     2820 2024-05-16 22:10:07.000000 wampproto-0.2.1/wampproto/serializers/serializer.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     6729 2024-05-16 21:37:40.000000 wampproto-0.2.1/wampproto/session.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1210 2024-05-14 23:27:14.000000 wampproto-0.2.1/wampproto/types.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      153 2024-05-16 21:37:40.000000 wampproto-0.2.1/wampproto/uris.py
+drwxrwxr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-16 22:12:41.069400 wampproto-0.2.1/wampproto.egg-info/
+-rw-r--r--   0 om26er    (1000) om26er    (1000)     2320 2024-05-16 22:12:41.000000 wampproto-0.2.1/wampproto.egg-info/PKG-INFO
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1625 2024-05-16 22:12:41.000000 wampproto-0.2.1/wampproto.egg-info/SOURCES.txt
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)        1 2024-05-16 22:12:41.000000 wampproto-0.2.1/wampproto.egg-info/dependency_links.txt
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)       73 2024-05-16 22:12:41.000000 wampproto-0.2.1/wampproto.egg-info/requires.txt
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)       10 2024-05-16 22:12:41.000000 wampproto-0.2.1/wampproto.egg-info/top_level.txt
```

### Comparing `wampproto-0.2.0/LICENSE` & `wampproto-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wampproto-0.2.0/PKG-INFO` & `wampproto-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wampproto
-Version: 0.2.0
+Version: 0.2.1
 Summary: https://github.com/xconnio/wampproto.py
 Author-email: Omer Akram <omer@thing.com>, Mahad Munir <mahad@xconn.io>
 License: MIT License
         
         Copyright (c) 2024 Simple Things Inc.
         Copyright (c) 2024 XConnIO Ltd.
```

### Comparing `wampproto-0.2.0/pyproject.toml` & `wampproto-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wampproto"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   {name="Omer Akram", email="omer@thing.com"},
   {name="Mahad Munir", email="mahad@xconn.io"},
 ]
 description = "https://github.com/xconnio/wampproto.py"
 readme = "README.md"
 license = {file = "LICENSE"}
@@ -100,7 +100,10 @@
 
 # Set the line length limit used when formatting code snippets in
 # docstrings.
 #
 # This only has an effect when the `docstring-code-format` setting is
 # enabled.
 docstring-code-line-length = "dynamic"
+
+[tool.pytest.ini_options]
+addopts = "-p no:warnings"
```

### Comparing `wampproto-0.2.0/wampproto/acceptor.py` & `wampproto-0.2.1/wampproto/acceptor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 import binascii
 import random
 
 from wampproto import messages, auth, serializers
 from wampproto.types import SessionDetails
 
-ROUTER_ROLES = {"dealer": {}, "broker": {}}
+ROUTER_ROLES = {
+    "dealer": {"features": {}},
+    "broker": {"features": {}},
+}
 
 
 def get_session_id() -> int:
-    return random.randint(0, 9007199254740992)
+    return random.randint(1, 9007199254740992)
 
 
 class Acceptor:
     STATE_NONE = 0
     STATE_HELLO_RECEIVED = 1
     STATE_CHALLENGE_SENT = 2
     STATE_WELCOME_SENT = 3
     STATE_ERRORED = 4
 
     def __init__(
         self,
         serializer: serializers.Serializer = serializers.JSONSerializer(),
         authenticator: auth.IServerAuthenticator = None,
+        roles: dict[str, dict[str, dict[str, bool]]] = None,
     ):
         self._serializer = serializer
         self._authenticator = authenticator
+        self._roles = roles if roles is not None else ROUTER_ROLES
+
         self._state = Acceptor.STATE_NONE
         self._session_id = get_session_id()
 
         self._auth_method: str = None
         self._hello: messages.Hello = None
         self._response: auth.Response = None
         self._session_details: SessionDetails = None
@@ -49,15 +55,15 @@
 
         if isinstance(msg, messages.Hello):
             if self._state != Acceptor.STATE_NONE:
                 raise ValueError("unknown state")
 
             if self._authenticator is None:
                 self._state = Acceptor.STATE_WELCOME_SENT
-                welcome = messages.Welcome(self._session_id, ROUTER_ROLES, "anonymous", "anonymous", "anonymous")
+                welcome = messages.Welcome(self._session_id, self._roles, "anonymous", "anonymous", "anonymous")
                 self._session_details = SessionDetails(welcome.session_id, msg.realm, welcome.authid, welcome.authrole)
 
                 return welcome
 
             method = msg.authmethods[0]
             self._auth_method = method
             self._hello = msg
@@ -65,15 +71,15 @@
             match method:
                 case "anonymous":
                     request = auth.Request(method, msg.realm, msg.authid, msg.authextra)
                     response = self._authenticator.authenticate(request)
                     self._state = Acceptor.STATE_WELCOME_SENT
 
                     welcome = messages.Welcome(
-                        self._session_id, ROUTER_ROLES, response.authid, response.authrole, method
+                        self._session_id, self._roles, response.authid, response.authrole, method
                     )
                     self._session_details = SessionDetails(
                         welcome.session_id, msg.realm, welcome.authid, welcome.authrole
                     )
 
                     return welcome
                 case "cryptosign":
@@ -115,38 +121,38 @@
                 raise ValueError("unknown state")
 
             match self._auth_method:
                 case "cryptosign":
                     auth.verify_cryptosign_signature(msg.signature, binascii.unhexlify(self._public_key))
                     self._state = Acceptor.STATE_WELCOME_SENT
                     welcome = messages.Welcome(
-                        self._session_id, ROUTER_ROLES, authid=self._response.authid, authrole=self._response.authrole
+                        self._session_id, self._roles, authid=self._response.authid, authrole=self._response.authrole
                     )
                     self._session_details = SessionDetails(
                         welcome.session_id, self._hello.realm, welcome.authid, welcome.authrole
                     )
                     return welcome
                 case "wampcra":
                     auth.verify_wampcra_signature(msg.signature, self._challenge, self._secret.encode())
                     self._state = Acceptor.STATE_WELCOME_SENT
                     welcome = messages.Welcome(
-                        self._session_id, ROUTER_ROLES, authid=self._response.authid, authrole=self._response.authrole
+                        self._session_id, self._roles, authid=self._response.authid, authrole=self._response.authrole
                     )
                     self._session_details = SessionDetails(
                         welcome.session_id, self._hello.realm, welcome.authid, welcome.authrole
                     )
                     return welcome
                 case "ticket":
                     request = auth.TicketRequest(
                         self._hello.realm, self._hello.authid, self._hello.authextra, msg.signature
                     )
                     response = self._authenticator.authenticate(request)
                     self._state = Acceptor.STATE_WELCOME_SENT
                     welcome = messages.Welcome(
-                        self._session_id, ROUTER_ROLES, authid=response.authid, authrole=response.authrole
+                        self._session_id, self._roles, authid=response.authid, authrole=response.authrole
                     )
                     self._session_details = SessionDetails(
                         welcome.session_id, self._hello.realm, welcome.authid, welcome.authrole
                     )
 
                     return welcome
         elif isinstance(msg, messages.Abort):
```

### Comparing `wampproto-0.2.0/wampproto/auth/__init__.py` & `wampproto-0.2.1/wampproto/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.2.0/wampproto/auth/auth.py` & `wampproto-0.2.1/wampproto/auth/auth.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.2.0/wampproto/auth/cryptosign.py` & `wampproto-0.2.1/wampproto/auth/cryptosign.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.2.0/wampproto/auth/wampcra.py` & `wampproto-0.2.1/wampproto/auth/wampcra.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.2.0/wampproto/broker.py` & `wampproto-0.2.1/wampproto/broker.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,46 +11,50 @@
 
 
 class Broker:
     def __init__(self):
         super().__init__()
         self.subscriptions_by_topic: dict[str, Subscription] = {}
         self.subscriptions_by_session: dict[int, dict[int, Subscription]] = {}
-        self.id_gen = idgen.SessionScopeIDGenerator()
+        self.sessions: dict[int, types.SessionDetails] = {}
+        self.idgen = idgen.SessionScopeIDGenerator()
 
-    def add_session(self, sid: int):
-        if sid in self.subscriptions_by_session:
+    def add_session(self, details: types.SessionDetails):
+        if details.session_id in self.subscriptions_by_session:
             raise ValueError("cannot add session twice")
 
-        self.subscriptions_by_session[sid] = {}
+        self.subscriptions_by_session[details.session_id] = {}
+        self.sessions[details.session_id] = details
 
     def remove_session(self, sid: int):
         if sid not in self.subscriptions_by_session:
             raise ValueError("cannot remove non-existing session")
 
         subscriptions = self.subscriptions_by_session.pop(sid)
         for subscription_id, sub in subscriptions.items():
             subscription = self.subscriptions_by_topic[sub.topic]
             if sid in subscription.subscribers:
                 del subscription.subscribers[sid]
 
             if len(subscription.subscribers) == 0:
                 del self.subscriptions_by_topic[subscription.topic]
 
+        del self.sessions[sid]
+
     def has_subscription(self, topic: str):
         return topic in self.subscriptions_by_topic
 
     def receive_message(self, session_id: int, message: messages.Message) -> types.MessageWithRecipient:
         if isinstance(message, messages.Subscribe):
             if session_id not in self.subscriptions_by_session:
                 raise ValueError(f"cannot subscribe, session {session_id} doesn't exist")
 
             subscription = self.subscriptions_by_topic.get(message.topic)
             if subscription is None:
-                subscription = Subscription(self.id_gen.next(), message.topic, {session_id: session_id})
+                subscription = Subscription(self.idgen.next(), message.topic, {session_id: session_id})
                 self.subscriptions_by_topic[message.topic] = subscription
             else:
                 subscription.subscribers[session_id] = session_id
 
             self.subscriptions_by_session[session_id][subscription.id] = subscription
 
             subscribed = messages.Subscribed(message.request_id, subscription.id)
@@ -76,15 +80,15 @@
             raise ValueError("message type not supported")
 
     def receive_publish(self, session_id: int, message: messages.Publish) -> types.Publication:
         if session_id not in self.subscriptions_by_session:
             raise ValueError(f"cannot publish, session {session_id} doesn't exist")
 
         result = types.Publication(recipients=[])
-        publication_id = self.id_gen.next()
+        publication_id = self.idgen.next()
 
         subscription = self.subscriptions_by_topic.get(message.uri)
         if subscription is not None:
             event = messages.Event(subscription.id, publication_id, message.args, message.kwargs)
             result.event = event
             for subscriber_id in subscription.subscribers.keys():
                 result.recipients.append(subscriber_id)
```

### Comparing `wampproto-0.2.0/wampproto/joiner.py` & `wampproto-0.2.1/wampproto/joiner.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,18 +26,21 @@
         self._realm = realm
         self._serializer = serializer
         self._authenticator = authenticator if authenticator is not None else auth.AnonymousAuthenticator("", {})
         self._state = Joiner.STATE_NONE
 
         self._session_details: SessionDetails = None
 
-    def send_hello(self) -> bytes:
+    def send_hello(self, roles: dict[str, dict[str, dict[str, bool]]] = None) -> bytes:
+        if roles is None:
+            roles = CLIENT_ROLES
+
         hello = messages.Hello(
             realm=self._realm,
-            roles=CLIENT_ROLES,
+            roles=roles,
             authid=self._authenticator.authid,
             authmethods=[self._authenticator.auth_method],
             authextra=self._authenticator.auth_extra,
         )
 
         self._state = Joiner.STATE_HELLO_SENT
         return self._serializer.serialize(hello)
```

### Comparing `wampproto-0.2.0/wampproto/messages/__init__.py` & `wampproto-0.2.1/wampproto/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.2.0/wampproto/messages/abort.py` & `wampproto-0.2.1/wampproto/messages/abort.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,19 +11,19 @@
     TYPE = 3
 
     def __init__(self, details: dict, reason: str):
         super().__init__()
         self.details = details
         self.reason = reason
 
-    @staticmethod
-    def parse(msg: list[Any]) -> Abort:
-        util.sanity_check(msg, 3, 3, Abort.TYPE, Abort.TEXT)
+    @classmethod
+    def parse(cls, msg: list[Any]) -> Abort:
+        util.sanity_check(msg, 3, 3, cls.TYPE, cls.TEXT)
 
-        details = util.validate_details_or_raise(msg[1], Abort.TEXT)
+        details = util.validate_details_or_raise(msg[1], cls.TEXT)
 
-        reason = util.validate_uri_or_raise(msg[2], Abort.TEXT)
+        reason = util.validate_uri_or_raise(msg[2], cls.TEXT)
 
         return Abort(details, reason)
 
     def marshal(self) -> list[Any]:
-        return [Abort.TYPE, self.details, self.reason]
+        return [self.TYPE, self.details, self.reason]
```

### Comparing `wampproto-0.2.0/wampproto/messages/call.py` & `wampproto-0.2.1/wampproto/messages/publish.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 from typing import Any
 
 from wampproto.messages.message import Message
-from wampproto.messages import util, exceptions
+from wampproto.messages import util
 
 
-class Call(Message):
-    TEXT = "CALL"
-    TYPE = 48
+class Publish(Message):
+    TEXT = "PUBLISH"
+    TYPE = 16
 
     def __init__(
         self,
         request_id: int,
         uri: str,
         args: list | None = None,
         kwargs: dict | None = None,
@@ -21,38 +21,34 @@
         super().__init__()
         self.request_id = request_id
         self.uri = uri
         self.args = args
         self.kwargs = kwargs
         self.options = options if options is not None else {}
 
-    @staticmethod
-    def parse(msg: list[Any]) -> Call:
-        util.sanity_check(msg, 4, 6, Call.TYPE, Call.TEXT)
-
-        request_id = util.validate_session_id_or_raise(msg[1], Call.TEXT, "request ID")
-        options = util.validate_details_or_raise(msg[2], Call.TEXT, "options")
-        uri = util.validate_uri_or_raise(msg[3], Call.TEXT)
+    @classmethod
+    def parse(cls, msg: list[Any]) -> Publish:
+        util.sanity_check(msg, 4, 6, cls.TYPE, cls.TEXT)
+
+        request_id = util.validate_session_id_or_raise(msg[1], cls.TEXT, "request ID")
+        options = util.validate_details_or_raise(msg[2], cls.TEXT, "options")
+        uri = util.validate_uri_or_raise(msg[3], cls.TEXT)
 
-        args = None
+        args = []
         if len(msg) > 4:
             args = msg[4]
-            if not isinstance(args, list):
-                raise exceptions.InvalidTypeError(list, type(msg[4]), "args", Call.TEXT)
 
-        kwargs = None
+        kwargs = {}
         if len(msg) > 5:
             kwargs = msg[5]
-            if not isinstance(kwargs, dict):
-                raise exceptions.InvalidTypeError(dict, type(msg[5]), "kwargs", Call.TEXT)
 
-        return Call(request_id, uri, args, kwargs, options)
+        return Publish(request_id, uri, args, kwargs, options)
 
     def marshal(self) -> list[Any]:
-        message = [Call.TYPE, self.request_id, self.options, self.uri]
+        message = [self.TYPE, self.request_id, self.options, self.uri]
         if self.args is not None:
             message.append(self.args)
 
         if self.kwargs is not None:
             if self.args is None:
                 message.append([])
```

### Comparing `wampproto-0.2.0/wampproto/messages/cancel.py` & `wampproto-0.2.1/wampproto/messages/cancel.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,18 +16,18 @@
         call_request_id: int,
         options: dict | None = None,
     ):
         super().__init__()
         self.call_request_id = call_request_id
         self.options = options if options is not None else {}
 
-    @staticmethod
-    def parse(msg: list[Any]) -> Cancel:
-        util.sanity_check(msg, Cancel.MIN_LENGTH, Cancel.MAX_LENGTH, Cancel.TYPE, Cancel.TEXT)
+    @classmethod
+    def parse(cls, msg: list[Any]) -> Cancel:
+        util.sanity_check(msg, cls.MIN_LENGTH, cls.MAX_LENGTH, cls.TYPE, cls.TEXT)
 
-        request_id = util.validate_session_id_or_raise(msg[1], Cancel.TEXT, "call request ID")
-        options = util.validate_details_or_raise(msg[2], Cancel.TEXT, "options")
+        request_id = util.validate_session_id_or_raise(msg[1], cls.TEXT, "call request ID")
+        options = util.validate_details_or_raise(msg[2], cls.TEXT, "options")
 
         return Cancel(request_id, options)
 
     def marshal(self) -> list[Any]:
-        return [Cancel.TYPE, self.call_request_id, self.options]
+        return [self.TYPE, self.call_request_id, self.options]
```

### Comparing `wampproto-0.2.0/wampproto/messages/challenge.py` & `wampproto-0.2.1/wampproto/messages/challenge.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,21 +11,21 @@
     TYPE = 4
 
     def __init__(self, authmethod: str, extra: dict | None = None):
         super().__init__()
         self.authmethod = authmethod
         self.extra = {} if extra is None else extra
 
-    @staticmethod
-    def parse(msg: list[Any]) -> Challenge:
-        util.sanity_check(msg, 3, 3, Challenge.TYPE, Challenge.TEXT)
+    @classmethod
+    def parse(cls, msg: list[Any]) -> Challenge:
+        util.sanity_check(msg, 3, 3, cls.TYPE, cls.TEXT)
 
         authmethod = msg[1]
         if not isinstance(authmethod, str):
-            raise exceptions.ProtocolError(f"invalid type {type(authmethod)} for 'authmethod' in {Challenge.TEXT}")
+            raise exceptions.ProtocolError(f"invalid type {type(authmethod)} for 'authmethod' in {cls.TEXT}")
 
-        extra = util.validate_details_or_raise(msg[2], Challenge.TEXT)
+        extra = util.validate_details_or_raise(msg[2], cls.TEXT)
 
         return Challenge(authmethod, extra)
 
     def marshal(self) -> list[Any]:
-        return [Challenge.TYPE, self.authmethod, self.extra]
+        return [self.TYPE, self.authmethod, self.extra]
```

### Comparing `wampproto-0.2.0/wampproto/messages/error.py` & `wampproto-0.2.1/wampproto/messages/error.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,39 +23,39 @@
         self.message_type = message_type
         self.request_id = request_id
         self.uri = uri
         self.args = args
         self.kwargs = kwargs
         self.details = details if details is not None else {}
 
-    @staticmethod
-    def parse(msg: list[Any]) -> Error:
-        util.sanity_check(msg, 5, 7, Error.TYPE, Error.TEXT)
-
-        message_type = util.validate_session_id_or_raise(msg[1], Error.TEXT, "error ID")
-        request_id = util.validate_session_id_or_raise(msg[2], Error.TEXT, "request ID")
-        details = util.validate_details_or_raise(msg[3], Error.TEXT, "details")
-        uri = util.validate_uri_or_raise(msg[4], Error.TEXT)
+    @classmethod
+    def parse(cls, msg: list[Any]) -> Error:
+        util.sanity_check(msg, 5, 7, cls.TYPE, cls.TEXT)
+
+        message_type = util.validate_session_id_or_raise(msg[1], cls.TEXT, "error ID")
+        request_id = util.validate_session_id_or_raise(msg[2], cls.TEXT, "request ID")
+        details = util.validate_details_or_raise(msg[3], cls.TEXT, "details")
+        uri = util.validate_uri_or_raise(msg[4], cls.TEXT)
 
         args = None
         if len(msg) > 5:
             args = msg[5]
             if not isinstance(args, list):
-                raise exceptions.InvalidTypeError(list, type(msg[5]), "args", Error.TEXT)
+                raise exceptions.InvalidTypeError(list, type(msg[5]), "args", cls.TEXT)
 
         kwargs = None
         if len(msg) == 7:
             kwargs = msg[6]
             if not isinstance(kwargs, dict):
-                raise exceptions.InvalidTypeError(dict, type(msg[6]), "kwargs", Error.TEXT)
+                raise exceptions.InvalidTypeError(dict, type(msg[6]), "kwargs", cls.TEXT)
 
         return Error(message_type, request_id, uri, args, kwargs, details)
 
     def marshal(self) -> list[Any]:
-        message = [Error.TYPE, self.message_type, self.request_id, self.details, self.uri]
+        message = [self.TYPE, self.message_type, self.request_id, self.details, self.uri]
         if self.args is not None:
             message.append(self.args)
 
         if self.kwargs is not None:
             if self.args is None:
                 message.append([])
```

### Comparing `wampproto-0.2.0/wampproto/messages/event.py` & `wampproto-0.2.1/wampproto/messages/event.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,34 +21,34 @@
         super().__init__()
         self.subscription_id = subscription_id
         self.publication_id = publication_id
         self.args = args
         self.kwargs = kwargs
         self.details = details if details is not None else {}
 
-    @staticmethod
-    def parse(msg: list[Any]) -> Event:
-        util.sanity_check(msg, 4, 6, Event.TYPE, Event.TEXT)
-
-        subscription_id = util.validate_session_id_or_raise(msg[1], Event.TEXT, "subscription ID")
-        publication_id = util.validate_session_id_or_raise(msg[2], Event.TEXT, "publication ID")
-        options = util.validate_details_or_raise(msg[3], Event.TEXT, "options")
+    @classmethod
+    def parse(cls, msg: list[Any]) -> Event:
+        util.sanity_check(msg, 4, 6, cls.TYPE, cls.TEXT)
+
+        subscription_id = util.validate_session_id_or_raise(msg[1], cls.TEXT, "subscription ID")
+        publication_id = util.validate_session_id_or_raise(msg[2], cls.TEXT, "publication ID")
+        options = util.validate_details_or_raise(msg[3], cls.TEXT, "options")
 
         args = []
         if len(msg) > 4:
             args = msg[4]
 
         kwargs = {}
         if len(msg) > 5:
             kwargs = msg[5]
 
         return Event(subscription_id, publication_id, args, kwargs, options)
 
     def marshal(self) -> list[Any]:
-        message = [Event.TYPE, self.subscription_id, self.publication_id, self.details]
+        message = [self.TYPE, self.subscription_id, self.publication_id, self.details]
         if self.args is not None:
             message.append(self.args)
 
         if self.kwargs is not None:
             if self.args is None:
                 message.append([])
```

### Comparing `wampproto-0.2.0/wampproto/messages/exceptions.py` & `wampproto-0.2.1/wampproto/messages/exceptions.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.2.0/wampproto/messages/goodbye.py` & `wampproto-0.2.1/wampproto/messages/goodbye.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,19 +11,19 @@
     TYPE = 6
 
     def __init__(self, details: dict, reason: str):
         super().__init__()
         self.details = details
         self.reason = reason
 
-    @staticmethod
-    def parse(msg: list[Any]) -> Goodbye:
-        util.sanity_check(msg, 3, 3, Goodbye.TYPE, Goodbye.TEXT)
+    @classmethod
+    def parse(cls, msg: list[Any]) -> Goodbye:
+        util.sanity_check(msg, 3, 3, cls.TYPE, cls.TEXT)
 
-        details = util.validate_details_or_raise(msg[1], Goodbye.TEXT)
+        details = util.validate_details_or_raise(msg[1], cls.TEXT)
 
-        reason = util.validate_uri_or_raise(msg[2], Goodbye.TEXT)
+        reason = util.validate_uri_or_raise(msg[2], cls.TEXT)
 
         return Goodbye(details, reason)
 
     def marshal(self) -> list[Any]:
-        return [Goodbye.TYPE, self.details, self.reason]
+        return [self.TYPE, self.details, self.reason]
```

### Comparing `wampproto-0.2.0/wampproto/messages/hello.py` & `wampproto-0.2.1/wampproto/messages/hello.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,57 +23,57 @@
         self.realm = realm
         self.roles = roles
         self.authid = authid
         self.authrole = authrole
         self.authmethods = authmethods
         self.authextra = authextra
 
-    @staticmethod
-    def parse(msg: list[Any]) -> Hello:
-        util.sanity_check(msg, 3, 3, Hello.TYPE, Hello.TEXT)
+    @classmethod
+    def parse(cls, msg: list[Any]) -> Hello:
+        util.sanity_check(msg, 3, 3, cls.TYPE, cls.TEXT)
 
-        realm = util.validate_realm_or_raise(msg[1], Hello.TEXT)
-        details = util.validate_details_or_raise(msg[2], Hello.TEXT)
+        realm = util.validate_realm_or_raise(msg[1], cls.TEXT)
+        details = util.validate_details_or_raise(msg[2], cls.TEXT)
 
         roles = details.get("roles", {})
         if not isinstance(roles, dict):
-            raise exceptions.ProtocolError(f"invalid type for 'roles' in details for {Hello.TEXT}")
+            raise exceptions.ProtocolError(f"invalid type for 'roles' in details for {cls.TEXT}")
 
         if len(roles) == 0:
-            raise exceptions.ProtocolError(f"roles are missing in details for {Hello.TEXT}")
+            raise exceptions.ProtocolError(f"roles are missing in details for {cls.TEXT}")
 
         for role in roles.keys():
             if role not in util.AllowedRoles.__members__.values():
-                raise exceptions.ProtocolError(f"invalid role '{role}' in 'roles' details for {Hello.TEXT}")
+                raise exceptions.ProtocolError(f"invalid role '{role}' in 'roles' details for {cls.TEXT}")
 
         authid = details.get("authid", None)
         if authid is not None:
             if not isinstance(authid, str):
-                raise exceptions.ProtocolError(f"authid must be a type string for {Hello.TEXT}")
+                raise exceptions.ProtocolError(f"authid must be a type string for {cls.TEXT}")
 
         authrole = details.get("authrole", None)
         if authrole is not None:
             if not isinstance(authrole, str):
-                raise exceptions.ProtocolError(f"authrole must be a type string for {Hello.TEXT}")
+                raise exceptions.ProtocolError(f"authrole must be a type string for {cls.TEXT}")
 
         authmethods = details.get("authmethods", None)
         if authmethods is not None:
             if not isinstance(authmethods, list):
-                raise exceptions.InvalidTypeError(list, type(authmethods), "authmethods", Hello.TEXT)
+                raise exceptions.InvalidTypeError(list, type(authmethods), "authmethods", cls.TEXT)
 
             for authmethod in authmethods:
                 if not isinstance(authmethod, str):
                     raise exceptions.InvalidTypeError(
-                        str, type(authmethod), f"item '{authmethod}' in 'authmethods'", Hello.TEXT
+                        str, type(authmethod), f"item '{authmethod}' in 'authmethods'", cls.TEXT
                     )
 
         authextra = details.get("authextra", None)
         if authextra is not None:
             if not isinstance(authextra, dict):
-                raise exceptions.InvalidTypeError(dict, type(authextra), "authextra", Hello.TEXT)
+                raise exceptions.InvalidTypeError(dict, type(authextra), "authextra", cls.TEXT)
 
         return Hello(
             realm=realm, roles=roles, authid=authid, authrole=authrole, authmethods=authmethods, authextra=authextra
         )
 
     def marshal(self) -> list[Any]:
         details: dict[str, Any] = {"roles": self.roles}
```

### Comparing `wampproto-0.2.0/wampproto/messages/interrupt.py` & `wampproto-0.2.1/wampproto/messages/interrupt.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,18 +16,18 @@
         inv_request_id: int,
         options: dict | None = None,
     ):
         super().__init__()
         self.inv_request_id = inv_request_id
         self.options = options if options is not None else {}
 
-    @staticmethod
-    def parse(msg: list[Any]) -> Interrupt:
-        util.sanity_check(msg, Interrupt.MIN_LENGTH, Interrupt.MAX_LENGTH, Interrupt.TYPE, Interrupt.TEXT)
+    @classmethod
+    def parse(cls, msg: list[Any]) -> Interrupt:
+        util.sanity_check(msg, cls.MIN_LENGTH, cls.MAX_LENGTH, cls.TYPE, cls.TEXT)
 
-        request_id = util.validate_session_id_or_raise(msg[1], Interrupt.TEXT, "invocation request ID")
-        options = util.validate_details_or_raise(msg[2], Interrupt.TEXT, "options")
+        request_id = util.validate_session_id_or_raise(msg[1], cls.TEXT, "invocation request ID")
+        options = util.validate_details_or_raise(msg[2], cls.TEXT, "options")
 
         return Interrupt(request_id, options)
 
     def marshal(self) -> list[Any]:
-        return [Interrupt.TYPE, self.inv_request_id, self.options]
+        return [self.TYPE, self.inv_request_id, self.options]
```

### Comparing `wampproto-0.2.0/wampproto/messages/invocation.py` & `wampproto-0.2.1/wampproto/messages/result.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,57 +2,54 @@
 
 from typing import Any
 
 from wampproto.messages import util, exceptions
 from wampproto.messages.message import Message
 
 
-class Invocation(Message):
-    TEXT = "INVOCATION"
-    TYPE = 68
+class Result(Message):
+    TEXT = "RESULT"
+    TYPE = 50
 
     def __init__(
         self,
         request_id: int,
-        registration_id: int,
         args: list | None = None,
         kwargs: dict | None = None,
-        details: dict | None = None,
+        options: dict | None = None,
     ):
         super().__init__()
         self.request_id = request_id
-        self.registration_id = registration_id
         self.args = args
         self.kwargs = kwargs
-        self.details = details if details is not None else {}
+        self.options = options if options is not None else {}
 
-    @staticmethod
-    def parse(msg: list[Any]) -> Invocation:
-        util.sanity_check(msg, 4, 6, Invocation.TYPE, Invocation.TEXT)
-
-        request_id = util.validate_session_id_or_raise(msg[1], Invocation.TEXT, "request ID")
-        registration_id = util.validate_session_id_or_raise(msg[2], Invocation.TEXT, "registration ID")
-        options = util.validate_details_or_raise(msg[3], Invocation.TEXT, "options")
+    @classmethod
+    def parse(cls, msg: list[Any]) -> Result:
+        util.sanity_check(msg, 3, 5, cls.TYPE, cls.TEXT)
+
+        request_id = util.validate_session_id_or_raise(msg[1], cls.TEXT, "request ID")
+        options = util.validate_details_or_raise(msg[2], cls.TEXT, "options")
 
         args = None
-        if len(msg) > 4:
-            args = msg[4]
+        if len(msg) > 3:
+            args = msg[3]
             if not isinstance(args, list):
-                raise exceptions.InvalidTypeError(list, type(msg[4]), "args", Invocation.TEXT)
+                raise exceptions.InvalidTypeError(list, type(msg[3]), "args", cls.TEXT)
 
         kwargs = None
-        if len(msg) > 5:
-            kwargs = msg[5]
+        if len(msg) > 4:
+            kwargs = msg[4]
             if not isinstance(kwargs, dict):
-                raise exceptions.InvalidTypeError(dict, type(msg[5]), "kwargs", Invocation.TEXT)
+                raise exceptions.InvalidTypeError(dict, type(msg[4]), "kwargs", cls.TEXT)
 
-        return Invocation(request_id, registration_id, args, kwargs, options)
+        return Result(request_id, args, kwargs, options)
 
     def marshal(self) -> list[Any]:
-        message = [Invocation.TYPE, self.request_id, self.registration_id, self.details]
+        message = [self.TYPE, self.request_id, self.options]
         if self.args is not None:
             message.append(self.args)
 
         if self.kwargs is not None:
             if self.args is None:
                 message.append([])
```

### Comparing `wampproto-0.2.0/wampproto/messages/publish.py` & `wampproto-0.2.1/wampproto/messages/yield_.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 from __future__ import annotations
 
 from typing import Any
 
+from wampproto.messages import util, exceptions
 from wampproto.messages.message import Message
-from wampproto.messages import util
 
 
-class Publish(Message):
-    TEXT = "PUBLISH"
-    TYPE = 16
+class Yield(Message):
+    TEXT = "YIELD"
+    TYPE = 70
 
     def __init__(
         self,
         request_id: int,
-        uri: str,
         args: list | None = None,
         kwargs: dict | None = None,
         options: dict | None = None,
     ):
         super().__init__()
         self.request_id = request_id
-        self.uri = uri
         self.args = args
         self.kwargs = kwargs
         self.options = options if options is not None else {}
 
-    @staticmethod
-    def parse(msg: list[Any]) -> Publish:
-        util.sanity_check(msg, 4, 6, Publish.TYPE, Publish.TEXT)
-
-        request_id = util.validate_session_id_or_raise(msg[1], Publish.TEXT, "request ID")
-        options = util.validate_details_or_raise(msg[2], Publish.TEXT, "options")
-        uri = util.validate_uri_or_raise(msg[3], Publish.TEXT)
+    @classmethod
+    def parse(cls, msg: list[Any]) -> Yield:
+        util.sanity_check(msg, 3, 5, cls.TYPE, cls.TEXT)
+
+        request_id = util.validate_session_id_or_raise(msg[1], cls.TEXT, "request ID")
+        options = util.validate_details_or_raise(msg[2], cls.TEXT, "options")
+
+        args = None
+        if len(msg) > 3:
+            args = msg[3]
+            if not isinstance(args, list):
+                raise exceptions.InvalidTypeError(list, type(msg[3]), "args", cls.TEXT)
 
-        args = []
+        kwargs = None
         if len(msg) > 4:
-            args = msg[4]
+            kwargs = msg[4]
+            if not isinstance(kwargs, dict):
+                raise exceptions.InvalidTypeError(dict, type(msg[4]), "kwargs", cls.TEXT)
 
-        kwargs = {}
-        if len(msg) > 5:
-            kwargs = msg[5]
-
-        return Publish(request_id, uri, args, kwargs, options)
+        return Yield(request_id, args, kwargs, options)
 
     def marshal(self) -> list[Any]:
-        message = [Publish.TYPE, self.request_id, self.options, self.uri]
+        message = [self.TYPE, self.request_id, self.options]
         if self.args is not None:
             message.append(self.args)
 
         if self.kwargs is not None:
             if self.args is None:
                 message.append([])
```

### Comparing `wampproto-0.2.0/wampproto/messages/published.py` & `wampproto-0.2.1/wampproto/messages/register.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 
 from typing import Any
 
 from wampproto.messages.message import Message
 from wampproto.messages import util
 
 
-class Published(Message):
-    TEXT = "PUBLISHED"
-    TYPE = 17
+class Register(Message):
+    TEXT = "REGISTER"
+    TYPE = 64
 
-    def __init__(self, request_id: int, publication_id: int):
+    def __init__(self, request_id: int, uri: str, options: dict = None):
         super().__init__()
         self.request_id = request_id
-        self.publication_id = publication_id
+        self.uri = uri
+        self.options = options
 
-    @staticmethod
-    def parse(msg: list[Any]) -> Published:
-        util.sanity_check(msg, 3, 3, Published.TYPE, Published.TEXT)
+    @classmethod
+    def parse(cls, msg: list[Any]) -> Register:
+        util.sanity_check(msg, 4, 4, cls.TYPE, cls.TEXT)
+
+        request_id = util.validate_session_id_or_raise(msg[1], cls.TEXT, "request ID")
+        options = util.validate_details_or_raise(msg[2], cls.TEXT, "options")
+        uri = util.validate_uri_or_raise(msg[3], cls.TEXT)
 
-        request_id = util.validate_session_id_or_raise(msg[1], Published.TEXT, "request ID")
-        publication_id = util.validate_session_id_or_raise(msg[2], Published.TEXT, "publication ID")
-
-        return Published(request_id, publication_id)
+        return Register(request_id, uri, options)
 
     def marshal(self) -> list[Any]:
-        return [Published.TYPE, self.request_id, self.publication_id]
+        return [self.TYPE, self.request_id, self.options, self.uri]
```

### Comparing `wampproto-0.2.0/wampproto/messages/register.py` & `wampproto-0.2.1/wampproto/messages/subscribed.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,29 +2,27 @@
 
 from typing import Any
 
 from wampproto.messages.message import Message
 from wampproto.messages import util
 
 
-class Register(Message):
-    TEXT = "REGISTER"
-    TYPE = 64
+class Subscribed(Message):
+    TEXT = "SUBSCRIBED"
+    TYPE = 33
 
-    def __init__(self, request_id: int, uri: str, options: dict = None):
+    def __init__(self, request_id: int, subscription_id: int):
         super().__init__()
         self.request_id = request_id
-        self.uri = uri
-        self.options = options
+        self.subscription_id = subscription_id
 
-    @staticmethod
-    def parse(msg: list[Any]) -> Register:
-        util.sanity_check(msg, 4, 4, Register.TYPE, Register.TEXT)
-
-        request_id = util.validate_session_id_or_raise(msg[1], Register.TEXT, "request ID")
-        options = util.validate_details_or_raise(msg[2], Register.TEXT, "options")
-        uri = util.validate_uri_or_raise(msg[3], Register.TEXT)
+    @classmethod
+    def parse(cls, msg: list[Any]) -> Subscribed:
+        util.sanity_check(msg, 3, 3, cls.TYPE, cls.TEXT)
 
-        return Register(request_id, uri, options)
+        request_id = util.validate_session_id_or_raise(msg[1], cls.TEXT, "request ID")
+        subscription_id = util.validate_session_id_or_raise(msg[2], cls.TEXT, "subscription ID")
+
+        return Subscribed(request_id, subscription_id)
 
     def marshal(self) -> list[Any]:
-        return [Register.TYPE, self.request_id, self.options, self.uri]
+        return [self.TYPE, self.request_id, self.subscription_id]
```

### Comparing `wampproto-0.2.0/wampproto/messages/registered.py` & `wampproto-0.2.1/wampproto/messages/registered.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Any
 
 from wampproto.messages.message import Message
 from wampproto.messages import util
 
 
 class Registered(Message):
@@ -9,18 +11,18 @@
     TYPE = 65
 
     def __init__(self, request_id: int, registration_id: int):
         super().__init__()
         self.request_id = request_id
         self.registration_id = registration_id
 
-    @staticmethod
-    def parse(msg: list[Any]) -> "Registered":
-        util.sanity_check(msg, 3, 3, Registered.TYPE, Registered.TEXT)
+    @classmethod
+    def parse(cls, msg: list[Any]) -> Registered:
+        util.sanity_check(msg, 3, 3, cls.TYPE, cls.TEXT)
 
-        request_id = util.validate_session_id_or_raise(msg[1], Registered.TEXT, "request ID")
-        registration_id = util.validate_session_id_or_raise(msg[2], Registered.TEXT, "registration ID")
+        request_id = util.validate_session_id_or_raise(msg[1], cls.TEXT, "request ID")
+        registration_id = util.validate_session_id_or_raise(msg[2], cls.TEXT, "registration ID")
 
         return Registered(request_id, registration_id)
 
     def marshal(self) -> list[Any]:
-        return [Registered.TYPE, self.request_id, self.registration_id]
+        return [self.TYPE, self.request_id, self.registration_id]
```

### Comparing `wampproto-0.2.0/wampproto/messages/result.py` & `wampproto-0.2.1/wampproto/messages/invocation.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,54 +2,57 @@
 
 from typing import Any
 
 from wampproto.messages import util, exceptions
 from wampproto.messages.message import Message
 
 
-class Result(Message):
-    TEXT = "RESULT"
-    TYPE = 50
+class Invocation(Message):
+    TEXT = "INVOCATION"
+    TYPE = 68
 
     def __init__(
         self,
         request_id: int,
+        registration_id: int,
         args: list | None = None,
         kwargs: dict | None = None,
-        options: dict | None = None,
+        details: dict | None = None,
     ):
         super().__init__()
         self.request_id = request_id
+        self.registration_id = registration_id
         self.args = args
         self.kwargs = kwargs
-        self.options = options if options is not None else {}
+        self.details = details if details is not None else {}
 
-    @staticmethod
-    def parse(msg: list[Any]) -> Result:
-        util.sanity_check(msg, 3, 5, Result.TYPE, Result.TEXT)
-
-        request_id = util.validate_session_id_or_raise(msg[1], Result.TEXT, "request ID")
-        options = util.validate_details_or_raise(msg[2], Result.TEXT, "options")
+    @classmethod
+    def parse(cls, msg: list[Any]) -> Invocation:
+        util.sanity_check(msg, 4, 6, cls.TYPE, cls.TEXT)
+
+        request_id = util.validate_session_id_or_raise(msg[1], cls.TEXT, "request ID")
+        registration_id = util.validate_session_id_or_raise(msg[2], cls.TEXT, "registration ID")
+        options = util.validate_details_or_raise(msg[3], cls.TEXT, "options")
 
         args = None
-        if len(msg) > 3:
-            args = msg[3]
+        if len(msg) > 4:
+            args = msg[4]
             if not isinstance(args, list):
-                raise exceptions.InvalidTypeError(list, type(msg[3]), "args", Result.TEXT)
+                raise exceptions.InvalidTypeError(list, type(msg[4]), "args", cls.TEXT)
 
         kwargs = None
-        if len(msg) > 4:
-            kwargs = msg[4]
+        if len(msg) > 5:
+            kwargs = msg[5]
             if not isinstance(kwargs, dict):
-                raise exceptions.InvalidTypeError(dict, type(msg[4]), "kwargs", Result.TEXT)
+                raise exceptions.InvalidTypeError(dict, type(msg[5]), "kwargs", cls.TEXT)
 
-        return Result(request_id, args, kwargs, options)
+        return Invocation(request_id, registration_id, args, kwargs, options)
 
     def marshal(self) -> list[Any]:
-        message = [Result.TYPE, self.request_id, self.options]
+        message = [self.TYPE, self.request_id, self.registration_id, self.details]
         if self.args is not None:
             message.append(self.args)
 
         if self.kwargs is not None:
             if self.args is None:
                 message.append([])
```

### Comparing `wampproto-0.2.0/wampproto/messages/subscribe.py` & `wampproto-0.2.1/wampproto/messages/subscribe.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Any
 
 from wampproto.messages.message import Message
 from wampproto.messages import util
 
 
 class Subscribe(Message):
@@ -10,19 +12,19 @@
 
     def __init__(self, request_id: int, topic: str, options: dict = None):
         super().__init__()
         self.request_id = request_id
         self.topic: str = topic
         self.options = options if options else {}
 
-    @staticmethod
-    def parse(msg: list[Any]) -> "Subscribe":
-        util.sanity_check(msg, 4, 4, Subscribe.TYPE, Subscribe.TEXT)
+    @classmethod
+    def parse(cls, msg: list[Any]) -> Subscribe:
+        util.sanity_check(msg, 4, 4, cls.TYPE, cls.TEXT)
 
-        request_id = util.validate_session_id_or_raise(msg[1], Subscribe.TEXT, "request ID")
-        options = util.validate_details_or_raise(msg[2], Subscribe.TEXT, "options")
+        request_id = util.validate_session_id_or_raise(msg[1], cls.TEXT, "request ID")
+        options = util.validate_details_or_raise(msg[2], cls.TEXT, "options")
         topic = util.validate_uri_or_raise(msg[3], "topic")
 
         return Subscribe(request_id, topic, options)
 
     def marshal(self) -> list[Any]:
-        return [Subscribe.TYPE, self.request_id, self.options, self.topic]
+        return [self.TYPE, self.request_id, self.options, self.topic]
```

### Comparing `wampproto-0.2.0/wampproto/messages/subscribed.py` & `wampproto-0.2.1/wampproto/messages/unsubscribe.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,28 @@
+from __future__ import annotations
+
 from typing import Any
 
 from wampproto.messages.message import Message
 from wampproto.messages import util
 
 
-class Subscribed(Message):
-    TEXT = "SUBSCRIBED"
-    TYPE = 33
+class UnSubscribe(Message):
+    TEXT = "UNSUBSCRIBE"
+    TYPE = 34
 
     def __init__(self, request_id: int, subscription_id: int):
         super().__init__()
         self.request_id = request_id
         self.subscription_id = subscription_id
 
-    @staticmethod
-    def parse(msg: list[Any]) -> "Subscribed":
-        util.sanity_check(msg, 3, 3, Subscribed.TYPE, Subscribed.TEXT)
+    @classmethod
+    def parse(cls, msg: list[Any]) -> UnSubscribe:
+        util.sanity_check(msg, 3, 3, cls.TYPE, cls.TEXT)
 
-        request_id = util.validate_session_id_or_raise(msg[1], Subscribed.TEXT, "request ID")
-        subscription_id = util.validate_session_id_or_raise(msg[2], Subscribed.TEXT, "subscription ID")
+        request_id = util.validate_session_id_or_raise(msg[1], cls.TEXT, "request ID")
+        subscription_id = util.validate_session_id_or_raise(msg[2], cls.TEXT, "subscription ID")
 
-        return Subscribed(request_id, subscription_id)
+        return UnSubscribe(request_id, subscription_id)
 
     def marshal(self) -> list[Any]:
-        return [Subscribed.TYPE, self.request_id, self.subscription_id]
+        return [self.TYPE, self.request_id, self.subscription_id]
```

### Comparing `wampproto-0.2.0/wampproto/messages/unregister.py` & `wampproto-0.2.1/wampproto/messages/unregister.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Any
 
 from wampproto.messages.message import Message
 from wampproto.messages import util
 
 
 class UnRegister(Message):
@@ -9,18 +11,18 @@
     TYPE = 66
 
     def __init__(self, request_id: int, registration_id: int):
         super().__init__()
         self.request_id = request_id
         self.registration_id = registration_id
 
-    @staticmethod
-    def parse(msg: list[Any]) -> "UnRegister":
-        util.sanity_check(msg, 3, 3, UnRegister.TYPE, UnRegister.TEXT)
+    @classmethod
+    def parse(cls, msg: list[Any]) -> UnRegister:
+        util.sanity_check(msg, 3, 3, cls.TYPE, cls.TEXT)
 
-        request_id = util.validate_session_id_or_raise(msg[1], UnRegister.TEXT, "request ID")
-        registration_id = util.validate_session_id_or_raise(msg[2], UnRegister.TEXT, "registration ID")
+        request_id = util.validate_session_id_or_raise(msg[1], cls.TEXT, "request ID")
+        registration_id = util.validate_session_id_or_raise(msg[2], cls.TEXT, "registration ID")
 
         return UnRegister(request_id, registration_id)
 
     def marshal(self) -> list[Any]:
-        return [UnRegister.TYPE, self.request_id, self.registration_id]
+        return [self.TYPE, self.request_id, self.registration_id]
```

### Comparing `wampproto-0.2.0/wampproto/messages/unsubscribed.py` & `wampproto-0.2.1/wampproto/messages/unregistered.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,26 @@
+from __future__ import annotations
+
 from typing import Any
 
 from wampproto.messages.message import Message
 from wampproto.messages import util
 
 
-class UnSubscribed(Message):
-    TEXT = "UNSUBSCRIBED"
-    TYPE = 35
+class UnRegistered(Message):
+    TEXT = "UNREGISTERED"
+    TYPE = 67
 
     def __init__(self, request_id: int):
         super().__init__()
         self.request_id = request_id
 
-    @staticmethod
-    def parse(msg: list[Any]) -> "UnSubscribed":
-        util.sanity_check(msg, 2, 2, UnSubscribed.TYPE, UnSubscribed.TEXT)
+    @classmethod
+    def parse(cls, msg: list[Any]) -> UnRegistered:
+        util.sanity_check(msg, 2, 2, cls.TYPE, cls.TEXT)
 
-        request_id = util.validate_session_id_or_raise(msg[1], UnSubscribed.TEXT, "request ID")
+        request_id = util.validate_session_id_or_raise(msg[1], cls.TEXT, "request ID")
 
-        return UnSubscribed(request_id)
+        return UnRegistered(request_id)
 
     def marshal(self) -> list[Any]:
-        return [UnSubscribed.TYPE, self.request_id]
+        return [self.TYPE, self.request_id]
```

### Comparing `wampproto-0.2.0/wampproto/messages/welcome.py` & `wampproto-0.2.1/wampproto/messages/welcome.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,51 +23,51 @@
         self.session_id = session_id
         self.roles = roles
         self.authid = authid
         self.authrole = authrole
         self.authmethod = authmethod
         self.authextra = authextra
 
-    @staticmethod
-    def parse(msg: list[Any]) -> Welcome:
-        util.sanity_check(msg, 3, 3, Welcome.TYPE, Welcome.TEXT)
+    @classmethod
+    def parse(cls, msg: list[Any]) -> Welcome:
+        util.sanity_check(msg, 3, 3, cls.TYPE, cls.TEXT)
 
-        session_id = util.validate_session_id_or_raise(msg[1], Welcome.TEXT)
-        details = util.validate_details_or_raise(msg[2], Welcome.TEXT)
+        session_id = util.validate_session_id_or_raise(msg[1], cls.TEXT)
+        details = util.validate_details_or_raise(msg[2], cls.TEXT)
 
         roles = details.get("roles", {})
         if not isinstance(roles, dict):
-            raise exceptions.ProtocolError(f"invalid type for 'roles' in details for {Welcome.TEXT}")
+            raise exceptions.ProtocolError(f"invalid type for 'roles' in details for {cls.TEXT}")
 
         if len(roles) == 0:
-            raise exceptions.ProtocolError(f"roles are missing in details for {Welcome.TEXT}")
+            raise exceptions.ProtocolError(f"roles are missing in details for {cls.TEXT}")
 
         # for role in roles.keys():
         #     if role not in util.AllowedRoles.__members__.values():
         #         raise exceptions.ProtocolError(f"invalid role '{role}' in 'roles' details for {Welcome.WELCOME_TEXT}")
 
         authid = details.get("authid", None)
         if authid is not None:
             if not isinstance(authid, str):
-                raise exceptions.ProtocolError(f"authid must be a type string for {Welcome.TEXT}")
+                raise exceptions.ProtocolError(f"authid must be a type string for {cls.TEXT}")
 
         authrole = details.get("authrole", None)
         if authrole is not None:
             if not isinstance(authrole, str):
-                raise exceptions.ProtocolError(f"authrole must be a type string for {Welcome.TEXT}")
+                raise exceptions.ProtocolError(f"authrole must be a type string for {cls.TEXT}")
 
         authmethod = details.get("authmethod", None)
         if authmethod is not None:
             if not isinstance(authmethod, str):
-                raise exceptions.InvalidTypeError(str, type(authmethod), "authmethod", Welcome.TEXT)
+                raise exceptions.InvalidTypeError(str, type(authmethod), "authmethod", cls.TEXT)
 
         authextra = details.get("authextra", None)
         if authextra is not None:
             if not isinstance(authextra, dict):
-                raise exceptions.InvalidTypeError(dict, type(authextra), "authextra", Welcome.TEXT)
+                raise exceptions.InvalidTypeError(dict, type(authextra), "authextra", cls.TEXT)
 
         return Welcome(
             session_id=session_id,
             roles=roles,
             authid=authid,
             authrole=authrole,
             authmethod=authmethod,
```

### Comparing `wampproto-0.2.0/wampproto/messages/yield_.py` & `wampproto-0.2.1/wampproto/messages/call.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 from __future__ import annotations
 
 from typing import Any
 
-from wampproto.messages import util, exceptions
+from wampproto.messages import util
 from wampproto.messages.message import Message
+from wampproto.messages.validation_spec import ValidationSpec
 
 
-class Yield(Message):
-    TEXT = "YIELD"
-    TYPE = 70
+class Call(Message):
+    TEXT = "CALL"
+    TYPE = 48
+
+    # index number mapped to validation interface
+    VALIDATION_SPEC = ValidationSpec(
+        min_length=4,
+        max_length=6,
+        spec={
+            1: util.validate_request_id,
+            2: util.validate_options,
+            3: util.validate_uri,
+            4: util.validate_args,
+            5: util.validate_kwargs,
+        },
+    )
 
     def __init__(
         self,
         request_id: int,
+        uri: str,
         args: list | None = None,
         kwargs: dict | None = None,
         options: dict | None = None,
     ):
         super().__init__()
         self.request_id = request_id
+        self.uri = uri
         self.args = args
         self.kwargs = kwargs
         self.options = options if options is not None else {}
 
-    @staticmethod
-    def parse(msg: list[Any]) -> Yield:
-        util.sanity_check(msg, 3, 5, Yield.TYPE, Yield.TEXT)
-
-        request_id = util.validate_session_id_or_raise(msg[1], Yield.TEXT, "request ID")
-        options = util.validate_details_or_raise(msg[2], Yield.TEXT, "options")
-
-        args = None
-        if len(msg) > 3:
-            args = msg[3]
-            if not isinstance(args, list):
-                raise exceptions.InvalidTypeError(list, type(msg[3]), "args", Yield.TEXT)
-
-        kwargs = None
-        if len(msg) > 4:
-            kwargs = msg[4]
-            if not isinstance(kwargs, dict):
-                raise exceptions.InvalidTypeError(dict, type(msg[4]), "kwargs", Yield.TEXT)
-
-        return Yield(request_id, args, kwargs, options)
+    @classmethod
+    def parse(cls, msg: list[Any]) -> Call:
+        f = util.validate_message(msg, cls.TYPE, cls.TEXT, cls.VALIDATION_SPEC)
+        return Call(f.request_id, f.uri, f.args, f.kwargs, f.options)
 
     def marshal(self) -> list[Any]:
-        message = [Yield.TYPE, self.request_id, self.options]
+        message = [self.TYPE, self.request_id, self.options, self.uri]
         if self.args is not None:
             message.append(self.args)
 
         if self.kwargs is not None:
             if self.args is None:
                 message.append([])
```

### Comparing `wampproto-0.2.0/wampproto/serializers/serializer.py` & `wampproto-0.2.1/wampproto/serializers/serializer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from wampproto import messages
 
 
 class Serializer:
-    def serialize(self, message: messages.Message) -> bytes:
+    def serialize(self, message: messages.Message) -> bytes | str:
         raise NotImplementedError()
 
     def deserialize(self, data: bytes | str) -> messages.Message:
         raise NotImplementedError()
 
 
 def to_message(message: list) -> messages.Message:
```

### Comparing `wampproto-0.2.0/wampproto/session.py` & `wampproto-0.2.1/wampproto/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             self._subscribe_requests[msg.request_id] = msg.request_id
         elif isinstance(msg, messages.UnSubscribe):
             self._unsubscribe_requests[msg.request_id] = msg.subscription_id
         elif isinstance(msg, messages.Error):
             if msg.message_type != messages.Invocation.TYPE:
                 raise ValueError("send only supported for invocation error")
 
-            del self._invocation_requests[msg.request_id]
+            self._invocation_requests.pop(msg.request_id, None)
         else:
             raise ValueError(f"unknown message type {type(msg)}")
 
         return self._serializer.serialize(msg)
 
     def receive(self, data: bytes) -> messages.Message:
         msg = self._serializer.deserialize(data)
```

### Comparing `wampproto-0.2.0/wampproto/types.py` & `wampproto-0.2.1/wampproto/types.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.2.0/wampproto.egg-info/PKG-INFO` & `wampproto-0.2.1/wampproto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wampproto
-Version: 0.2.0
+Version: 0.2.1
 Summary: https://github.com/xconnio/wampproto.py
 Author-email: Omer Akram <omer@thing.com>, Mahad Munir <mahad@xconn.io>
 License: MIT License
         
         Copyright (c) 2024 Simple Things Inc.
         Copyright (c) 2024 XConnIO Ltd.
```

### Comparing `wampproto-0.2.0/wampproto.egg-info/SOURCES.txt` & `wampproto-0.2.1/wampproto.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 wampproto/acceptor.py
 wampproto/broker.py
 wampproto/dealer.py
 wampproto/idgen.py
 wampproto/joiner.py
 wampproto/session.py
 wampproto/types.py
+wampproto/uris.py
 wampproto.egg-info/PKG-INFO
 wampproto.egg-info/SOURCES.txt
 wampproto.egg-info/dependency_links.txt
 wampproto.egg-info/requires.txt
 wampproto.egg-info/top_level.txt
 wampproto/auth/__init__.py
 wampproto/auth/anonymous.py
@@ -43,14 +44,15 @@
 wampproto/messages/subscribe.py
 wampproto/messages/subscribed.py
 wampproto/messages/unregister.py
 wampproto/messages/unregistered.py
 wampproto/messages/unsubscribe.py
 wampproto/messages/unsubscribed.py
 wampproto/messages/util.py
+wampproto/messages/validation_spec.py
 wampproto/messages/welcome.py
 wampproto/messages/yield_.py
 wampproto/serializers/__init__.py
 wampproto/serializers/cbor.py
 wampproto/serializers/json.py
 wampproto/serializers/msgpack.py
 wampproto/serializers/serializer.py
```

