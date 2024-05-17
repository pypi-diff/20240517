# Comparing `tmp/textlong-0.1.1.tar.gz` & `tmp/textlong-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textlong-0.1.1.tar", max compression
+gzip compressed data, was "textlong-0.1.2.tar", max compression
```

## Comparing `textlong-0.1.1.tar` & `textlong-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1066 2024-05-17 12:44:59.600013 textlong-0.1.1/LICENSE
--rw-r--r--   0        0        0      888 2024-05-17 12:49:54.271837 textlong-0.1.1/README.md
--rw-r--r--   0        0        0      890 2024-05-17 12:50:26.007061 textlong-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-17 12:44:59.600533 textlong-0.1.1/textlong/.pypirc
--rw-r--r--   0        0        0      974 2024-05-17 12:44:59.600747 textlong-0.1.1/textlong/__init__.py
--rw-r--r--   0        0        0       22 2024-05-17 12:44:59.600866 textlong-0.1.1/textlong/__version__.py
--rw-r--r--   0        0        0        0 2024-05-17 12:44:59.601026 textlong-0.1.1/textlong/agents/__init__.py
--rw-r--r--   0        0        0     2722 2024-05-17 12:44:59.601163 textlong-0.1.1/textlong/agents/base.py
--rw-r--r--   0        0        0     7036 2024-05-17 12:44:59.601410 textlong-0.1.1/textlong/agents/prompt.py
--rw-r--r--   0        0        0     4988 2024-05-17 12:44:59.601632 textlong-0.1.1/textlong/ai.py
--rw-r--r--   0        0        0     6780 2024-05-17 12:44:59.601940 textlong-0.1.1/textlong/base.py
--rw-r--r--   0        0        0     2442 2024-05-17 12:44:59.602176 textlong-0.1.1/textlong/command.py
--rw-r--r--   0        0        0        0 2024-05-17 12:44:59.602426 textlong-0.1.1/textlong/document_loaders/__init__.py
--rw-r--r--   0        0        0     8955 2024-05-17 12:44:59.602748 textlong-0.1.1/textlong/document_loaders/base.py
--rw-r--r--   0        0        0       57 2024-05-17 12:44:59.602930 textlong-0.1.1/textlong/langgraph/__init__.py
--rw-r--r--   0        0        0     5269 2024-05-17 12:44:59.603160 textlong-0.1.1/textlong/langgraph/tools_calling.py
--rw-r--r--   0        0        0       77 2024-05-17 12:44:59.603326 textlong-0.1.1/textlong/memory/__init__.py
--rw-r--r--   0        0        0    10213 2024-05-17 12:44:59.603589 textlong-0.1.1/textlong/memory/base.py
--rw-r--r--   0        0        0     3839 2024-05-17 12:44:59.603829 textlong-0.1.1/textlong/memory/history.py
--rw-r--r--   0        0        0     3131 2024-05-17 12:44:59.603975 textlong-0.1.1/textlong/memory/memory_manager.py
--rw-r--r--   0        0        0     8962 2024-05-17 12:44:59.604170 textlong-0.1.1/textlong/node.py
--rw-r--r--   0        0        0      936 2024-05-17 12:44:59.604351 textlong-0.1.1/textlong/prompts/main.py
--rw-r--r--   0        0        0     3314 2024-05-17 12:44:59.604491 textlong-0.1.1/textlong/prompts/task_prompt.py
--rw-r--r--   0        0        0      385 2024-05-17 12:44:59.604603 textlong-0.1.1/textlong/prompts/translate.py
--rw-r--r--   0        0        0        0 2024-05-17 12:44:59.604711 textlong-0.1.1/textlong/retrievers/__init__.py
--rw-r--r--   0        0        0     2999 2024-05-17 12:44:59.604917 textlong-0.1.1/textlong/retrievers/base.py
--rw-r--r--   0        0        0     3141 2024-05-17 12:44:59.605124 textlong-0.1.1/textlong/serialize.py
--rw-r--r--   0        0        0     1949 2024-05-17 12:44:59.605319 textlong-0.1.1/textlong/state.py
--rw-r--r--   0        0        0     2406 2024-05-17 12:44:59.605464 textlong-0.1.1/textlong/task.py
--rw-r--r--   0        0        0     1824 2024-05-17 12:44:59.605581 textlong-0.1.1/textlong/tree.py
--rw-r--r--   0        0        0     1839 1970-01-01 00:00:00.000000 textlong-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-17 12:44:59.600013 textlong-0.1.2/LICENSE
+-rw-r--r--   0        0        0      938 2024-05-17 12:53:58.250212 textlong-0.1.2/README.md
+-rw-r--r--   0        0        0      880 2024-05-17 15:02:21.088990 textlong-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-17 12:44:59.600533 textlong-0.1.2/textlong/.pypirc
+-rw-r--r--   0        0        0      848 2024-05-17 14:19:13.587368 textlong-0.1.2/textlong/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-17 15:02:16.813315 textlong-0.1.2/textlong/__version__.py
+-rw-r--r--   0        0        0        0 2024-05-17 12:44:59.601026 textlong-0.1.2/textlong/agents/__init__.py
+-rw-r--r--   0        0        0     2722 2024-05-17 12:44:59.601163 textlong-0.1.2/textlong/agents/base.py
+-rw-r--r--   0        0        0     7036 2024-05-17 12:44:59.601410 textlong-0.1.2/textlong/agents/prompt.py
+-rw-r--r--   0        0        0     4988 2024-05-17 12:44:59.601632 textlong-0.1.2/textlong/ai.py
+-rw-r--r--   0        0        0     6780 2024-05-17 12:44:59.601940 textlong-0.1.2/textlong/base.py
+-rw-r--r--   0        0        0     2442 2024-05-17 12:44:59.602176 textlong-0.1.2/textlong/command.py
+-rw-r--r--   0        0        0        0 2024-05-17 12:44:59.602426 textlong-0.1.2/textlong/document_loaders/__init__.py
+-rw-r--r--   0        0        0     8955 2024-05-17 12:44:59.602748 textlong-0.1.2/textlong/document_loaders/base.py
+-rw-r--r--   0        0        0       57 2024-05-17 12:44:59.602930 textlong-0.1.2/textlong/langgraph/__init__.py
+-rw-r--r--   0        0        0     5269 2024-05-17 12:44:59.603160 textlong-0.1.2/textlong/langgraph/tools_calling.py
+-rw-r--r--   0        0        0       77 2024-05-17 12:44:59.603326 textlong-0.1.2/textlong/memory/__init__.py
+-rw-r--r--   0        0        0    10213 2024-05-17 12:44:59.603589 textlong-0.1.2/textlong/memory/base.py
+-rw-r--r--   0        0        0     3839 2024-05-17 12:44:59.603829 textlong-0.1.2/textlong/memory/history.py
+-rw-r--r--   0        0        0     3131 2024-05-17 12:44:59.603975 textlong-0.1.2/textlong/memory/memory_manager.py
+-rw-r--r--   0        0        0     9410 2024-05-17 14:58:44.781290 textlong-0.1.2/textlong/node.py
+-rw-r--r--   0        0        0      936 2024-05-17 12:44:59.604351 textlong-0.1.2/textlong/prompts/main.py
+-rw-r--r--   0        0        0     3314 2024-05-17 12:44:59.604491 textlong-0.1.2/textlong/prompts/task_prompt.py
+-rw-r--r--   0        0        0      385 2024-05-17 12:44:59.604603 textlong-0.1.2/textlong/prompts/translate.py
+-rw-r--r--   0        0        0        0 2024-05-17 12:44:59.604711 textlong-0.1.2/textlong/retrievers/__init__.py
+-rw-r--r--   0        0        0     2999 2024-05-17 12:44:59.604917 textlong-0.1.2/textlong/retrievers/base.py
+-rw-r--r--   0        0        0     3141 2024-05-17 13:56:55.783580 textlong-0.1.2/textlong/serialize.py
+-rw-r--r--   0        0        0     1949 2024-05-17 12:44:59.605319 textlong-0.1.2/textlong/state.py
+-rw-r--r--   0        0        0     2406 2024-05-17 12:44:59.605464 textlong-0.1.2/textlong/task.py
+-rw-r--r--   0        0        0     2003 2024-05-17 15:01:02.849565 textlong-0.1.2/textlong/tree.py
+-rw-r--r--   0        0        0     1839 1970-01-01 00:00:00.000000 textlong-0.1.2/PKG-INFO
```

### Comparing `textlong-0.1.1/LICENSE` & `textlong-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `textlong-0.1.1/README.md` & `textlong-0.1.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# 🦜🇨🇳 LangChain-Chinese
+# 🦜🦜🦜 textlong
 [![PyPI version](https://img.shields.io/pypi/v/textlong.svg)](https://pypi.org/project/textlong/)
 
 **textlong** 的目标是基于大语言模型提供结构化的长文本生成能力。
 
 ## 一、安装
 
 你可以使用 pip 安装：
@@ -16,15 +16,15 @@
 ```
 
 ## 二、结构化长文生成能力
 
 `textlong` 中提供如下结构化长文档的创作模式：
 
 - 一键直出：输入写作要求后，由AI直接创作
-- （其他模式正在研发中，请参考路线图说明 roadmap.md）
+- （其他模式正在研发中，请参考路线图说明 [路线图](https://github.com/arcstep/textlong/blob/main/roadmap.md)）
 
 **应用示范：**
 
 ```python
 import os
 from dotenv import load_dotenv, find_dotenv
 load_dotenv(find_dotenv(), override=True)
```

### Comparing `textlong-0.1.1/pyproject.toml` & `textlong-0.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "textlong"
-version = "0.1.1"
-description = "A framework designed to produce extensive texts utilizing GPT or other large language models."
+version = "0.1.2"
+description = "A framework designed to produce long-texts with GPT or other large language models."
 authors = ["arcstep <43801@qq.com>"]
 homepage = "https://github.com/arcstep/textlong"
 repository = "https://github.com/arcstep/textlong.git"
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
-asyncio = "^3.4.3"
 pydantic = ">=1,<3"
 langchain = "^0.1.20"
 langchain-community = "^0.0.38"
 python-dotenv = "^1.0.1"
 python-statemachine = "^2.2.0"
 pydot = "^2.0.0"
 
 [tool.poetry.group.dev.dependencies]
+asyncio = "^3.4.3"
 setuptools = "^69.1.0"
 poetry2setup = "^1.1.0"
 ipykernel = "^6.29.2"
 pytest = "^8.0.1"
 pydantic = "1.10.13"
 docx2txt = "^0.8"
 pypdf = "^4.1.0"
```

### Comparing `textlong-0.1.1/textlong/agents/base.py` & `textlong-0.1.2/textlong/agents/base.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.1/textlong/agents/prompt.py` & `textlong-0.1.2/textlong/agents/prompt.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.1/textlong/ai.py` & `textlong-0.1.2/textlong/ai.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.1/textlong/base.py` & `textlong-0.1.2/textlong/base.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.1/textlong/command.py` & `textlong-0.1.2/textlong/command.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.1/textlong/document_loaders/base.py` & `textlong-0.1.2/textlong/document_loaders/base.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.1/textlong/langgraph/tools_calling.py` & `textlong-0.1.2/textlong/langgraph/tools_calling.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.1/textlong/memory/base.py` & `textlong-0.1.2/textlong/memory/base.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.1/textlong/memory/history.py` & `textlong-0.1.2/textlong/memory/history.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.1/textlong/memory/memory_manager.py` & `textlong-0.1.2/textlong/memory/memory_manager.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.1/textlong/node.py` & `textlong-0.1.2/textlong/node.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         words_limit: int=500,
         words_advice: int=None,
         title: str=None,
         howto: str=None,
         summarise: str=None,
         text: str=None,
         last_ai_reply_json: Dict[str, Any]={},
+        is_draft=False,
         **kwargs,
     ):
         ContentState.__init__(self)
         ContentSerialize.__init__(self, **kwargs)
 
         self.type = type
 
@@ -41,16 +42,15 @@
 
         # 段落
         self.summarise = summarise
         self.text = text
 
         # 最后的AI回复
         self.last_ai_reply_json = last_ai_reply_json
-
-        self.is_draft: bool = False
+        self.is_draft: bool = is_draft
         self.ai = BaseAI()
 
     howto_commands = ["title", "words_advice", "howto"]
     result_commands = ["summarise", "text"]
     state_commands = ["state", "memory", "ok", "todo", "modi", "task"]
 
     # inherit
@@ -124,15 +124,15 @@
         elif self.state == "todo":
             prompt = self.ai.prompt_todo(
                 title=self.title,
                 content_type=self.type,
                 words_limit=self.words_limit,
                 words_advice=self.words_advice,
                 howto=self.howto,
-                outline_exist=self.root.all_outlines
+                outline_exist=self.root.get_outlines()
             )
 
         else:
             raise NotImplementedError(f"<{self.id}> 对象在状态[{self.state}]没有指定提示语模板")
 
         chain = self.ai.get_chain(prompt)
         json = self.ai.ask_ai(task or default_task, chain, return_json=True)
@@ -173,19 +173,28 @@
             if self.type == "outline":
                 # 删除旧的子项，逐个添加新的子项
                 self._children = {}
                 self.reply_json_validator(self.last_ai_reply_json, ["大纲列表"])
 
                 for item in self.last_ai_reply_json['大纲列表']:
                     self.reply_json_validator(item, ["标题名称", "总字数要求", "扩写指南"])
-                    self.add_item(
-                        item_class=ContentNode,
+                    words_advice = item["总字数要求"]
+                    type = "outline" if words_advice > self.words_limit else "paragraph"
+                    title = item["标题名称"]
+                    howto = item["扩写指南"]
+                    node = self.add_item(
+                        type=type,
+                        title=title,
+                        howto=howto,
+                        words_advice=words_advice,
                         last_ai_reply_json=item,
-                        is_draft=True
+                        is_draft=False,
+                        item_class=ContentNode,
                     )
+                    node.edit()
 
             elif self.type == "paragraph":
                 self.reply_json_validator(self.last_ai_reply_json, ["内容摘要", "详细内容"])
                 self.summarise = self.last_ai_reply_json["内容摘要"]
                 self.text = self.last_ai_reply_json["详细内容"]
 
             else:
@@ -246,23 +255,21 @@
             "words_advice": self.words_advice,
             "title": self.title or "",
             "howto": self.howto or "",
             "summarise": self.summarise or None,
             "text": self.text or "",
         }
 
-    @property
-    def all_outlines(self) -> List[Dict[str, Union[str, int]]]:
+    def get_outlines(self) -> List[Dict[str, Union[str, int]]]:
         """获得大纲清单"""
         outlines = [
             f"{x['id']} {x['title']} \n  扩写指南 >>> {x['howto']}\n  内容摘要 >>> {x['summarise']}"
             for x in self.all_content
         ]
         return '\n'.join(outlines)
 
-    @property
-    def all_text(self):
+    def get_texts(self):
         outlines = [
             f"{x['id']} {x['title']} \n {x['text']}"
             for x in self.all_content
         ]
         return '\n'.join(outlines)
```

### Comparing `textlong-0.1.1/textlong/prompts/main.py` & `textlong-0.1.2/textlong/prompts/main.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.1/textlong/prompts/task_prompt.py` & `textlong-0.1.2/textlong/prompts/task_prompt.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.1/textlong/retrievers/base.py` & `textlong-0.1.2/textlong/retrievers/base.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.1/textlong/serialize.py` & `textlong-0.1.2/textlong/serialize.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.1/textlong/state.py` & `textlong-0.1.2/textlong/state.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.1/textlong/task.py` & `textlong-0.1.2/textlong/task.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.1/textlong/tree.py` & `textlong-0.1.2/textlong/tree.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     @property
     def default_command(self) -> str:
         return self.todo_node.default_command
 
     # inherit
     @property
     def commands(self) -> List[str]:
-        return ["move", "todo", "draft", "all"] + self.todo_node.commands
+        return ["move", "todo", "draft", "outlines", "nodes", "texts"] + self.todo_node.commands
 
     # inherit
     def call(self, command, args, **kwargs):
         if command == 'move' and args:
             # 转移到新的指定对象
             obj = self.root.get_item_by_id(args)
             self.todo_node = obj or self.todo_node
@@ -51,12 +51,16 @@
             if not self.todo_node.is_draft:
                 obj = self.root.find_draft_node()
                 if obj:
                     self.todo_node = obj
             else:
                 obj = self.todo_node
             return obj.id if obj else None
-        elif command == "all":
+        elif command == "nodes":
             return self.root.all_content
+        elif command == "outlines":
+            return self.root.get_outlines()
+        elif command == "texts":
+            return self.root.get_texts()
         else:
             return self.todo_node.call(command, args, **kwargs)
```

### Comparing `textlong-0.1.1/PKG-INFO` & `textlong-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: textlong
-Version: 0.1.1
-Summary: A framework designed to produce extensive texts utilizing GPT or other large language models.
+Version: 0.1.2
+Summary: A framework designed to produce long-texts with GPT or other large language models.
 Home-page: https://github.com/arcstep/textlong
 License: MIT
 Author: arcstep
 Author-email: 43801@qq.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: langchain (>=0.1.20,<0.2.0)
 Requires-Dist: langchain-community (>=0.0.38,<0.0.39)
 Requires-Dist: pydantic (>=1,<3)
 Requires-Dist: pydot (>=2.0.0,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: python-statemachine (>=2.2.0,<3.0.0)
 Project-URL: Repository, https://github.com/arcstep/textlong.git
 Description-Content-Type: text/markdown
 
-# 🦜🇨🇳 LangChain-Chinese
+# 🦜🦜🦜 textlong
 [![PyPI version](https://img.shields.io/pypi/v/textlong.svg)](https://pypi.org/project/textlong/)
 
 **textlong** 的目标是基于大语言模型提供结构化的长文本生成能力。
 
 ## 一、安装
 
 你可以使用 pip 安装：
@@ -40,15 +39,15 @@
 ```
 
 ## 二、结构化长文生成能力
 
 `textlong` 中提供如下结构化长文档的创作模式：
 
 - 一键直出：输入写作要求后，由AI直接创作
-- （其他模式正在研发中，请参考路线图说明 roadmap.md）
+- （其他模式正在研发中，请参考路线图说明 [路线图](https://github.com/arcstep/textlong/blob/main/roadmap.md)）
 
 **应用示范：**
 
 ```python
 import os
 from dotenv import load_dotenv, find_dotenv
 load_dotenv(find_dotenv(), override=True)
```

