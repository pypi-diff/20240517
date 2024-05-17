# Comparing `tmp/woodAI-1.0.1-py3-none-any.whl.zip` & `tmp/woodAI-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 4030 bytes, number of entries: 7
--rw-r--r--  2.0 unx       47 b- defN 24-May-15 06:19 woodAI/__init__.py
+Zip file size: 4417 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       92 b- defN 24-May-17 07:07 woodAI/__init__.py
+-rw-rw-r--  2.0 unx      282 b- defN 24-May-17 07:13 woodAI/__init__.pyi
 -rw-r--r--  2.0 unx     5558 b- defN 24-May-16 11:02 woodAI/ai_chat.py
--rw-rw-r--  2.0 unx     1081 b- defN 24-May-16 11:03 woodAI-1.0.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      231 b- defN 24-May-16 11:03 woodAI-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-16 11:03 woodAI-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-May-16 11:03 woodAI-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      530 b- defN 24-May-16 11:03 woodAI-1.0.1.dist-info/RECORD
-7 files, 7546 bytes uncompressed, 3090 bytes compressed:  59.1%
+-rw-rw-r--  2.0 unx     1081 b- defN 24-May-17 07:23 woodAI-1.0.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      231 b- defN 24-May-17 07:23 woodAI-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-17 07:23 woodAI-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-May-17 07:23 woodAI-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      605 b- defN 24-May-17 07:23 woodAI-1.0.2.dist-info/RECORD
+8 files, 7948 bytes uncompressed, 3363 bytes compressed:  57.7%
```

## zipnote {}

```diff
@@ -1,22 +1,25 @@
 Filename: woodAI/__init__.py
 Comment: 
 
+Filename: woodAI/__init__.pyi
+Comment: 
+
 Filename: woodAI/ai_chat.py
 Comment: 
 
-Filename: woodAI-1.0.1.dist-info/LICENSE.txt
+Filename: woodAI-1.0.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: woodAI-1.0.1.dist-info/METADATA
+Filename: woodAI-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: woodAI-1.0.1.dist-info/WHEEL
+Filename: woodAI-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: woodAI-1.0.1.dist-info/top_level.txt
+Filename: woodAI-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: woodAI-1.0.1.dist-info/RECORD
+Filename: woodAI-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## woodAI/__init__.py

```diff
@@ -1 +1,2 @@
+__all__ = ['chat_set', 'chat', 'chat_clear']
 from .ai_chat import chat_set, chat, chat_clear
```

## Comparing `woodAI-1.0.1.dist-info/LICENSE.txt` & `woodAI-1.0.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

