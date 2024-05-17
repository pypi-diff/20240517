# Comparing `tmp/spacy-llm-0.7.1.tar.gz` & `tmp/spacy_llm-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy-llm-0.7.1.tar", last modified: Mon Jan 29 13:37:45 2024, max compression
+gzip compressed data, was "spacy_llm-0.7.2.tar", last modified: Fri May 17 09:30:26 2024, max compression
```

## Comparing `spacy-llm-0.7.1.tar` & `spacy_llm-0.7.2.tar`

### file list

```diff
@@ -1,298 +1,298 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.071457 spacy-llm-0.7.1/
--rw-r--r--   0 vsts      (1001) docker     (127)     1066 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      147 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     9994 2024-01-29 13:37:45.071457 spacy-llm-0.7.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8450 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)     1483 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     1815 2024-01-29 13:37:45.071457 spacy-llm-0.7.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)      153 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.023457 spacy-llm-0.7.1/spacy_llm/
--rw-r--r--   0 vsts      (1001) docker     (127)      232 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10403 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/cache.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1585 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/compat.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.027457 spacy-llm-0.7.1/spacy_llm/models/
--rw-r--r--   0 vsts      (1001) docker     (127)      309 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/models/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.027457 spacy-llm-0.7.1/spacy_llm/models/hf/
--rw-r--r--   0 vsts      (1001) docker     (127)      361 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/models/hf/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7029 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/models/hf/base.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2695 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/models/hf/dolly.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3334 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/models/hf/falcon.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2793 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/models/hf/llama2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3953 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/models/hf/mistral.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3823 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/models/hf/openllama.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5343 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/models/hf/stablelm.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.027457 spacy-llm-0.7.1/spacy_llm/models/langchain/
--rw-r--r--   0 vsts      (1001) docker     (127)      227 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/models/langchain/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7637 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/models/langchain/model.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.027457 spacy-llm-0.7.1/spacy_llm/models/rest/
--rw-r--r--   0 vsts      (1001) docker     (127)      156 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/models/rest/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.027457 spacy-llm-0.7.1/spacy_llm/models/rest/anthropic/
--rw-r--r--   0 vsts      (1001) docker     (127)      997 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/models/rest/anthropic/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5244 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/models/rest/anthropic/model.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26092 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/models/rest/anthropic/registry.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.027457 spacy-llm-0.7.1/spacy_llm/models/rest/azure/
--rw-r--r--   0 vsts      (1001) docker     (127)      145 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/models/rest/azure/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6559 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/models/rest/azure/model.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5964 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/models/rest/azure/registry.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6397 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/models/rest/base.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.031457 spacy-llm-0.7.1/spacy_llm/models/rest/cohere/
--rw-r--r--   0 vsts      (1001) docker     (127)      167 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/models/rest/cohere/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5311 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/models/rest/cohere/model.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3905 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/models/rest/cohere/registry.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.031457 spacy-llm-0.7.1/spacy_llm/models/rest/noop/
--rw-r--r--   0 vsts      (1001) docker     (127)      123 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/models/rest/noop/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      938 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/models/rest/noop/model.py
--rw-r--r--   0 vsts      (1001) docker     (127)      371 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/models/rest/noop/registry.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.031457 spacy-llm-0.7.1/spacy_llm/models/rest/openai/
--rw-r--r--   0 vsts      (1001) docker     (127)     1335 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/models/rest/openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6444 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/models/rest/openai/model.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30014 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/models/rest/openai/registry.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.031457 spacy-llm-0.7.1/spacy_llm/models/rest/palm/
--rw-r--r--   0 vsts      (1001) docker     (127)      147 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/models/rest/palm/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4956 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/models/rest/palm/model.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4100 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/models/rest/palm/registry.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.031457 spacy-llm-0.7.1/spacy_llm/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (127)       54 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15373 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/pipeline/llm.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.031457 spacy-llm-0.7.1/spacy_llm/registry/
--rw-r--r--   0 vsts      (1001) docker     (127)      262 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/registry/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      606 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/registry/normalizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2976 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/registry/reader.py
--rw-r--r--   0 vsts      (1001) docker     (127)      450 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/registry/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.035457 spacy-llm-0.7.1/spacy_llm/tasks/
--rw-r--r--   0 vsts      (1001) docker     (127)     2113 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16856 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/builtin_task.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.035457 spacy-llm-0.7.1/spacy_llm/tasks/entity_linker/
--rw-r--r--   0 vsts      (1001) docker     (127)      179 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/entity_linker/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2941 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/entity_linker/candidate_selector.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1810 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/entity_linker/parser.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5836 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/entity_linker/registry.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18832 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/entity_linker/task.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1609 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/entity_linker/ty.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8178 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/entity_linker/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.035457 spacy-llm-0.7.1/spacy_llm/tasks/lemma/
--rw-r--r--   0 vsts      (1001) docker     (127)      157 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/lemma/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1348 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/lemma/parser.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2465 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/lemma/registry.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3361 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/lemma/task.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1464 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/lemma/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.035457 spacy-llm-0.7.1/spacy_llm/tasks/ner/
--rw-r--r--   0 vsts      (1001) docker     (127)      244 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/ner/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9353 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/ner/registry.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4491 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/ner/task.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1605 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/ner/util.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1660 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/noop.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.039457 spacy-llm-0.7.1/spacy_llm/tasks/raw/
--rw-r--r--   0 vsts      (1001) docker     (127)      145 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/raw/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      675 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/raw/parser.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2283 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/raw/registry.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3284 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/raw/task.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1187 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/raw/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.039457 spacy-llm-0.7.1/spacy_llm/tasks/rel/
--rw-r--r--   0 vsts      (1001) docker     (127)      244 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/rel/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      372 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/rel/items.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1501 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/rel/parser.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3172 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/rel/registry.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7443 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/rel/task.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3241 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/rel/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.039457 spacy-llm-0.7.1/spacy_llm/tasks/sentiment/
--rw-r--r--   0 vsts      (1001) docker     (127)      181 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/sentiment/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      995 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/sentiment/parser.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2439 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/sentiment/registry.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3820 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/sentiment/task.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1999 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/sentiment/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.039457 spacy-llm-0.7.1/spacy_llm/tasks/span/
--rw-r--r--   0 vsts      (1001) docker     (127)      361 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/span/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3309 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/span/examples.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6464 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/span/parser.py
--rw-r--r--   0 vsts      (1001) docker     (127)      534 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/span/registry.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5298 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/span/task.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4021 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/span/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.039457 spacy-llm-0.7.1/spacy_llm/tasks/spancat/
--rw-r--r--   0 vsts      (1001) docker     (127)      284 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/spancat/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9927 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/spancat/registry.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4980 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/spancat/task.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1806 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/spancat/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.043457 spacy-llm-0.7.1/spacy_llm/tasks/summarization/
--rw-r--r--   0 vsts      (1001) docker     (127)      205 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/summarization/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      771 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/summarization/parser.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2478 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/summarization/registry.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4841 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/summarization/task.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1469 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/summarization/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.047457 spacy-llm-0.7.1/spacy_llm/tasks/templates/
--rw-r--r--   0 vsts      (1001) docker     (127)      288 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/templates/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2624 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/templates/entity_linker.v1.jinja
--rw-r--r--   0 vsts      (1001) docker     (127)     1017 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/templates/lemma.v1.jinja
--rw-r--r--   0 vsts      (1001) docker     (127)      746 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/templates/ner.v1.jinja
--rw-r--r--   0 vsts      (1001) docker     (127)     1410 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/templates/ner.v2.jinja
--rw-r--r--   0 vsts      (1001) docker     (127)     2261 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/templates/ner.v3.jinja
--rw-r--r--   0 vsts      (1001) docker     (127)      309 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/templates/raw.v1.jinja
--rw-r--r--   0 vsts      (1001) docker     (127)     1585 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/templates/rel.v1.jinja
--rw-r--r--   0 vsts      (1001) docker     (127)      540 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/templates/sentiment.v1.jinja
--rw-r--r--   0 vsts      (1001) docker     (127)      769 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/templates/spancat.v1.jinja
--rw-r--r--   0 vsts      (1001) docker     (127)     1479 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/templates/spancat.v2.jinja
--rw-r--r--   0 vsts      (1001) docker     (127)     2318 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/templates/spancat.v3.jinja
--rw-r--r--   0 vsts      (1001) docker     (127)      675 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/templates/summarization.v1.jinja
--rw-r--r--   0 vsts      (1001) docker     (127)     1251 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/templates/textcat.v1.jinja
--rw-r--r--   0 vsts      (1001) docker     (127)     1717 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/templates/textcat.v2.jinja
--rw-r--r--   0 vsts      (1001) docker     (127)     2162 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/templates/textcat.v3.jinja
--rw-r--r--   0 vsts      (1001) docker     (127)      589 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/templates/translation.v1.jinja
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.047457 spacy-llm-0.7.1/spacy_llm/tasks/textcat/
--rw-r--r--   0 vsts      (1001) docker     (127)      284 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/textcat/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2106 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/textcat/parser.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10358 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/textcat/registry.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6617 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/textcat/task.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2375 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/textcat/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.047457 spacy-llm-0.7.1/spacy_llm/tasks/translation/
--rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/translation/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      607 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/translation/parser.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2568 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/translation/registry.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3453 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/translation/task.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1234 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/translation/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.047457 spacy-llm-0.7.1/spacy_llm/tasks/util/
--rw-r--r--   0 vsts      (1001) docker     (127)       68 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1355 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/util/parsing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4668 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tasks/util/sharding.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.051457 spacy-llm-0.7.1/spacy_llm/tests/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      302 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/compat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1372 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/conftest.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.051457 spacy-llm-0.7.1/spacy_llm/tests/models/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2556 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/models/test_anthropic.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3329 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/models/test_cohere.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1812 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/models/test_dolly.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/models/test_falcon.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2639 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/models/test_hf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1954 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/models/test_langchain.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1958 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/models/test_llama2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1692 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/models/test_mistral.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2320 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/models/test_openllama.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2427 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/models/test_palm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4333 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/models/test_rest.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2382 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/models/test_stablelm.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.051457 spacy-llm-0.7.1/spacy_llm/tests/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14715 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/pipeline/test_llm.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.051457 spacy-llm-0.7.1/spacy_llm/tests/sharding/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/sharding/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11459 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/sharding/test_sharding.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2757 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/sharding/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.055457 spacy-llm-0.7.1/spacy_llm/tests/tasks/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      214 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/custom.cfg
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.063458 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/
--rw-r--r--   0 vsts      (1001) docker     (127)     1449 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/entity_linker.json
--rw-r--r--   0 vsts      (1001) docker     (127)     1244 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/entity_linker.jsonl
--rw-r--r--   0 vsts      (1001) docker     (127)     1392 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/entity_linker.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     1115 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/lemma.json
--rw-r--r--   0 vsts      (1001) docker     (127)      841 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/lemma.jsonl
--rw-r--r--   0 vsts      (1001) docker     (127)      930 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/lemma.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      608 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/ner.json
--rw-r--r--   0 vsts      (1001) docker     (127)      366 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/ner.jsonl
--rw-r--r--   0 vsts      (1001) docker     (127)      410 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/ner.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     1097 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/ner_inconsistent.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      384 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/raw.json
--rw-r--r--   0 vsts      (1001) docker     (127)      373 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/raw.jsonl
--rw-r--r--   0 vsts      (1001) docker     (127)      366 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/raw.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      579 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/rel.jsonl
--rw-r--r--   0 vsts      (1001) docker     (127)      249 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/sentiment.json
--rw-r--r--   0 vsts      (1001) docker     (127)      186 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/sentiment.jsonl
--rw-r--r--   0 vsts      (1001) docker     (127)      174 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/sentiment.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      745 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/spancat.json
--rw-r--r--   0 vsts      (1001) docker     (127)      449 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/spancat.jsonl
--rw-r--r--   0 vsts      (1001) docker     (127)      549 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/spancat.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     3126 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/summarization.json
--rw-r--r--   0 vsts      (1001) docker     (127)     3093 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/summarization.jsonl
--rw-r--r--   0 vsts      (1001) docker     (127)     3089 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/summarization.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      411 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/textcat_binary.json
--rw-r--r--   0 vsts      (1001) docker     (127)      355 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/textcat_binary.jsonl
--rw-r--r--   0 vsts      (1001) docker     (127)      359 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/textcat_binary.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      417 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/textcat_multi_excl.json
--rw-r--r--   0 vsts      (1001) docker     (127)      367 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/textcat_multi_excl.jsonl
--rw-r--r--   0 vsts      (1001) docker     (127)      379 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/textcat_multi_excl.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      433 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl.json
--rw-r--r--   0 vsts      (1001) docker     (127)      383 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl.jsonl
--rw-r--r--   0 vsts      (1001) docker     (127)      395 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      280 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/translation.json
--rw-r--r--   0 vsts      (1001) docker     (127)      268 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/translation.jsonl
--rw-r--r--   0 vsts      (1001) docker     (127)      256 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/translation.yml
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.063458 spacy-llm-0.7.1/spacy_llm/tests/tasks/legacy/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/legacy/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.063458 spacy-llm-0.7.1/spacy_llm/tests/tasks/legacy/examples/
--rw-r--r--   0 vsts      (1001) docker     (127)      409 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/legacy/examples/ner.json
--rw-r--r--   0 vsts      (1001) docker     (127)      233 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/legacy/examples/ner.jsonl
--rw-r--r--   0 vsts      (1001) docker     (127)      255 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/legacy/examples/ner.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      349 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/legacy/examples/ner_inconsistent.yml
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.063458 spacy-llm-0.7.1/spacy_llm/tests/tasks/legacy/templates/
--rw-r--r--   0 vsts      (1001) docker     (127)      183 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/legacy/templates/ner.jinja2
--rw-r--r--   0 vsts      (1001) docker     (127)    24791 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/legacy/test_ner.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17874 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/legacy/test_spancat.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.063458 spacy-llm-0.7.1/spacy_llm/tests/tasks/misc/
--rw-r--r--   0 vsts      (1001) docker     (127)     2075 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/misc/el_kb_data.yml
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.067458 spacy-llm-0.7.1/spacy_llm/tests/tasks/templates/
--rw-r--r--   0 vsts      (1001) docker     (127)       68 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/templates/entity_linker.jinja2
--rw-r--r--   0 vsts      (1001) docker     (127)       59 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/templates/lemma.jinja2
--rw-r--r--   0 vsts      (1001) docker     (127)      930 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/templates/ner.jinja2
--rw-r--r--   0 vsts      (1001) docker     (127)       57 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/templates/raw.jinja2
--rw-r--r--   0 vsts      (1001) docker     (127)       27 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/templates/sentiment.jinja2
--rw-r--r--   0 vsts      (1001) docker     (127)      984 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/templates/spancat.jinja2
--rw-r--r--   0 vsts      (1001) docker     (127)       67 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/templates/summarization.jinja2
--rw-r--r--   0 vsts      (1001) docker     (127)      191 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/templates/textcat.jinja2
--rw-r--r--   0 vsts      (1001) docker     (127)       29 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/templates/translation.jinja2
--rw-r--r--   0 vsts      (1001) docker     (127)      962 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/test_custom.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26370 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/test_entity_linker.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9672 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/test_lemma.py
--rw-r--r--   0 vsts      (1001) docker     (127)    32774 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/test_ner.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7097 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/test_raw.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8066 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/test_rel.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7539 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/test_sentiment.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1654 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/test_span_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20542 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/test_spancat.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13875 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/test_summarization.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24956 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/test_textcat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8151 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/tasks/test_translation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9352 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/test_cache.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1944 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/test_combinations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      325 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/tests/test_registry.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16249 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/ty.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1742 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/spacy_llm/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.071457 spacy-llm-0.7.1/spacy_llm.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     9994 2024-01-29 13:37:44.000000 spacy-llm-0.7.1/spacy_llm.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     9335 2024-01-29 13:37:45.000000 spacy-llm-0.7.1/spacy_llm.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-01-29 13:37:44.000000 spacy-llm-0.7.1/spacy_llm.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      182 2024-01-29 13:37:44.000000 spacy-llm-0.7.1/spacy_llm.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-01-29 13:37:44.000000 spacy-llm-0.7.1/spacy_llm.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      163 2024-01-29 13:37:44.000000 spacy-llm-0.7.1/spacy_llm.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       25 2024-01-29 13:37:44.000000 spacy-llm-0.7.1/spacy_llm.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.067458 spacy-llm-0.7.1/usage_examples/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/usage_examples/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.067458 spacy-llm-0.7.1/usage_examples/el_openai/
--rw-r--r--   0 vsts      (1001) docker     (127)       67 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/usage_examples/el_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1379 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/usage_examples/el_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.067458 spacy-llm-0.7.1/usage_examples/multitask_openai/
--rw-r--r--   0 vsts      (1001) docker     (127)       67 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/usage_examples/multitask_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1244 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/usage_examples/multitask_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.067458 spacy-llm-0.7.1/usage_examples/ner_dolly/
--rw-r--r--   0 vsts      (1001) docker     (127)       67 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/usage_examples/ner_dolly/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      972 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/usage_examples/ner_dolly/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.067458 spacy-llm-0.7.1/usage_examples/ner_langchain_openai/
--rw-r--r--   0 vsts      (1001) docker     (127)       67 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/usage_examples/ner_langchain_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/usage_examples/ner_langchain_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.067458 spacy-llm-0.7.1/usage_examples/ner_v3_openai/
--rw-r--r--   0 vsts      (1001) docker     (127)       67 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/usage_examples/ner_v3_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      845 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/usage_examples/ner_v3_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.067458 spacy-llm-0.7.1/usage_examples/rel_openai/
--rw-r--r--   0 vsts      (1001) docker     (127)       67 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/usage_examples/rel_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1337 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/usage_examples/rel_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.071457 spacy-llm-0.7.1/usage_examples/tests/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/usage_examples/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      166 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/usage_examples/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5896 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/usage_examples/tests/test_readme_examples.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5109 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/usage_examples/tests/test_usage_examples.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.071457 spacy-llm-0.7.1/usage_examples/textcat_dolly/
--rw-r--r--   0 vsts      (1001) docker     (127)       67 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/usage_examples/textcat_dolly/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1173 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/usage_examples/textcat_dolly/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-29 13:37:45.071457 spacy-llm-0.7.1/usage_examples/textcat_openai/
--rw-r--r--   0 vsts      (1001) docker     (127)       67 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/usage_examples/textcat_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1173 2024-01-29 13:37:32.000000 spacy-llm-0.7.1/usage_examples/textcat_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.991455 spacy_llm-0.7.2/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1066 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      147 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    10045 2024-05-17 09:30:26.991455 spacy_llm-0.7.2/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8450 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)     1483 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     1855 2024-05-17 09:30:26.991455 spacy_llm-0.7.2/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)      153 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.959455 spacy_llm-0.7.2/spacy_llm/
+-rw-r--r--   0 vsts      (1001) docker     (127)      232 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10403 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/cache.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1585 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/compat.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.959455 spacy_llm-0.7.2/spacy_llm/models/
+-rw-r--r--   0 vsts      (1001) docker     (127)      309 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/models/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.959455 spacy_llm-0.7.2/spacy_llm/models/hf/
+-rw-r--r--   0 vsts      (1001) docker     (127)      361 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/models/hf/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7029 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/models/hf/base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2695 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/models/hf/dolly.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3334 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/models/hf/falcon.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2793 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/models/hf/llama2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3953 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/models/hf/mistral.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3823 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/models/hf/openllama.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/models/hf/stablelm.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.959455 spacy_llm-0.7.2/spacy_llm/models/langchain/
+-rw-r--r--   0 vsts      (1001) docker     (127)      227 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/models/langchain/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7637 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/models/langchain/model.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.959455 spacy_llm-0.7.2/spacy_llm/models/rest/
+-rw-r--r--   0 vsts      (1001) docker     (127)      156 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/models/rest/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.959455 spacy_llm-0.7.2/spacy_llm/models/rest/anthropic/
+-rw-r--r--   0 vsts      (1001) docker     (127)      997 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/models/rest/anthropic/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5244 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/models/rest/anthropic/model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26092 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/models/rest/anthropic/registry.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.963455 spacy_llm-0.7.2/spacy_llm/models/rest/azure/
+-rw-r--r--   0 vsts      (1001) docker     (127)      145 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/models/rest/azure/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6559 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/models/rest/azure/model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5964 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/models/rest/azure/registry.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6397 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/models/rest/base.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.963455 spacy_llm-0.7.2/spacy_llm/models/rest/cohere/
+-rw-r--r--   0 vsts      (1001) docker     (127)      167 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/models/rest/cohere/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5311 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/models/rest/cohere/model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3905 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/models/rest/cohere/registry.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.963455 spacy_llm-0.7.2/spacy_llm/models/rest/noop/
+-rw-r--r--   0 vsts      (1001) docker     (127)      123 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/models/rest/noop/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      938 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/models/rest/noop/model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      371 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/models/rest/noop/registry.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.963455 spacy_llm-0.7.2/spacy_llm/models/rest/openai/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1335 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/models/rest/openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6444 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/models/rest/openai/model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30014 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/models/rest/openai/registry.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.963455 spacy_llm-0.7.2/spacy_llm/models/rest/palm/
+-rw-r--r--   0 vsts      (1001) docker     (127)      147 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/models/rest/palm/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4956 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/models/rest/palm/model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4100 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/models/rest/palm/registry.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.963455 spacy_llm-0.7.2/spacy_llm/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (127)       54 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15373 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/pipeline/llm.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.963455 spacy_llm-0.7.2/spacy_llm/registry/
+-rw-r--r--   0 vsts      (1001) docker     (127)      262 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/registry/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      606 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/registry/normalizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2976 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/registry/reader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      450 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/registry/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.963455 spacy_llm-0.7.2/spacy_llm/tasks/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2113 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16856 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/builtin_task.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.963455 spacy_llm-0.7.2/spacy_llm/tasks/entity_linker/
+-rw-r--r--   0 vsts      (1001) docker     (127)      179 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/entity_linker/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2941 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/entity_linker/candidate_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1810 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/entity_linker/parser.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5836 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/entity_linker/registry.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18832 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/entity_linker/task.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1609 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/entity_linker/ty.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8178 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/entity_linker/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.967455 spacy_llm-0.7.2/spacy_llm/tasks/lemma/
+-rw-r--r--   0 vsts      (1001) docker     (127)      157 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/lemma/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1348 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/lemma/parser.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2465 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/lemma/registry.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3361 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/lemma/task.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1464 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/lemma/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.967455 spacy_llm-0.7.2/spacy_llm/tasks/ner/
+-rw-r--r--   0 vsts      (1001) docker     (127)      244 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/ner/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9353 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/ner/registry.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4491 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/ner/task.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1605 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/ner/util.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1660 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/noop.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.967455 spacy_llm-0.7.2/spacy_llm/tasks/raw/
+-rw-r--r--   0 vsts      (1001) docker     (127)      145 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/raw/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      675 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/raw/parser.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2283 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/raw/registry.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3284 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/raw/task.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1187 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/raw/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.967455 spacy_llm-0.7.2/spacy_llm/tasks/rel/
+-rw-r--r--   0 vsts      (1001) docker     (127)      244 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/rel/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      372 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/rel/items.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1501 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/rel/parser.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3172 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/rel/registry.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7443 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/rel/task.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3241 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/rel/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.967455 spacy_llm-0.7.2/spacy_llm/tasks/sentiment/
+-rw-r--r--   0 vsts      (1001) docker     (127)      181 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/sentiment/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      995 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/sentiment/parser.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2439 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/sentiment/registry.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3820 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/sentiment/task.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1999 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/sentiment/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.967455 spacy_llm-0.7.2/spacy_llm/tasks/span/
+-rw-r--r--   0 vsts      (1001) docker     (127)      361 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/span/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3309 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/span/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6464 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/span/parser.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      534 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/span/registry.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5298 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/span/task.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4021 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/span/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.967455 spacy_llm-0.7.2/spacy_llm/tasks/spancat/
+-rw-r--r--   0 vsts      (1001) docker     (127)      284 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/spancat/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9927 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/spancat/registry.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4980 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/spancat/task.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1806 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/spancat/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.971455 spacy_llm-0.7.2/spacy_llm/tasks/summarization/
+-rw-r--r--   0 vsts      (1001) docker     (127)      205 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/summarization/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      771 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/summarization/parser.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2478 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/summarization/registry.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4841 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/summarization/task.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1469 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/summarization/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.971455 spacy_llm-0.7.2/spacy_llm/tasks/templates/
+-rw-r--r--   0 vsts      (1001) docker     (127)      288 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/templates/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2624 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/templates/entity_linker.v1.jinja
+-rw-r--r--   0 vsts      (1001) docker     (127)     1017 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/templates/lemma.v1.jinja
+-rw-r--r--   0 vsts      (1001) docker     (127)      746 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/templates/ner.v1.jinja
+-rw-r--r--   0 vsts      (1001) docker     (127)     1410 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/templates/ner.v2.jinja
+-rw-r--r--   0 vsts      (1001) docker     (127)     2261 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/templates/ner.v3.jinja
+-rw-r--r--   0 vsts      (1001) docker     (127)      309 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/templates/raw.v1.jinja
+-rw-r--r--   0 vsts      (1001) docker     (127)     1585 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/templates/rel.v1.jinja
+-rw-r--r--   0 vsts      (1001) docker     (127)      540 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/templates/sentiment.v1.jinja
+-rw-r--r--   0 vsts      (1001) docker     (127)      769 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/templates/spancat.v1.jinja
+-rw-r--r--   0 vsts      (1001) docker     (127)     1479 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/templates/spancat.v2.jinja
+-rw-r--r--   0 vsts      (1001) docker     (127)     2318 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/templates/spancat.v3.jinja
+-rw-r--r--   0 vsts      (1001) docker     (127)      675 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/templates/summarization.v1.jinja
+-rw-r--r--   0 vsts      (1001) docker     (127)     1251 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/templates/textcat.v1.jinja
+-rw-r--r--   0 vsts      (1001) docker     (127)     1717 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/templates/textcat.v2.jinja
+-rw-r--r--   0 vsts      (1001) docker     (127)     2162 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/templates/textcat.v3.jinja
+-rw-r--r--   0 vsts      (1001) docker     (127)      589 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/templates/translation.v1.jinja
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.971455 spacy_llm-0.7.2/spacy_llm/tasks/textcat/
+-rw-r--r--   0 vsts      (1001) docker     (127)      284 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/textcat/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2106 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/textcat/parser.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10358 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/textcat/registry.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6617 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/textcat/task.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2375 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/textcat/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.971455 spacy_llm-0.7.2/spacy_llm/tasks/translation/
+-rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/translation/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      607 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/translation/parser.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2568 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/translation/registry.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3453 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/translation/task.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1234 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/translation/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.975455 spacy_llm-0.7.2/spacy_llm/tasks/util/
+-rw-r--r--   0 vsts      (1001) docker     (127)       68 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1355 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/util/parsing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4668 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tasks/util/sharding.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.975455 spacy_llm-0.7.2/spacy_llm/tests/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      302 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/compat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1372 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/conftest.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.975455 spacy_llm-0.7.2/spacy_llm/tests/models/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2556 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/models/test_anthropic.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3329 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/models/test_cohere.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1812 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/models/test_dolly.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/models/test_falcon.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2639 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/models/test_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1954 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/models/test_langchain.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1958 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/models/test_llama2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1692 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/models/test_mistral.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2320 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/models/test_openllama.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2427 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/models/test_palm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4333 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/models/test_rest.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2382 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/models/test_stablelm.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.975455 spacy_llm-0.7.2/spacy_llm/tests/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14715 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/pipeline/test_llm.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.975455 spacy_llm-0.7.2/spacy_llm/tests/sharding/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/sharding/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11459 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/sharding/test_sharding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2757 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/sharding/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.979455 spacy_llm-0.7.2/spacy_llm/tests/tasks/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      214 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/custom.cfg
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.983455 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1449 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/entity_linker.json
+-rw-r--r--   0 vsts      (1001) docker     (127)     1244 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/entity_linker.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (127)     1392 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/entity_linker.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)     1115 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/lemma.json
+-rw-r--r--   0 vsts      (1001) docker     (127)      841 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/lemma.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (127)      930 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/lemma.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)      608 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/ner.json
+-rw-r--r--   0 vsts      (1001) docker     (127)      366 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/ner.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (127)      410 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/ner.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)     1097 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/ner_inconsistent.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)      384 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/raw.json
+-rw-r--r--   0 vsts      (1001) docker     (127)      373 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/raw.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (127)      366 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/raw.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)      579 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/rel.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (127)      249 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/sentiment.json
+-rw-r--r--   0 vsts      (1001) docker     (127)      186 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/sentiment.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (127)      174 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/sentiment.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)      745 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/spancat.json
+-rw-r--r--   0 vsts      (1001) docker     (127)      449 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/spancat.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (127)      549 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/spancat.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)     3126 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/summarization.json
+-rw-r--r--   0 vsts      (1001) docker     (127)     3093 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/summarization.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (127)     3089 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/summarization.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)      411 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/textcat_binary.json
+-rw-r--r--   0 vsts      (1001) docker     (127)      355 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/textcat_binary.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (127)      359 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/textcat_binary.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)      417 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/textcat_multi_excl.json
+-rw-r--r--   0 vsts      (1001) docker     (127)      367 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/textcat_multi_excl.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (127)      379 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/textcat_multi_excl.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)      433 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl.json
+-rw-r--r--   0 vsts      (1001) docker     (127)      383 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (127)      395 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)      280 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/translation.json
+-rw-r--r--   0 vsts      (1001) docker     (127)      268 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/translation.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (127)      256 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/translation.yml
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.983455 spacy_llm-0.7.2/spacy_llm/tests/tasks/legacy/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/legacy/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.983455 spacy_llm-0.7.2/spacy_llm/tests/tasks/legacy/examples/
+-rw-r--r--   0 vsts      (1001) docker     (127)      409 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/legacy/examples/ner.json
+-rw-r--r--   0 vsts      (1001) docker     (127)      233 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/legacy/examples/ner.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (127)      255 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/legacy/examples/ner.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)      349 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/legacy/examples/ner_inconsistent.yml
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.983455 spacy_llm-0.7.2/spacy_llm/tests/tasks/legacy/templates/
+-rw-r--r--   0 vsts      (1001) docker     (127)      183 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/legacy/templates/ner.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (127)    24791 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/legacy/test_ner.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17874 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/legacy/test_spancat.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.983455 spacy_llm-0.7.2/spacy_llm/tests/tasks/misc/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2075 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/misc/el_kb_data.yml
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.983455 spacy_llm-0.7.2/spacy_llm/tests/tasks/templates/
+-rw-r--r--   0 vsts      (1001) docker     (127)       68 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/templates/entity_linker.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (127)       59 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/templates/lemma.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (127)      930 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/templates/ner.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (127)       57 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/templates/raw.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (127)       27 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/templates/sentiment.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (127)      984 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/templates/spancat.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (127)       67 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/templates/summarization.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (127)      191 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/templates/textcat.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (127)       29 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/templates/translation.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (127)      962 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/test_custom.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26370 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/test_entity_linker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9672 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/test_lemma.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    32774 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/test_ner.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7097 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/test_raw.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8066 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/test_rel.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7539 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/test_sentiment.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1654 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/test_span_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20542 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/test_spancat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13875 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/test_summarization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24956 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/test_textcat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8151 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/tasks/test_translation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9352 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/test_cache.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1944 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/test_combinations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      325 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/tests/test_registry.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16249 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/ty.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1742 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/spacy_llm/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.987455 spacy_llm-0.7.2/spacy_llm.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10045 2024-05-17 09:30:26.000000 spacy_llm-0.7.2/spacy_llm.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     9335 2024-05-17 09:30:26.000000 spacy_llm-0.7.2/spacy_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-17 09:30:26.000000 spacy_llm-0.7.2/spacy_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      182 2024-05-17 09:30:26.000000 spacy_llm-0.7.2/spacy_llm.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-17 09:30:26.000000 spacy_llm-0.7.2/spacy_llm.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      163 2024-05-17 09:30:26.000000 spacy_llm-0.7.2/spacy_llm.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       25 2024-05-17 09:30:26.000000 spacy_llm-0.7.2/spacy_llm.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.983455 spacy_llm-0.7.2/usage_examples/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/usage_examples/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.987455 spacy_llm-0.7.2/usage_examples/el_openai/
+-rw-r--r--   0 vsts      (1001) docker     (127)       67 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/usage_examples/el_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1379 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/usage_examples/el_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.987455 spacy_llm-0.7.2/usage_examples/multitask_openai/
+-rw-r--r--   0 vsts      (1001) docker     (127)       67 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/usage_examples/multitask_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1244 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/usage_examples/multitask_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.987455 spacy_llm-0.7.2/usage_examples/ner_dolly/
+-rw-r--r--   0 vsts      (1001) docker     (127)       67 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/usage_examples/ner_dolly/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      972 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/usage_examples/ner_dolly/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.987455 spacy_llm-0.7.2/usage_examples/ner_langchain_openai/
+-rw-r--r--   0 vsts      (1001) docker     (127)       67 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/usage_examples/ner_langchain_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/usage_examples/ner_langchain_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.987455 spacy_llm-0.7.2/usage_examples/ner_v3_openai/
+-rw-r--r--   0 vsts      (1001) docker     (127)       67 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/usage_examples/ner_v3_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      845 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/usage_examples/ner_v3_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.987455 spacy_llm-0.7.2/usage_examples/rel_openai/
+-rw-r--r--   0 vsts      (1001) docker     (127)       67 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/usage_examples/rel_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1337 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/usage_examples/rel_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.987455 spacy_llm-0.7.2/usage_examples/tests/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/usage_examples/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      166 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/usage_examples/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5896 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/usage_examples/tests/test_readme_examples.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5109 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/usage_examples/tests/test_usage_examples.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.987455 spacy_llm-0.7.2/usage_examples/textcat_dolly/
+-rw-r--r--   0 vsts      (1001) docker     (127)       67 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/usage_examples/textcat_dolly/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1173 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/usage_examples/textcat_dolly/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 09:30:26.987455 spacy_llm-0.7.2/usage_examples/textcat_openai/
+-rw-r--r--   0 vsts      (1001) docker     (127)       67 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/usage_examples/textcat_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1173 2024-05-17 09:30:21.000000 spacy_llm-0.7.2/usage_examples/textcat_openai/run_pipeline.py
```

### Comparing `spacy-llm-0.7.1/LICENSE` & `spacy_llm-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/PKG-INFO` & `spacy_llm-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-llm
-Version: 0.7.1
+Version: 0.7.2
 Summary: Integrating LLMs into structured NLP pipelines
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Project-URL: Release notes, https://github.com/explosion/spacy-llm/releases
 Project-URL: Source, https://github.com/explosion/spacy-llm
 Classifier: Development Status :: 4 - Beta
@@ -17,14 +17,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: spacy<4.0,>=3.5
 Requires-Dist: jinja2
 Requires-Dist: confection<1.0.0,>=0.1.3
```

#### html2text {}

```diff
@@ -1,29 +1,30 @@
-Metadata-Version: 2.1 Name: spacy-llm Version: 0.7.1 Summary: Integrating LLMs
+Metadata-Version: 2.1 Name: spacy-llm Version: 0.7.2 Summary: Integrating LLMs
 into structured NLP pipelines Author: Explosion Author-email:
 contact@explosion.ai License: MIT Project-URL: Release notes, https://
 github.com/explosion/spacy-llm/releases Project-URL: Source, https://
 github.com/explosion/spacy-llm Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: Microsoft :: Windows Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: spacy<4.0,>=3.5 Requires-Dist: jinja2 Requires-Dist:
-confection<1.0.0,>=0.1.3 Provides-Extra: langchain Requires-Dist:
-langchain<0.2,>=0.1; extra == "langchain" Provides-Extra: transformers
-Requires-Dist: torch<2.0,>=1.13.1; extra == "transformers" Requires-Dist:
-transformers<5.0,>=4.28.1; extra == "transformers" Requires-Dist: einops>=0.4;
-extra == "transformers" Requires-Dist: xformers; extra == "transformers"_[_h_t_t_p_s_:
-_/_/_e_x_p_l_o_s_i_o_n_._a_i_/_a_s_s_e_t_s_/_i_m_g_/_l_o_g_o_._s_v_g_]_[_a_s_s_e_t_s_/_l_o_g_o_._p_n_g_]
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering Requires-Python: >=3.7 Description-
+Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+spacy<4.0,>=3.5 Requires-Dist: jinja2 Requires-Dist: confection<1.0.0,>=0.1.3
+Provides-Extra: langchain Requires-Dist: langchain<0.2,>=0.1; extra ==
+"langchain" Provides-Extra: transformers Requires-Dist: torch<2.0,>=1.13.1;
+extra == "transformers" Requires-Dist: transformers<5.0,>=4.28.1; extra ==
+"transformers" Requires-Dist: einops>=0.4; extra == "transformers" Requires-
+Dist: xformers; extra == "transformers"_[_h_t_t_p_s_:_/_/_e_x_p_l_o_s_i_o_n_._a_i_/_a_s_s_e_t_s_/_i_m_g_/
+_l_o_g_o_._s_v_g_]_[_a_s_s_e_t_s_/_l_o_g_o_._p_n_g_]
                                ************ ssppaaccyy--llllmm
                         SSttrruuccttuurreedd NNLLPP wwiitthh LLLLMMss ************
 
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/
 status/explosion/spacy-llm/test.yml?branch=main)](https://github.com/explosion/
 spacy-llm/actions/workflows/test.yml) [![pypi Version](https://img.shields.io/
```

### Comparing `spacy-llm-0.7.1/README.md` & `spacy_llm-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/pyproject.toml` & `spacy_llm-0.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/setup.cfg` & `spacy_llm-0.7.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 0.7.1
+version = 0.7.2
 description = Integrating LLMs into structured NLP pipelines
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
@@ -17,14 +17,15 @@
 	Operating System :: Microsoft :: Windows
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Scientific/Engineering
 project_urls = 
 	Release notes = https://github.com/explosion/spacy-llm/releases
 	Source = https://github.com/explosion/spacy-llm
 
 [options]
 zip_safe = false
```

### Comparing `spacy-llm-0.7.1/spacy_llm/cache.py` & `spacy_llm-0.7.2/spacy_llm/cache.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/compat.py` & `spacy_llm-0.7.2/spacy_llm/compat.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/models/hf/base.py` & `spacy_llm-0.7.2/spacy_llm/models/hf/base.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/models/hf/dolly.py` & `spacy_llm-0.7.2/spacy_llm/models/hf/dolly.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/models/hf/falcon.py` & `spacy_llm-0.7.2/spacy_llm/models/hf/falcon.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/models/hf/llama2.py` & `spacy_llm-0.7.2/spacy_llm/models/hf/llama2.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/models/hf/mistral.py` & `spacy_llm-0.7.2/spacy_llm/models/hf/mistral.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/models/hf/openllama.py` & `spacy_llm-0.7.2/spacy_llm/models/hf/openllama.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/models/hf/stablelm.py` & `spacy_llm-0.7.2/spacy_llm/models/hf/stablelm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple
 
 from confection import SimpleFrozenDict
 
-from ...compat import Literal, has_transformers, torch, transformers
+from ...compat import Literal, has_torch, has_transformers, torch, transformers
 from ...registry.util import registry
 from .base import HuggingFace
 
-if has_transformers:
+if has_transformers and has_torch:
 
     class _StopOnTokens(transformers.StoppingCriteria):
         def __call__(
             self, input_ids: torch.LongTensor, scores: torch.FloatTensor, **kwargs
         ) -> bool:
             stop_ids = [50278, 50279, 50277, 1, 0]
             for stop_id in stop_ids:
```

### Comparing `spacy-llm-0.7.1/spacy_llm/models/langchain/model.py` & `spacy_llm-0.7.2/spacy_llm/models/langchain/model.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/models/rest/anthropic/__init__.py` & `spacy_llm-0.7.2/spacy_llm/models/rest/anthropic/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/models/rest/anthropic/model.py` & `spacy_llm-0.7.2/spacy_llm/models/rest/anthropic/model.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/models/rest/anthropic/registry.py` & `spacy_llm-0.7.2/spacy_llm/models/rest/anthropic/registry.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/models/rest/azure/model.py` & `spacy_llm-0.7.2/spacy_llm/models/rest/azure/model.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/models/rest/azure/registry.py` & `spacy_llm-0.7.2/spacy_llm/models/rest/azure/registry.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/models/rest/base.py` & `spacy_llm-0.7.2/spacy_llm/models/rest/base.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/models/rest/cohere/model.py` & `spacy_llm-0.7.2/spacy_llm/models/rest/cohere/model.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/models/rest/cohere/registry.py` & `spacy_llm-0.7.2/spacy_llm/models/rest/cohere/registry.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/models/rest/noop/model.py` & `spacy_llm-0.7.2/spacy_llm/models/rest/noop/model.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/models/rest/openai/__init__.py` & `spacy_llm-0.7.2/spacy_llm/models/rest/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/models/rest/openai/model.py` & `spacy_llm-0.7.2/spacy_llm/models/rest/openai/model.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/models/rest/openai/registry.py` & `spacy_llm-0.7.2/spacy_llm/models/rest/openai/registry.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/models/rest/palm/model.py` & `spacy_llm-0.7.2/spacy_llm/models/rest/palm/model.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/models/rest/palm/registry.py` & `spacy_llm-0.7.2/spacy_llm/models/rest/palm/registry.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/pipeline/llm.py` & `spacy_llm-0.7.2/spacy_llm/pipeline/llm.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/registry/normalizer.py` & `spacy_llm-0.7.2/spacy_llm/registry/normalizer.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/registry/reader.py` & `spacy_llm-0.7.2/spacy_llm/registry/reader.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/__init__.py` & `spacy_llm-0.7.2/spacy_llm/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/builtin_task.py` & `spacy_llm-0.7.2/spacy_llm/tasks/builtin_task.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/entity_linker/candidate_selector.py` & `spacy_llm-0.7.2/spacy_llm/tasks/entity_linker/candidate_selector.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/entity_linker/parser.py` & `spacy_llm-0.7.2/spacy_llm/tasks/entity_linker/parser.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/entity_linker/registry.py` & `spacy_llm-0.7.2/spacy_llm/tasks/entity_linker/registry.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/entity_linker/task.py` & `spacy_llm-0.7.2/spacy_llm/tasks/entity_linker/task.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/entity_linker/ty.py` & `spacy_llm-0.7.2/spacy_llm/tasks/entity_linker/ty.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/entity_linker/util.py` & `spacy_llm-0.7.2/spacy_llm/tasks/entity_linker/util.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/lemma/parser.py` & `spacy_llm-0.7.2/spacy_llm/tasks/lemma/parser.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/lemma/registry.py` & `spacy_llm-0.7.2/spacy_llm/tasks/lemma/registry.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/lemma/task.py` & `spacy_llm-0.7.2/spacy_llm/tasks/lemma/task.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/lemma/util.py` & `spacy_llm-0.7.2/spacy_llm/tasks/lemma/util.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/ner/registry.py` & `spacy_llm-0.7.2/spacy_llm/tasks/ner/registry.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/ner/task.py` & `spacy_llm-0.7.2/spacy_llm/tasks/ner/task.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/ner/util.py` & `spacy_llm-0.7.2/spacy_llm/tasks/ner/util.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/noop.py` & `spacy_llm-0.7.2/spacy_llm/tasks/noop.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/raw/parser.py` & `spacy_llm-0.7.2/spacy_llm/tasks/raw/parser.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/raw/registry.py` & `spacy_llm-0.7.2/spacy_llm/tasks/raw/registry.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/raw/task.py` & `spacy_llm-0.7.2/spacy_llm/tasks/raw/task.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/raw/util.py` & `spacy_llm-0.7.2/spacy_llm/tasks/raw/util.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/rel/parser.py` & `spacy_llm-0.7.2/spacy_llm/tasks/rel/parser.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/rel/registry.py` & `spacy_llm-0.7.2/spacy_llm/tasks/rel/registry.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/rel/task.py` & `spacy_llm-0.7.2/spacy_llm/tasks/rel/task.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/rel/util.py` & `spacy_llm-0.7.2/spacy_llm/tasks/rel/util.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/sentiment/parser.py` & `spacy_llm-0.7.2/spacy_llm/tasks/sentiment/parser.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/sentiment/registry.py` & `spacy_llm-0.7.2/spacy_llm/tasks/sentiment/registry.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/sentiment/task.py` & `spacy_llm-0.7.2/spacy_llm/tasks/sentiment/task.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/sentiment/util.py` & `spacy_llm-0.7.2/spacy_llm/tasks/sentiment/util.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/span/examples.py` & `spacy_llm-0.7.2/spacy_llm/tasks/span/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/span/parser.py` & `spacy_llm-0.7.2/spacy_llm/tasks/span/parser.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/span/registry.py` & `spacy_llm-0.7.2/spacy_llm/tasks/span/registry.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/span/task.py` & `spacy_llm-0.7.2/spacy_llm/tasks/span/task.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/span/util.py` & `spacy_llm-0.7.2/spacy_llm/tasks/span/util.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/spancat/registry.py` & `spacy_llm-0.7.2/spacy_llm/tasks/spancat/registry.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/spancat/task.py` & `spacy_llm-0.7.2/spacy_llm/tasks/spancat/task.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/spancat/util.py` & `spacy_llm-0.7.2/spacy_llm/tasks/spancat/util.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/summarization/parser.py` & `spacy_llm-0.7.2/spacy_llm/tasks/summarization/parser.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/summarization/registry.py` & `spacy_llm-0.7.2/spacy_llm/tasks/summarization/registry.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/summarization/task.py` & `spacy_llm-0.7.2/spacy_llm/tasks/summarization/task.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/summarization/util.py` & `spacy_llm-0.7.2/spacy_llm/tasks/summarization/util.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/templates/entity_linker.v1.jinja` & `spacy_llm-0.7.2/spacy_llm/tasks/templates/entity_linker.v1.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/templates/lemma.v1.jinja` & `spacy_llm-0.7.2/spacy_llm/tasks/templates/lemma.v1.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/templates/ner.v1.jinja` & `spacy_llm-0.7.2/spacy_llm/tasks/templates/ner.v1.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/templates/ner.v2.jinja` & `spacy_llm-0.7.2/spacy_llm/tasks/templates/ner.v2.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/templates/ner.v3.jinja` & `spacy_llm-0.7.2/spacy_llm/tasks/templates/ner.v3.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/templates/rel.v1.jinja` & `spacy_llm-0.7.2/spacy_llm/tasks/templates/rel.v1.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/templates/sentiment.v1.jinja` & `spacy_llm-0.7.2/spacy_llm/tasks/templates/sentiment.v1.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/templates/spancat.v1.jinja` & `spacy_llm-0.7.2/spacy_llm/tasks/templates/spancat.v1.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/templates/spancat.v2.jinja` & `spacy_llm-0.7.2/spacy_llm/tasks/templates/spancat.v2.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/templates/spancat.v3.jinja` & `spacy_llm-0.7.2/spacy_llm/tasks/templates/spancat.v3.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/templates/summarization.v1.jinja` & `spacy_llm-0.7.2/spacy_llm/tasks/templates/summarization.v1.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/templates/textcat.v1.jinja` & `spacy_llm-0.7.2/spacy_llm/tasks/templates/textcat.v1.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/templates/textcat.v2.jinja` & `spacy_llm-0.7.2/spacy_llm/tasks/templates/textcat.v2.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/templates/textcat.v3.jinja` & `spacy_llm-0.7.2/spacy_llm/tasks/templates/textcat.v3.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/templates/translation.v1.jinja` & `spacy_llm-0.7.2/spacy_llm/tasks/templates/translation.v1.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/textcat/parser.py` & `spacy_llm-0.7.2/spacy_llm/tasks/textcat/parser.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/textcat/registry.py` & `spacy_llm-0.7.2/spacy_llm/tasks/textcat/registry.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/textcat/task.py` & `spacy_llm-0.7.2/spacy_llm/tasks/textcat/task.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/textcat/util.py` & `spacy_llm-0.7.2/spacy_llm/tasks/textcat/util.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/translation/parser.py` & `spacy_llm-0.7.2/spacy_llm/tasks/translation/parser.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/translation/registry.py` & `spacy_llm-0.7.2/spacy_llm/tasks/translation/registry.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/translation/task.py` & `spacy_llm-0.7.2/spacy_llm/tasks/translation/task.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/translation/util.py` & `spacy_llm-0.7.2/spacy_llm/tasks/translation/util.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/util/parsing.py` & `spacy_llm-0.7.2/spacy_llm/tasks/util/parsing.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tasks/util/sharding.py` & `spacy_llm-0.7.2/spacy_llm/tasks/util/sharding.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/conftest.py` & `spacy_llm-0.7.2/spacy_llm/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/models/test_anthropic.py` & `spacy_llm-0.7.2/spacy_llm/tests/models/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/models/test_cohere.py` & `spacy_llm-0.7.2/spacy_llm/tests/models/test_cohere.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/models/test_dolly.py` & `spacy_llm-0.7.2/spacy_llm/tests/models/test_dolly.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/models/test_falcon.py` & `spacy_llm-0.7.2/spacy_llm/tests/models/test_falcon.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/models/test_hf.py` & `spacy_llm-0.7.2/spacy_llm/tests/models/test_hf.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/models/test_langchain.py` & `spacy_llm-0.7.2/spacy_llm/tests/models/test_langchain.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/models/test_llama2.py` & `spacy_llm-0.7.2/spacy_llm/tests/models/test_llama2.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/models/test_mistral.py` & `spacy_llm-0.7.2/spacy_llm/tests/models/test_mistral.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/models/test_openllama.py` & `spacy_llm-0.7.2/spacy_llm/tests/models/test_openllama.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/models/test_palm.py` & `spacy_llm-0.7.2/spacy_llm/tests/models/test_palm.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/models/test_rest.py` & `spacy_llm-0.7.2/spacy_llm/tests/models/test_rest.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/models/test_stablelm.py` & `spacy_llm-0.7.2/spacy_llm/tests/models/test_stablelm.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/pipeline/test_llm.py` & `spacy_llm-0.7.2/spacy_llm/tests/pipeline/test_llm.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/sharding/test_sharding.py` & `spacy_llm-0.7.2/spacy_llm/tests/sharding/test_sharding.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/sharding/util.py` & `spacy_llm-0.7.2/spacy_llm/tests/sharding/util.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/entity_linker.json` & `spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/entity_linker.json`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/entity_linker.jsonl` & `spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/entity_linker.jsonl`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/entity_linker.yml` & `spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/entity_linker.yml`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/lemma.json` & `spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/lemma.json`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/lemma.jsonl` & `spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/lemma.jsonl`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/lemma.yml` & `spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/lemma.yml`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/ner.json` & `spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/ner.json`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/ner_inconsistent.yml` & `spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/ner_inconsistent.yml`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/rel.jsonl` & `spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/rel.jsonl`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/spancat.json` & `spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/spancat.json`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/spancat.yml` & `spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/spancat.yml`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/summarization.json` & `spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/summarization.json`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/summarization.jsonl` & `spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/summarization.jsonl`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/tasks/examples/summarization.yml` & `spacy_llm-0.7.2/spacy_llm/tests/tasks/examples/summarization.yml`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/tasks/legacy/test_ner.py` & `spacy_llm-0.7.2/spacy_llm/tests/tasks/legacy/test_ner.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/tasks/legacy/test_spancat.py` & `spacy_llm-0.7.2/spacy_llm/tests/tasks/legacy/test_spancat.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/tasks/misc/el_kb_data.yml` & `spacy_llm-0.7.2/spacy_llm/tests/tasks/misc/el_kb_data.yml`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/tasks/templates/ner.jinja2` & `spacy_llm-0.7.2/spacy_llm/tests/tasks/templates/ner.jinja2`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/tasks/templates/spancat.jinja2` & `spacy_llm-0.7.2/spacy_llm/tests/tasks/templates/spancat.jinja2`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/tasks/test_custom.py` & `spacy_llm-0.7.2/spacy_llm/tests/tasks/test_custom.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/tasks/test_entity_linker.py` & `spacy_llm-0.7.2/spacy_llm/tests/tasks/test_entity_linker.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/tasks/test_lemma.py` & `spacy_llm-0.7.2/spacy_llm/tests/tasks/test_lemma.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/tasks/test_ner.py` & `spacy_llm-0.7.2/spacy_llm/tests/tasks/test_ner.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/tasks/test_raw.py` & `spacy_llm-0.7.2/spacy_llm/tests/tasks/test_raw.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/tasks/test_rel.py` & `spacy_llm-0.7.2/spacy_llm/tests/tasks/test_rel.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/tasks/test_sentiment.py` & `spacy_llm-0.7.2/spacy_llm/tests/tasks/test_sentiment.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/tasks/test_span_utils.py` & `spacy_llm-0.7.2/spacy_llm/tests/tasks/test_span_utils.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/tasks/test_spancat.py` & `spacy_llm-0.7.2/spacy_llm/tests/tasks/test_spancat.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/tasks/test_summarization.py` & `spacy_llm-0.7.2/spacy_llm/tests/tasks/test_summarization.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/tasks/test_textcat.py` & `spacy_llm-0.7.2/spacy_llm/tests/tasks/test_textcat.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/tasks/test_translation.py` & `spacy_llm-0.7.2/spacy_llm/tests/tasks/test_translation.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/test_cache.py` & `spacy_llm-0.7.2/spacy_llm/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/tests/test_combinations.py` & `spacy_llm-0.7.2/spacy_llm/tests/test_combinations.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/ty.py` & `spacy_llm-0.7.2/spacy_llm/ty.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm/util.py` & `spacy_llm-0.7.2/spacy_llm/util.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/spacy_llm.egg-info/PKG-INFO` & `spacy_llm-0.7.2/spacy_llm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-llm
-Version: 0.7.1
+Version: 0.7.2
 Summary: Integrating LLMs into structured NLP pipelines
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Project-URL: Release notes, https://github.com/explosion/spacy-llm/releases
 Project-URL: Source, https://github.com/explosion/spacy-llm
 Classifier: Development Status :: 4 - Beta
@@ -17,14 +17,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: spacy<4.0,>=3.5
 Requires-Dist: jinja2
 Requires-Dist: confection<1.0.0,>=0.1.3
```

#### html2text {}

```diff
@@ -1,29 +1,30 @@
-Metadata-Version: 2.1 Name: spacy-llm Version: 0.7.1 Summary: Integrating LLMs
+Metadata-Version: 2.1 Name: spacy-llm Version: 0.7.2 Summary: Integrating LLMs
 into structured NLP pipelines Author: Explosion Author-email:
 contact@explosion.ai License: MIT Project-URL: Release notes, https://
 github.com/explosion/spacy-llm/releases Project-URL: Source, https://
 github.com/explosion/spacy-llm Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: Microsoft :: Windows Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: spacy<4.0,>=3.5 Requires-Dist: jinja2 Requires-Dist:
-confection<1.0.0,>=0.1.3 Provides-Extra: langchain Requires-Dist:
-langchain<0.2,>=0.1; extra == "langchain" Provides-Extra: transformers
-Requires-Dist: torch<2.0,>=1.13.1; extra == "transformers" Requires-Dist:
-transformers<5.0,>=4.28.1; extra == "transformers" Requires-Dist: einops>=0.4;
-extra == "transformers" Requires-Dist: xformers; extra == "transformers"_[_h_t_t_p_s_:
-_/_/_e_x_p_l_o_s_i_o_n_._a_i_/_a_s_s_e_t_s_/_i_m_g_/_l_o_g_o_._s_v_g_]_[_a_s_s_e_t_s_/_l_o_g_o_._p_n_g_]
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering Requires-Python: >=3.7 Description-
+Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+spacy<4.0,>=3.5 Requires-Dist: jinja2 Requires-Dist: confection<1.0.0,>=0.1.3
+Provides-Extra: langchain Requires-Dist: langchain<0.2,>=0.1; extra ==
+"langchain" Provides-Extra: transformers Requires-Dist: torch<2.0,>=1.13.1;
+extra == "transformers" Requires-Dist: transformers<5.0,>=4.28.1; extra ==
+"transformers" Requires-Dist: einops>=0.4; extra == "transformers" Requires-
+Dist: xformers; extra == "transformers"_[_h_t_t_p_s_:_/_/_e_x_p_l_o_s_i_o_n_._a_i_/_a_s_s_e_t_s_/_i_m_g_/
+_l_o_g_o_._s_v_g_]_[_a_s_s_e_t_s_/_l_o_g_o_._p_n_g_]
                                ************ ssppaaccyy--llllmm
                         SSttrruuccttuurreedd NNLLPP wwiitthh LLLLMMss ************
 
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/
 status/explosion/spacy-llm/test.yml?branch=main)](https://github.com/explosion/
 spacy-llm/actions/workflows/test.yml) [![pypi Version](https://img.shields.io/
```

### Comparing `spacy-llm-0.7.1/spacy_llm.egg-info/SOURCES.txt` & `spacy_llm-0.7.2/spacy_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/usage_examples/el_openai/run_pipeline.py` & `spacy_llm-0.7.2/usage_examples/el_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/usage_examples/multitask_openai/run_pipeline.py` & `spacy_llm-0.7.2/usage_examples/multitask_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/usage_examples/ner_dolly/run_pipeline.py` & `spacy_llm-0.7.2/usage_examples/ner_dolly/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/usage_examples/ner_langchain_openai/run_pipeline.py` & `spacy_llm-0.7.2/usage_examples/ner_langchain_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/usage_examples/ner_v3_openai/run_pipeline.py` & `spacy_llm-0.7.2/usage_examples/ner_v3_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/usage_examples/rel_openai/run_pipeline.py` & `spacy_llm-0.7.2/usage_examples/rel_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/usage_examples/tests/test_readme_examples.py` & `spacy_llm-0.7.2/usage_examples/tests/test_readme_examples.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/usage_examples/tests/test_usage_examples.py` & `spacy_llm-0.7.2/usage_examples/tests/test_usage_examples.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/usage_examples/textcat_dolly/run_pipeline.py` & `spacy_llm-0.7.2/usage_examples/textcat_dolly/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.7.1/usage_examples/textcat_openai/run_pipeline.py` & `spacy_llm-0.7.2/usage_examples/textcat_openai/run_pipeline.py`

 * *Files identical despite different names*

