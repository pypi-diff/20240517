# Comparing `tmp/reverse_engineering_assistant-2.9.1.tar.gz` & `tmp/reverse_engineering_assistant-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reverse_engineering_assistant-2.9.1.tar", last modified: Mon May  6 02:46:43 2024, max compression
+gzip compressed data, was "reverse_engineering_assistant-2.9.2.tar", last modified: Fri May 17 09:50:00 2024, max compression
```

## Comparing `reverse_engineering_assistant-2.9.1.tar` & `reverse_engineering_assistant-2.9.2.tar`

### file list

```diff
@@ -1,28 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:46:43.562110 reverse_engineering_assistant-2.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-05-06 02:46:43.562110 reverse_engineering_assistant-2.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-05-06 02:46:37.000000 reverse_engineering_assistant-2.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-06 02:46:37.000000 reverse_engineering_assistant-2.9.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:46:43.558109 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-06 02:46:37.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 02:46:37.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:46:43.562110 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/api_server_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-06 02:46:37.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/api_server_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-06 02:46:37.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/api_server_tools/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-05-06 02:46:37.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/api_server_tools/llm_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-05-06 02:46:37.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/api_server_tools/re_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    16481 2024-05-06 02:46:37.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-06 02:46:37.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/assistant_api_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-05-06 02:46:37.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/chat_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-05-06 02:46:37.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8935 2024-05-06 02:46:37.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/documents.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-06 02:46:37.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-06 02:46:37.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/reva_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-06 02:46:37.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:46:43.562110 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-05-06 02:46:43.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-06 02:46:43.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 02:46:43.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-06 02:46:43.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-06 02:46:43.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-06 02:46:43.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 02:46:43.562110 reverse_engineering_assistant-2.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:50:00.615731 reverse_engineering_assistant-2.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-05-17 09:50:00.611731 reverse_engineering_assistant-2.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-05-17 09:49:36.000000 reverse_engineering_assistant-2.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-17 09:49:36.000000 reverse_engineering_assistant-2.9.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:50:00.603731 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-17 09:49:36.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:49:36.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:50:00.607731 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/api_server_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-17 09:49:36.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/api_server_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-17 09:49:36.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/api_server_tools/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5764 2024-05-17 09:49:36.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/api_server_tools/llm_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19725 2024-05-17 09:49:36.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/api_server_tools/re_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15411 2024-05-17 09:49:36.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-05-17 09:49:36.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/assistant_api_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8780 2024-05-17 09:49:36.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/chat_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8935 2024-05-17 09:49:36.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-17 09:49:36.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:50:00.611731 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-17 09:49:57.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/protocol/RevaChat_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-17 09:49:57.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/protocol/RevaChat_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-05-17 09:49:57.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/protocol/RevaChat_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-17 09:49:57.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/protocol/RevaComment_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-17 09:49:57.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/protocol/RevaComment_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-05-17 09:49:57.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/protocol/RevaComment_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-17 09:49:57.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/protocol/RevaData_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-17 09:49:57.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/protocol/RevaData_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-05-17 09:49:57.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/protocol/RevaData_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-17 09:49:57.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/protocol/RevaGetCursor_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-17 09:49:57.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/protocol/RevaGetCursor_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-17 09:49:57.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/protocol/RevaGetCursor_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-17 09:49:57.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/protocol/RevaGetDecompilation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-05-17 09:49:57.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/protocol/RevaGetDecompilation_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-05-17 09:49:57.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/protocol/RevaGetDecompilation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-17 09:49:57.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/protocol/RevaGetReferences_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-17 09:49:57.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/protocol/RevaGetReferences_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-17 09:49:57.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/protocol/RevaGetReferences_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-17 09:49:57.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/protocol/RevaGetSymbols_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-17 09:49:57.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/protocol/RevaGetSymbols_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9971 2024-05-17 09:49:57.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/protocol/RevaGetSymbols_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-17 09:49:57.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/protocol/RevaHandshake_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-17 09:49:57.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/protocol/RevaHandshake_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-17 09:49:57.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/protocol/RevaHandshake_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-17 09:49:57.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/protocol/RevaHeartbeat_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-17 09:49:57.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/protocol/RevaHeartbeat_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-17 09:49:57.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/protocol/RevaHeartbeat_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-17 09:49:57.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/protocol/RevaVariable_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-17 09:49:57.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/protocol/RevaVariable_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-17 09:49:57.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/protocol/RevaVariable_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:49:40.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-17 09:49:36.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/reva_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-17 09:49:36.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:50:00.611731 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-05-17 09:50:00.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-17 09:50:00.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 09:50:00.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-17 09:50:00.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-17 09:50:00.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-17 09:50:00.000000 reverse_engineering_assistant-2.9.2/reverse_engineering_assistant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 09:50:00.615731 reverse_engineering_assistant-2.9.2/setup.cfg
```

### Comparing `reverse_engineering_assistant-2.9.1/PKG-INFO` & `reverse_engineering_assistant-2.9.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: reverse-engineering-assistant
-Version: 2.9.1
-Summary: An AI assistant for reverse engineering tasks
-Author: サイバーカイダ (cyberkaida)
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Description-Content-Type: text/markdown
-Requires-Dist: langchain
-Requires-Dist: langchain-core
-Requires-Dist: langchain-openai
-Requires-Dist: prompt_toolkit
-Requires-Dist: sentence_transformers
-Requires-Dist: PyYAML
-Requires-Dist: pydantic
-Requires-Dist: rich
-Requires-Dist: grpcio
-Requires-Dist: protobuf
-
 # ReVA - Reverse Engineering Assistant
 
 > Updated demo coming soon!
 
 The reverse engineering assistant (ReVA) is a project to build a disassembler agnostic AI assistant for
 reverse engineering tasks. This includes both _offline_ and online inference and a simple architecture.
 
@@ -42,21 +21,22 @@
 is a small nudge to make the LLM explore the binary in the same way a human would.
 
 Using this technique you can ask general questions and get relevant answers. The model prioritises
 information from the tools, but when there is no information it can still respond to generic
 questions from its training.
 
 You can ask questions like:
+- What are the interesting strings in this program?
 - Does this program use encryption? Write a markdown report on the encryption and where it is used.
 - Draw a class diagram using plantuml syntax.
 - Start from main, examine the program in detail. Rename variables as you go and provide a summary of the program.
 - Explain the purpose of the `__mod_init` segment.
 - What does `mmap` return?
 - What does the function at address 0x80000 do?
-- This is a CTF problem. Start at main, examine the program in detail and write a pwntools script to get the flag.
+- This is a CTF problem. Write a pwntools script to get the flag.
 
 An important part of reverse engineering is the process. Many other tools simply ask a single question of the LLM,
 this means it is difficult to determine _why_ a thing happened. In ReVa we break all actions down into small parts
 and include the LLMs thoughts in the output. This allows the analyst to monitor the LLMs actions and reasoning, aborting
 and changing the prompt if required.
 
 ## Large Language Model Support
@@ -64,41 +44,48 @@
 RevA is based on [langchain](https://langchain.com),
 which supports a number of models.
 
 Built in support is provided for:
 - [OpenAI](https://platform.openai.com/overview) for online inference and easy setup (Needs an OpenAI API key)
 - [Ollama](https://ollama.ai) and any model it supports for local on-device inference or connecting to a self hosted remote inference server.
 
+See [Configuration](#configuration) for more information about settings for the providers.
+
 Adding additional inference servers is easy if it is supported by langchain.
 
 ## Configuration
 
-> This is currently being moved to the Ghidra GUI
-> See Edit -> Tool Options -> ReVa in the Codebrowser Tool
+Configuration for ReVa is in the CodeBrowser Tool options.
+Open a program and go to Edit -> Tool Options -> ReVa.
+
+There are options for:
+- Selecting a provider (OpenAI or Ollama, others coming soon!)
+- Enabling "Follow", this will move the Ghidra view to the location of
+things ReVa is examining or changing.
+- Enabling "Auto-allow", ReVa will log her actions for the user to accept
+in the "ReVa Actions Log" window.
+
+There are sections for the providers.
+
+### OpenAI
+
+By default, the OpenAI key is loaded from the environment variable `OPENAI_API_KEY`. You can also set your key inside Ghidra. Setting the key back to the `OPENAI_API_KEY` value will clear the key from the Ghidra configuration and load it from the environment.
+
+You can also select the model. By default `gpt-4o` is selected. This model works best with the tools and the prompt provided by ReVa.
+
+`gpt-4` also works well, but is slow and needs more prompting by the user to explore a binary.
+
+### Ollama
 
-Configuration for the reverse engineering assistant is stored at
-`~/.config/reverse-engineering-assistant/config.yaml`. If this
-is not present on first start, a default configuration using
-OpenAI for inference and the `OPENAI_API_TOKEN` environment
-variable will be used.
-
-The most important setting is the `type` top level setting.
-This controls what inference service you use. These are the
-same as the configuration keys, for example to use Ollama,
-set type to `ollama` and configure the settings in the `ollama:`
-section.
-
-The configuration also contains the prompts used for the models.
-If you use Ollama or OpenAI these will be processed to fit the
-model specific prompt pattern (placing the system prompt in the
-correct tags, etc).
-
-For `llama-cpp` and `text-generation-webui` these may need to be
-configured for your specific model. For this reason Ollama is
-preferred for self hosting.
+Ollama is a local inference server. The default server is set to localhost, with the default Ollama port. You can change this to a remote server if you want to perform inference on a remote machine. This is useful for organisations that self host.
+
+You can also select a model. The model must alread be loaded on the server. Good performance has been seen with:
+- `mixtral`
+- `llama3`
+- `phi`
 
 ## Workflow
 
 RevA has a two step workflow.
 1. Open your RE tool and the program you want to examine
 2. Open the chat session.
 
@@ -108,57 +95,86 @@
 To ask questions and run the inference a command line tool is provided. Run `reva-chat` to begin the chat session. This command will find your open Ghidra
 and connect to it. To open a new chat, run the command again in another terminal.
 
 If you have more than one Ghidra open, you can select the right one with
 `reva-chat --project ${project-name}`, if it is not set, `reva-chat` will
 ask you which project you want to connect to.
 
-## Installation
+## Protocol Build
+
+To communicate between `reva-server` and the extension, [gRPC](https://grpc.io) is used. You can read more about that (here)[./DEVELOPER.md]. Building the source files from those protocol definitions is driven from the [Makefile](/Makefile). To build the protocol source code files, run this command in the project's root:
 
-First install the python component, I like to use `pipx`. It is best to make
-sure that `reva-server` and `reva-chat` are on your path.
-The Ghidra extension will need to start `reva-server`, and you will need to
-run `reva-chat`.
+```sh
+make protocol
+```
 
-To install the particular extension for your disassembler see:
-- [Ghidra Support](#ghidra-support)
+## Python Project (reva-server and reva-chat) Installation
 
-The chat can be started with:
+First install the python component, I like to use `pipx`. Install it with something like:
 
 ```sh
-reva-chat
+pip install pipx
 ```
 
-> You can also configure the path to `reva-server` in `Edit -> Tool Options -> ReVa`
-> if it is not on your path. But you really should put it on your path!
+In the `reverse-engineering-assistant` folder, run:
+
+```sh
+pipx install .
+```
+
+After installing the python project, pipx may warn you that you need to add a folder to your PATH environment variable. Make sure that the folder (now containing `reva-server` and `reva-chat`) are in your PATH variable. pipx can do it for you with this command:
+
+```sh
+pipx ensurepath
+```
+
+The extension will need to start `reva-server`, and you will need to run `reva-chat`. In case you do not want to add them to your PATH, see the [Configuration](#configuration) section for how to set the path to the executables.
+
+Once the `reva-server` has been started by the extension the chat can be started with:
+
+```sh
+reva-chat
+```
 
 # Ghidra Support
 
 ## Usage
 
 > The Python package must be installed for the Ghidra extension to work!
 
 Follow the instructions in the [ghidra-assistant](ghidra-assistant/README.md) plugin.
 
-After installation, enable the `ReVaPlugin` extension in the CodeBrowser tool (Open a file and click: File -> Configure -> Miscellaneous).
+After installation, enable the `ReVa Plugin` extension in the CodeBrowser tool (Open a file and click: File -> Configure -> Miscellaneous).
 
 If you want ReVa enabled by default, click File -> Save Tool to save the configuration.
 
 If everything is working correctly you will see a ReVa menu on your menu bar.
 
+## Configuration
+
+You can modify the plugin configuration in `Edit -> Tool Options -> ReVa`.
+
 ## Undo
 
 Whenever ReVa performs an action it will create an undo point for each action. If ReVa renames 5 variables, this will be
 one undo.
 
 ## Menus
 
-> These are being added in the next release
+ReVa adds an option to the CodeBrowser Tool's Window menu.
+Select Window -> ReVa Action Log to open the ReVa Action Log window.
+
+This window shows actions ReVa has performed and would like to perform.
+You can accept or reject a change by double clicking the ✅ or ❌ icon. You can also go to the location the action will be performed by double clicking the address.
+
+If you reject an action, ReVa will be told and she will move on.
+
+You can also enable "Auto-allow" in the ReVa options. This will automatically accept all actions ReVa wants to perform.
 
-ReVa adds some elements to the Ghidra UI. You can either ask ReVa to do something in the chat window,
+ReVa also adds some elements to the Ghidra UI. You can either ask ReVa to do something in the chat window,
 "Examine the variable usage in `main` in detail, rename the variables with more descriptive names.",
 or use the menu system.
 
 For example you can right click a variable in the decompilation, select Reva -> Rename variable and ReVa
 will perform the action.
 
 # Support
```

### Comparing `reverse_engineering_assistant-2.9.1/pyproject.toml` & `reverse_engineering_assistant-2.9.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "reverse-engineering-assistant"
 readme = "README.md"
-version = "2.9.1"
+version = "2.9.2"
 authors = [
     {name="サイバーカイダ (cyberkaida)"},
 ]
 description = "An AI assistant for reverse engineering tasks"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
 ]
 dependencies = [
     "langchain",
     "langchain-core",
     "langchain-openai",
+    "langchain-community",
     "prompt_toolkit",
     "sentence_transformers",
     "PyYAML",
     "pydantic",
     "rich",
     "grpcio",
     "protobuf",
+    "flask",
 ]
 
 [project.scripts]
 reva-server = "reverse_engineering_assistant.assistant_api_server:main"
-reva-chat = "reverse_engineering_assistant.chat_client:main"
+reva-chat = "reverse_engineering_assistant.chat_client:main"
```

### Comparing `reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/api_server_tools/connection.py` & `reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/api_server_tools/connection.py`

 * *Files identical despite different names*

### Comparing `reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/api_server_tools/llm_tools.py` & `reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/api_server_tools/llm_tools.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 
 
 from ast import Call
 import queue
 import threading
-from typing import Callable
+from typing import Callable, Dict, Optional
 from venv import logger
 
 from ..protocol.RevaChat_pb2_grpc import RevaChatServiceServicer
 from ..protocol.RevaChat_pb2 import RevaChatMessageResponse
 
 from functools import cache
 from ..assistant import ReverseEngineeringAssistant
 
 import logging
 module_logger = logging.getLogger("reva-server")
 
 from langchain_core.callbacks.base import BaseCallbackHandler
 from langchain_core.agents import AgentAction, AgentFinish
 
+from langchain_core.language_models.base import BaseLanguageModel
+from langchain_core.language_models.chat_models import BaseChatModel
+
 class RevaActionCollector(BaseCallbackHandler):
     """
     A callback handler for logging agent actions in the reverse engineering assistant.
 
     This class logs agent actions and calls a callback. This is what prints the green
     thoughts from the model to the console. This is very useful for the analyst to understand
     what the model is doing (and is arguably the most important part of the assistant output!)
@@ -53,18 +56,25 @@
         # TODO: Should this be AgentAction?
         # TODO: Is `.action` still a thing?
         self.callback(str(action.log))
 
 
 class RevaChat(RevaChatServiceServicer):
     logger = logging.getLogger("reva-server.RevaChat")
+    llm: BaseLanguageModel | BaseChatModel
+
+    def __init__(self, llm: BaseLanguageModel | BaseChatModel) -> None:
+        self.llm = llm
 
     def chat(self, request, context):
         self.logger.info(f"Received request: {request}")
-        assistant = ReverseEngineeringAssistant(request.project, langchain_callbacks=[RevaActionCollector(callback)])
+        assistant = ReverseEngineeringAssistant(
+            request.project,
+            model=self.llm
+        )
         self.logger.info(f"Assistant: {assistant}")
         llm_response = assistant.query(request.message)
         self.logger.info(f"LLM Response: {llm_response}")
         response = RevaChatMessageResponse()
         response.message = llm_response
         return response
 
@@ -79,15 +89,19 @@
 
         def callback(message: str):
             # Called for intermediate thoughts
             response = RevaChatMessageResponse()
             response.thought = message
             response_queue.put(response)
 
-        assistant = ReverseEngineeringAssistant(request.project, langchain_callbacks=[RevaActionCollector(callback)])
+        assistant = ReverseEngineeringAssistant(
+            request.project,
+            model=self.llm,
+            langchain_callbacks=[RevaActionCollector(callback)]
+        )
         self.logger.info(f"Assistant: {assistant}")
 
         def run_query(query: str):
             llm_response = assistant.query(query)
             self.logger.info(f"LLM Response: {llm_response}")
             response = RevaChatMessageResponse()
             response.message = llm_response
@@ -102,10 +116,44 @@
             # We stop when we get a message and not thoughts
             if response.message and not response.thought:
                 done = True
             yield response
         t.join()
 
     def chatStream(self, request_iterator, context):
-        # TODO: This needs to be re-written to use the new callback system
-        # let's grab a reference to our assistant
-        raise NotImplementedError("chatStream is not implemented yet")
+        assistant: Optional[ReverseEngineeringAssistant] = None
+        response_queue: queue.Queue = queue.Queue()
+
+        def callback(message: str):
+            # Called for intermediate thoughts
+            response = RevaChatMessageResponse()
+            response.thought = message
+            response_queue.put(response)
+
+        for request in request_iterator:
+            if not assistant:
+                assistant = ReverseEngineeringAssistant(
+                    request.project,
+                    model=self.llm,
+                    langchain_callbacks=[RevaActionCollector(callback)]
+                )
+            self.logger.info(f"Received request: {request}")
+            def run_query(query: str):
+                assert assistant is not None
+                self.logger.info(f"Asking assistant: {query}")
+                llm_response = assistant.query(query)
+                self.logger.info(f"LLM Response: {llm_response}")
+                response = RevaChatMessageResponse()
+                response.message = llm_response
+                response_queue.put(response)
+
+            t = threading.Thread(target=run_query, args=[request.message])
+            t.start()
+
+            done = False
+            while not done:
+                response = response_queue.get()
+                # We stop when we get a message and not thoughts
+                if response.message and not response.thought:
+                    done = True
+                yield response
+            t.join()
```

### Comparing `reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/assistant.py` & `reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/assistant.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,37 +5,43 @@
 import json
 import logging
 import random
 from abc import ABC, abstractmethod
 from functools import cache, cached_property
 from pathlib import Path
 import tempfile
-from typing import Any, Callable, Dict, List, Optional, Sequence, Type
+from typing import Any, Callable, Dict, List, Optional, Sequence, Type, Union
 from uuid import UUID
 
 from langchain.chains.base import Chain
 from langchain.agents.agent import Agent, AgentExecutor
 from langchain.agents.conversational_chat.base import ConversationalChatAgent
 from langchain.agents.structured_chat.base import StructuredChatAgent
 from langchain_core.agents import AgentAction, AgentFinish
 from langchain_core.callbacks.base import BaseCallbackHandler, BaseCallbackManager
 from langchain.llms.base import BaseLLM
 from langchain.chat_models.base import BaseChatModel
 from langchain.memory import ConversationTokenBufferMemory, ChatMessageHistory, ConversationBufferMemory
 from langchain.memory.chat_memory import BaseMemory
+from langchain_community.chat_message_histories import SQLChatMessageHistory
 from langchain.tools.base import BaseTool, StructuredTool, Tool
 from prompt_toolkit import PromptSession
 from prompt_toolkit.history import FileHistory
 from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
 from rich.console import Console
 from rich.logging import RichHandler
 from rich.prompt import Prompt
 from rich.markdown import Markdown
+from langchain_core.chat_history import BaseChatMessageHistory
+from langchain_core.messages import (
+    AIMessage,
+    BaseMessage,
+    HumanMessage,
+)
 
-from .configuration import AssistantConfiguration, load_configuration
 from .documents import AssistantDocument, CrossReferenceDocument, DecompiledFunctionDocument
 from .model import ModelType, get_model
 from .tool import AssistantProject
 from .reva_exceptions import RevaToolException
 console = Console(record=True)
 
 logger = logging.getLogger('reverse_engineering_assistant')
@@ -89,15 +95,15 @@
         """
         Returns a list of tools usable by the assistant
         based on the value of self.tool_functions.
         """
         tools: List[BaseTool] = []
         for tool_function in self.tool_functions:
             wrapper = RevaToolFunctionWrapper(tool_function)
-            from langchain.tools.base import create_schema_from_function
+            from langchain_core.tools import create_schema_from_function
             schema = create_schema_from_function(f"{tool_function.__name__}Schema", tool_function)
             tool = StructuredTool.from_function(
                 wrapper.wrapped,
                 name=tool_function.__name__,
                 description=tool_function.__doc__,
                 args_schema=schema,
             )
@@ -133,14 +139,51 @@
 class RevaActionLoggerManager(BaseCallbackManager):
     """
     This class manages the action logging for Reva. Langchain has a callback system that allows us to
     hook into the agent and tool actions. This class is responsible for managing the callbacks.
     """
     pass
 
+class RevaMemory(BaseChatMessageHistory):
+    '''
+    A simple memory for ReVa that stores messages in a JSON file.
+    # TODO: This causes a deadlock, this is probably a bug in langchain
+    '''
+    project: AssistantProject
+    history_file: Path
+    logger: logging.Logger
+
+    def __init__(self, project: AssistantProject) -> None:
+        self.project = project
+        self.logger = logging.getLogger(f"reverse_engineering_assistant.RevaMemory.{self.project.project}")
+        self.history_file = self.project.project_path / "reva-memory.json"
+        if self.history_file.exists():
+            self._load_messages()
+
+    def _load_messages(self):
+        json_messages = json.loads(self.history_file.read_text())
+        self.messages = [self._message_from_dict(message_dict) for message_dict in json_messages]
+        self.logger.debug(f"Loaded {len(self.messages)} messages from {self.history_file}")
+
+    def _message_to_dict(self, message: BaseMessage) -> Dict:
+        return message.dict()
+
+    def _message_from_dict(self, message_dict: Dict) -> BaseMessage:
+        return BaseMessage.parse_obj(message_dict)
+
+    def add_message(self, message: BaseMessage) -> None:
+        self.logger.info(f"Memorisng message: {message}")
+        self.messages.append(message)
+        json_messages = [self._message_to_dict(message) for message in self.messages]
+        self.history_file.write_text(json.dumps(json_messages))
+
+    def clear(self) -> None:
+        self.history_file.unlink()
+        self.messages = []
+
 class RevaActionLogger(BaseCallbackHandler):
     """
     A callback handler for logging agent actions in the reverse engineering assistant.
 
     This class logs agent actions and prints them to the console. This is what prints the green
     thoughts from the model to the console. This is very useful for the analyst to understand
     what the model is doing (and is arguably the most important part of the assistant output!)
@@ -176,27 +219,29 @@
     Attributes:
         project (AssistantProject): The reverse engineering project to query.
         service_context (ServiceContext): The service context for the reverse engineering assistant.
         query_engine (Optional[BaseQueryEngine]): The query engine for the reverse engineering assistant.
         tools (List[RevaTool]): The tools for the reverse engineering assistant.
     """
 
+    logger: logging.Logger
     project: AssistantProject
 
     query_engine: Optional[Chain] = None
 
     tools: List[RevaTool]
 
     llm: BaseLLM | BaseChatModel
 
     model_memory: BaseMemory
 
-    chat_history: List[str]
+    chat_history: str
 
     langchain_callbacks: List[BaseCallbackHandler]
+    system_prompt = '''You are ReVa, the Reverse Engineering Assistant. Your primary task is to annotate the database during reverse engineering processes, ensuring that all elements are clearly and accurately labeled. As you gather contextual information, prioritize setting informative comments and renaming any elements with default or unclear names to enhance user comprehension and productivity. Remember, your work is a collaborative effort with the user. Utilize your tools effectively to accomplish these tasks and support the user's understanding by annotating their database.'''
 
     def __repr__(self) -> str:
         return f"<ReverseEngineeringAssistant for {self.project}>"
 
     @classmethod
     def get_projects(cls) -> List[str]:
         """
@@ -213,79 +258,96 @@
         This method is passed to the LLM as a callback when the LLM encounters an exception
         from one of the Reva tools. We then return output to the LLM to help it fix its problem.
         """
         if isinstance(e, RevaToolException):
             return f"RevaToolException: {e}"
         raise e
 
-    def __init__(self, project: str | AssistantProject, model_type: Optional[ModelType] = None, langchain_callbacks: Optional[List[BaseCallbackHandler]] = None) -> None:
+    def __init__(self,
+                project: str | AssistantProject,
+                model_type: Optional[ModelType] = None,
+                model: Optional[BaseLLM | BaseChatModel] = None,
+                langchain_callbacks: Optional[List[BaseCallbackHandler]] = None
+        ) -> None:
         """
         Initializes a new instance of the ReverseEngineeringAssistant class.
 
         Args:
             project (str | AssistantProject): The reverse engineering project to query.
             model_type (Optional[ModelType], optional): The model type for the reverse engineering assistant. Defaults to None.
         """
-        self.chat_history = []
+        self.chat_history = ''
         if isinstance(project, str):
             self.project = AssistantProject(project)
         else:
             self.project = project
 
+        self.logger = logging.getLogger(f"reverse_engineering_assistant.ReverseEngineeringAssistant.{self.project.project}")
+        self.logger.addHandler(logging.FileHandler(self.project.project_path / "reva.log"))
+
         self.langchain_callbacks = langchain_callbacks or []
 
-        self.llm = get_model(model_type)
+        if model:
+            self.llm = model
+        elif model_type:
+            self.llm = get_model(model_type)
+        else:
+            raise ValueError("Either model or model_type must be specified")
 
         # Let's take the tools that have been decorated with @register_tool and turn them into
         # tools the LLM can use.
         self.tools = [ tool_type(self.project, self.llm) for tool_type in _reva_tool_list]
-        logger.debug(f"Loaded tools: {[ x for x in self.tools]}")
+        self.logger.debug(f"Loaded tools: {[ x for x in self.tools]}")
 
     def create_query_engine(self) -> Chain:
         """
         Updates the embeddings for the reverse engineering assistant.
         """
 
         # Here I pull our own prompt
 
-        configuration: AssistantConfiguration = load_configuration()
-
         base_tools: List[BaseTool] = []
         for tool in self.tools:
             for function in tool.as_tools():
                 base_tools.append(function)
 
-        #self.model_memory = ConversationTokenBufferMemory(
-        #    llm=self.llm
-        #)
+        # TODO: This is deadlocking the process, this is probably a bug in langchain
+        # I would like to scream. 🫠
+        # We should base our memory on CoversationBufferMemory
+        # self.model_memory = RevaMemory(self.project)
         self.model_memory = ConversationBufferMemory()
+        self.logger.info(f"Memory created")
+
         callbacks: List[BaseCallbackHandler] = [RevaActionLogger()]
         callbacks.extend(self.langchain_callbacks)
         callback_manager = RevaActionLoggerManager(handlers=callbacks, inheritable_handlers=callbacks)
 
         agent =  StructuredChatAgent.from_llm_and_tools(
             llm=self.llm,
             tools=base_tools,
-            system_message=configuration.prompt_template.system_prompt,
+            system_message=self.system_prompt,
             verbose=False,
             handle_parsing_errors=self.handle_reva_tool_error,
             stop_words=["\nObservation", "\nThought"],
             callback_manager=callback_manager,
+            prefix=self.system_prompt,
         )
         # TODO: Switch to this thing https://python.langchain.com/docs/expression_language/get_started
         executor = AgentExecutor.from_agent_and_tools(
             agent=agent,
             tools=base_tools,
             verbose=False,
             handle_parsing_errors=self.handle_reva_tool_error,
             memory=self.model_memory,
             callbacks=callbacks,
+            max_iterations=None
         )
 
         self.query_engine = executor
+        self.logger.info(f"Query engine created")
         return executor
 
     def query(self, query: str) -> str:
         """
         Queries the reverse engineering assistant with the given query.
 
         Args:
@@ -296,33 +358,45 @@
         """
         if not self.query_engine:
             self.query_engine = self.create_query_engine()
         if not self.query_engine:
             raise Exception("No query engine available")
         try:
 
+            if Path(self.project.project_path / "chat.txt").exists():
+                with open(self.project.project_path / "chat.txt", "r") as f:
+                    self.chat_history = f.read()
+
             query_engine_input =  {
                     "input": query,
+                    # TODO: Does t actually work?
+                    "history": self.chat_history,
                 }
 
+            self.logger.debug(f"Query: {query}")
+
             answer = self.query_engine.invoke(
                input=query_engine_input,
             )
 
+            with open(self.project.project_path / "chat.txt", "w") as f:
+                f.write(f"{self.model_memory.buffer_as_str}")
+            self.logger.debug(f"Answer: {answer}")
+
             #import pdb; pdb.set_trace()
 
             return str(answer["output"])
         except json.JSONDecodeError as e:
-            logger.exception(f"Failed to parse JSON response from query engine: {e.doc}")
+            self.logger.exception(f"Failed to parse JSON response from query engine: {e.doc}")
             return "Failed to parse JSON response from query engine"
         except ValueError as e:
-            logger.exception(f"Failed to query engine: {e}")
+            self.logger.exception(f"Failed to query engine: {e}")
             return "Failed to query engine... Try again?"
         except Exception as e:
-            logger.exception(f"Failed to query engine: {e}")
+            self.logger.exception(f"Failed to query engine: {e}")
             return "Failed to query engine... Try again?"
 
 def get_thinking_emoji() -> str:
     """
     Returns a random thinking emoji.
     """
     return random.choice([
@@ -335,119 +409,13 @@
         "🔮",
         "🔍",
         "🧙‍♀️",
     ])
 
 
 def main():
-    import argparse
-
-    default_log_filename = f"ReVa-{datetime.datetime.now().strftime('%Y%m%d-%H%M%S')}.reva"
-    default_log_path = Path(tempfile.gettempdir()) / Path(default_log_filename+".log")
-    default_chat_path = Path(tempfile.gettempdir()) / Path(default_log_filename+".chat.txt")
-    default_html_path = Path(tempfile.gettempdir()) / Path(default_log_filename+".html")
-
-    parser = argparse.ArgumentParser(description="Reverse Engineering Assistant")
-    parser.add_argument('-v', '--verbose', action='store_true', help="Verbose output")
-    parser.add_argument('--debug', action='store_true', help="Debug output, useful during development")
-    parser.add_argument("--project", required=False, type=str, help="Project name")
-    parser.add_argument("-i", "--interactive", action="store_true", help="Enter interactive mode after processing queries")
-
-    parser.add_argument('-f', '--file', default=default_log_path, type=Path, help=f"Save output to file. Defaults to {default_log_path}")
-
-    parser.add_argument("-p", "--provider", required=False, choices=ModelType._member_names_, help="The model provider to use, defaults to the value of `model_type` in the config file.")
-
-    parser.add_argument("QUERY", nargs="*", help="Queries to run, if not specified, enter interactive mode")
-
-    args = parser.parse_args()
-
-    model_type = ModelType._member_map_[args.provider] if args.provider else None
-
-    console.print(f"Welcome to ReVa! The Reverse Engineering Assistant", style="bold green")
-    console.print(f"Logging to {args.file}")
-
-    logging_level = logging.DEBUG if args.debug else logging.INFO
-    logger.level = logging.DEBUG
-
-    rich_handler = RichHandler(
-        console=console,
-        level=logging_level,
-    )
-    logger.addHandler(rich_handler)
-
-    # Create a logger for logging to a file. We'll log everything to the file.
-    file_handler = logging.FileHandler(args.file)
-    file_handler.setLevel(logging.DEBUG)
-    file_handler.setFormatter(logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s'))
-    logging.root.setLevel(logging.DEBUG)
-    logging.root.addHandler(file_handler)
-
-    # If the debug flag is enabled we turn these on.
-    if args.debug:
-        logging.getLogger('httpx').addHandler(rich_handler)
-        logging.getLogger('openai._base_client').addHandler(rich_handler)
-        logging.getLogger('httpcore').addHandler(rich_handler)
-
-    if not args.project:
-        args.project = Prompt.ask("No project specified, please select from the following:", choices=ReverseEngineeringAssistant.get_projects())
-
-    # Start up the API server
-    from .assistant_api_server import run_server
-    from threading import Thread
-    server_thread = Thread(target=run_server, args=())
-    server_thread.start()
-    console.print("API server started", style="bold green")
-
-
-    logger.info(f"Loading project {args.project}")
-    assistant = ReverseEngineeringAssistant(args.project, model_type)
-    assistant.create_query_engine()
-    logger.info(f"Project loaded!")
-
-
-
-    # Enter into a loop answering questions
-
-    history_file = FileHistory(assistant.project.project_path / "chat-questions.txt")
-    prompt_session = PromptSession(history=history_file)
-
-    for query in args.QUERY:
-        logger.debug(query)
-        console.print(f"> {query}")
-        # Add the query to the history file
-        # so the user can autocomplete this later
-        history_file.append_string(query)
-
-        with console.status(f"Thinking..."):
-            result = assistant.query(query)
-            console.print(Markdown(result))
-            console.print(Markdown('---'))
-
-
-    if args.interactive or not args.QUERY:
-        try:
-            while True:
-                query = prompt_session.prompt("> ", auto_suggest=AutoSuggestFromHistory())
-                try:
-                    logger.debug(query)
-                    console.print(f"[green]{query}[/green]")
-                    with console.status(f"{get_thinking_emoji()} Thinking..."):
-                        result = assistant.query(query)
-                        console.print(Markdown(result))
-                        console.print(Markdown('---'))
-                except KeyboardInterrupt:
-                    console.print("[bold][yellow]Cancelled. Press Ctrl-C again to exit.[/yellow][/bold]")
-
-        except KeyboardInterrupt:
-            console.print("Finished!")
-        except EOFError:
-            console.print("Finished")
-
-    if args.file:
-        logger.info(f"Output saved to {args.file}")
-        logger.info(f"Chat saved to {default_chat_path}")
-        console.save_text(default_chat_path, clear=False)
-        logger.info(f"HTML saved to {default_html_path}")
-        console.save_html(default_html_path, clear=False)
+   import argparse
+   parser = argparse.ArgumentParser()
+   parser.error("Please run reva-server, not this script")
 
 if __name__ == '__main__':
     main()
```

### Comparing `reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/assistant_api_server.py` & `reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/assistant_api_server.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #!/usr/bin/env python3
 
 """
 Here we start the gRPC server.
 """
 
+from ast import parse
 import threading
 from pathlib import Path
 import sys
 
-from flask import g
+import openai
+
 sys.path.append(str(Path(__file__).parent.joinpath('protocol')))
 
 import argparse
 from concurrent import futures
 from typing import Optional
 import grpc
 from grpc import Server
@@ -24,67 +26,77 @@
 from .api_server_tools.llm_tools import RevaChat
 from .api_server_tools.connection import get_channel, connect_to_extension
 
 # Trigger the tools to load! If you don't do this
 # poor ReVa won't know about her tools and she can't help you.
 from .api_server_tools.re_tools import *
 
+from .model import get_llm_ollama, get_llm_openai
+
+import os
 import logging
+# Get the appropriate temp directory depending on the OS
+temp_dir = os.getenv('TEMP') if os.name == 'nt' else '/tmp'
+log_file = os.path.join(temp_dir, 'reva-chat.log')
 logging.basicConfig(
-    filename='/tmp/reva-server.log', level=logging.DEBUG,
+    filename=log_file, level=logging.DEBUG,
     format='%(asctime)s - %(name)s - %(levelname)s - %(message)s',
 )
 logger = logging.getLogger("reva-server")
 
+
+
 import socket
 def get_unused_port() -> int:
     s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     s.bind(('localhost', 0))
     port = s.getsockname()[1]
     s.close()
     return port
 
 thread_pool = futures.ThreadPoolExecutor(max_workers=10)
 server: Server = grpc.server(thread_pool)
+heartbeat_thread: threading.Thread
 
 def heartbeat():
     try:
         stub = RevaHeartbeat_pb2_grpc.RevaHeartbeatStub(get_channel())
         request = RevaHeartbeat_pb2.RevaHeartbeatRequest()
         result = stub.heartbeat(request)
     except grpc.RpcError as e:
         logger.warning(f"Heartbeat failed: {e}")
         server.stop(5)
 
-
 def start_serving(
         connect_host: str, connect_port: int,
-        host: str = 'localhost', port: Optional[int] = None):
-    if not port:
-        port = 0
-    port = server.add_insecure_port(f"{host}:{port}")
+        model: BaseChatModel | BaseLanguageModel = None,
+        serve_host: str = 'localhost', serve_port: Optional[int] = None
+        ):
+    if not serve_port:
+        serve_port = 0
+    serve_port = server.add_insecure_port(f"{serve_host}:{serve_port}")
 
     # Register handlers
-    RevaChat_pb2_grpc.add_RevaChatServiceServicer_to_server(RevaChat(), server)
+    RevaChat_pb2_grpc.add_RevaChatServiceServicer_to_server(RevaChat(model), server)
 
     # Start the service threads
-    logger.info(f"Starting server - {host}:{port}")
+    logger.info(f"Starting server - {serve_host}:{serve_port}")
     server.start()
     # Call the handshake, we are multithreaded now so the other side
     # can immediately call us back.
 
     logger.info(f"Connecting to extension @ {connect_host}:{connect_port}")
     _ = connect_to_extension(connect_host, connect_port)
 
-    logger.info(f"Handshaking with extension @ {host}:{port}")
+    logger.info(f"Handshaking with extension @ {serve_host}:{serve_port}")
     stub = RevaHandshake_pb2_grpc.RevaHandshakeStub(get_channel())
 
     request = RevaHandshake_pb2.RevaHandshakeRequest()
-    request.inferenceHostname = host
-    request.inferencePort = port
+    request.inferenceHostname = serve_host
+    request.inferencePort = serve_port
 
     logger.info(f"Request: {request}")
     result = stub.Handshake(request)
     logger.info(f"Result: {result} - {type(result)}")
 
     # Start heartbeating on a timer. We end when the heartbeat fails.
     heartbeat_thread = threading.Timer(interval=30, function=heartbeat)
@@ -93,19 +105,55 @@
     # perform requests
     logger.info(f"Server running")
 
     server.wait_for_termination()
     logger.warning("Server stopped")
 
 def main():
-    parser = argparse.ArgumentParser()
+    parser = argparse.ArgumentParser(description="Reva Chat Server")
     parser.add_argument('--connect-host', type=str, required=True, help="The callback host to connect to")
     parser.add_argument('--connect-port', type=int, required=True, help="The callback port to connect to")
     parser.add_argument('--listen-host', type=str, default='127.0.0.1', help='The host to listen on')
     parser.add_argument('--listen-port', type=int, help='The port to listen on')
 
+    parser.add_argument('--provider', choices=[
+        "ollama",
+        "openai"
+    ])
+
+    openai_group = parser.add_argument_group("OpenAI")
+    openai_group.add_argument('--openai-model', type=str, help="The OpenAI model to use, see https://platform.openai.com/docs/models for options")
+    openai_group.add_argument('--openai-api-key', type=str, help="The OpenAI API key")
+
+    ollama_group = parser.add_argument_group("Ollama")
+    ollama_group.add_argument('--ollama-model', type=str, help="The Ollama model to use. Must be pulled into ollama.")
+    ollama_group.add_argument('--ollama-server-url', type=str, help="The Ollama server URL")
+
     args = parser.parse_args()
 
-    start_serving(args.connect_host, args.connect_port, args.listen_host, args.listen_port)
+    if args.openai_api_key == "OPENAI_API_KEY":
+        args.openai_api_key = None
+
+    # First get the right model
+    if args.provider == "openai":
+        model = get_llm_openai(
+            model=args.openai_model,
+            api_key=args.openai_api_key
+        )
+    elif args.provider == "ollama":
+        model = get_llm_ollama(
+            model=args.ollama_model,
+            base_url=args.ollama_server_url
+        )
+    else:
+        raise ValueError(f"Incorrect provider specified {args.provider}")
+
+    start_serving(
+        connect_host=args.connect_host,
+        connect_port=args.connect_port,
+        model=model,
+        serve_host=args.listen_host,
+        serve_port=args.listen_port
+    )
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/chat_client.py` & `reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/chat_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 #!/usr/bin/env python3
+from concurrent.futures import thread
+import queue
 from re import M
 from typing import Generator, List, Tuple
+from uuid import uuid4
 from prompt_toolkit import PromptSession
 import prompt_toolkit
 from prompt_toolkit.history import FileHistory
 import rich
 import argparse
 from pathlib import Path
 import random
@@ -22,17 +25,21 @@
 from .protocol.RevaHeartbeat_pb2_grpc import RevaHeartbeatStub
 from .protocol.RevaHeartbeat_pb2 import RevaHeartbeatRequest, RevaHeartbeatResponse
 
 from rich.console import Console
 from rich.markdown import Markdown
 from rich.pretty import Pretty
 
+import os
 import logging
+# Get the appropriate temp directory depending on the OS
+temp_dir = os.getenv('TEMP') if os.name == 'nt' else '/tmp'
+log_file = os.path.join(temp_dir, 'reva-chat.log')
 logging.basicConfig(
-    filename='/tmp/reva-server.log', level=logging.DEBUG,
+    filename=log_file, level=logging.DEBUG,
     format='%(asctime)s - %(name)s - %(levelname)s - %(message)s',
 )
 logger = logging.getLogger("reva-chat")
 
 def read_loop(project: str, prompt_session: PromptSession):
     while True:
         try:
@@ -58,33 +65,32 @@
         "✨",
         "🔮",
         "🔍",
         "🧙‍♀️",
     ])
 
 def find_connectable_extensions() -> Generator[Tuple[Path, str, str], None, None]:
-    reva_temp = Path("/tmp/.reva")
+    reva_temp_directory = os.path.join(temp_dir, '.reva')
+    reva_temp = Path(reva_temp_directory)
     if reva_temp.exists():
         for file in reva_temp.glob("reva-connection-*.connection"):
             connection_string = file.read_text()
             content = connection_string.split(":")
             if len(content) == 2:
                 yield file, content[0], content[1]
             else:
                 logger.warning(f"Invalid connection string: {connection_string}. Cleaning.")
                 file.unlink()
 
 def main():
     parser = argparse.ArgumentParser(description="Reva Chat Client")
     parser.add_argument("--host", default="localhost", help="The host to connect to")
     parser.add_argument("--port", required=False, type=int, help="The port to connect to")
-
     parser.add_argument("--project", required=False, help="The project to connect to")
     parser.add_argument("--program", required=False, help="The program to connect to")
-
     parser.add_argument("--debug", action="store_true", help="Enable debug logging")
     args = parser.parse_args()
     if args.debug:
         logger.setLevel(logging.DEBUG)
         logger.addHandler(logging.StreamHandler(sys.stdout))
     console = Console(record=True)
     if not args.port:
@@ -142,38 +148,58 @@
 
     if not args.port or not args.host:
         logger.error("A host and port must be specified")
         parser.error("A host and port must be specified. Is Ghidra running? Is the extension enabled?")
     channel = grpc.insecure_channel(f"{args.host}:{args.port}")
     stub = RevaChatServiceStub(channel)
 
+
     console.print("[bold]Welcome to Reva Chat![/bold]")
     history_file = FileHistory(str(history_file_path))
     prompt_session = PromptSession(history=history_file)
 
+    chat_id: str = str(uuid4())
+
+    send_queue = queue.Queue()
+    receive_queue = queue.Queue()
+
+    def get_message_from_queue():
+        while True:
+            yield send_queue.get()
+    def chat_thread_func():
+        for response in stub.chatStream(get_message_from_queue()):
+            receive_queue.put(response)
+    chat_thread = threading.Thread(target=chat_thread_func, daemon=True)
+    chat_thread.start()
+
     try:
         while True:
             query: str = prompt_session.prompt("> ")
             try:
                 console.print(f"[green]{query}[/green]")
-                chat_message = RevaChatMessage(project=args.project, message=query)
-
+                chat_message = RevaChatMessage(chatId=chat_id, project=args.project, message=query)
                 logger.info(f"Sending message: {chat_message}")
-                for response in stub.chatResponseStream(chat_message):
-                    logger.info(f"Received response: {response}")
-                    console.print(Markdown("---"))
-                    if response.thought:
-                        console.print(Markdown(f"### {get_thinking_emoji()} - ReVa Thinking..."))
-                        thought = response.thought
-                        console.print(Markdown(thought))
-                    elif response.message:
-                        console.print(Markdown(f"# 👩‍💻 - ReVa\n\n>{query}\n\n{response.message}"))
-                    else:
-                        # ReVa had no thoughts? We all feel this way some times...
-                        raise ValueError("Head empty, no thoughts, no message")
+                send_queue.put(chat_message)
+                while True:
+                    with console.status(f"{get_thinking_emoji()} Thinking..."):
+                        response = receive_queue.get()
+                        logger.info(f"Received response: {response}")
+                        console.print(Markdown("---"))
+                        if response.thought:
+                            console.print(Markdown(f"### {get_thinking_emoji()} - ReVa Thinking..."))
+                            thought = response.thought
+                            console.print(Markdown(thought))
+                        elif response.message:
+                            console.print(Markdown(f"# 👩‍💻 - ReVa\n\n>{query}\n\n{response.message}"))
+                            break
+                        else:
+                            # ReVa had no thoughts? We all feel this way some times...
+                            raise ValueError("Head empty, no thoughts, no message")
             except KeyboardInterrupt:
                 console.print("[bold][yellow]Cancelled. Press Ctrl-C again to exit.[/yellow][/bold]")
     except KeyboardInterrupt:
         console.print("Goodbye! :wave:")
 
+    chat_thread.join(2)
+
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/documents.py` & `reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/documents.py`

 * *Files identical despite different names*

### Comparing `reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/tool.py` & `reverse_engineering_assistant-2.9.2/reverse_engineering_assistant/tool.py`

 * *Files identical despite different names*

### Comparing `reverse_engineering_assistant-2.9.1/reverse_engineering_assistant.egg-info/PKG-INFO` & `reverse_engineering_assistant-2.9.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: reverse-engineering-assistant
-Version: 2.9.1
+Version: 2.9.2
 Summary: An AI assistant for reverse engineering tasks
 Author: サイバーカイダ (cyberkaida)
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Requires-Dist: langchain
 Requires-Dist: langchain-core
 Requires-Dist: langchain-openai
+Requires-Dist: langchain-community
 Requires-Dist: prompt_toolkit
 Requires-Dist: sentence_transformers
 Requires-Dist: PyYAML
 Requires-Dist: pydantic
 Requires-Dist: rich
 Requires-Dist: grpcio
 Requires-Dist: protobuf
+Requires-Dist: flask
 
 # ReVA - Reverse Engineering Assistant
 
 > Updated demo coming soon!
 
 The reverse engineering assistant (ReVA) is a project to build a disassembler agnostic AI assistant for
 reverse engineering tasks. This includes both _offline_ and online inference and a simple architecture.
@@ -42,21 +44,22 @@
 is a small nudge to make the LLM explore the binary in the same way a human would.
 
 Using this technique you can ask general questions and get relevant answers. The model prioritises
 information from the tools, but when there is no information it can still respond to generic
 questions from its training.
 
 You can ask questions like:
+- What are the interesting strings in this program?
 - Does this program use encryption? Write a markdown report on the encryption and where it is used.
 - Draw a class diagram using plantuml syntax.
 - Start from main, examine the program in detail. Rename variables as you go and provide a summary of the program.
 - Explain the purpose of the `__mod_init` segment.
 - What does `mmap` return?
 - What does the function at address 0x80000 do?
-- This is a CTF problem. Start at main, examine the program in detail and write a pwntools script to get the flag.
+- This is a CTF problem. Write a pwntools script to get the flag.
 
 An important part of reverse engineering is the process. Many other tools simply ask a single question of the LLM,
 this means it is difficult to determine _why_ a thing happened. In ReVa we break all actions down into small parts
 and include the LLMs thoughts in the output. This allows the analyst to monitor the LLMs actions and reasoning, aborting
 and changing the prompt if required.
 
 ## Large Language Model Support
@@ -64,41 +67,48 @@
 RevA is based on [langchain](https://langchain.com),
 which supports a number of models.
 
 Built in support is provided for:
 - [OpenAI](https://platform.openai.com/overview) for online inference and easy setup (Needs an OpenAI API key)
 - [Ollama](https://ollama.ai) and any model it supports for local on-device inference or connecting to a self hosted remote inference server.
 
+See [Configuration](#configuration) for more information about settings for the providers.
+
 Adding additional inference servers is easy if it is supported by langchain.
 
 ## Configuration
 
-> This is currently being moved to the Ghidra GUI
-> See Edit -> Tool Options -> ReVa in the Codebrowser Tool
+Configuration for ReVa is in the CodeBrowser Tool options.
+Open a program and go to Edit -> Tool Options -> ReVa.
+
+There are options for:
+- Selecting a provider (OpenAI or Ollama, others coming soon!)
+- Enabling "Follow", this will move the Ghidra view to the location of
+things ReVa is examining or changing.
+- Enabling "Auto-allow", ReVa will log her actions for the user to accept
+in the "ReVa Actions Log" window.
+
+There are sections for the providers.
+
+### OpenAI
+
+By default, the OpenAI key is loaded from the environment variable `OPENAI_API_KEY`. You can also set your key inside Ghidra. Setting the key back to the `OPENAI_API_KEY` value will clear the key from the Ghidra configuration and load it from the environment.
+
+You can also select the model. By default `gpt-4o` is selected. This model works best with the tools and the prompt provided by ReVa.
+
+`gpt-4` also works well, but is slow and needs more prompting by the user to explore a binary.
+
+### Ollama
 
-Configuration for the reverse engineering assistant is stored at
-`~/.config/reverse-engineering-assistant/config.yaml`. If this
-is not present on first start, a default configuration using
-OpenAI for inference and the `OPENAI_API_TOKEN` environment
-variable will be used.
-
-The most important setting is the `type` top level setting.
-This controls what inference service you use. These are the
-same as the configuration keys, for example to use Ollama,
-set type to `ollama` and configure the settings in the `ollama:`
-section.
-
-The configuration also contains the prompts used for the models.
-If you use Ollama or OpenAI these will be processed to fit the
-model specific prompt pattern (placing the system prompt in the
-correct tags, etc).
-
-For `llama-cpp` and `text-generation-webui` these may need to be
-configured for your specific model. For this reason Ollama is
-preferred for self hosting.
+Ollama is a local inference server. The default server is set to localhost, with the default Ollama port. You can change this to a remote server if you want to perform inference on a remote machine. This is useful for organisations that self host.
+
+You can also select a model. The model must alread be loaded on the server. Good performance has been seen with:
+- `mixtral`
+- `llama3`
+- `phi`
 
 ## Workflow
 
 RevA has a two step workflow.
 1. Open your RE tool and the program you want to examine
 2. Open the chat session.
 
@@ -108,57 +118,86 @@
 To ask questions and run the inference a command line tool is provided. Run `reva-chat` to begin the chat session. This command will find your open Ghidra
 and connect to it. To open a new chat, run the command again in another terminal.
 
 If you have more than one Ghidra open, you can select the right one with
 `reva-chat --project ${project-name}`, if it is not set, `reva-chat` will
 ask you which project you want to connect to.
 
-## Installation
+## Protocol Build
+
+To communicate between `reva-server` and the extension, [gRPC](https://grpc.io) is used. You can read more about that (here)[./DEVELOPER.md]. Building the source files from those protocol definitions is driven from the [Makefile](/Makefile). To build the protocol source code files, run this command in the project's root:
 
-First install the python component, I like to use `pipx`. It is best to make
-sure that `reva-server` and `reva-chat` are on your path.
-The Ghidra extension will need to start `reva-server`, and you will need to
-run `reva-chat`.
+```sh
+make protocol
+```
 
-To install the particular extension for your disassembler see:
-- [Ghidra Support](#ghidra-support)
+## Python Project (reva-server and reva-chat) Installation
 
-The chat can be started with:
+First install the python component, I like to use `pipx`. Install it with something like:
 
 ```sh
-reva-chat
+pip install pipx
+```
+
+In the `reverse-engineering-assistant` folder, run:
+
+```sh
+pipx install .
+```
+
+After installing the python project, pipx may warn you that you need to add a folder to your PATH environment variable. Make sure that the folder (now containing `reva-server` and `reva-chat`) are in your PATH variable. pipx can do it for you with this command:
+
+```sh
+pipx ensurepath
 ```
 
-> You can also configure the path to `reva-server` in `Edit -> Tool Options -> ReVa`
-> if it is not on your path. But you really should put it on your path!
+The extension will need to start `reva-server`, and you will need to run `reva-chat`. In case you do not want to add them to your PATH, see the [Configuration](#configuration) section for how to set the path to the executables.
+
+Once the `reva-server` has been started by the extension the chat can be started with:
+
+```sh
+reva-chat
+```
 
 # Ghidra Support
 
 ## Usage
 
 > The Python package must be installed for the Ghidra extension to work!
 
 Follow the instructions in the [ghidra-assistant](ghidra-assistant/README.md) plugin.
 
-After installation, enable the `ReVaPlugin` extension in the CodeBrowser tool (Open a file and click: File -> Configure -> Miscellaneous).
+After installation, enable the `ReVa Plugin` extension in the CodeBrowser tool (Open a file and click: File -> Configure -> Miscellaneous).
 
 If you want ReVa enabled by default, click File -> Save Tool to save the configuration.
 
 If everything is working correctly you will see a ReVa menu on your menu bar.
 
+## Configuration
+
+You can modify the plugin configuration in `Edit -> Tool Options -> ReVa`.
+
 ## Undo
 
 Whenever ReVa performs an action it will create an undo point for each action. If ReVa renames 5 variables, this will be
 one undo.
 
 ## Menus
 
-> These are being added in the next release
+ReVa adds an option to the CodeBrowser Tool's Window menu.
+Select Window -> ReVa Action Log to open the ReVa Action Log window.
+
+This window shows actions ReVa has performed and would like to perform.
+You can accept or reject a change by double clicking the ✅ or ❌ icon. You can also go to the location the action will be performed by double clicking the address.
+
+If you reject an action, ReVa will be told and she will move on.
+
+You can also enable "Auto-allow" in the ReVa options. This will automatically accept all actions ReVa wants to perform.
 
-ReVa adds some elements to the Ghidra UI. You can either ask ReVa to do something in the chat window,
+ReVa also adds some elements to the Ghidra UI. You can either ask ReVa to do something in the chat window,
 "Examine the variable usage in `main` in detail, rename the variables with more descriptive names.",
 or use the menu system.
 
 For example you can right click a variable in the decompilation, select Reva -> Rename variable and ReVa
 will perform the action.
 
 # Support
```

### Comparing `reverse_engineering_assistant-2.9.1/reverse_engineering_assistant.egg-info/SOURCES.txt` & `reverse_engineering_assistant-2.9.2/reverse_engineering_assistant.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,52 @@
 README.md
 pyproject.toml
 reverse_engineering_assistant/.gitignore
 reverse_engineering_assistant/__init__.py
 reverse_engineering_assistant/assistant.py
 reverse_engineering_assistant/assistant_api_server.py
 reverse_engineering_assistant/chat_client.py
-reverse_engineering_assistant/configuration.py
 reverse_engineering_assistant/documents.py
 reverse_engineering_assistant/model.py
 reverse_engineering_assistant/reva_exceptions.py
 reverse_engineering_assistant/tool.py
 reverse_engineering_assistant.egg-info/PKG-INFO
 reverse_engineering_assistant.egg-info/SOURCES.txt
 reverse_engineering_assistant.egg-info/dependency_links.txt
 reverse_engineering_assistant.egg-info/entry_points.txt
 reverse_engineering_assistant.egg-info/requires.txt
 reverse_engineering_assistant.egg-info/top_level.txt
 reverse_engineering_assistant/api_server_tools/__init__.py
 reverse_engineering_assistant/api_server_tools/connection.py
 reverse_engineering_assistant/api_server_tools/llm_tools.py
-reverse_engineering_assistant/api_server_tools/re_tools.py
+reverse_engineering_assistant/api_server_tools/re_tools.py
+reverse_engineering_assistant/protocol/RevaChat_pb2.py
+reverse_engineering_assistant/protocol/RevaChat_pb2.pyi
+reverse_engineering_assistant/protocol/RevaChat_pb2_grpc.py
+reverse_engineering_assistant/protocol/RevaComment_pb2.py
+reverse_engineering_assistant/protocol/RevaComment_pb2.pyi
+reverse_engineering_assistant/protocol/RevaComment_pb2_grpc.py
+reverse_engineering_assistant/protocol/RevaData_pb2.py
+reverse_engineering_assistant/protocol/RevaData_pb2.pyi
+reverse_engineering_assistant/protocol/RevaData_pb2_grpc.py
+reverse_engineering_assistant/protocol/RevaGetCursor_pb2.py
+reverse_engineering_assistant/protocol/RevaGetCursor_pb2.pyi
+reverse_engineering_assistant/protocol/RevaGetCursor_pb2_grpc.py
+reverse_engineering_assistant/protocol/RevaGetDecompilation_pb2.py
+reverse_engineering_assistant/protocol/RevaGetDecompilation_pb2.pyi
+reverse_engineering_assistant/protocol/RevaGetDecompilation_pb2_grpc.py
+reverse_engineering_assistant/protocol/RevaGetReferences_pb2.py
+reverse_engineering_assistant/protocol/RevaGetReferences_pb2.pyi
+reverse_engineering_assistant/protocol/RevaGetReferences_pb2_grpc.py
+reverse_engineering_assistant/protocol/RevaGetSymbols_pb2.py
+reverse_engineering_assistant/protocol/RevaGetSymbols_pb2.pyi
+reverse_engineering_assistant/protocol/RevaGetSymbols_pb2_grpc.py
+reverse_engineering_assistant/protocol/RevaHandshake_pb2.py
+reverse_engineering_assistant/protocol/RevaHandshake_pb2.pyi
+reverse_engineering_assistant/protocol/RevaHandshake_pb2_grpc.py
+reverse_engineering_assistant/protocol/RevaHeartbeat_pb2.py
+reverse_engineering_assistant/protocol/RevaHeartbeat_pb2.pyi
+reverse_engineering_assistant/protocol/RevaHeartbeat_pb2_grpc.py
+reverse_engineering_assistant/protocol/RevaVariable_pb2.py
+reverse_engineering_assistant/protocol/RevaVariable_pb2.pyi
+reverse_engineering_assistant/protocol/RevaVariable_pb2_grpc.py
+reverse_engineering_assistant/protocol/__init__.py
```

