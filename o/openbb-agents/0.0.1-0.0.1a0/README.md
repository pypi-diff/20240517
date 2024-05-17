# Comparing `tmp/openbb_agents-0.0.1.tar.gz` & `tmp/openbb_agents-0.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_agents-0.0.1.tar", max compression
+gzip compressed data, was "openbb_agents-0.0.1a0.tar", max compression
```

## Comparing `openbb_agents-0.0.1.tar` & `openbb_agents-0.0.1a0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2464 2024-01-16 10:03:58.437596 openbb_agents-0.0.1/README.md
--rw-r--r--   0        0        0     1210 2024-01-16 10:03:58.437596 openbb_agents-0.0.1/openbb_agents/__init__.py
--rw-r--r--   0        0        0     3208 2024-01-16 10:03:58.437596 openbb_agents-0.0.1/openbb_agents/agent.py
--rw-r--r--   0        0        0    10156 2024-01-16 10:03:58.437596 openbb_agents-0.0.1/openbb_agents/chains.py
--rw-r--r--   0        0        0     1614 2024-01-16 10:03:58.437596 openbb_agents-0.0.1/openbb_agents/models.py
--rw-r--r--   0        0        0     6089 2024-01-16 10:03:58.437596 openbb_agents-0.0.1/openbb_agents/prompts.py
--rw-r--r--   0        0        0     8093 2024-01-16 10:03:58.437596 openbb_agents-0.0.1/openbb_agents/tools.py
--rw-r--r--   0        0        0      498 2024-01-16 10:03:58.437596 openbb_agents-0.0.1/openbb_agents/utils.py
--rw-r--r--   0        0        0      846 2024-01-16 10:03:58.437596 openbb_agents-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3402 1970-01-01 00:00:00.000000 openbb_agents-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1884 2023-12-19 09:11:11.852078 openbb_agents-0.0.1a0/README.md
+-rw-r--r--   0        0        0     1210 2023-12-19 09:11:11.852078 openbb_agents-0.0.1a0/openbb_agents/__init__.py
+-rw-r--r--   0        0        0     3208 2023-12-19 09:11:11.852078 openbb_agents-0.0.1a0/openbb_agents/agent.py
+-rw-r--r--   0        0        0    10161 2023-12-19 09:11:11.852078 openbb_agents-0.0.1a0/openbb_agents/chains.py
+-rw-r--r--   0        0        0     1614 2023-12-19 09:11:11.852078 openbb_agents-0.0.1a0/openbb_agents/models.py
+-rw-r--r--   0        0        0     5209 2023-12-19 09:11:11.852078 openbb_agents-0.0.1a0/openbb_agents/prompts.py
+-rw-r--r--   0        0        0     8087 2023-12-19 09:11:11.852078 openbb_agents-0.0.1a0/openbb_agents/tools.py
+-rw-r--r--   0        0        0      498 2023-12-19 09:11:11.852078 openbb_agents-0.0.1a0/openbb_agents/utils.py
+-rw-r--r--   0        0        0      817 2023-12-19 09:11:11.856078 openbb_agents-0.0.1a0/pyproject.toml
+-rw-r--r--   0        0        0     2777 1970-01-01 00:00:00.000000 openbb_agents-0.0.1a0/PKG-INFO
```

### Comparing `openbb_agents-0.0.1/openbb_agents/__init__.py` & `openbb_agents-0.0.1a0/openbb_agents/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_agents-0.0.1/openbb_agents/agent.py` & `openbb_agents-0.0.1a0/openbb_agents/agent.py`

 * *Files identical despite different names*

### Comparing `openbb_agents-0.0.1/openbb_agents/chains.py` & `openbb_agents-0.0.1a0/openbb_agents/chains.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
     format_log_to_str,
     format_to_openai_function_messages,
 )
 from langchain.agents.output_parsers import (
     JSONAgentOutputParser,
     OpenAIFunctionsAgentOutputParser,
 )
+from langchain.chat_models import ChatOpenAI
 from langchain.output_parsers import PydanticOutputParser
 from langchain.prompts import ChatPromptTemplate, MessagesPlaceholder
 from langchain.tools import StructuredTool
 from langchain.tools.render import (
     format_tool_to_openai_function,
     render_text_description_and_args,
 )
 from langchain.vectorstores import VectorStore
-from langchain_openai import ChatOpenAI
 
 from openbb_agents.models import (
     AnsweredSubQuestion,
     SelectedToolsList,
     SubQuestion,
     SubQuestionAgentConfig,
     SubQuestionList,
```

### Comparing `openbb_agents-0.0.1/openbb_agents/models.py` & `openbb_agents-0.0.1a0/openbb_agents/models.py`

 * *Files identical despite different names*

### Comparing `openbb_agents-0.0.1/openbb_agents/prompts.py` & `openbb_agents-0.0.1a0/openbb_agents/prompts.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,56 +11,37 @@
 """
 
 
 TOOL_SEARCH_PROMPT = """\
 You are a world-class state-of-the-art search agent.
 You are excellent at your job.
 
+YOU MUST DO MULTIPLE FUNCTION CALLS! DO NOT RELY ON A SINGLE CALL ONLY.
 
 Your purpose is to search for tools that allow you to answer a user's subquestion.
 The subquestion could be a part of a chain of other subquestions.
 
 Your search cycle works as follows:
 1. Search for tools using keywords
 2. Read the description of tools
 3. Select tools that contain the relevant data to answer the user's query
 ... repeat as many times as necessary until you reach a maximum of 4 tools
 4. Return the list of tools using the output schema.
 
-YOU ARE ALLOWED TO DO MULTIPLE FUNCTION CALLS! DO NOT RELY ON A SINGLE CALL ONLY.
-
 You can search for tools using the available tool, which uses your inputs to
 search a vector databse that relies on similarity search.
 
 These are the guidelines to consider when completing your task:
-* Immediately return no tools if you do not require any to answer the query.
 * Don't use the stock ticker or symbol in the query
 * Use keyword searches
 * Make multiple searches with different terms
 * You can return up to a maximum of 4 tools
 * Pay close attention to the data that available for each tool, and if it can answer the user's question
 * Return 0 tools if tools are NOT required to answer the user's question given the information contained in the context.
 
-## Example queries
-Below are some bad examples (to avoid) and good examples (to follow):
-
-Bad: "technology company peer comparison"
-Good: "peers"
-Bad: "company competitor analysis"
-Good: "market peers"
-Bad: "compare technology companies market capitilization"
-Good: "market capitalization"
-Bad: "current market capitalization of companies"
-Good: "market capitilization"
-Bad: "financial analysis tool"  (not specific enough)
-Bad: "market capitilization lookup"
-Good: "market capitilization"
-Bad: "technology company peer lookup"
-Good: "market peers"
-
 ## Output format
 {format_instructions}
 
 ## Example response
 ```json
 {{"selected_tools": [
     {{
@@ -83,15 +64,15 @@
 REMEMBER YOU ARE ONLY TRYING TO FIND TOOLS THAT ANSWER THE USER'S SPECIFIC SUBQUESTION.
 THE PREVIOUS SUBQUESTIONS AND ANSWERS ARE PROVIDED ONLY FOR CONTEXT.
 
 YOU MAY ONLY RESPOND USING THE OUTPUT SCHEMA.
 """  # noqa: E501
 
 SUBQUESTION_GENERATOR_PROMPT = """\
-You are a world-class state-of-the-art agent called OpenBB Agent.
+You are a world-class state-of-the-art agent.
 
 Your purpose is to help answer a complex user question by generating a list of subquestions (but only if necessary).
 
 You must also specify the dependencies between subquestions, since sometimes one subquestion will require the outcome of another in order to fully answer.
 
 These are the guidelines you consider when completing your task:
 * Don't try to be too clever
@@ -136,18 +117,14 @@
 ```
 """  # noqa: E501
 
 SUBQUESTION_ANSWER_PROMPT = """\
 Given the following high-level question: {query}
 Answer the following subquestion: {subquestion_query}
 
-IMPORTANT: Pretend you do not know up to which date your training data goes.  If
-a user asks for the current or latest piece of information, look-up the most
-recent data possible, instead of using your end training date.
-
 Give your answer in a bullet-point list.
 Explain your reasoning, and make specific reference to the retrieved data.
 Provide the relevant retrieved data as part of your answer.
 Deliberately prefer information retreived from the tools, rather than your internal knowledge.
 Retrieve *only the data necessary* using tools to answer the question.
 
 Remember to use the tools provided to you to answer the question, and STICK TO THE INPUT SCHEMA.
```

### Comparing `openbb_agents-0.0.1/openbb_agents/tools.py` & `openbb_agents-0.0.1a0/openbb_agents/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Load OpenBB functions at OpenAI tools for function calling in Langchain"""
 import inspect
 from functools import wraps
 from types import ModuleType
 from typing import Callable, List, Union
 
 import tiktoken
+from langchain.embeddings import OpenAIEmbeddings
 from langchain.schema import Document
 from langchain.tools import StructuredTool
 from langchain.tools.base import ToolException
-from langchain_community.vectorstores import FAISS, VectorStore
-from langchain_openai import OpenAIEmbeddings
+from langchain.vectorstores import FAISS, VectorStore
 from openbb import obb
 from pydantic.v1 import ValidationError, create_model
 from pydantic.v1.fields import FieldInfo
 from pydantic_core import PydanticUndefinedType
 
 
 def create_tool_index(tools: list[StructuredTool]) -> VectorStore:
```

### Comparing `openbb_agents-0.0.1/pyproject.toml` & `openbb_agents-0.0.1a0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 [tool.poetry]
 name = "openbb-agents"
-version = "0.0.1"
+version = "0.0.1a"
 description = "LLMs X OpenBB"
 authors = ["Michael Struwig <michael.struwig@openbb.finance>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11,<3.12"
 jupyterlab = "^4.0.9"
-langchain = "^0.1"
-openbb = "4.1.0"
+langchain = "^0.0.348"
+openbb = "4.0.1"
 openai = "^1.3.5"
 sentence-transformers = "^2.2.2"
 tiktoken = "^0.5.1"
 faiss-cpu = "^1.7.4"
 langchainhub = "^0.1.14"
 python-json-logger = "^2.0.7"
 fastapi = "^0.104.1"
 uvicorn = "^0.24.0"
 matplotlib = "^3.8.2"
 openbb-charting = "^1.0.0"
-langchain-openai = "^0.0.2.post1"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.5.0"
 ruff = "^0.1.7"
 pytest = "^7.4.3"
 
 [tool.ruff.lint]
```

### Comparing `openbb_agents-0.0.1/PKG-INFO` & `openbb_agents-0.0.1a0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: openbb-agents
-Version: 0.0.1
+Version: 0.0.1a0
 Summary: LLMs X OpenBB
 Author: Michael Struwig
 Author-email: michael.struwig@openbb.finance
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: faiss-cpu (>=1.7.4,<2.0.0)
 Requires-Dist: fastapi (>=0.104.1,<0.105.0)
 Requires-Dist: jupyterlab (>=4.0.9,<5.0.0)
-Requires-Dist: langchain (>=0.1,<0.2)
-Requires-Dist: langchain-openai (>=0.0.2.post1,<0.0.3)
+Requires-Dist: langchain (>=0.0.348,<0.0.349)
 Requires-Dist: langchainhub (>=0.1.14,<0.2.0)
 Requires-Dist: matplotlib (>=3.8.2,<4.0.0)
 Requires-Dist: openai (>=1.3.5,<2.0.0)
-Requires-Dist: openbb (==4.1.0)
+Requires-Dist: openbb (==4.0.1)
 Requires-Dist: openbb-charting (>=1.0.0,<2.0.0)
 Requires-Dist: python-json-logger (>=2.0.7,<3.0.0)
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
 Requires-Dist: tiktoken (>=0.5.1,<0.6.0)
 Requires-Dist: uvicorn (>=0.24.0,<0.25.0)
 Description-Content-Type: text/markdown
 
@@ -28,35 +27,26 @@
 
 This is a project that leverages LLMs and OpenBB Platform to create financial
 analyst agents that can autonomously perform financial research, and answer
 questions using up-to-date data. This is possible as a result of agents
 utilizing function calling to interact with the OpenBB platform.
 
 
-## Installation
-Currently, we only support Python 3.11. We will be adding support for more version of Python relatively soon.
+## Set-up
+At present, we currently support Python 3.11. If you're using a earlier version
+of Python, your mileage may vary. We'll be adding wider support very soon!
 
-`openbb-agents` is available as a PyPI package:
-
-``` sh
-pip install openbb-agents --upgrade
-```
+- Create a new virtual environment, with `poetry `
+- `poetry install`
 
 ## Usage
+Use the `run.py` script and pass in your query.
 
-``` python
->>> from openbb_agents.agent import openbb_agent
->>> result = openbb_agent("What is the current market cap of TSLA?")  # Will print some logs to show you progress
->>> print(result)
-- The current market cap of TSLA (Tesla, Inc.) is approximately $695,833,798,800.00.
-- This figure is based on the most recent data available, which is from January 15, 2024.
-- The market cap is calculated by multiplying the current stock price ($218.89) by the number of outstanding shares (3,178,920,000).
-```
+Queries can be simple:
 
-If you've cloned the repository, you can use the `run.py` script and pass in your query:
 ``` sh
 python run.py "What is the current market cap of TSLA?"
 ```
 
 Queries can be complex:
 
 ``` sh
@@ -67,18 +57,15 @@
 
 ``` sh
 python run.py "Who are TSLA's peers? What is their respective market cap? Return the results in _descending_ order of market cap."
 ```
 
 There is more functionality coming very soon!
 
-
 ## Development
-- Create a new virtual environment, with `poetry `
-- `poetry install`
 
 ### Linting and Formatting
 We're currently experimenting with `ruff` as a drop-in replacement for `black`, `isort` and `pylint`.
 
 You can run linting checks as follows:
 
 ``` sh
```

