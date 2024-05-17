# Comparing `tmp/filedata-0.2.5.tar.gz` & `tmp/filedata-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filedata-0.2.5.tar", last modified: Wed Feb 21 17:36:59 2024, max compression
+gzip compressed data, was "filedata-0.2.6.tar", last modified: Fri May 17 09:29:23 2024, max compression
```

## Comparing `filedata-0.2.5.tar` & `filedata-0.2.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2024-02-21 17:36:59.967810 filedata-0.2.5/
--rw-r--r--   0 jadbin     (501) staff       (20)      107 2024-02-21 17:30:13.000000 filedata-0.2.5/MANIFEST.in
--rw-r--r--   0 jadbin     (501) staff       (20)      719 2024-02-21 17:36:59.967645 filedata-0.2.5/PKG-INFO
--rw-r--r--   0 jadbin     (501) staff       (20)       57 2024-02-21 17:30:13.000000 filedata-0.2.5/README.rst
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2024-02-21 17:36:59.965968 filedata-0.2.5/filedata/
--rw-r--r--   0 jadbin     (501) staff       (20)       22 2024-02-21 17:36:37.000000 filedata-0.2.5/filedata/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)      841 2024-02-21 17:30:13.000000 filedata-0.2.5/filedata/config.py
--rw-r--r--   0 jadbin     (501) staff       (20)     3437 2024-02-21 17:33:19.000000 filedata-0.2.5/filedata/file.py
--rw-r--r--   0 jadbin     (501) staff       (20)     2895 2024-02-21 17:30:13.000000 filedata-0.2.5/filedata/html.py
--rw-r--r--   0 jadbin     (501) staff       (20)     6497 2024-02-21 17:31:41.000000 filedata-0.2.5/filedata/image.py
--rw-r--r--   0 jadbin     (501) staff       (20)      801 2024-02-21 17:30:13.000000 filedata-0.2.5/filedata/pdf.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1198 2024-02-21 17:30:13.000000 filedata-0.2.5/filedata/retry.py
--rw-r--r--   0 jadbin     (501) staff       (20)      624 2024-02-21 17:30:13.000000 filedata-0.2.5/filedata/text.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2024-02-21 17:36:59.966850 filedata-0.2.5/filedata/text_algo/
--rw-r--r--   0 jadbin     (501) staff       (20)        0 2024-02-21 17:30:13.000000 filedata-0.2.5/filedata/text_algo/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)     4274 2024-02-21 17:30:13.000000 filedata-0.2.5/filedata/text_algo/ac.py
--rw-r--r--   0 jadbin     (501) staff       (20)       94 2024-02-21 17:30:13.000000 filedata-0.2.5/filedata/time.py
--rw-r--r--   0 jadbin     (501) staff       (20)      466 2024-02-21 17:30:13.000000 filedata-0.2.5/filedata/utils.py
--rw-r--r--   0 jadbin     (501) staff       (20)      252 2024-02-21 17:30:13.000000 filedata-0.2.5/filedata/video.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2024-02-21 17:36:59.967480 filedata-0.2.5/filedata.egg-info/
--rw-r--r--   0 jadbin     (501) staff       (20)      719 2024-02-21 17:36:59.000000 filedata-0.2.5/filedata.egg-info/PKG-INFO
--rw-r--r--   0 jadbin     (501) staff       (20)      578 2024-02-21 17:36:59.000000 filedata-0.2.5/filedata.egg-info/SOURCES.txt
--rw-r--r--   0 jadbin     (501) staff       (20)        1 2024-02-21 17:36:59.000000 filedata-0.2.5/filedata.egg-info/dependency_links.txt
--rw-r--r--   0 jadbin     (501) staff       (20)        1 2024-02-21 17:36:59.000000 filedata-0.2.5/filedata.egg-info/not-zip-safe
--rw-r--r--   0 jadbin     (501) staff       (20)      124 2024-02-21 17:36:59.000000 filedata-0.2.5/filedata.egg-info/requires.txt
--rw-r--r--   0 jadbin     (501) staff       (20)       15 2024-02-21 17:36:59.000000 filedata-0.2.5/filedata.egg-info/top_level.txt
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2024-02-21 17:36:59.966998 filedata-0.2.5/requirements/
--rw-r--r--   0 jadbin     (501) staff       (20)       18 2024-02-21 17:30:13.000000 filedata-0.2.5/requirements/test.txt
--rw-r--r--   0 jadbin     (501) staff       (20)       38 2024-02-21 17:36:59.967855 filedata-0.2.5/setup.cfg
--rw-r--r--   0 jadbin     (501) staff       (20)     1549 2024-02-21 17:30:13.000000 filedata-0.2.5/setup.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2024-02-21 17:36:59.967109 filedata-0.2.5/tests/
--rw-r--r--   0 jadbin     (501) staff       (20)        0 2024-02-21 17:30:13.000000 filedata-0.2.5/tests/__init__.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2024-02-21 17:36:59.967305 filedata-0.2.5/tests/test_text_algo/
--rw-r--r--   0 jadbin     (501) staff       (20)        0 2024-02-21 17:30:13.000000 filedata-0.2.5/tests/test_text_algo/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1292 2024-02-21 17:30:13.000000 filedata-0.2.5/tests/test_text_algo/test_ac.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 09:29:23.322972 filedata-0.2.6/
+-rwxrwxrwx   0 root         (0) root         (0)      107 2023-06-21 00:08:49.000000 filedata-0.2.6/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)      546 2024-05-17 09:29:23.321053 filedata-0.2.6/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       57 2023-06-21 00:08:49.000000 filedata-0.2.6/README.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 09:29:23.078340 filedata-0.2.6/filedata/
+-rwxrwxrwx   0 root         (0) root         (0)       22 2024-05-17 09:28:10.000000 filedata-0.2.6/filedata/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      841 2023-06-21 00:08:49.000000 filedata-0.2.6/filedata/config.py
+-rwxrwxrwx   0 root         (0) root         (0)     3437 2024-02-26 23:43:01.000000 filedata-0.2.6/filedata/file.py
+-rwxrwxrwx   0 root         (0) root         (0)     2895 2023-06-21 00:08:49.000000 filedata-0.2.6/filedata/html.py
+-rwxrwxrwx   0 root         (0) root         (0)     6497 2024-02-26 23:43:01.000000 filedata-0.2.6/filedata/image.py
+-rwxrwxrwx   0 root         (0) root         (0)      801 2023-06-21 00:08:49.000000 filedata-0.2.6/filedata/pdf.py
+-rwxrwxrwx   0 root         (0) root         (0)     1198 2023-06-21 00:08:49.000000 filedata-0.2.6/filedata/retry.py
+-rwxrwxrwx   0 root         (0) root         (0)      624 2023-06-21 01:07:06.000000 filedata-0.2.6/filedata/text.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 09:29:23.259722 filedata-0.2.6/filedata/text_algo/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 00:11:15.000000 filedata-0.2.6/filedata/text_algo/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4560 2024-05-17 09:28:44.000000 filedata-0.2.6/filedata/text_algo/ac.py
+-rwxrwxrwx   0 root         (0) root         (0)       94 2023-06-21 00:08:49.000000 filedata-0.2.6/filedata/time.py
+-rwxrwxrwx   0 root         (0) root         (0)      466 2023-06-21 00:08:49.000000 filedata-0.2.6/filedata/utils.py
+-rwxrwxrwx   0 root         (0) root         (0)      252 2023-06-21 00:08:49.000000 filedata-0.2.6/filedata/video.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 09:29:23.233071 filedata-0.2.6/filedata.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      546 2024-05-17 09:29:22.000000 filedata-0.2.6/filedata.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      578 2024-05-17 09:29:22.000000 filedata-0.2.6/filedata.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-17 09:29:22.000000 filedata-0.2.6/filedata.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-21 01:08:29.000000 filedata-0.2.6/filedata.egg-info/not-zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)      124 2024-05-17 09:29:22.000000 filedata-0.2.6/filedata.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       15 2024-05-17 09:29:22.000000 filedata-0.2.6/filedata.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 09:29:23.274732 filedata-0.2.6/requirements/
+-rwxrwxrwx   0 root         (0) root         (0)       18 2023-06-21 00:08:49.000000 filedata-0.2.6/requirements/test.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-17 09:29:23.322972 filedata-0.2.6/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1549 2023-06-21 00:08:49.000000 filedata-0.2.6/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 09:29:23.281645 filedata-0.2.6/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 00:08:49.000000 filedata-0.2.6/tests/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 09:29:23.305356 filedata-0.2.6/tests/test_text_algo/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 00:58:58.000000 filedata-0.2.6/tests/test_text_algo/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1688 2024-05-17 09:25:53.000000 filedata-0.2.6/tests/test_text_algo/test_ac.py
```

### Comparing `filedata-0.2.5/filedata/config.py` & `filedata-0.2.6/filedata/config.py`

 * *Files identical despite different names*

### Comparing `filedata-0.2.5/filedata/file.py` & `filedata-0.2.6/filedata/file.py`

 * *Files identical despite different names*

### Comparing `filedata-0.2.5/filedata/html.py` & `filedata-0.2.6/filedata/html.py`

 * *Files identical despite different names*

### Comparing `filedata-0.2.5/filedata/image.py` & `filedata-0.2.6/filedata/image.py`

 * *Files identical despite different names*

### Comparing `filedata-0.2.5/filedata/pdf.py` & `filedata-0.2.6/filedata/pdf.py`

 * *Files identical despite different names*

### Comparing `filedata-0.2.5/filedata/retry.py` & `filedata-0.2.6/filedata/retry.py`

 * *Files identical despite different names*

### Comparing `filedata-0.2.5/filedata/text.py` & `filedata-0.2.6/filedata/text.py`

 * *Files identical despite different names*

### Comparing `filedata-0.2.5/filedata/text_algo/ac.py` & `filedata-0.2.6/filedata/text_algo/ac.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,33 +71,41 @@
                         break
                     else:
                         if p.is_root:
                             node.fail = weakref.ref(self._root)
                             break
                         p = p.fail()
 
-    def find_all(self, content: str):
+    def find_all(self, content: str, from_start: bool = False):
         result: List[MatchResult] = []
         if not content:
             return result
 
         current_node: ACNode = self._root
         for i, ch in enumerate(content):
             while True:
                 if ch not in current_node:
+                    if from_start:
+                        result.sort(key=lambda x: x.position)
+                        return result
+
                     if current_node.is_root:
                         break
                     current_node = current_node.fail()
                 else:
                     current_node = current_node[ch]
                     for w in current_node.words:
+                        idx = i - len(w) + 1
+                        if from_start and idx != 0:
+                            continue
+
                         result.append(
                             MatchResult(
                                 word=w,
-                                position=(i - len(w) + 1, i + 1)
+                                position=(idx, i + 1)
                             )
                         )
                     break
         result.sort(key=lambda x: x.position)
         return result
 
     def find_all_from_segments(self, segments: List[str]):
```

### Comparing `filedata-0.2.5/filedata.egg-info/SOURCES.txt` & `filedata-0.2.6/filedata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `filedata-0.2.5/setup.py` & `filedata-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `filedata-0.2.5/tests/test_text_algo/test_ac.py` & `filedata-0.2.6/tests/test_text_algo/test_ac.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,27 @@
 
     assert len(result) == 6
     for r in result:
         assert r.word in words
         assert content[r.position[0]:r.position[1]] == r.word
 
 
+def test_find_all_from_start():
+    words = ['测试', '方案', '测试方案', '软件']
+    content = '测试方案是用来测试软件是否正常运行的方案。'
+
+    ac = ACAutomaton(words)
+    result = ac.find_all(content, from_start=True)
+
+    assert len(result) == 2
+    for r in result:
+        assert r.word in words
+        assert content[r.position[0]:r.position[1]] == r.word
+
+
 def test_find_all2():
     words = ['软件测试方案', '测试方案', '测试', '方案', '软件测试']
     content = '这是一个软件测试方案，用来测试软件是否正常运行的方案。'
 
     ac = ACAutomaton(words)
     result = ac.find_all(content)
```

