# Comparing `tmp/mdxcanvas-0.1.7.tar.gz` & `tmp/mdxcanvas-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdxcanvas-0.1.7.tar", max compression
+gzip compressed data, was "mdxcanvas-0.1.9.tar", max compression
```

## Comparing `mdxcanvas-0.1.7.tar` & `mdxcanvas-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1065 2023-08-18 21:11:52.811761 mdxcanvas-0.1.7/LICENSE
--rw-r--r--   0        0        0      156 2024-02-22 01:16:53.597390 mdxcanvas-0.1.7/mdxcanvas/__init__.py
--rw-r--r--   0        0        0    23994 2024-05-10 18:37:50.963637 mdxcanvas-0.1.7/mdxcanvas/canvas_creator.py
--rw-r--r--   0        0        0     1053 2024-05-10 18:35:51.774805 mdxcanvas-0.1.7/mdxcanvas/deploy.py
--rw-r--r--   0        0        0     3393 2024-05-03 23:06:22.147341 mdxcanvas-0.1.7/mdxcanvas/document_schema.py
--rw-r--r--   0        0        0     2381 2024-05-10 18:37:50.964019 mdxcanvas-0.1.7/mdxcanvas/extensions.py
--rw-r--r--   0        0        0     2689 2024-05-01 19:18:15.400257 mdxcanvas-0.1.7/mdxcanvas/jinja_parser.py
--rw-r--r--   0        0        0    25647 2024-05-10 18:35:51.775044 mdxcanvas-0.1.7/mdxcanvas/parser.py
--rw-r--r--   0        0        0      559 2024-04-16 18:49:19.290278 mdxcanvas-0.1.7/mdxcanvas/question_schema.py
--rw-r--r--   0        0        0     1878 2024-04-16 18:48:46.610576 mdxcanvas-0.1.7/mdxcanvas/templating.py
--rw-r--r--   0        0        0    15263 2024-05-03 23:06:22.147893 mdxcanvas-0.1.7/mdxcanvas/yaml_parser.py
--rw-r--r--   0        0        0      651 2024-05-10 18:37:50.964243 mdxcanvas-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 mdxcanvas-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-18 21:11:52.811761 mdxcanvas-0.1.9/LICENSE
+-rw-r--r--   0        0        0      156 2024-02-22 01:16:53.597390 mdxcanvas-0.1.9/mdxcanvas/__init__.py
+-rw-r--r--   0        0        0    24001 2024-05-17 17:52:45.112664 mdxcanvas-0.1.9/mdxcanvas/canvas_creator.py
+-rw-r--r--   0        0        0     1053 2024-05-10 18:35:51.774805 mdxcanvas-0.1.9/mdxcanvas/deploy.py
+-rw-r--r--   0        0        0     3393 2024-05-03 23:06:22.147341 mdxcanvas-0.1.9/mdxcanvas/document_schema.py
+-rw-r--r--   0        0        0     2381 2024-05-17 17:52:45.113016 mdxcanvas-0.1.9/mdxcanvas/extensions.py
+-rw-r--r--   0        0        0     2689 2024-05-01 19:18:15.400257 mdxcanvas-0.1.9/mdxcanvas/jinja_parser.py
+-rw-r--r--   0        0        0    25520 2024-05-17 17:52:47.600436 mdxcanvas-0.1.9/mdxcanvas/parser.py
+-rw-r--r--   0        0        0      559 2024-04-16 18:49:19.290278 mdxcanvas-0.1.9/mdxcanvas/question_schema.py
+-rw-r--r--   0        0        0     1878 2024-04-16 18:48:46.610576 mdxcanvas-0.1.9/mdxcanvas/templating.py
+-rw-r--r--   0        0        0    15263 2024-05-03 23:06:22.147893 mdxcanvas-0.1.9/mdxcanvas/yaml_parser.py
+-rw-r--r--   0        0        0      651 2024-05-17 17:52:47.601034 mdxcanvas-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 mdxcanvas-0.1.9/PKG-INFO
```

### Comparing `mdxcanvas-0.1.7/LICENSE` & `mdxcanvas-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.7/mdxcanvas/canvas_creator.py` & `mdxcanvas-0.1.9/mdxcanvas/canvas_creator.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 def get_canvas_folder(course: Course, folder_name: str, parent_folder_path="") -> Folder:
     """
     Retrieves an object representing a digital folder in Canvas. If the folder does not exist, it is created.
     """
     folders = list(course.get_folders())
     if not any(fl.name == folder_name for fl in folders):
         print(f"Created {folder_name} folder")
-        course.create_folder(name=folder_name, parent_folder_path=parent_folder_path, hidden=True)
+        return course.create_folder(name=folder_name, parent_folder_path=parent_folder_path, hidden=True)
     matches = [fl for fl in folders if fl.name == folder_name]
     return matches[0]
 
 
 def create_resource_folder(course, quiz_title: str, course_folders):
     """
     Creates a folder in Canvas to store images and other resources.
```

### Comparing `mdxcanvas-0.1.7/mdxcanvas/deploy.py` & `mdxcanvas-0.1.9/mdxcanvas/deploy.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.7/mdxcanvas/document_schema.py` & `mdxcanvas-0.1.9/mdxcanvas/document_schema.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.7/mdxcanvas/extensions.py` & `mdxcanvas-0.1.9/mdxcanvas/extensions.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.7/mdxcanvas/jinja_parser.py` & `mdxcanvas-0.1.9/mdxcanvas/jinja_parser.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.7/mdxcanvas/parser.py` & `mdxcanvas-0.1.9/mdxcanvas/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,42 +20,41 @@
         if isinstance(value, dict):
             new_list.append((key, order_elements(value)))
         else:
             new_list.append((key, value))
     return OrderedDict(sorted(element.items(), key=lambda x: x[0]))
 
 
-def get_corrects_and_incorrects(question_tag):
-    corrects = question_tag.css.filter('correct')
-    incorrects = question_tag.css.filter('incorrect')
-    return corrects, incorrects
+def get_corrects(question_tag):
+    corrects = question_tag.select('correct')
+    return corrects
 
 
 def get_correct_comments(question_tag):
-    feedback = question_tag.css.filter('correct-comments')
+    feedback = question_tag.select('correct-comments')
     return get_text_contents(feedback[0]) if feedback else None
 
 
 def get_incorrect_comments(question_tag):
-    feedback = question_tag.css.filter('incorrect-comments')
+    feedback = question_tag.select('incorrect-comments')
     return get_text_contents(feedback[0]) if feedback else None
 
 
 def get_points(question_tag, default=1):
     points = question_tag.get("points", default)
     try:
         return int(points)
     except ValueError:
         print("Invalid points value: " + points)
         return default
 
 
 def get_answers(question_tag):
-    corrects, incorrects = get_corrects_and_incorrects(question_tag)
-    return corrects + incorrects
+    return question_tag.select('correct, incorrect')
+
 
 
 def string_is_date(date: str):
     # For templating. The string might not be a date yet.
     # Once the template arguments are filled in, we will apply make_iso.
     if date.startswith("{") or "due" in date.lower() or "lock" in date.lower():
         return False
@@ -185,15 +184,15 @@
 
 
 class TrueFalseProcessor:
     @staticmethod
     def process(question_tag, markdown_processor: ResourceExtractor):
         answers = get_answers(question_tag)
 
-        check_correct_size(answers, 1, "True/False")
+        check_answer_size(answers, 1, "True/False question must have exactly 1 answer!")
 
         question, resources = process(TFConverter(), answers[0], markdown_processor)
         if not get_points(answers[0], 0):
             points = get_points(question_tag)
             question["points_possible"] = points
         if not question["correct_comments"]:
             question["correct_comments"] = get_correct_comments(question_tag)
@@ -214,32 +213,32 @@
         for answer in get_answers(question_tag):
             tf_question, res = process(TFConverter(), answer, markdown_processor)
             questions.append(tf_question)
             resources.extend(res)
         return questions, resources
 
 
-def check_correct_size(corrects: list, num, question_type):
-    if num is not None and len(corrects) != num:
-        raise Exception(f"{question_type} must have exactly {num} correct answer(s)\n"
-                        "Answers: " + str(corrects))
+def check_answer_size(answers: list, num, explanation):
+    if num is not None and len(answers) != num:
+        raise Exception(f"{explanation}\n"
+                        "Answers: " + str(answers))
 
 
 class MultipleCommonProcessor:
     question_type: str
     num_correct: Union[int, None]
 
     def process(self, question_tag, markdown_processor: ResourceExtractor):
-        corrects, incorrects = get_corrects_and_incorrects(question_tag)
-        check_correct_size(corrects, self.num_correct, self.question_type)
+        corrects = get_corrects(question_tag)
+        check_answer_size(corrects, self.num_correct, f"{self.question_type} questions must have exactly {self.num_correct} correct answer!")
 
         question_text, resources = markdown_processor(
             get_text_contents(question_tag, ["correct", "incorrect", "correct-comments", "incorrect-comments"]))
         answers = []
-        for answer in corrects + incorrects:
+        for answer in get_answers(question_tag):
             answer_html, res = markdown_processor(get_text_contents(answer))
             answers.append((True if answer in corrects else False, answer_html))
             resources.extend(res)
 
         question = {
             "question_text": question_text,
             "question_type": self.question_type,
@@ -271,21 +270,21 @@
     def process(self, question_tag, markdown_processor: ResourceExtractor):
         return super().process(question_tag, markdown_processor)
 
 
 class MatchingProcessor:
     @staticmethod
     def process(question_tag, markdown_processor: ResourceExtractor):
-        pairs = question_tag.css.filter('pair')
+        pairs = question_tag.select('pair')
         matches = []
         for pair in pairs:
-            answer_left, answer_right = pair.css.filter('left')[0], pair.css.filter('right')[0]
+            answer_left, answer_right = pair.select('left')[0], pair.select('right')[0]
             matches.append((answer_left.string.strip(), answer_right.string.strip()))
 
-        distractors = question_tag.css.filter('distractors')
+        distractors = question_tag.select('distractors')
         distractor_text = get_text_contents(distractors[0]).strip() if len(distractors) > 0 else None
         question_text, resources = markdown_processor(
             get_text_contents(question_tag, ["pair", "correct-comments", "incorrect-comments"]))
         question = {
             "question_text": question_text,
             "question_type": 'matching_question',
             "points_possible": get_points(question_tag),
```

### Comparing `mdxcanvas-0.1.7/mdxcanvas/question_schema.py` & `mdxcanvas-0.1.9/mdxcanvas/question_schema.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.7/mdxcanvas/templating.py` & `mdxcanvas-0.1.9/mdxcanvas/templating.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.7/mdxcanvas/yaml_parser.py` & `mdxcanvas-0.1.9/mdxcanvas/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.7/pyproject.toml` & `mdxcanvas-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mdxcanvas"
-version = "0.1.7"
+version = "0.1.9"
 description = "A Canvas LMS API wrapper for maintaining content in markdown"
 authors = ["Gordon Bean <gbean@cs.byu.edu>", "Preston Raab <phr23@byu.edu>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Jinja2 = "^3.1.2"
```

### Comparing `mdxcanvas-0.1.7/PKG-INFO` & `mdxcanvas-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdxcanvas
-Version: 0.1.7
+Version: 0.1.9
 Summary: A Canvas LMS API wrapper for maintaining content in markdown
 License: MIT
 Author: Gordon Bean
 Author-email: gbean@cs.byu.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

