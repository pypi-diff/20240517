# Comparing `tmp/taskgen_ai-2.1.1.tar.gz` & `tmp/taskgen_ai-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskgen_ai-2.1.1.tar", last modified: Fri May 10 15:56:25 2024, max compression
+gzip compressed data, was "taskgen_ai-2.2.0.tar", last modified: Fri May 17 17:17:09 2024, max compression
```

## Comparing `taskgen_ai-2.1.1.tar` & `taskgen_ai-2.2.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-10 15:56:25.922655 taskgen_ai-2.1.1/
--rw-rw-r--   0 tanchongmin   (501) staff       (20)     1073 2024-02-26 00:45:10.000000 taskgen_ai-2.1.1/LICENSE
--rw-r--r--   0 tanchongmin   (501) staff       (20)    21666 2024-05-10 15:56:25.922048 taskgen_ai-2.1.1/PKG-INFO
--rw-rw-r--   0 tanchongmin   (501) staff       (20)    21057 2024-05-10 14:48:38.000000 taskgen_ai-2.1.1/README.md
--rw-rw-r--   0 tanchongmin   (501) staff       (20)      664 2024-05-10 14:48:40.000000 taskgen_ai-2.1.1/pyproject.toml
--rw-r--r--   0 tanchongmin   (501) staff       (20)       38 2024-05-10 15:56:25.922839 taskgen_ai-2.1.1/setup.cfg
--rw-rw-r--   0 tanchongmin   (501) staff       (20)      202 2024-05-10 15:55:09.000000 taskgen_ai-2.1.1/setup.py
-drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-10 15:56:25.917526 taskgen_ai-2.1.1/taskgen/
--rw-rw-r--   0 tanchongmin   (501) staff       (20)      213 2024-05-08 15:44:50.000000 taskgen_ai-2.1.1/taskgen/__init__.py
--rw-r--r--   0 tanchongmin   (501) staff       (20)    32850 2024-05-10 15:47:39.000000 taskgen_ai-2.1.1/taskgen/agent.py
--rw-r--r--   0 tanchongmin   (501) staff       (20)    51250 2024-05-10 15:55:08.000000 taskgen_ai-2.1.1/taskgen/base.py
-drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-10 15:56:25.921333 taskgen_ai-2.1.1/taskgen_ai.egg-info/
--rw-r--r--   0 tanchongmin   (501) staff       (20)    21666 2024-05-10 15:56:25.000000 taskgen_ai-2.1.1/taskgen_ai.egg-info/PKG-INFO
--rw-r--r--   0 tanchongmin   (501) staff       (20)      263 2024-05-10 15:56:25.000000 taskgen_ai-2.1.1/taskgen_ai.egg-info/SOURCES.txt
--rw-r--r--   0 tanchongmin   (501) staff       (20)        1 2024-05-10 15:56:25.000000 taskgen_ai-2.1.1/taskgen_ai.egg-info/dependency_links.txt
--rw-r--r--   0 tanchongmin   (501) staff       (20)       26 2024-05-10 15:56:25.000000 taskgen_ai-2.1.1/taskgen_ai.egg-info/requires.txt
--rw-r--r--   0 tanchongmin   (501) staff       (20)        8 2024-05-10 15:56:25.000000 taskgen_ai-2.1.1/taskgen_ai.egg-info/top_level.txt
+drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-17 17:17:09.323959 taskgen_ai-2.2.0/
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)     1073 2024-02-26 00:45:10.000000 taskgen_ai-2.2.0/LICENSE
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    21698 2024-05-17 17:17:09.323257 taskgen_ai-2.2.0/PKG-INFO
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)    21057 2024-05-17 17:12:55.000000 taskgen_ai-2.2.0/README.md
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)      684 2024-05-17 17:16:37.000000 taskgen_ai-2.2.0/pyproject.toml
+-rw-r--r--   0 tanchongmin   (501) staff       (20)       38 2024-05-17 17:17:09.324112 taskgen_ai-2.2.0/setup.cfg
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)      230 2024-05-17 17:16:48.000000 taskgen_ai-2.2.0/setup.py
+drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-17 17:17:09.319006 taskgen_ai-2.2.0/taskgen/
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)      237 2024-05-17 02:04:12.000000 taskgen_ai-2.2.0/taskgen/__init__.py
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    34033 2024-05-17 17:11:48.000000 taskgen_ai-2.2.0/taskgen/agent.py
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    32033 2024-05-17 09:37:37.000000 taskgen_ai-2.2.0/taskgen/base.py
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    19279 2024-05-17 05:44:25.000000 taskgen_ai-2.2.0/taskgen/function.py
+drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-17 17:17:09.322212 taskgen_ai-2.2.0/taskgen_ai.egg-info/
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    21698 2024-05-17 17:17:09.000000 taskgen_ai-2.2.0/taskgen_ai.egg-info/PKG-INFO
+-rw-r--r--   0 tanchongmin   (501) staff       (20)      283 2024-05-17 17:17:09.000000 taskgen_ai-2.2.0/taskgen_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 tanchongmin   (501) staff       (20)        1 2024-05-17 17:17:09.000000 taskgen_ai-2.2.0/taskgen_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 tanchongmin   (501) staff       (20)       43 2024-05-17 17:17:09.000000 taskgen_ai-2.2.0/taskgen_ai.egg-info/requires.txt
+-rw-r--r--   0 tanchongmin   (501) staff       (20)        8 2024-05-17 17:17:09.000000 taskgen_ai-2.2.0/taskgen_ai.egg-info/top_level.txt
```

### Comparing `taskgen_ai-2.1.1/LICENSE` & `taskgen_ai-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskgen_ai-2.1.1/PKG-INFO` & `taskgen_ai-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: taskgen-ai
-Version: 2.1.1
+Version: 2.2.0
 Summary: A Task-based agentic framework building on StrictJSON outputs by LLM agents
 Author-email: John Tan Chong Min <tanchongmin@gmail.com>
 Project-URL: Homepage, https://github.com/simbianai/taskgen
 Project-URL: Issues, https://github.com/simbianai/taskgen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.3.6
 Requires-Dist: dill>=0.3.7
+Requires-Dist: termcolor>=2.3.0
 
-# TaskGen v2.1.1
+# TaskGen v2.2.0
 ### A Task-based agentic framework building on StrictJSON outputs by LLM agents
 - Related Repositories: StrictJSON (https://github.com/tanchongmin/strictjson)
 - Video (Part 1): https://www.youtube.com/watch?v=O_XyTT7QGH4
 - Video (Part 2): https://www.youtube.com/watch?v=OWk7moRfTPE
 - TaskGen Ask Me Anything: https://www.youtube.com/watch?v=mheIWKugqF4
 
 ### Creator's Preamble
```

### Comparing `taskgen_ai-2.1.1/README.md` & `taskgen_ai-2.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# TaskGen v2.1.1
+# TaskGen v2.2.0
 ### A Task-based agentic framework building on StrictJSON outputs by LLM agents
 - Related Repositories: StrictJSON (https://github.com/tanchongmin/strictjson)
 - Video (Part 1): https://www.youtube.com/watch?v=O_XyTT7QGH4
 - Video (Part 2): https://www.youtube.com/watch?v=OWk7moRfTPE
 - TaskGen Ask Me Anything: https://www.youtube.com/watch?v=mheIWKugqF4
 
 ### Creator's Preamble
```

### Comparing `taskgen_ai-2.1.1/pyproject.toml` & `taskgen_ai-2.2.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "taskgen-ai"
-version = "2.1.1"
+version = "2.2.0"
 authors = [
   { name="John Tan Chong Min", email="tanchongmin@gmail.com" },
 ]
 description = "A Task-based agentic framework building on StrictJSON outputs by LLM agents"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = ["openai>=1.3.6", "dill>=0.3.7"]
+dependencies = ["openai>=1.3.6", "dill>=0.3.7", "termcolor>=2.3.0"]
 
 [project.urls]
 Homepage = "https://github.com/simbianai/taskgen"
 Issues = "https://github.com/simbianai/taskgen/issues"
```

### Comparing `taskgen_ai-2.1.1/taskgen/agent.py` & `taskgen_ai-2.2.0/taskgen/agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 import heapq
 import openai
 from openai import OpenAI
 import numpy as np
 import copy
 import dill as pickle
+from termcolor import colored
+
 from .base import *
+from .function import *
 
 ### Helper Functions
 def top_k_index(lst, k):
     ''' Given a list lst, find the top k indices corresponding to the top k values '''
     indexed_lst = list(enumerate(lst))
     top_k_values_with_indices = heapq.nlargest(k, indexed_lst, key=lambda x: x[1])
     top_k_indices = [index for index, _ in top_k_values_with_indices]
     return top_k_indices
 
 ### Main Classes
 class Ranker:
     ''' This defines the ranker which outputs a similarity score given a query and a key'''
-    def __init__(self, model = "text-embedding-3-small", ranking_fn = None, database = dict()):
+    def __init__(self, model = "text-embedding-3-small", ranking_fn = None, database = None):
         '''
         model: Str. The name of the model for the host
         ranking_fn: Function. If provided, this will be used to do similarity ranking instead. 
             No database storage possible when using ranking_fn as this function may not generate embeddings
         database: None / Dict (Key is str for query/key, Value is embedding in List[float])
         Takes in database (dict) of currently generated queries / keys and checks them
         so that you do not need to redo already obtained embeddings. 
         New embeddings will also be automatically stored to the database so that you do not have to redo in the future'''
         
+        if database is None:
+            database = {}
+            
         self.model = model
         self.ranking_fn = ranking_fn
         self.database = database
             
     def __call__(self, query, key) -> float:
         ''' Takes in a query and a key and outputs a similarity score 
         Inputs:
@@ -71,28 +77,37 @@
             - Example mapping: `lambda x: x.fn_description` (If x is a Class and the string you want to compare for similarity is the fn_description attribute of that class)
         - `approach`: str. Either `retrieve_by_ranker` or `retrieve_by_llm` to retrieve memory items
             - Ranker is faster and cheaper as it compares via embeddings, but are inferior to LLM-based methods for contextual information
         - `llm`: Function. The llm to use for `strict_json` llm retriever
         - `ranker`: `Ranker`. The Ranker which defines a similarity score between a query and a key. Default: OpenAI `text-embedding-3-small` model. 
             - Can be replaced with a function which returns similarity score from 0 to 1 when given a query and key
      '''
-    def __init__(self, memory: list = [], top_k: int = 3, mapper = lambda x: x, approach = 'retrieve_by_ranker', llm = None, ranker = Ranker()):
+    
+    def __init__(self, memory: list = [], top_k: int = 3, mapper = lambda x: x, approach = 'retrieve_by_ranker', llm = None, retrieve_fn = None, ranker = None):
         self.memory = memory
         self.top_k = top_k
         self.mapper = mapper
         self.approach = approach
-        self.ranker = ranker
+        if ranker is None:
+            self.ranker = Ranker()
+        else:
+            self.ranker = ranker
+        self.retrieve_fn = retrieve_fn
         self.llm = llm
         
     def retrieve(self, task: str) -> list:
         ''' Performs retrieval of top_k similar memories according to approach stated '''
-        if self.approach == 'retrieve_by_ranker':
-            return self.retrieve_by_ranker(task)
+        # if you have your own vector search function, implement it in retrieve_fn. Takes in a task and outputs the top-k results
+        if self.retrieve_fn is not None:
+            return self.retrieve_fn(task)
         else:
-            return self.retrieve_by_llm(task)
+            if self.approach == 'retrieve_by_ranker':
+                return self.retrieve_by_ranker(task)
+            else:
+                return self.retrieve_by_llm(task)
         
     def retrieve_by_ranker(self, task: str) -> list:
         ''' Performs retrieval of top_k similar memories 
         Returns the memory list items corresponding to top_k matches '''
         memory_score = [self.ranker(self.mapper(memory_chunk), task) for memory_chunk in self.memory]
         top_k_indices = top_k_index(memory_score, self.top_k)
         return [self.memory[index] for index in top_k_indices]
@@ -128,16 +143,17 @@
         ''' Returns whether or not the memory is empty '''
         return self.memory == []
     
 class Agent:
     def __init__(self, agent_name: str = 'Helpful Assistant',
                  agent_description: str = 'A generalist agent meant to help solve problems',
                  max_subtasks: int = 5,
-                 memory_bank = {'Function': Memory(top_k = 5, mapper = lambda x: x.fn_name + ': ' + x.fn_description, approach = 'retrieve_by_ranker')},
-                 shared_variables = dict(),
+                 summarise_subtasks_count: int = 3,
+                 memory_bank = None,
+                 shared_variables = None,
                  get_global_context = None,
                  default_to_llm = True,
                  verbose: bool = True,
                  debug: bool = False,
                  llm = None,
                  **kwargs):
         ''' 
@@ -146,65 +162,74 @@
         Design Philosophy:
         - Give only enough context needed to solve problem
         - Modularise components for greater accuracy of each component
         
         Inputs:
         - agent_name: String. Name of agent, hinting at what the agent does
         - agent_description: String. Short description of what the agent does
-        - max_subtasks: Int. The maximum number of subtasks the agent can have
+        - max_subtasks: Int. Default: 5. The maximum number of subtasks the agent can have
+        - summarise_subtasks_count: Int. Default: 3. The maximum number of subtasks in Subtasks Completed before summary happens
         - memory_bank: class Dict[Memory]. Stores multiple types of memory for use by the agent. Customise the Memory config within the Memory class.
             - Key: `Function` (Already Implemented Natively) - Does RAG over Task -> Function mapping
             - Can add in more keys that would fit your use case. Retrieves similar items to task / overall plan (if able) for additional context in `get_next_subtasks()` and `use_llm()` function
             - For RAG over Documents, it is best done in a function of the Agent to retrieve more information when needed (so that we do not overload the Agent with information)
-        - shared_variables. Dict. Default: empty dict. Stores the variables to be shared amongst inner functions and agents. 
+        - shared_variables. Dict. Default: None. Stores the variables to be shared amongst inner functions and agents. 
             If not empty, will pass this dictionary by reference down to the inner agents and functions
         - get_global_context. Function. Takes in self (agent variable) and returns the additional prompt (str) to be appended to `get_next_subtask` and `use_llm`. Allows for persistent agent states to be added to the prompt
         - default_to_llm. Bool. Default: True. Whether to default to use_llm function if there is no match to other functions. If False, use_llm will not be given to Agent
         - verbose: Bool. Default: True. Whether to print out intermediate thought processes of the Agent
         - debug: Bool. Default: False. Whether to debug StrictJSON messages
         - llm: Function. The llm parameter that gets passed into Function/strict_json
         
         Inputs (optional):
         - **kwargs: Dict. Additional arguments you would like to pass on to the strict_json function
         
         '''
         self.agent_name = agent_name
         self.agent_description = agent_description
         self.max_subtasks = max_subtasks
+        self.summarise_subtasks_count = summarise_subtasks_count
         self.verbose = verbose
-        self.memory_bank = memory_bank
-        self.shared_variables = shared_variables
         self.default_to_llm = default_to_llm
         self.get_global_context = get_global_context
 
         self.debug = debug
         self.llm = llm
-
+        
+        # set shared variables
+        if shared_variables is None:
+            self.shared_variables = {}
+        else:
+            self.shared_variables = shared_variables
+        # set memory bank
+        if memory_bank is None:
+            self.memory_bank = {'Function': Memory(top_k = 5, mapper = lambda x: x.fn_name + ': ' + x.fn_description, approach = 'retrieve_by_ranker')}
+            self.memory_bank['Function'].reset()
+        else:
+            self.memory_bank = memory_bank
+            
         # reset agent's state
         self.reset()
 
         self.kwargs = kwargs
 
         # start with default of only llm as the function
         self.function_map = {}
         # stores all existing function descriptions - prevent duplicate assignment of functions
         self.fn_description_list = []
         
-        # reset the memory bank
-        if 'Function' in self.memory_bank:
-            memory_bank['Function'].reset()
         # adds the use llm function
         if self.default_to_llm:
             self.assign_functions([Function(fn_name = 'use_llm', 
-                                        fn_description = f'Used only when no other function can do the task', 
+                                        fn_description = f'For general tasks. Used only when no other function can do the task', 
                                         is_compulsory = True,
                                         output_format = {"Output": "Output of LLM"})])
         # adds the end task function
         self.assign_functions([Function(fn_name = 'end_task',
-                                       fn_description = 'Use only when task is completed',
+                                       fn_description = 'Use only after task is completed',
                                        is_compulsory = True,
                                        output_format = {})])
         
     def save_agent(self, filename: str):
         ''' Saves the entire agent to filename for reuse next time '''
         
         if not isinstance(filename, str):
@@ -254,15 +279,17 @@
         If task is provided, we will filter the functions according to the task
         If you want to provide the agent with the context of functions available to it, set provide_function_list to True (default: False)
         If task is given, then we will use it to do RAG over functions'''
         
         # if we have a task to focus on, we can filter the functions (other than use_llm and end_task) by that task
         filtered_fn_list = None
         if task != '':
+            # filter the functions
             filtered_fn_list = self.memory_bank['Function'].retrieve(task)
+            
             # add back compulsory functions (default: use_llm, end_task) if present in function_map
             for name, function in self.function_map.items():
                 if function.is_compulsory:
                     filtered_fn_list.append(function)
                 
         # add in global context to the prompt
         global_context = ''
@@ -289,21 +316,22 @@
         ''' Prints prettily the update of the agent's status. 
         If you would want to reference any agent-specific variable, just do so directly without calling this function '''
         print('Agent Name:', self.agent_name)
         print('Agent Description:', self.agent_description)
         print('Available Functions:', list(self.function_map.keys()))
         if len(self.shared_variables) > 0:
             print('Shared Variables:', list(self.shared_variables.keys()))
-        print('Task:', self.task)
+        print(colored(f'Task: {self.task}', 'green', attrs = ['bold']))
         if len(self.subtasks_completed) == 0: 
-            print("Subtasks Completed: None")
+            print(colored("Subtasks Completed: None", 'blue', attrs = ['bold']))
         else:
-            print('Subtasks Completed:')
+            print(colored('Subtasks Completed:', 'black', attrs = ['bold']))
             for key, value in self.subtasks_completed.items():
-                print(f"Subtask: {key}\n{value}\n")
+                print(colored(f"Subtask: {key}", 'blue', attrs = ['bold']))
+                print(f'{value}\n')
         print('Is Task Completed:', self.task_completed)
         
     ## Functions for function calling ##
     def assign_functions(self, function_list: list):
         ''' Assigns a list of functions to be used in function_map '''
         if not isinstance(function_list, list):
             function_list = [function_list]
@@ -323,15 +351,15 @@
                 stored_fn_name += '_1'
 
             # add in the function into the function_map
             self.function_map[stored_fn_name] = function
             
             # add function's description into fn_description_list
             self.fn_description_list.append(function.fn_description)
-                                    
+                        
             # add function to memory bank for RAG over functions later on if is not a compulsory functions
             if not function.is_compulsory:
                 self.memory_bank['Function'].append(function)
             
         return self
         
     def remove_function(self, function_name: str):
@@ -379,41 +407,35 @@
              # Add in memory to the LLM
             rag_info = ''
             for name in self.memory_bank.keys():
                 # Function is done separately
                 if name == 'Function': continue
                 # Do not need to add to context if the memory item is empty
                 if self.memory_bank[name].isempty(): continue
-                rag_info += f'Related {name}: ```{self.memory_bank[name].retrieve(subtask)}```\n'
+                rag_info += f'Memory for {name}: ```{self.memory_bank[name].retrieve(subtask)}```\n'
 
-            res = self.query(query = f'{rag_info}Context:```{self.overall_task}\n{self.subtasks_completed}```\nAssigned Subtask: ```{function_params["instruction"]}```\nGenerate a response for Assigned Subtask only - do not just state what has or can be done or apologise or repeat Assigned Subtask - actually generate the outcome of Assigned Subtask fully according to your Agent Capabilities. Any mention of `use_llm` function refers to you', 
-                            output_format = {"Output": "Generate a full response to the Assigned Subtask"},
+            res = self.query(query = f'{rag_info}Subtasks Completed:```{self.subtasks_completed}```\nAssigned Subtask: ```{function_params["instruction"]}```\n\nYou are the use_llm function that generates a detailed outcome for the Assigned Subtask. You do not need to talk to the user, just give the output', 
+                            output_format = {"Output": "Your detailed outcome for Assigned Subtask"},
                             provide_function_list = False)
             
-            # res = res["Output"]
-            
             if self.verbose: 
-                print('>', res["Output"])
+                print(f"> {res['Output']}")
                 print()
             
         elif function_name == "end_task":
             return
         
         else:
             if self.verbose: 
                 print(f'Calling function {function_name} with parameters {function_params}')
                 
             res = self.function_map[function_name](**function_params, shared_variables = self.shared_variables)
-
-            # if only one Output key for the json, then omit the output key
-            # if len(res) == 1 and "Output" in res:
-            #     res = res["Output"]
             
             if self.verbose and res != '': 
-                print('>', res)
+                print(f"> {res}")
                 print()
                 
         if stateful:
             if res == '':
                 res = {'Status': 'Completed'}
             
             self.add_subtask_result(subtask, res)
@@ -435,22 +457,29 @@
         rag_info = ''
         for name in self.memory_bank.keys():
             # Function RAG is done separately in self.query()
             if name == 'Function': continue
             # Do not need to add to context if the memory item is empty
             if self.memory_bank[name].isempty(): continue
             else:
-                rag_info += f'Related {name}: ```{self.memory_bank[name].retrieve(task)}```\n'
+                rag_info += f'Memory for {name}: ```{self.memory_bank[name].retrieve(task)}```\n'
                 
         # First select the Equipped Function
-        res = self.query(query = f'''{background_info}{rag_info}\nBased on Context and Subtasks Completed, provide the Current Subtask and the corresponding Equipped Function to complete a part of Assigned Task. If Assigned Task is completed, Current Subtask is End Task and Equipped Function is end_task''',
-                         output_format = {"Thoughts": "How to complete Assigned Task, End Task if completed", "Observation": "Reflect on what has been done so far for Assigned Task", "Current Subtask": "What to do now in detail, End Task if completed", "Equipped Function": "Name of Equipped Function to use for Current Subtask, end_task if completed"},
-                         provide_function_list = True,
-                         task = task)
-        
+        res = self.query(query = f'''{background_info}{rag_info}\nBased on Context, Memory and Subtasks Completed, provide the Current Subtask and the corresponding Equipped Function to complete a part of Assigned Task''',
+         output_format = {"Observation": "Reflect on what has been done in Subtasks Completed for Assigned Task", 
+                          "Thoughts": "Brainstorm on how to complete the remainder of Assigned Task, if any, using Equipped Functions. End Task if Assigned Task completed", 
+                          "Current Subtask": "What to do now in detail that can be done by one Equipped Function for Assigned Task", 
+                          "Equipped Function": "Name of Equipped Function to use for Current Subtask"},
+         provide_function_list = True,
+         task = task)
+
+        if self.verbose:
+            print(colored(f"Observation: {res['Observation']}", 'black', attrs = ['bold']))
+            print(colored(f"Thoughts: {res['Thoughts']}", 'green', attrs = ['bold']))
+            
         # end task if equipped function is incorrect
         if res["Equipped Function"] not in self.function_map:
             res["Equipped Function"] = "end_task"
                 
         # If equipped function is use_llm, or end_task, we don't need to do another query
         cur_function = self.function_map[res["Equipped Function"]]
         
@@ -477,15 +506,15 @@
                     input_format[match] = 'A suitable value'
                     
             # if there is no input, then do not need LLM to extract out function's input
             if input_format == {}:
                 res["Equipped Function Inputs"] = {}
                     
             else:    
-                res2 = self.query(query = f'''{background_info}{rag_info}\nCurrent Subtask: {res["Current Subtask"]}\nEquipped Function Details: {str(cur_function)}\nOutput suitable values for the input parameters of the Equipped Function to fulfil Current Subtask''',
+                res2 = self.query(query = f'''{background_info}{rag_info}\n\nCurrent Subtask: {res["Current Subtask"]}\nEquipped Function Details: {str(cur_function)}\nOutput suitable values for the input parameters of the Equipped Function to fulfil Current Subtask''',
                              output_format = input_format,
                              provide_function_list = False)
                 res["Equipped Function Inputs"] = res2
             
         return res["Current Subtask"], res["Equipped Function"], res["Equipped Function Inputs"]
         
     def add_subtask_result(self, subtask, result):
@@ -570,30 +599,30 @@
             # otherwise do the task
             for i in range(num_subtasks):           
                 # Determine next subtask, or if task is complete. Always execute if it is the first subtask
                 subtask, function_name, function_params = self.get_next_subtask()
                 if function_name == 'end_task':
                     self.task_completed = True
                     if self.verbose:
+                        print(colored(f"Subtask identified: End Task", "blue", attrs=['bold']))
                         print('Task completed successfully!\n')
                     break
                     
-                if self.verbose: print('Subtask identified:', subtask)
+                if self.verbose: 
+                    print(colored(f"Subtask identified: {subtask}", "blue", attrs=['bold']))
 
                 # Execute the function for next step
                 res = self.use_function(function_name, function_params, subtask)
-                         
-            # check if overall task is complete at the last step if num_steps > 1
-            if not self.task_completed and num_subtasks > 1:
-                subtask, function_name, function_params = self.get_next_subtask()
-                if function_name == "end_task":
-                    self.task_completed = True
-                    if self.verbose:
-                        print('Task completed successfully!\n')
-
+                
+                # Summarise Subtasks Completed if necessary
+                if len(self.subtasks_completed) > self.summarise_subtasks_count:
+                    print('### Auto-summarising Subtasks Completed ###')
+                    self.summarise_subtasks_completed(f'progress for {self.overall_task}')
+                    print('### End of Auto-summary ###\n')
+          
         return list(self.subtasks_completed.values())
     
     ## This is for Multi-Agent uses
     def to_function(self, meta_agent):
         ''' Converts the agent to a function so that it can be called by another agent
         The agent will take in an instruction, and output the result after processing'''
```

### Comparing `taskgen_ai-2.1.1/taskgen/base.py` & `taskgen_ai-2.2.0/taskgen/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         else:
             thoughts, requirement_met, action_needed = '', False, res
             
     return requirement_met, action_needed
 
 def check_datatype(field, key: dict, data_type: str, **kwargs):
     ''' Ensures that output field of the key of JSON dictionary is of data_type 
-    Currently supports int, float, enum, lists and nested lists
+    Currently supports int, float, str, code, enum, lists, nested lists, dict, dict with keys
     Takes in **kwargs for the LLM model
     Returns corrected output field that matches the datatype'''
     data_type = data_type.strip()
     
     # check if we want an LLM-based correction
     if data_type.lower()[:6] == 'ensure':
         llm_check_msg = data_type[6:].strip()
@@ -143,14 +143,26 @@
         if data_type.lower() == 'str':
             try:
                 field = str(field)
             except Exception as e:
                 pass
             if not isinstance(field, str):
                 raise Exception(f'''Output field of "{key}" not of data type {data_type}. If not possible to match, output '' ''')
+        # special case of str is code, where we remove double backslashes
+        if data_type.lower() == 'code':
+            try:
+                field = str(field)
+            except Exception as e:
+                pass
+            if not isinstance(field, str):
+                raise Exception(f'''Output field of "{key}" not of data type {data_type}. If not possible to match, output '' ''')
+            # do decoding for double backslashes
+            field = bytes(field, "utf-8").decode("unicode_escape")
+            # replace aprostrophes
+            field = field.replace("â\x80\x99", "'")
                 
         # check for int
         if data_type.lower() == 'int':
             try:
                 field = int(field)
             except Exception as e:
                 pass
@@ -255,48 +267,28 @@
             
         # check that list has at least same number of elements as the input
         if len(field) < len(output_format):
             raise Exception(f'''Output "{field}" has fewer elements than required by "{output_format}". Add in more list elements.''')
         
         return [check_key(str(field[num]), output_format[num], new_output_format[num], delimiter, delimiter_num+1) for num in range(len(output_format))]
     
-    # if string, then do literal eval, then decode unicode escape characters for code to run
+    # if string, then do literal eval to convert output field for further processing
     elif isinstance(output_format, str):
         # if literal eval fails, just leave it as string, no need to raise error
         try:
             field = ast.literal_eval(field)
         except Exception as e:
             pass
-        return remove_unicode_escape(field)
+        
+        return field
     
     # otherwise just return the value
     else:
         return field
     
-def remove_unicode_escape(my_datatype):
-    ''' Removes the unicode escape character from the ending string in my_datatype (can be nested) '''
-    if isinstance(my_datatype, dict):
-        output_d = {}
-        # wrap keys with delimiters
-        for key, value in my_datatype.items():
-            output_d[key] = remove_unicode_escape(value)
-        return output_d
-    elif isinstance(my_datatype, list):
-        return [remove_unicode_escape(item) for item in my_datatype]
-    # if it is a string, remove the unicode escape characters from it, so code can be run
-    elif isinstance(my_datatype, str):
-        # only do decoding for code if backslash present
-        if '\\' in my_datatype:
-            my_datatype = bytes(my_datatype, "utf-8").decode("unicode_escape")
-        # replace aprostrophes
-        my_datatype = my_datatype.replace("â\x80\x99", "'")
-        return my_datatype
-    else:
-        return my_datatype
-    
 def wrap_with_angle_brackets(d: dict, delimiter: str, delimiter_num: int) -> dict:
     ''' Changes d to output_d by wrapping delimiters over the keys, and putting angle brackets on the values 
     Also changes all mention of `list` after type: to `array` for better processing '''
     if isinstance(d, dict):
         output_d = {}
         # wrap keys with delimiters
         for key, value in d.items():
@@ -327,16 +319,15 @@
     - llm: User-made llm function.
         - Inputs:
             - system_prompt: String. Write in whatever you want the LLM to become. e.g. "You are a \<purpose in life\>"
             - user_prompt: String. The user input. Later, when we use it as a function, this is the function input
         - Output:
             - res: String. The response of the LLM call
     - **kwargs: Dict. Additional arguments for LLM chat
-    
-    TODO: Incorporate other open-sourced LLMs in the future'''
+    '''
     if llm is not None:
         ''' If you specified your own LLM, then we just feed in the system and user prompt 
         LLM function should take in system prompt (str) and user prompt (str), and output a response (str) '''
         res = llm(system_prompt = system_prompt, user_prompt = user_prompt)
     
     ## This part here is for llms that are OpenAI based
     elif host == 'openai':
@@ -379,16 +370,15 @@
     - llm: User-made llm function.
         - Inputs:
             - system_prompt: String. Write in whatever you want the LLM to become. e.g. "You are a \<purpose in life\>"
             - user_prompt: String. The user input. Later, when we use it as a function, this is the function input
         - Output:
             - res: String. The response of the LLM call
     - **kwargs: Dict. Additional arguments for LLM chat
-    
-    TODO: Incorporate other open-sourced LLMs in the future'''
+    '''
     if llm_async is not None:
         ''' If you specified your own LLM, then we just feed in the system and user prompt 
         LLM function should take in system prompt (str) and user prompt (str), and output a response (str) '''
         res = await llm_async(system_prompt = system_prompt, user_prompt = user_prompt)
     
     ## This part here is for llms that are OpenAI based
     elif host == 'openai':
@@ -415,115 +405,18 @@
     if verbose:
         print('System prompt:', system_prompt)
         print('\nUser prompt:', user_prompt)
         print('\nGPT response:', res)
             
     return res
 
-def get_clean_typename(typ) -> str:
-    """Returns a clean, readable name for a type, including handling generics."""
-    if hasattr(typ, '__origin__'):  # Check for generic types
-        if typ.__origin__ is not None:  # Generic types, e.g., List, Dict
-            base_name = typ.__origin__.__name__
-            if hasattr(typ, '__args__') and typ.__args__ is not None:
-                args = [get_clean_typename(arg) for arg in typ.__args__]
-                return f"{base_name}[{', '.join(args)}]"
-            else:
-                return base_name  # Handle cases like `Dict` without specified parameters
-        else:  # Non-generic but special types, e.g., typing.List without parameters
-            return typ._name if hasattr(typ, '_name') else str(typ)
-    elif hasattr(typ, '__name__'):
-        return typ.__name__  # Simple types, e.g., int, str
-    else:
-        return str(typ)  # Fallback, should rarely be used
-
-def get_fn_description(my_function) -> (str, list):
-    ''' Returns the modified docstring of my_function, that takes into account input variable names and types in angle brackets
-    Also returns the list of input parameters to the function in sequence
-    e.g.: Adds numbers x and y -> Adds numbers <x: int> and <y: int>
-    Input variables that are optional (already assigned a default value) need not be in the docstring
-    args and kwargs variables are not parsed '''
-     
-    if not inspect.isfunction(my_function):
-        raise Exception(f'{my_function} is not a Python function')
-        
-    # Get the signature and type hints of the function
-    # if my_function.__doc__ == None:
-    #     return '', []
-
-    signature = inspect.signature(my_function)
-    full_type_hints = get_type_hints(my_function)
-    my_fn_description = my_function.__doc__ if my_function.__doc__ else ''
-
-    param_list = []
-    # Access parameters and their types
-    parameters = signature.parameters
-    for param_name, param in parameters.items():
-        # skip args and kwargs and shared variables
-        if param_name in ['shared_variables', 'args', 'kwargs']:
-            continue
-        
-        param_type = param.annotation.__name__ if param.annotation != inspect.Parameter.empty else "unannotated"
-        # Handle specific typing
-        if param_name in full_type_hints:
-            param_type = get_clean_typename(full_type_hints[param_name])
-
-        # Create new_param representation
-        new_param = f'<{param_name}: {param_type}>' if param_type != "unannotated" else f'<{param_name}>'
-
-        # Pattern to find the parameter in the docstring
-        pattern = re.compile(fr'\b({param_name})\b')
-        
-        # Substitute the parameter in the docstring
-        if pattern.search(my_fn_description):
-            my_fn_description = pattern.sub(new_param, my_fn_description)
-            param_list.append(param_name)
-            
-        # otherwise, function description will just be the function signature
-        else:
-            # add a continuation if description is current empty
-            if my_fn_description != '':
-                my_fn_description += ', '
-                
-            param_list.append(param_name)
-            print(f'Input variable "{param_name}" not in docstring of "{my_function.__name__}". Adding it to docstring')
-            my_fn_description += f'Input: {new_param}'
-            
-            if param.default != inspect.Parameter.empty:
-                my_fn_description += f', default: {param.default}'
-
-    return my_fn_description, param_list
-
-def get_fn_output(my_function) -> dict:
-    ''' Returns the dictionary of output parameters and types of the form {"Output 1": "Type", "Output 2": "Type"}'''
-     
-    if not inspect.isfunction(my_function):
-        raise Exception(f'{my_function} is not a Python function')
-        
-    # Initialize the output format dictionary
-    output_format = {}
-
-    full_type_hints = get_type_hints(my_function)
-    my_fn_description = my_function.__doc__
-
-    # Check for return annotation
-    if 'return' in full_type_hints:
-        return_type = full_type_hints['return']
-        # Adjust dictionary according to the return type
-        if isinstance(return_type, tuple):
-            for idx, type_hint in enumerate(return_type):
-                output_format[f"output_{idx + 1}"] = get_clean_typename(type_hint)
-        else:
-            output_format["output_1"] = get_clean_typename(return_type)
 
-    return output_format
 
 ### Main Functions ###
-                
-def strict_json(system_prompt: str, user_prompt: str, output_format: dict, return_as_json = False, custom_checks: dict = dict(), check_data = None, delimiter: str = '###', num_tries: int = 3, openai_json_mode: bool = False, **kwargs):
+def strict_json(system_prompt: str, user_prompt: str, output_format: dict, return_as_json = False, custom_checks: dict = None, check_data = None, delimiter: str = '###', num_tries: int = 3, openai_json_mode: bool = False, **kwargs):
     ''' Ensures that OpenAI will always adhere to the desired output JSON format defined in output_format. 
     Uses rule-based iterative feedback to ask GPT to self-correct.
     Keeps trying up to num_tries it it does not. Returns empty JSON if unable to after num_tries iterations.
     
     Inputs (compulsory):
     - system_prompt: String. Write in whatever you want GPT to become. e.g. "You are a \<purpose in life\>"
     - user_prompt: String. The user input. Later, when we use it as a function, this is the function input
@@ -537,14 +430,18 @@
     - num_tries: Integer (default: 3). The number of tries to iteratively prompt GPT to generate correct json format
     - openai_json_mode: Boolean (default: False). Whether or not to use OpenAI JSON Mode
     - **kwargs: Dict. Additional arguments for LLM chat
     
     Output:
     - res: Dict. The JSON output of the model. Returns {} if JSON parsing failed.
     '''
+    # default initialise custom_checks to {}
+    if custom_checks is None:
+        custom_checks = {}
+        
     # If OpenAI JSON mode is selected, then just let OpenAI do the processing
     if openai_json_mode:
         # add in code to warn user if type is defined for external function
         type_check = False
         for value in output_format.values():
             if 'type:' in str(value):
                 type_check = True
@@ -619,15 +516,15 @@
                 error_msg = f"\n\nPrevious json: {res}\njson error: {str(e)}\nFix the error."                
                 print("An exception occurred:", str(e))
                 print("Current invalid json format:", res)
 
         return {}
     
     
-async def strict_json_async(system_prompt: str, user_prompt: str, output_format: dict, return_as_json = False, custom_checks: dict = dict(), check_data = None, delimiter: str = '###', num_tries: int = 3, openai_json_mode: bool = False, **kwargs):
+async def strict_json_async(system_prompt: str, user_prompt: str, output_format: dict, return_as_json = False, custom_checks: dict = None, check_data = None, delimiter: str = '###', num_tries: int = 3, openai_json_mode: bool = False, **kwargs):
     ''' Ensures that OpenAI will always adhere to the desired output JSON format defined in output_format. 
     Uses rule-based iterative feedback to ask GPT to self-correct.
     Keeps trying up to num_tries it it does not. Returns empty JSON if unable to after num_tries iterations.
     
     Inputs (compulsory):
     - system_prompt: String. Write in whatever you want GPT to become. e.g. "You are a \<purpose in life\>"
     - user_prompt: String. The user input. Later, when we use it as a function, this is the function input
@@ -641,14 +538,18 @@
     - num_tries: Integer (default: 3). The number of tries to iteratively prompt GPT to generate correct json format
     - openai_json_mode: Boolean (default: False). Whether or not to use OpenAI JSON Mode
     - **kwargs: Dict. Additional arguments for LLM chat
     
     Output:
     - res: Dict. The JSON output of the model. Returns {} if JSON parsing failed.
     '''
+    # default initialise custom_checks to {}
+    if custom_checks is None:
+        custom_checks = {}
+        
     # If OpenAI JSON mode is selected, then just let OpenAI do the processing
     if openai_json_mode:
         # add in code to warn user if type is defined for external function
         type_check = False
         for value in output_format.values():
             if 'type:' in str(value):
                 type_check = True
@@ -722,288 +623,11 @@
             except Exception as e:
                 error_msg = f"\n\nPrevious json: {res}\njson error: {str(e)}\nFix the error."                
                 print("An exception occurred:", str(e))
                 print("Current invalid json format:", res)
 
         return {}
 
-class Function:
-    def __init__(self,
-                 fn_description: str = '', 
-                 output_format: dict = {},
-                 examples = None,
-                 external_fn = None,
-                 is_compulsory = False,
-                 fn_name = None,
-                 llm = None,
-                 llm_async = None,
-                 **kwargs):
-        ''' 
-        Creates an LLM-based function or wraps an external function using fn_description and outputs JSON based on output_format. 
-        (Optional) Can define the function based on examples (list of Dict containing input and output variables for each example)
-        (Optional) If you would like greater specificity in your function's input, you can describe the variable after the : in the input variable name, e.g. `<var1: an integer from 10 to 30`. Here, `var1` is the input variable and `an integer from 10 to 30` is the description.
-        
-        Inputs (primary):
-        - fn_description: String. Function description to describe process of transforming input variables to output variables. Variables must be enclosed in <> and listed in order of appearance in function input.
-Can also be done automatically by providing docstring with input variable names in external_fn
-        - output_format: Dict. Dictionary containing output variables names and description for each variable.
-           
-        Inputs (optional):
-        - examples: Dict or List[Dict]. Examples in Dictionary form with the input and output variables (list if more than one)
-        - external_fn: Python Function. If defined, instead of using LLM to process the function, we will run the external function. 
-            If there are multiple outputs of this function, we will map it to the keys of `output_format` in a one-to-one fashion
-        - is_compulsory: Bool. Default: False. This is whether to always use the Function when doing planning in Agents
-        - fn_name: String. If provided, this will be the name of the function. Otherwise, if `external_fn` is provided, it will be the name of `external_fn`. Otherwise, we will use LLM to generate a function name from the `fn_description`
-        - llm: Function. The llm parameter to pass into strict_json
-        - **kwargs: Dict. Additional arguments you would like to pass on to the strict_json function
-        
-        ## Example
-        fn_description = 'Output the sum of <num1> and <num2>'
-        output_format = {'output': 'sum of two numbers'}
-        examples = [{'num1': 5, 'num2': 6, 'output': 11}, {'num1': 2, 'num2': 4, 'output': 6}]
-        '''
-        
-        self.fn_description = ''
-        self.output_format = {}
-        
-        # this is only for external functions
-        self.external_param_list = [] 
-        if external_fn is not None:
-            # add in code to warn user if type is defined for external function
-            type_check = False
-            for value in output_format.values():
-                if 'type:' in str(value):
-                    type_check = True
-            if type_check:
-                print('Note: Type checking (type:) not done for External Functions')
-            
-            # get details from docstring of external function only if fn_description is not given
-            if fn_description == '':
-                self.fn_description, self.external_param_list = get_fn_description(external_fn)
-            
-            # get the output format from the function signature if output format is not given
-            if output_format == {}:
-                self.output_format = get_fn_output(external_fn)             
-            
-        # if function description provided, use it to update the function description
-        if fn_description != '':
-            self.fn_description = fn_description
-
-        # if output format is provided, use it to update the function output format
-        if output_format != {}:
-            self.output_format = output_format
-            
-        self.examples = examples
-        self.external_fn = external_fn
-        self.is_compulsory = is_compulsory
-        self.fn_name = fn_name
-        self.llm = llm
-        self.llm_async = llm_async
-        self.kwargs = kwargs
-        
-        self.variable_names = []
-        self.shared_variable_names = []
-        # use regex to extract variables from function description
-        matches = re.findall(r'<(.*?)>', self.fn_description)
-            
-        for match in matches:
-            first_half = match.split(':')[0]
-            if first_half not in self.variable_names:
-                # if the first two characters of variable are s_, means take from shared_variables
-                if first_half[:2] != 's_':
-                    self.variable_names.append(first_half)
-                # otherwise we take from shared_variables
-                else:
-                    self.shared_variable_names.append(first_half)
-                    # replace the original variable without the <> so as not to confuse the LLM
-                    self.fn_description = self.fn_description.replace(f'<{match}>', first_half)
-                    
-        # make it such that we follow the same order for variable names as per the external function only if there are external function params
-        if self.external_param_list != []:
-            self.variable_names = [x for x in self.external_param_list if x in self.variable_names]
-                
-        # generate function name if not defined
-        if self.fn_name is None:
-            # if external function has a name, use it
-            if self.external_fn is not None and hasattr(self.external_fn, '__name__') and self.external_fn.__name__ != '<lambda>':
-                self.fn_name = self.external_fn.__name__
-            # otherwise, generate name out
-            else:
-                res = strict_json(system_prompt = "Output a function name to summarise the usage of this function.",
-                                  user_prompt = str(self.fn_description),
-                                  output_format = {"Thoughts": "What function does", "Name": "Function name with _ separating words that summarises what function does"},
-                                 llm = self.llm,
-                                 **self.kwargs)
-                self.fn_name = res['Name']
-                
-        # change instance's name to function's name
-        self.__name__ = self.fn_name
-
-        # Append examples to description
-        if self.examples is not None:
-            self.fn_description += '\nExamples:\n' + str(examples)
-      
-    def __str__(self):
-        ''' Prints out the function's parameters '''
-        return f'Description: {self.fn_description}\nInput: {self.variable_names}\nOutput: {self.output_format}\n'
-        
-    def __call__(self, *args, **kwargs):
-        ''' Describes the function, and inputs the relevant parameters as either unnamed variables (args) or named variables (kwargs)
-        
-        Inputs:
-        - shared_varables: Dict. Default: empty dict. The variables which will be shared between functions. Only passed in if required by function 
-        - *args: Tuple. Unnamed input variables of the function. Will be processed to var1, var2 and so on based on order in the tuple
-        - **kwargs: Dict. Named input variables of the function. Can also be variables to pass into strict_json
-        
-        Output:
-        - res: Dict. JSON containing the output variables'''
-        
-        # get the shared_variables if there are any
-        shared_variables = kwargs.get('shared_variables', {})
-        # remove the mention of shared_variables in kwargs
-        if 'shared_variables' in kwargs:
-            del kwargs['shared_variables']
-        
-        # extract out only variables listed in variable_list from kwargs
-        function_kwargs = {my_key: kwargs[my_key] for my_key in kwargs if my_key in self.variable_names}
-        # additionally, if function references something in shared_variables, add that in
-        for variable in self.shared_variable_names:
-            if variable in shared_variables:
-                function_kwargs[variable] = shared_variables[variable]
-        
-        # extract out only variables not listed in variable list
-        strict_json_kwargs = {my_key: kwargs[my_key] for my_key in kwargs if my_key not in self.variable_names}
-        
-        # Do the auto-naming of variables as var1, var2, or as variable names defined in variable_names
-        for num, arg in enumerate(args):
-            if len(self.variable_names) > num:
-                function_kwargs[self.variable_names[num]] = arg
-            else:
-                function_kwargs['var'+str(num+1)] = arg
-                
-        # If strict_json function, do the function. 
-        if self.external_fn is None:
-            res = strict_json(system_prompt = self.fn_description,
-                            user_prompt = function_kwargs,
-                            output_format = self.output_format,
-                            llm = self.llm,
-                            **self.kwargs, **strict_json_kwargs)
-            
-        # Else run the external function
-        else:
-            res = {}
-            # if external function uses shared_variables, pass it in
-            argspec = inspect.getfullargspec(self.external_fn)
-            if 'shared_variables' in argspec.args:
-                fn_output = self.external_fn(shared_variables = shared_variables, **function_kwargs)
-            else:
-                fn_output = self.external_fn(**function_kwargs)
-                
-            # if there is nothing in fn_output, skip this part
-            if fn_output is not None:
-                output_keys = list(self.output_format.keys())
-                # convert the external function into a tuple format to parse it through the JSON dictionary output format
-                if not isinstance(fn_output, tuple):
-                    fn_output = [fn_output]
-
-                for i in range(len(fn_output)):
-                    if len(output_keys) > i:
-                        res[output_keys[i]] = fn_output[i]
-                    else:
-                        res[f'output_{i+1}'] = fn_output[i]
-        
-        # check if any of the output variables have a s_, which means we update the shared_variables and not output it
-        keys = list(res.keys())
-        for each in keys:
-            if each[:2] == 's_':
-                shared_variables[each] = res[each]
-                del res[each]
-                
-        if res == {}:
-            res = {'Status': 'Completed'}
-
-        return res
-    
-    async def async_call(self, *args, **kwargs):
-        ''' Describes the function, and inputs the relevant parameters as either unnamed variables (args) or named variables (kwargs)
-        
-        Inputs:
-        - shared_varables: Dict. Default: empty dict. The variables which will be shared between functions. Only passed in if required by function 
-        - *args: Tuple. Unnamed input variables of the function. Will be processed to var1, var2 and so on based on order in the tuple
-        - **kwargs: Dict. Named input variables of the function. Can also be variables to pass into strict_json
-        
-        Output:
-        - res: Dict. JSON containing the output variables'''
-        
-        # get the shared_variables if there are any
-        shared_variables = kwargs.get('shared_variables', {})
-        # remove the mention of shared_variables in kwargs
-        if 'shared_variables' in kwargs:
-            del kwargs['shared_variables']
-        
-        # extract out only variables listed in variable_list from kwargs
-        function_kwargs = {my_key: kwargs[my_key] for my_key in kwargs if my_key in self.variable_names}
-        # additionally, if function references something in shared_variables, add that in
-        for variable in self.shared_variable_names:
-            if variable in shared_variables:
-                function_kwargs[variable] = shared_variables[variable]
-        
-        # extract out only variables not listed in variable list
-        strict_json_kwargs = {my_key: kwargs[my_key] for my_key in kwargs if my_key not in self.variable_names}
-        
-        # Do the auto-naming of variables as var1, var2, or as variable names defined in variable_names
-        for num, arg in enumerate(args):
-            if len(self.variable_names) > num:
-                function_kwargs[self.variable_names[num]] = arg
-            else:
-                function_kwargs['var'+str(num+1)] = arg
-                
-        # If strict_json function, do the function. 
-        if self.external_fn is None:
-            res = await strict_json_async(system_prompt = self.fn_description,
-                            user_prompt = function_kwargs,
-                            output_format = self.output_format,
-                            llm_async = self.llm_async,
-                            **self.kwargs, **strict_json_kwargs)
-            
-        # Else run the external function
-        else:
-            res = {}
-            # if external function uses shared_variables, pass it in
-            argspec = inspect.getfullargspec(self.external_fn)
-            if 'shared_variables' in argspec.args:
-                fn_output = self.external_fn(shared_variables = shared_variables, **function_kwargs)
-            else:
-                fn_output = self.external_fn(**function_kwargs)
-                
-            # if there is nothing in fn_output, skip this part
-            if fn_output is not None:
-                output_keys = list(self.output_format.keys())
-                # convert the external function into a tuple format to parse it through the JSON dictionary output format
-                if not isinstance(fn_output, tuple):
-                    fn_output = [fn_output]
-
-                for i in range(len(fn_output)):
-                    if len(output_keys) > i:
-                        res[output_keys[i]] = fn_output[i]
-                    else:
-                        res[f'output_{i+1}'] = fn_output[i]
-        
-        # check if any of the output variables have a s_, which means we update the shared_variables and not output it
-        keys = list(res.keys())
-        for each in keys:
-            if each[:2] == 's_':
-                shared_variables[each] = res[each]
-                del res[each]
-                
-        if res == {}:
-            res = {'Status': 'Completed'}
-
-        return res
-    
 ### Legacy Support ###
 # alternative names for strict_json
 strict_text = strict_json
-strict_output = strict_json
-
-# alternative name for strict_function (it is now called Function)
-strict_function = Function
+strict_output = strict_json
```

### Comparing `taskgen_ai-2.1.1/taskgen_ai.egg-info/PKG-INFO` & `taskgen_ai-2.2.0/taskgen_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: taskgen-ai
-Version: 2.1.1
+Version: 2.2.0
 Summary: A Task-based agentic framework building on StrictJSON outputs by LLM agents
 Author-email: John Tan Chong Min <tanchongmin@gmail.com>
 Project-URL: Homepage, https://github.com/simbianai/taskgen
 Project-URL: Issues, https://github.com/simbianai/taskgen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.3.6
 Requires-Dist: dill>=0.3.7
+Requires-Dist: termcolor>=2.3.0
 
-# TaskGen v2.1.1
+# TaskGen v2.2.0
 ### A Task-based agentic framework building on StrictJSON outputs by LLM agents
 - Related Repositories: StrictJSON (https://github.com/tanchongmin/strictjson)
 - Video (Part 1): https://www.youtube.com/watch?v=O_XyTT7QGH4
 - Video (Part 2): https://www.youtube.com/watch?v=OWk7moRfTPE
 - TaskGen Ask Me Anything: https://www.youtube.com/watch?v=mheIWKugqF4
 
 ### Creator's Preamble
```

